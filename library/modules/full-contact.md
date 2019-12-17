# Full Contact

![Build realtime customer intelligence into everything you do.](../../.gitbook/assets/full_contact.png)

{% hint style="info" %}
Check out Full Contact on [GitHub](https://github.com/fullcontact/fullcontact.py).
{% endhint %}

## 🏢 Company Lookup

### 📥 Inputs

* Company Domain / URL

### 📤 Output

```graphql
Company = {
    name : String, 
    num_employees : Int, 
    key_people : [
        {
            name : String, 
            title : String, 
        },
    ],
}
```

## 👤 Person Lookup

### 📥 Inputs

* Email Address

### 📤 Output

```graphql
Person = {
    contact_info : {
        last_name : String, 
        full_name : String, 
        first_name : String, 
        websites : [
            Url,
        ],
    },
    demographics : {
        age : Int, 
        age_range : String, 
        gender : String, 
        location : {
            city : String, 
            continent : String, 
            country : String, 
            county : String, 
            full : String, 
            state : {
                code : String, 
                name : String, 
            },
        },
    },
    likelihood : Float, 
    organizations : [
        {
            current : Bool, 
            primary : Bool,
            name : String, 
            start_date : String, 
            title : String,
        },
    ],
    social_profiles : {
        facebook : Url, 
        instagram : Url, 
        linkedin : Url, 
        twitter : Url, 
        youtube : Url,
    },
}
```


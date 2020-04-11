---
description: >-
  Seamlessly integrate Yelp with your favorite APIs, databases, and programming
  languages, using WayScript.
---

# Yelp

![Look up business information from Yelp.](../../.gitbook/assets/yelp%20%281%29.png)

## ⚙ Settings

* **Search Radius \(Miles\)** - Maxiumum distance of business from **Location Input** 
* **Number of Results** - Number of Businesses to return

## 📥 Inputs

* **Search Term** - The search term of the business \(example - "pizza" or "auto shop"\)
* **Location** - Location you are looking for \(example - "New York, NY"\)

## 📤 Output

```graphql
Businesses = [
    {
        name : String,
        location : {
            address1 : String, 
            address2 : String, 
            address3 : String, 
            city : String, 
            country : String,
            display_address : [
                String,
            ],
            state : String, 
            zipcode : String, 
            full_address : String, 
        },
        display_phone : Stirng, 
        coordinates : {
            lat : Float, 
            long : Float,
        },
        image_url : Url,
        is_closed : Bool,
        phone : String, 
        price : String, 
        rating : Float, 
        review_count : Int,
        yelp_url : Url,
    },
]
```




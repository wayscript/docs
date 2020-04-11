---
description: >-
  Seamlessly integrate Crunchbase with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Crunchbase

![Find business information about private and public companies.](../../.gitbook/assets/crunchbase.png)

{% hint style="info" %}
Check out the Crunchbase [website](https://data.crunchbase.com/reference).
{% endhint %}

## 🗝 Authorization

Crunchbase is available to users who have their own API key.

If not authorized, you will be prompted to enter your API Key when you add the Crunchbase Module to your program. You can edit your key later if it changes.

![](../../.gitbook/assets/screen-shot-2019-07-16-at-3.06.22-pm.png)

## 📥 Inputs

* Organization Name or Website
* Pull Investment Data if Org is an Investor

## 📤 Outputs

```graphql
CB_Data = {
    name : String, 
    short_description : String, 
    description : String, 
    num_employees_min : Int, 
    num_employees_max : Int, 
    total_funding_usd : Int, 
    founders : [
        {
            name : String, 
            bio : String, 
        },    
    ],
    team : [
        {
            name : String, 
            title : String, 
        },
    ],
    investments : [
        {
            name : String, 
            permalink : String, 
            url : Url, 
            investment_amount_usd : Int,
        },
    ]
}
```


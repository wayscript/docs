---
description: >-
  Seamlessly integrate Yellow Pages with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Yellow Pages

![Look up business information from Yellow Pages.](../../.gitbook/assets/yellow_pages%20%281%29.png)

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
        street : String, 
        city : String, 
        state : String, 
        zipcode : String, 
        full_address : String, 
        phone : String, 
        payment_methods : String,
        slogan : String, 
        latitude : String, 
        longitude : String, 
        average_rating : Int,
    },
]
```


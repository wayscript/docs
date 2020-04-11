---
description: >-
  Seamlessly integrate the New York Times with your favorite APIs, databases,
  and programming languages, using WayScript.
---

# NY Times

![Pull articles from the NY Times.](../../.gitbook/assets/ny_times.png)

## 📰 Get Top Stories

### 📥 Inputs

* Section
  * Home
  * Arts
  * Automobiles
  * Books
  * Business
  * Fashion
  * Food
  * Health
  * Insider
  * Magazine
  * Movies
  * National
  * NY Region
  * Obituaries
  * Opinion
  * Politics
  * Real Estate
  * Science
  * Sports
  * Sunday Review
  * Technology
  * Theater
  * T Magazine
  * Travel
  * Upshot
  * World

### 📤 Output

```graphql
Articles = [
    {
        title : String, 
        author : String, 
        abstract : String, 
        date_published : Date, 
        url : Url, 
        des_facet : [
            String,
        ],
        geo_facet : [
            String,
        ],
        org_facet : [
            String, 
        ],
        person_facet : [
            String,
        ],
        section : String, 
        short_url : Url, 
        subsection : String, 
        updated_date : Date, 
        multimedia : [
            {
                caption : String, 
                copyright : String, 
                format : String, 
                height : Int, 
                subtype : String, 
                type : String, 
                url : Url, 
                width : Int,
            },
        ],
    },
]
```


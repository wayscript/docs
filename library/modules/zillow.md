---
description: >-
  Seamlessly integrate Zillow with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Zillow

![Real estate data.](../../.gitbook/assets/zillow_data.png)

{% hint style="info" %}
Check out python-zillow on [GitHub](https://github.com/seme0021/python-zillow).
{% endhint %}

## 🔑 Registering for an API Key

{% hint style="warning" %}
The Zillow module requires you to create an API Key on Zillow.
{% endhint %}

### 1\) Go to [Zillow API Signup Dashboard](https://www.zillow.com/user/Register.htm)

### 2\) Click the 'New Account' tab and submit the required information. 

![](../../.gitbook/assets/zillow_auth_1.png)

### 3\) Fill out the API Sign Up

{% hint style="info" %}
CHECK ALL APIs under the select API\(s\) section!
{% endhint %}

![Check all apis under Select API\(s\)](../../.gitbook/assets/zillow_auth_2.png)

### 4\) You will recieve your Zillow Identification Key \(ZWSID\) via email. 

## 📥 Inputs

* **Address** - Format: Street, Town, State
  * Ex: 3400 Pacific Ave., Marina Del Rey, CA
* **Zip Code** - United States Zip \(postal\) Code
  * Ex: 90292

## 📤 Outputs

{% hint style="info" %}
Outputs are [single Items](../../getting_started/variables.md#single-item) if mode is "Get Data on an Address." Outputs are [lists](../../getting_started/variables.md#lists) if mode is "Get Comparables to an Address."
{% endhint %}

```graphql
Property = {
    value : Number, 
    amount_change_30days : Number, 
    amount_last_updated : Date, 
    valuation_range_high : Number, 
    valuation_range_low : Number,
    num_bathrooms : Float, 
    num_bedrooms : Number, 
    finished_sqft : Number, 
    last_sold_date : Date, 
    last_sold_price : Number, 
    lot_size_sqft : Number, 
    tax_assessment : Number, 
    tax_assessment_year : Date, 
    year_built : Date, 
    usecode : String, 
    complete : Bool,
    currency : String, 
    zpid : String, 
    links : {
        comparables : Url,
        graphs_and_data : Url,
        home_details : Url,
        map_this_home : Url,
    },
    full_address : {
        city : String, 
        latitude : String, 
        longitude : String, 
        state : String, 
        street : String, 
        zipcode : String,
    },
}
```


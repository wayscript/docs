# Clearbit

![Enrich your data with Clearbit.](../../.gitbook/assets/clearbit.png)

## 🗝 Authorization

Clearbit is available to users who have their own API key.

If not authorized, you will be prompted to enter your API Key when you add the Clearbit Module to your program. You can edit your key later if it changes.

![](../../.gitbook/assets/screen-shot-2019-07-16-at-2.32.17-pm.png)

## 📥 Inputs

All Inputs accept manual, variable, or combined inputs.

![](../../.gitbook/assets/screen-shot-2019-07-16-at-2.43.30-pm.png)

{% hint style="info" %}
Optional Inputs will can help improve the accuracy of your search
{% endhint %}

## 🏢 Lookup Company

### 📥 Inputs

* Company Domain Name _\(Required\)_
* Company Name _\(Optional\)_
* LinkedIn URL _\(Optional\)_
* Twitter Handle _\(Optional\)_
* Facebook URL _\(Optional\)_

### 📤 Outputs

```graphql
Company_Data = {
    company_name : String, 
    company_legal_name : String, 
    industry : String, 
    sector : String, 
    sic_code : Int, 
    naics_code : Int, 
    technologies : [
        String,
    ],
    tags : [
        String,
    ],
    type : String, 
    description : String, 
    year_founded : String, 
    ein : String, 
    address : String,
    number_of_employees : Int, 
    fiscal_year_end : String, 
    annual_revenue : Int, 
    alexa_us_rank : Int, 
    alexa_global_rank : Int, 
    phone_number : String, 
    facebook_url : Url,
    twitter_url : Url, 
    linkedin_url : Url, 
    crunchbase_url : Url,
}
```

## 👤 Lookup Person

### 📥 Inputs

* Email Address _\(Required\)_
* First Name _\(Optional\)_
* Last Name _\(Optional\)_
* Location _\(Optional\)_
* Person's Employer _\(Optional\)_
* Person's Company Domain Name _\(Optional\)_
* LinkedIn URL _\(Optional\)_
* Twitter Handle _\(Optional\)_
* Facebook URL _\(Optional\)_

### 📤 Outputs

```graphql
Person_Data = {
    name : String, 
    email : String, 
    bio : String, 
    website : String, 
    location : String, 
    employer : String, 
    employer_website : Url,
    job_title : String,
    job_role : String, 
    seniority : String, 
    facebook_url : Url,
    twitter_url : Url, 
    github_url : Url,   
}
```

## 🕵♀ Lookup Combined

### 📥 Inputs

* Email Address _\(Required\)_
* First Name _\(Optional\)_
* Last Name _\(Optional\)_
* Location _\(Optional\)_
* Person's Employer _\(Optional\)_
* Person's Company Domain Name _\(Optional\)_
* LinkedIn URL _\(Optional\)_
* Twitte Handle _\(Optional\)_
* Facebook URL _\(Optional\)_

### 📤 Outputs

Returns both the Company\_Data and Person\_Data objects from above


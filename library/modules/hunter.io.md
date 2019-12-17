# Hunter.io

![Find the email address of any professional with the most advanced email-finding tool.](../../.gitbook/assets/hunter_io.png)

{% hint style="warning" %}
In the free tier, this library requires an API Key, which you can get on the [Hunter.io website](https://hunter.io).
{% endhint %}

## 📧 Email Finder

### 📥 Inputs

* **Company Domain/URL**
  * example - tesla.com
* **First Name**
  * example - Elon
* **Last Name**
  * example - Musk

### 📤 Outputs

```graphql
HunterIO_Data = {
    email : String, 
    company : String, 
    linkedin_url : Url, 
    twitter : String, 
    phone_number : String, 
    position : String, 
    score : Int,
}
```

## ✅ Email Verification

This mode tests whether an email address is real/valid.

### 📥 Inputs

* **Email Address**

### 📤 Outputs

* **Result** - Returns Deliverable or Undeliverable \(String\)
* **SMTP Check** - Returns True or False \(Bool\)
* **JSON Data** - Raw JSON from the API query


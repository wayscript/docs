---
description: >-
  Seamlessly integrate Salesforce with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Salesforce Trigger

![Run your script when a Salesforce object is created or updated.](../../.gitbook/assets/salesforce.png)

{% hint style="info" %}
To create, edit, and query Salesforce objects, use the [Salesforce module](../modules/salesforce.md).
{% endhint %}

## ⚙ Setup

### 🔗 Link Your Salesforce Account

When you drag in a Salesforce Trigger for the first time, follow the prompt to authorize access.

### 🔑 API Access

First make sure you have API access enabled in Salesforce. To do this, follow [these instructions](https://ebstalimited.zendesk.com/hc/en-us/articles/229295368-How-do-I-enable-API-access-in-Salesforce).

## ![](../../.gitbook/assets/salesforce.png) New Object Created

![Select New Object Created Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.44.24-am.png)

{% hint style="success" %}
Your script will run when a new Salesforce object is created.
{% endhint %}

### 🌟 New Account

![Select New Account Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.46.22-am.png)

{% hint style="success" %}
Your script will run when a new account is created.
{% endhint %}

#### 📤 Outputs

```graphql
Account = {
            id               : String,
            name             : String,
            parent_id        : String,
            number           : String,
            site             : String,
            type             : String,
            industry         : String,
            annual_rev       : Number,
            rating           : String,
            phone            : String,
            fax              : String,
            website          : String,
            ticker           : String,
            ownership        : String,
            employees        : String,
            sic_code         : String,
            billing_street   : String,
            billing_city     : String,
            billing_state    : String,
            billing_zip      : String,
            billing_country  : String,
            shipping_street  : String,
            shipping_city    : String,
            shipping_state   : String,
            shipping_zip     : String,
            shipping_country : String,
            description      : String
}
```

* JSON Data
  * Raw JSON data received from the API

### 📈 New Campaign

![Select New Campaign Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.52.40-am.png)

{% hint style="success" %}
Your script will run when a new campaign is created.
{% endhint %}

#### 📤 Outputs

```graphql
Campaign = {
             id                : String,
             name              : String,
             active            : String,
             type              : String,
             status            : String,
             start_date        : Date,
             end_date          : Date,
             expected_rev      : Number,
             budgeted_cost     : Number,
             actual_cost       : Number,
             expected_response : Number,
             num_sent          : Number,
             parent_id         : String,
             description       : String
}
```

* JSON Data
  * Raw JSON data received from the API

### 💼 New Case

![Select New Case Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.56.22-am.png)

{% hint style="success" %}
Your script will run when a new case is created.
{% endhint %}

#### 📤 Outputs

```graphql
Case = { 
         id          : String,
         subject     : String,
         status      : String,
         origin      : String,
         contact     : String,
         account_id  : String,
         type        : String,
         reason      : String,
         priority    : String,
         web_email   : String,
         web_name    : String,
         web_company : String,
         web_phone   : String,
         description : String
}
```

* JSON Data
  * Raw JSON data received from the API

### 👤 New Contact

![Select New Contact Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.59.47-am.png)

{% hint style="success" %}
Your script will run when a new contact is created.
{% endhint %}

#### 📤 Outputs

```graphql
Contact = {
            id              : String,
            name            : String,
            salutation      : String,
            acct_id         : String,
            title           : String,
            department      : String,
            birthdate       : Date,
            reports_to      : String,
            lead_source     : String,
            phone           : String,
            home_phone      : String,
            mobile          : String,
            other_phone     : String,
            fax             : String,
            email           : String,
            asst_name       : String,
            asst_phone      : String,
            mailing_street  : String,
            mailing_city    : String,
            mailing_state   : String,
            mailing_zip     : String,
            mailing_country : String,
            other_street    : String,
            other_city      : String,
            other_state     : String,
            other_zip       : String,
            other_country   : String,
            description     : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### 🗓 New Event

![Select New Event Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.05.45-pm.png)

{% hint style="success" %}
Your script will run when a new event is created.
{% endhint %}

#### 📤 Outputs

```graphql
Event = {
          id          : String,
          subject     : String,
          all_day     : String,
          start       : DateType,
          end         : DateType,
          location    : String,
          name_id     : String,
          related_to  : String,
          description : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### 🕵 New Lead

![Select New Lead Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.08.33-pm.png)

{% hint style="success" %}
Your script will run when a new lead is created.
{% endhint %}

#### 📤Outputs

```graphql
Lead = {  
          id          : String,
          name        : String,
          salutation  : String,
          status      : String,
          company     : String,
          title       : String,
          source      : String,
          industry    : String,
          annual_rev  : Number,
          phone       : String,
          mobile      : String,
          fax         : String,
          email       : String,
          website     : String,
          rating      : String,
          employees   : Int,
          street      : String,
          city        : String,
          state       : String,
          zip         : String,
          country     : String,
          description : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### 🗒 New Note

![Select New Note Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.11.28-pm.png)

{% hint style="success" %}
Your script will run when a new note is created.
{% endhint %}

#### 📤 Outputs

```graphql
Note = {  
          id         : String,
          title      : String,
          body       : String,
          is_private : String,
          parent_id  : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### ✨ New Opportunity

![Select New Opportunity Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.13.32-pm.png)

{% hint style="success" %}
Your script will run when a new opportunity is created.
{% endhint %}

#### 📤Outputs

```graphql
Opportunity = {  
                 id          : String,
                 is_private  : String,
                 name        : String,
                 close_date  : Date,
                 stage       : String,
                 account_id  : String,
                 type        : String,
                 lead_source : String,
                 amount      : Number,
                 next_step   : String,
                 probability : Number,
                 campaign_id : String,
                 description : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### 📋 New Task

![Select New Task Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.16.50-pm.png)

{% hint style="success" %}
Your script will run when a new task is created.
{% endhint %}

#### 📤Outputs

```graphql
Task = {  
          id          : String,
          subject     : String,
          due_date    : Date,
          priority    : String,
          status      : String,
          name_id     : String,
          related_to  : String,
          description : String
}
```

* JSON Data
  * Raw JSON data received from the API

## ![](../../.gitbook/assets/salesforce.png) Object Updated

![Select Object Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.19.46-pm.png)

{% hint style="success" %}
Your script will run when a Salesforce object is updated.
{% endhint %}

### 📈 Campaign Updated

![Select Campaign Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.21.16-pm.png)

{% hint style="success" %}
Your script will run when a campaign is updated.
{% endhint %}

#### 📤Outputs

```graphql
Campaign = {
             id                : String,
             name              : String,
             active            : String,
             type              : String,
             status            : String,
             start_date        : Date,
             end_date          : Date,
             expected_rev      : Number,
             budgeted_cost     : Number,
             actual_cost       : Number,
             expected_response : Number,
             num_sent          : Number,
             parent_id         : String,
             description       : String
}
```

* JSON Data
  * Raw JSON data received from the API

### 💼 Case Updated

![Select Case Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.23.43-pm.png)

{% hint style="success" %}
Your script will run when a case is updated.
{% endhint %}

#### 📤Outputs

```graphql
Case = { 
         id          : String,
         subject     : String,
         status      : String,
         origin      : String,
         contact     : String,
         account_id  : String,
         type        : String,
         reason      : String,
         priority    : String,
         web_email   : String,
         web_name    : String,
         web_company : String,
         web_phone   : String,
         description : String
}
```

* JSON Data
  * Raw JSON data received from the API

### 🕵 Lead Updated

![Select Lead Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.25.06-pm.png)

{% hint style="success" %}
Your script will run when a lead is updated.
{% endhint %}

#### 📤Outputs

```graphql
Lead = {  
          id          : String,
          name        : String,
          salutation  : String,
          status      : String,
          company     : String,
          title       : String,
          source      : String,
          industry    : String,
          annual_rev  : Number,
          phone       : String,
          mobile      : String,
          fax         : String,
          email       : String,
          website     : String,
          rating      : String,
          employees   : Int,
          street      : String,
          city        : String,
          state       : String,
          zip         : String,
          country     : String,
          description : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### ✨ Opportunity Updated

![Select Opportunity Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.26.14-pm.png)

{% hint style="success" %}
Your script will run when an opportunity is updated.
{% endhint %}

#### 📤Outputs

```graphql
Opportunity = {  
                 id          : String,
                 is_private  : String,
                 name        : String,
                 close_date  : Date,
                 stage       : String,
                 account_id  : String,
                 type        : String,
                 lead_source : String,
                 amount      : Number,
                 next_step   : String,
                 probability : Number,
                 campaign_id : String,
                 description : String 
}
```

* JSON Data
  * Raw JSON data received from the API

### 📋 Task Updated

![Select Task Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.27.34-pm.png)

{% hint style="success" %}
Your script will run when a task is updated.
{% endhint %}

#### 📤Outputs

```graphql
Task = {  
          id          : String,
          subject     : String,
          due_date    : Date,
          priority    : String,
          status      : String,
          name_id     : String,
          related_to  : String,
          description : String
}
```

* JSON Data
  * Raw JSON data received from the API


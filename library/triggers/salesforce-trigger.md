# Salesforce Trigger

![Run a program when a Salesforce object is created or updated.](../../.gitbook/assets/salesforce.png)

{% hint style="info" %}
To create, edit, and query Salesforce objects, use the [Salesforce Module](../modules/salesforce.md).
{% endhint %}

## ⚙ Setup

### 🔗 Link Your Salesforce Account

When you drag in a Salesforce Trigger for the first time, follow the prompt to authorize access.

### 🔑 API Access

First make sure you have API access enabled in Salesforce. To do this, follow [these instructions](https://ebstalimited.zendesk.com/hc/en-us/articles/229295368-How-do-I-enable-API-access-in-Salesforce).

## ![](../../.gitbook/assets/salesforce.png) New Object Created

![Select New Object Created Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.44.24-am.png)

Run the program whenever a new Salesforce object is created.

### 🌟 New Account

![Select New Account Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.46.22-am.png)

{% hint style="success" %}
Program will run when a new account is created.
{% endhint %}

#### 📤 Outputs

* Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Account Name
* Account Parent ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Account Number
* Account Site
* Account Type
* Account Industry
* Account Annual Revenue
* Account Rating
* Account Phone
* Account Fax
* Account Website
* Account Ticker Symbol
* Account Ownership
* Account Employees
* Account SIC Code
* Account Billing Street
* Account Billing City
* Account Billing State
* Account Billing Zipcode
* Account Billing Country
* Account Shipping Street
* Account Shipping City
* Account Shipping State
* Account Shipping Zipcode
* Account Shipping Country
* Account Description
* JSON Data
  * Raw JSON data received from the API

### 📈 New Campaign

![Select New Campaign Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.52.40-am.png)

{% hint style="success" %}
Program will run when a new campaign is created.
{% endhint %}

#### 📤 Outputs

* Campaign ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Campaign Name
* Campaign Active
  * Indicates whether the campaign is currently active \(True/False\)
* Campaign Type
* Campaign Status
* Campaign Start Date
* Campaign End Date
* Campaign Expected Revenue
* Campaign Budgeted Cost
* Campaign Actual Cost
* Campaign Expected Response
* Campaign Num Sent
* Campaign Parent ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Campaign Description
* JSON Data
  * Raw JSON data received from the API.

### 💼 New Case

![Select New Case Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.56.22-am.png)

{% hint style="success" %}
Program will run when a new case is created.
{% endhint %}

#### 📤 Outputs

* Case ID
  *  Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Subject
* Case Status
* Case Origin
* Case Contact ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Type
* Case Reason
* Case Priority
* Case Web Email
* Case Web Name
* Case Web Company
* Case Web Phone
* Case Description
* JSON Data
  * Raw JSON data received from the API.

### 👤 New Contact

![Select New Contact Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-11.59.47-am.png)

{% hint style="success" %}
Program will run when a new contact is created.
{% endhint %}

#### 📤 Outputs

* Contact ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Contact Name
* Contact Salutation
* Contact Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Contact Title
* Contact Department
* Contact Birthdate
* Contact Reports To ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Contact Lead Source
* Contact Phone
* Contact Home Phone
* Contact Mobile
* Contact Other Phone
* Contact Fax
* Contact Email
* Contact Assistant Name
* Contact Assistant Phone
* Contact Mailing Street
* Contact Mailing City
* Contact Mailing State
* Contact Mailing Zipcode
* Contact Mailing Country
* Contact Other Street
* Contact Other City
* Contact Other State
* Contact Other Zipcode
* Contact Other Country
* Contact Description
* JSON Data
  * Raw JSON data received from the API.

### 🗓 New Event

![Select New Event Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.05.45-pm.png)

{% hint style="success" %}
Program will run when a new event is created.
{% endhint %}

#### 📤 Outputs

* Event ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Event Subject
* Event All Day
* Event Start Date/Time
* Event End Date/Time
* Event Location
* Event Name ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Event Related To ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Event Description
* JSON Data
  * Raw JSON data received from the API.

### 🕵 New Lead

![Select New Lead Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.08.33-pm.png)

{% hint style="success" %}
Program will run when a new lead is created.
{% endhint %}

#### 📤 Outputs

* Lead ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Lead Name
* Lead Salutation
* Lead Status
* Lead Company
* Lead Title
* Lead Source
* Lead Industry
* Lead Annual Revenue
* Lead Phone
* Lead Mobile
* Lead Fax
* Lead Email
* Lead Website
* Lead Rating
* Lead No. of Employees
* Lead Street
* Lead City
* Lead State
* Lead Zipcode
* Lead Country
* Lead Description
* JSON Data
  * Raw JSON data received from the API.

### 🗒 New Note

![Select New Note Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.11.28-pm.png)

{% hint style="success" %}
Program will run when a new note is created.
{% endhint %}

#### 📤 Outputs

* Note ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Note Title
* Note Body
* Note Private
* Note Parent ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* JSON Data
  * Raw JSON data received from the API.

### ✨ New Opportunity

![Select New Opportunity Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.13.32-pm.png)

{% hint style="success" %}
Program will run when a new opportunity is created.
{% endhint %}

#### 📤 Outputs

* Opportunity ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Private
* Opportunity Name
* Opportunity Close Date
* Opportunity Stage
* Opportunity Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Type
* Opportunity Lead Source
* Opportunity Amount
* Opportunity Next Step
* Opportunity Probability
* Opportunity Campaign ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Description
* JSON Data
  * Raw JSON data received from the API.

### 📋 New Task

![Select New Task Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.16.50-pm.png)

{% hint style="success" %}
Program will run when a new task is created.
{% endhint %}

#### 📤 Outputs

* Task ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Subject
* Task Due Date
* Task Priority
* Task Status
* Task Name ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Related To ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Description
* JSON Data
  * Raw JSON data received from the API.

## ![](../../.gitbook/assets/salesforce.png) Object Updated

![Select Object Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.19.46-pm.png)

Run the program whenever a Salesforce object is updated.

### 📈 Campaign Updated

![Select Campaign Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.21.16-pm.png)

{% hint style="success" %}
Program will run when a campaign is updated.
{% endhint %}

#### 📤 Outputs

* Campaign ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Campaign Name
* Campaign Active
  * Indicates whether the campaign is currently active \(True/False\)
* Campaign Type
* Campaign Status
* Campaign Start Date
* Campaign End Date
* Campaign Expected Revenue
* Campaign Budgeted Cost
* Campaign Actual Cost
* Campaign Expected Response
* Campaign Num Sent
* Campaign Parent ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Campaign Description
* JSON Data
  * Raw JSON data received from the API.

### 💼 Case Updated

![Select Case Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.23.43-pm.png)

{% hint style="success" %}
Program will run when a case is updated.
{% endhint %}

#### 📤 Outputs

* Case ID
  *  Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Subject
* Case Status
* Case Origin
* Case Contact ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Case Type
* Case Reason
* Case Priority
* Case Web Email
* Case Web Name
* Case Web Company
* Case Web Phone
* Case Description
* JSON Data
  * Raw JSON data received from the API.

### 🕵 Lead Updated

![Select Lead Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.25.06-pm.png)

{% hint style="success" %}
Program will run when a lead is updated.
{% endhint %}

#### 📤 Outputs

* Lead ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Lead Name
* Lead Salutation
* Lead Status
* Lead Company
* Lead Title
* Lead Source
* Lead Industry
* Lead Annual Revenue
* Lead Phone
* Lead Mobile
* Lead Fax
* Lead Email
* Lead Website
* Lead Rating
* Lead No. of Employees
* Lead Street
* Lead City
* Lead State
* Lead Zipcode
* Lead Country
* Lead Description
* JSON Data
  * Raw JSON data received from the API.

### ✨ Opportunity Updated

![Select Opportunity Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.26.14-pm.png)

{% hint style="success" %}
Program will run when an opportunity is updated.
{% endhint %}

#### 📤 Outputs

* Opportunity ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Private
* Opportunity Name
* Opportunity Close Date
* Opportunity Stage
* Opportunity Account ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Type
* Opportunity Lead Source
* Opportunity Amount
* Opportunity Next Step
* Opportunity Probability
* Opportunity Campaign ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Opportunity Description
* JSON Data
  * Raw JSON data received from the API.

### 📋 Task Updated

![Select Task Updated Mode](../../.gitbook/assets/screen-shot-2019-07-23-at-12.27.34-pm.png)

{% hint style="success" %}
Program will run when a task is updated.
{% endhint %}

#### 📤 Outputs

* Task ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Subject
* Task Due Date
* Task Priority
* Task Status
* Task Name ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Related To ID
  * Click [here](../modules/salesforce.md#object-ids) for more information about object IDs.
* Task Description
* JSON Data
  * Raw JSON data received from the API.


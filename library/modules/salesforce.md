---
description: >-
  Seamlessly integrate Salesforce with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Salesforce

![Create, edit, and query Salesforce objects.](../../.gitbook/assets/salesforce.png)

{% hint style="info" %}
To run your script when a Salesforce object is created or updated, use the [Salesforce Trigger](../triggers/salesforce-trigger.md).
{% endhint %}

## ⚙ Setup

### 🔑 API Access

First make sure you have API access enabled in Salesforce. To do this, follow [these instructions](https://ebstalimited.zendesk.com/hc/en-us/articles/229295368-How-do-I-enable-API-access-in-Salesforce).

### 💡 Object IDs

Many of the modes of the Salesforce module utilize object IDs. This is how the API identifies the Salesforce objects. These IDs can be found in the url when viewing the object.

For Salesforce classic the ID will be at the end of the url. In the following example url, **0014P000025KpT7** is the object ID:                                                                               [https://na132.salesforce.com/0014P000025KpT7](https://na132.salesforce.com/0014P000025KpT7)

For Salesforce Lighting Experience, the ID is the second to last section of the url. In the following example url, **7014P000000vMXUQA2** is the object ID: [https://na132.lightning.force.com/lightning/r/Campaign/7014P000000vMXUQA2/view](https://na132.lightning.force.com/lightning/r/Campaign/7014P000000vMXUQA2/view)

## ![](../../.gitbook/assets/salesforce.png) New Object

![Select New Object Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-12.56.47-pm.png)

### 🌟 Create New Account

![Select Create New Account](../../.gitbook/assets/screen-shot-2019-07-16-at-12.57.13-pm.png)

#### 📥 Inputs

* **Account Name** 
  * Required
* **Parent Account ID**
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Account Number**
* **Account Site**
* **Type**
* **Industry**
* **Annual Revenue**
* **Phone Number**
* **Fax**
* **Website**
* **Rating**
* **Ticker Symbol**
* **Ownership**
* **Employees**
* **SIC Code**
* **Billing Address**
  * Separated by Street, City, State, Zip, and Country fields
* **Shipping Address**
  * Separated by Street, City, State, Zip, and Country fields
* **Description**

#### 📤 Outputs

* **New Account ID**
  * After successfully running the program and creating a new account, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 📈 Create New Campaign

![Select Create New Campaign](../../.gitbook/assets/screen-shot-2019-07-16-at-1.02.40-pm.png)

#### 📥 Inputs

* **Campaign Name**
  * Required
* **Active**
  * Check the box if you wish the new campaign to be marked as active.
* **Type**
* **Status**
* **Start Date**
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **End Date**
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **Expected Revenue**
* **Budgeted Cost**
* **Actual Cost**
* **Expected Response**
* **Number Sent in Campaign**
* **Parent Campaign ID**
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Description**

#### 📤 Outputs

* **New Campaign ID**
  * After successfully running the program and creating a new campaign, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 💼 Create New Case

![Select Create New Case](../../.gitbook/assets/screen-shot-2019-07-16-at-1.03.24-pm.png)

#### 📥 Inputs

* **Subject**
* **Status**
* **Case Origin**
* **Contact ID**
  * ID of the associated contact.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Account ID**
  * ID of the associated account.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Type**
* **Case Reason**
* **Priority**
* **Web Email**
* **Web Name**
* **Web Company**
* **Web Phone**
* **Description**

#### 📤 Outputs

* **New Case ID**
  * After successfully running the program and creating a new case, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 💬 Create New Case Comment

![Select Create New Case Comment](../../.gitbook/assets/screen-shot-2019-07-16-at-1.03.36-pm.png)

#### 📥 Inputs

* **Body**
  * Required
* **Published**
  * Check the box if you wish the new case comment to be visible to customers in the Self-Service portal.
* **Parent ID**
  * Required
  * The ID of the case that the comment is being added to.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

#### 📤 Outputs

* **New Case Comment ID**
  * After successfully running the program and creating a new case comment, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 👤 Create New Contact

![Select Create New Contact](../../.gitbook/assets/screen-shot-2019-07-16-at-1.03.46-pm.png)

#### 📥 Inputs

* **Salutation**
* **First Name**
* **Last Name**
  * Required
* **Account ID**
  * ID of the account that is the parent of this contact.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Title**
* **Department**
* **Birthdate**
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **Reports To \(ID\)**
  * The ID of who this contact reports to.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Lead Source**
* **Phone Number**
* **Home Phone**
* **Mobile**
* **Other Phone**
* **Fax**
* **Email**
* **Assistant**
  * The name of the assistant.
* **Asst. Phone**
  * The phone number of the assistant.
* **Mailing Address**
  * Separated by Street, City, State, Zip, and Country fields
* **Other Address**
  * Separated by Street, City, State, Zip, and Country fields
* **Description**

#### 📤 Outputs

* **New Contact ID**
  * After successfully running the program and creating a new contact, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 🗓 Create New Event

![Select Create New Event](../../.gitbook/assets/screen-shot-2019-07-16-at-1.03.55-pm.png)

#### 📥 Inputs

* **Subject**
  * Required
* **All-Day Event**
  * Check this box if the event takes all day \(can span multiple days as well\)
* **Start Date**
  * Required
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **Start Time**
  * This is only visible if **All-Day Event** is unchecked.
  * This is in your local time.
* **End Date**
  * Required
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
  * If **All-Day Event** is checked, setting this to the same day as the start will create an event lasting that whole day. If **End Date** is set to the next day, a two-day event will be created.
* **End Time**
  * This is only visible if All-Day Event is unchecked.
  * This is in your local time.
* **Location**
* **Name ID**
  * The ID of a human object, such as a contact or lead that is involved with the event.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Related To ID**
  * The ID of a non-human object, such as an opportunity or campaign that this event is related to.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Description**

#### 📤 Outputs

* **New Event ID**
  * After successfully running the program and creating a new event, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 🕵 Create New Lead

![Select Create New Lead](../../.gitbook/assets/screen-shot-2019-07-16-at-1.04.08-pm.png)

#### 📥 Inputs

* **Salutation**
* **First Name**
* **Last Name**
  * Required
* **Company**
  * Required
* **Lead Status**
* **Title**
* **Lead Source**
* **Industry**
* **Annual Revenue**
* **Phone Number**
* **Mobile**
* **Fax**
* **Email**
* **Website**
* **Rating**
* **No. of Employees**
* **Address**
  * Separated by Street, City, State, Zip, and Country fields
* **Description**

#### 📤 Outputs

* **New Lead ID**
  * After successfully running the program and creating a new lead, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 🗒 Create New Note

![Select Create New Note](../../.gitbook/assets/screen-shot-2019-07-16-at-1.04.17-pm.png)

#### 📥 Inputs

* **Parent ID**
  * Required
  * The ID of the object this note will be attached to.
  * Can only be an account, contact, lead, or opportunity.
* **Title**
  * Required
* **Body**
* **Private**
  * Check this box if you want to be the only one who can see this note.

#### 📤 Outputs

* **New Note ID**
  * After successfully running the program and creating a new note, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### ✨ Create New Opportunity

![Select Create New Opportunity](../../.gitbook/assets/screen-shot-2019-07-16-at-1.04.29-pm.png)

#### 📥 Inputs

* **Private**
  * Check this box if you want the new opportunity to be private.
* **Opportunity Name**
  * Required
* **Close Date**
  * Required
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **Stage**
* **Account ID**
  * ID of the associated account.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Type**
* **Lead Source**
* **Amount**
* **Next Step**
* **Probability \(%\)**
* **Primary Campaign Source ID**
  * ID of the primary campaign source.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Description**

#### 📤 Outputs

* **New Opportunity ID**
  * After successfully running the program and creating a new opportunity, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 📋 Create New Task

![Select Create New Task](../../.gitbook/assets/screen-shot-2019-07-16-at-1.04.43-pm.png)

#### 📥 Inputs

* **Subject**
  * Required
* **Due Date**
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* **Priority**
* **Status**
* **Name ID**
  * The ID of a human object, such as a contact or lead that is involved with the event.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Related To \(ID\)**
  * The ID of a non-human object, such as an opportunity or campaign that this event is related to.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Description**

#### 📤 Outputs

* **New Task ID**
  * After successfully running the program and creating a new task, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

### 👥 Add New Campaign Member

![Select Add New Campaign Member](../../.gitbook/assets/screen-shot-2019-07-16-at-1.04.55-pm.png)

![Select Campaign Member Type](../../.gitbook/assets/screen-shot-2019-07-16-at-1.09.51-pm.png)

#### 📥 Inputs

* **Campaign ID**
  * The ID of the campaign you are adding a member to.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Member Lead/Contact ID**
  * The ID of the lead/contact \(depending on which type you selected earlier\) you are adding to the campaign.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* **Member Status**

#### 📤 Outputs

* **New Campaign Member ID**
  * After successfully running the program and adding a new campaign member, this output will be the corresponding object ID.
  * Click [here](salesforce.md#object-ids) for more information about object IDs.

## ❔ Query

![Select Query Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.15.41-pm.png)

### 🔎 Interacting With Query Results

After executing a successful query, you will see something like this under **Outputs**.

![](../../.gitbook/assets/screen-shot-2019-07-16-at-3.38.40-pm.png)

To make a column into a variable, simply assign the column a name. The resulting variable will look like this:

![](../../.gitbook/assets/screen-shot-2019-07-16-at-3.37.31-pm.png)

If you wish to view the raw JSON returned from the query, simply select the **JSON Data** checkbox under **Outputs**.

### ✂ Custom Query

![Select Custom Query Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.21.53-pm.png)

Write the query code in the code box, using Salesforce's SOQL querying language.

{% hint style="info" %}
See [https://developer.salesforce.com/docs/atlas.en-us.soql\_sosl.meta/soql\_sosl/sforce\_api\_calls\_soql.htm](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm) for more details.
{% endhint %}

Example:

```sql
SELECT id, name
FROM Account
WHERE name = 'Example Account'
LIMIT 1
```

Click the run button to execute the query.

[Interacting with query results.](salesforce.md#interacting-with-query-results)

### 👤 Query Accounts

![Select Query Accounts Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.22.10-pm.png)

#### ☑ Select Fields to be Returned

* Account ID
* Account Name
* Account Number
* Account Phone

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Accounts
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Accounts
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Account Name
* Type
* Industry
* Rating

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png)Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 📈 Query Campaigns

![Select Query Campaigns Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.22.27-pm.png)

#### ☑ Select Fields to be Returned

* Campaign ID
* Campaign Name
* Campaign Active?
* Campaign Type
* Campaign Status
* Campaign Start Date
* Campaign End Date

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Campaigns
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Campaigns
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Campaign Name
* Active
* Type
* Status

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 💼 Query Cases

![Select Query Cases Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.22.43-pm.png)

#### ☑ Select Fields to be Returned

* Case ID
* Case Subject
* Case Number
* Case Status

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Cases
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Cases
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Case Subject
* Type
* Case Reason
* Status
* Priority

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 👥 Query Contacts

![Select Query Contacts Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.22.55-pm.png)

#### ☑ Select Fields to be Returned

* Contact ID
* Contact Name
* Contact Phone Number
* Contact Email

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Contacts
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Contacts
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Contact Name
* Department

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 🗓 Query Events

![Select Query Events Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.23.04-pm.png)

#### ☑ Select Fields to be Returned

* Event ID
* Event Subject
* Event Location
* Event Start Date/Time
* Event End Date/Time

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Events
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Events
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Subject
* Location
* Activity Date
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 🕵 Query Leads

![Select Query Leads Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.23.16-pm.png)

#### ☑ Select Fields to be Returned

* Lead ID
* Lead Name
* Lead Company
* Lead Status
* Lead Phone
* Lead Email

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Leads
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Leads
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Lead Name
* Company
* Lead Status
* Rating

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### ✨ Query Opportunities

![Select Query Opportunities Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.23.29-pm.png)

#### ☑ Select Fields to be Returned

* Opportunity ID
* Opportunity Name
* Opportunity Type
* Opportunity Close Date
* Opportunity Stage

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Opportunities
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Opportunities
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Opportunity Name
* Private
* Type
* Lead Source
* Stage

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

### 📋 Query Tasks

![Select Query Tasks Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-3.23.45-pm.png)

#### ☑ Select Fields to be Returned

* Task ID
* Task Subject
* Task Due Date
* Task Priority
* Task Status

These represent the columns of results from a successful query.

#### 📥 Inputs

{% hint style="success" %}
Query All Tasks
{% endhint %}

If selected, the query will not filter its results.

{% hint style="warning" %}
Query All Tasks
{% endhint %}

If unselected, there will be options to filter results by any of the following fields.

* ID
  * Click [here](salesforce.md#object-ids) for more information about object IDs.
* Subject
* Due Date
  * Must be of the format YYYY-MM-DD
  * Example: 2020-07-04
* Priority
* Status

This will return results that match any fields with inputted values.

**Limit** - Optional limit on the number of rows to be returned.

![](../../.gitbook/assets/query_button.png) Click the **Query** button to execute the query.

{% hint style="info" %}
If you wish to create more customizable queries, try the [custom query mode](salesforce.md#custom-query).
{% endhint %}

## ✏ Update Existing Object

![Select Update Existing Object Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.31.02-pm.png)

### 👤 Update Account

![Select Update Account Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.33.30-pm.png)

#### Account ID

Enter the ID of the account you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new account](salesforce.md#create-new-account).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}

### 📈 Update Campaign

![Select Update Campaign Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.33.42-pm.png)

#### Campaign ID

Enter the ID of the campaign you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new campaign](salesforce.md#create-new-campaign).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}

### 💼 Update Case

![Select Update Case Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.33.56-pm.png)

#### Case ID

Enter the ID of the case you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new case](salesforce.md#create-new-case).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}

### 👥 Update Contact

![Select Update Contact Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.34.06-pm.png)

#### Contact ID

Enter the ID of the contact you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new contact](salesforce.md#create-new-contact).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}

### 🕵♀ Update Lead

![Select Update Lead Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.34.22-pm.png)

#### Lead ID

Enter the ID of the lead you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new lead](salesforce.md#create-new-lead).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}

### ✨ Update Opportunity

![Select Update Opportunity Mode](../../.gitbook/assets/screen-shot-2019-07-16-at-4.34.36-pm.png)

#### Opportunity ID

Enter the ID of the opportunity you want to edit. Click [here](salesforce.md#object-ids) for more information about object IDs.

If the ID is valid, all the fields will be displayed with the current values. Then you can edit any field the same way you would for [creating a new opportunity](salesforce.md#create-new-opportunity).

{% hint style="info" %}
You must run the program for the changes to be committed.
{% endhint %}


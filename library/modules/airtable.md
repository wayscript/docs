# Airtable

![Airtable works like a spreadsheet, but gives you the power of a database to organize anything.](../../.gitbook/assets/airtable.png)

## ![](../../.gitbook/assets/airtable.png) Functionality

With the Airtable module you can:

* Read Table Data into WayScript
* Delete Table Rows
* Create New Table Rows

## ⚙Setting Up Your Airtable Account

### 1. Drag the Airtable module into your WayScript program

![](../../.gitbook/assets/airtable_flow.png)

### 2. **In the Airtable Module, select "Add an Account" in the "Select an API Key" input**

![](../../.gitbook/assets/add_an_account.png)

### **3. A form will pop-up that allows you to connect your Airtable account**

Follow the instructions below for setting up each of these form inputs.

![](../../.gitbook/assets/modal.png)

### 4. Navigate to the [**Airtable API page**](https://airtable.com/api)\*\*\*\*

![https://airtable.com/api](../../.gitbook/assets/api_landing_page.png)

### **5. Select the "base" you want to automate with WayScript**

In this example, we are using the "Event Marketing" base. Click on the base.

![](../../.gitbook/assets/event_marketing.png)

### **6. Add the name of the base to the "Workspace Name" field of the WayScript form**

![](../../.gitbook/assets/table_name_input.png)

### 7. **On the base API page, select "AUTHENTICATION" on the left navigation bar**

![](../../.gitbook/assets/authentication.png)

### **8. On the right side of the page, this highlighted key is your Base Key. Copy this key**

![](../../.gitbook/assets/base_key_highlight.png)

### **9. Paste the Base Key into the corresponding field of the WayScript form**

![](../../.gitbook/assets/base_key_input.png)

### 10. Go to your [Airtable account page](https://airtable.com/account)

![https://airtable.com/account](../../.gitbook/assets/account.png)

### 11. **Double Click on and copy your API Key**

![](../../.gitbook/assets/api_key.png)

### **12. Paste the API Key into the corresponding field of the WayScript form**

![](../../.gitbook/assets/api_key_input.png)

### **13. Press the submit button on the form and you're ready to get started!**

![](../../.gitbook/assets/submitted.png)

## 💼Working with a Table

Choose the table you want to work with in the "Table Name" input. \(In this case, the "Events" table.\)

![](../../.gitbook/assets/events.png)

![](../../.gitbook/assets/table_input.png)

### 🔎 Select an Operation

Choose whether you would like to **Get Records**, **Delete Rows**, or **Create a New Record**.

![What would you like to do?](../../.gitbook/assets/screen-shot-2019-07-15-at-7.55.25-pm.png)

### 🗃Get Records

The "Get Records" option allows you to retrieve data from a table.

You can choose whether you want to retrieve **All Rows**, rows that match a **Filter**, or a **Single Row**.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-7.55.46-pm.png)

#### Filter Results

If you choose the "Filter" or "Single Row" option, you will need to define the filter you want to match on.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-7.55.59-pm.png)

#### Matching Rows

All rows matching your settings above will display in the "Inputs" section.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-8.10.10-pm.png)

{% hint style="info" %}
Click the "Refresh" button for the most up-to-date results.
{% endhint %}

### ❌Delete Rows

The "Delete Rows" option works much in the same way as the "Get Records" option, but deletes any matching records instead of retrieving them.

### 🌟Create a New Record

You also have the option to Create a New Record. 

If you choose this option, you can either:

* Build the data you would like to create using WayScript
* Input raw JSON

#### Build Data

If you opt to build Data yourself, you will need to define each of the fields you wish to input into the table.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-8.08.59-pm.png)

#### Raw JSON

If you opt to input raw JSON, you will need to select the WayScript variable that contains that JSON.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-8.13.08-pm.png)

## 📤 Outputs

Each column of your table will be available to select as an output from the Airtable module.


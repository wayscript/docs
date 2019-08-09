# Google Sheets Trigger

![Run your program when a Google Sheet changes.](../../.gitbook/assets/google_sheets.png)

{% hint style="info" %}
To read and write to Google Sheets, use the [Google Sheets module](../modules/google-sheets.md).
{% endhint %}

## 🔗 Link Your Google Account

In order to use the Google Sheets Trigger, you must first link your Google account.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-11.11.36-am.png)

{% hint style="info" %}
You can add additional accounts from the Google Sheets Trigger settings.
{% endhint %}

## ⚙ Settings

### ⚡ Choose a Trigger

Select what type of change to a Google Sheet will trigger your program:

* A new row is added to a worksheet
* A row is updated or a new row is added to a worksheet
* A new worksheet is added to a spreadsheet

![](../../.gitbook/assets/screen-shot-2019-07-15-at-11.23.05-am.png)

### ![](../../.gitbook/assets/google_sheets.png) Choose a Spreadsheet/Worksheet

Depending on what type of Google Sheets change you selected in the step above, you will need to choose a Spreadsheet and Worksheet.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-11.27.31-am.png)

{% hint style="info" %}
If you do not see the spreadsheet you are looking for, click the refresh button.
{% endhint %}

## 📤 Outputs

If your selected change involves a row being added or updated, you will have the changed row's data available as an output.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-11.12.32-am.png)

Depending on the option you select, you may have the Spreadsheet or Worksheet Name available as an output.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-11.12.49-am.png)

#### Default Values

* **Row Data** - While building with the Google Sheets trigger, you are going to want sample data to work with. To do this, you can make a change in your google sheet that triggers the event. Alternatively, you can enter comma separated values into your default value. These values will represent the row data brought into your program. These values will be overwritten with real data when the program triggers. 
* **Spreadsheet Name -** The name of the spreadsheet you are using

![](../../.gitbook/assets/row_data_trigger.png)

#### **Columns**

If you are triggering your program based on a row being updated or a new row being added, each of you columns will appear as a unique variable. If you update your spreadsheet, just press the refresh button next to your Worksheet and the columns will update. 

![You can import the values of each column as variables](../../.gitbook/assets/gs_trigger_cols.png)


---
description: Work with Google Sheets
---

# Google Sheets

## Link Your Google Account

In order to use the Google Sheets module, you must first link your Google account.

![](../.gitbook/assets/screen-shot-2019-07-15-at-11.35.20-am.png)

## Read Files

When the Google Sheets module is activated, the default setting is to read a file.

Reading files allows you to import columns into WayScript as variables.

### Choose File to Read

![](../.gitbook/assets/screen-shot-2019-07-15-at-11.57.31-am.png)

{% hint style="info" %}
If you do not see the Google Sheet you are looking for, click the refresh button.
{% endhint %}

### Importing Columns as Variables

Once a spreadsheet is selected, the spreadsheet will populate on the page.

* The **Choose Worksheet to Read** selector can be used to pull in data from different tabs on a spreadsheet.
* The **Ignore Headers** checkbox can be used to prevent WayScript from pulling in column headers if they exist in the file.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.03.49-pm.png)

{% hint style="info" %}
In order to import a column as a variable, the column must be labelled. Once labelled, the column will appear under variables.
{% endhint %}

## Write Files

### Choose File to Write

Pick the Google Sheet you want your WayScript program to write to.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.08.45-pm.png)

{% hint style="info" %}
If you do not see the Google Sheet you are looking for, click the refresh button.
{% endhint %}

### Choose a Worksheet

Select the Worksheet you would like to write.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.13.10-pm.png)

### Include Headers

If "Include Headers" is selected, data headers will be written to your Google Sheet.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.14.36-pm.png)

### Write Mode

* **Add To File:** Every time the program runs, new rows of data will be added to the bottom of the spreadsheet.
* **Replace File:** Every time the program runs, the file will be wiped clean before it is written.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.14.40-pm.png)

### Ignore Duplicates

The Google Sheets module allows you to ignore duplicates. If the same data already exists as a row in the spreadsheet, it will not be written to the file again.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.20.51-pm.png)

#### Ignore All Columns

If the entire row is equal to another entire row in the spreadsheet, it will not write the row again. 

#### Ignore a Specific Column

If the selected column already contains the value about to be written to that row, the row will not be written.

### Add Your Variables

You need to assign values to columns by pressing the **+** button under "Add Your Variables."

The values of these variables will be written to your Google Sheets spreadsheet when your program runs.

You can add as many columns as you like.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.14.52-pm.png)

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.28.51-pm.png)

### Fire Notification

By default, changes WayScript makes to your Google Sheets do not fire notifications. This is to prevent your program from triggering another program with a [Google Sheets Trigger](../triggers/google-sheets-trigger.md).

If you want your changes to fire a notification, enable this setting.

![](../.gitbook/assets/screen-shot-2019-07-15-at-12.09.29-pm.png)

### Writing a List Variable to a Spreadsheet Column

{% hint style="info" %}
To learn how to write each item of a list variable to a separate cell in a single column of your spreadsheet, see [Protip: Writing Lists to Spreadsheets](https://wayscript.com/blog_entry/38).
{% endhint %}


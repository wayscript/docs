---
description: >-
  Seamlessly integrate Dropbox with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Dropbox

![Work with Dropbox.](../../.gitbook/assets/dropbox.png)

## 🗝 Authorization

When you first drag in the Dropbox module, you will be asked to authenticate Dropbox with your WayScript account. Follow the prompts on the Dropbox site and authorize WayScript to access your Dropbox files.

## ![](../../.gitbook/assets/dropbox.png) Select an Account

You can connect multiple Dropbox accounts to WayScript. Select the one you would like to use.

![Select the Dropbox account you want to use.](../../.gitbook/assets/select_an_account_dropbox%20%281%29%20%281%29%20%282%29%20%282%29%20%281%29.png)

## 📖 Read File from Dropbox

### 📁 Choose the File Type to Read

WayScript currently supports reading the following file types from Dropbox:

* [Word Documents](word.md) \(.docx\)
* [Excel Spreadsheets](excel.md) \(.xlsx\)
* [CSV Files](csv.md) \(.csv\)

![Choose the File Type to Read](../../.gitbook/assets/choose_file_type.png)

### 👓 Choose a File Path to Read

Once you have selected a file type, select the path of the file you want to read.

![Choose a File Path to Read](../../.gitbook/assets/choose_a_file_path.png)

### 📤 Outputs

#### ![](../../.gitbook/assets/word.png) Word

When you select a Word document, the following output is available:

```graphql
Doc = {
         paragraphs : [ String ],  
         full_text  : String, 
         words      : [ String ]
}
```

#### ![](../../.gitbook/assets/excel_128x128.png) Excel or CSV

When you select an Excel or CSV file, you will see a preview of the contents in the Outputs section. Assign a name to each column whose contents you would like exported as a List.

![Labeling the second column &quot;Data&quot; creates a List output called &quot;Data&quot; with the contents of that column.](../../.gitbook/assets/screen-shot-2019-07-17-at-9.09.19-am.png)

## ✍ Write File to Dropbox

This mode allows you to upload a [file you have stored in WayScript](../../account-management/managing-your-files.md) to Dropbox.

### ⬆ Choose File to Upload to Dropbox

You will start by selecting one of your files to upload to Dropbox. Alternatively, you can upload a new file to WayScript.

![Select a file to upload to Dropbox](../../.gitbook/assets/choose_file_to_upload.png)

### 📂 Provide a File Path and File Name

Once you have selected the file you wish to upload, provide the path in your Dropbox where you would like the file uploaded, as well as the name for the file.

{% hint style="info" %}
The default file path is the root folder of your Dropbox and the default file name is the name of the file you selected to upload.
{% endhint %}

![Optionally provide a Dropbox file path and name](../../.gitbook/assets/screen-shot-2019-07-17-at-9.14.50-am.png)


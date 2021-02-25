---
description: >-
  Seamlessly integrate Microsoft Word with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Word

![Work with Microsoft Word. Read file data, and build Word documents.](../../.gitbook/assets/word_128x128.png)

## 📖 Read File

### 📂 Choose File To Read

![Select a Word Document](../../.gitbook/assets/screenshot-2019-07-16-17.04.18.png)

You can upload a Word document to WayScript or select a document you have already uploaded.

### 📤 Outputs

```graphql
Doc = {
         paragraphs : [ String ], 
         full_text  : String, 
         words      : [ String ]
}
```

## ✍ Write File

### 🌟 Create a File

Under Settings &gt; Choose File to Write, select 'Create New File'

![Create New File](../../.gitbook/assets/screenshot-2019-07-16-17.13.06.png)

In the modal, create a name for your file.

![](../../.gitbook/assets/screenshot-2019-07-16-17.14.38.png)

### 🖋 Write Mode

* **Add to File** - This mode will add any new contents as a new paragraph below any data already in the word document. 
* **Overwrite File** - This mode will overwrite your old document with the new information.

{% hint style="warning" %}
Be careful with **Overwrite File** - this will delete all content in your word document and cannot be undone.
{% endhint %}

### ➕ Add Contents

You can include variables in your text document.

![](../../.gitbook/assets/screenshot-2019-07-16-17.16.32.png)

### ⬇ Download Document

When your program runs, you can download your Word document directly from the log.

![Download Button in Log](../../.gitbook/assets/screenshot-2019-07-16-17.17.41.png)

{% hint style="info" %}
You can manage and download files anytime from your [file manager](https://wayscript.com/file_manager). For more information, see [Managing Your Files]().
{% endhint %}


---
description: 'Tips, tricks, and features for building scripts even faster'
---

# Power Users

## Editor Hot Keys

{% tabs %}
{% tab title="Mac" %}
| To do this | Press | When |
| :--- | :--- | :--- |
| Open 'Add Step' dialog in leftmost function | Tab | No Inputs Selected |
| Create empty variable 'pill'  | ![COMMAND](https://support.content.office.net/en-us/media/314f2d55-e8b8-4417-9d4b-b3908c1ebd0c.gif)+ i | Editing text |
| Undo last action | ![COMMAND](https://support.content.office.net/en-us/media/314f2d55-e8b8-4417-9d4b-b3908c1ebd0c.gif)+ z | No Inputs Selected |
| Undo last action | ![COMMAND](https://support.content.office.net/en-us/media/314f2d55-e8b8-4417-9d4b-b3908c1ebd0c.gif)+ y | No Inputs Selected |
{% endtab %}

{% tab title="Windows" %}
| To do this | Press | When |
| :--- | :--- | :--- |
| Open 'Add Step' dialog in leftmost function | Tab | No Inputs Selected |
| Create empty variable 'pill'  | Ctrl + i | Editing text |
| Undo last action | Ctrl + z | No Inputs Selected |
| Undo last action | Ctrl + y | No Inputs Selected |
{% endtab %}
{% endtabs %}

## Variable Wildcards

The asterisk \(wildcard\) character can be using within variable pills to reformat data. For example, imagine you have a list of tweets called `Tweets`, but instead want a list of the username associated with each  tweet. You could create a pill `Tweets.*.username`, which would build a list by pulling the `username` key from each tweet item. The wildcard here would be replaced with each possible value within the Tweets list to build the resulting list, ie `Tweets.0.username`, `Tweets.1.username`, etc.

## Editor Power Features

### Create Variable Shortcut

1. Open 'Add Step' dialog.
2. Type variable definition\* in search input.
3. Press 'Enter' to create variable.

![](../.gitbook/assets/screen-shot-2020-06-09-at-12.07.46-pm.png)

\*Not all variable types are supported in this shortcut. Supported types are:

* String
* Number
* List\( String \)
* List\( Number \)


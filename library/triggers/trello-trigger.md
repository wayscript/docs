---
description: >-
  Seamlessly integrate Trello with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Trello Trigger

![Run your script when changes are made to your Trello boards, lists, and cards.](../../.gitbook/assets/trello%20%281%29%20%282%29%20%282%29%20%282%29%20%282%29%20%281%29.png)

{% hint style="info" %}
To get data from Trello or automate creating new cards, use the [Trello module](../modules/trello.md).
{% endhint %}

## 🔗 Link Your Trello Account

When you add a Trello Trigger to your program, you will be prompted to link an account if you have not done so already.

## ⚡ Event Types

Choose when you would like the trigger to run:

1. When one of my boards changes
2. When a list on one of my boards changes
3. When a specific card changes

![](../../.gitbook/assets/screen-shot-2019-07-15-at-5.15.53-pm.png)

{% hint style="info" %}
If the trigger is set to run "when a specific card changes," you will be able to select one of the 1000 most-recent cards on your Trello board.
{% endhint %}

## 📤 Outputs

Select which Trello event data to retrieve as program variables.

### ![](../../.gitbook/assets/trello%20%281%29%20%282%29%20%282%29%20%282%29%20%282%29.png) Always Available

The following outputs are always available, regardless of event type:

```graphql
Changed_Action = {
                   type     : String,
                   date     : String,
                   name     : String,
                   username : String
}

Changed_Board = {
                   name : String,
                   id   : String
}
```

### 📜 List Outputs

List change events produce the following additional outputs:

```graphql
Changed_List = {
                 name : String,
                 id   : String
}
```

### 🃏 Card Outputs

Card change events produce the following additional outputs:

```graphql
Changed_Card = {
                 name        : String,
                 id          : String,
                 description : String,
                 due_date    : String,
                 url         : String
}

```

### 💡 Advanced Outputs

In the advanced settings, you can choose to output the raw JSON data sent by Trello in the webhook event.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-5.44.41-pm.png)


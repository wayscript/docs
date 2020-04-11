---
description: >-
  Seamlessly integrate Trello with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Trello

![Trello is a team collaboration tool that lets you organize and keep projects on task.](../../.gitbook/assets/trello%20%281%29.png)

{% hint style="info" %}
Check out py-trello on [GitHub](https://github.com/sarumont/py-trello).
{% endhint %}

{% hint style="info" %}
To run your script when changes are made to your Trello boards, lists, and cards, use the [Trello Trigger](../triggers/trello-trigger.md).
{% endhint %}

## 🔗 Link Your Trello Account

When you add a Trello Trigger to your script, you will be prompted to link an account, if you have not done so already.

## ![](../../.gitbook/assets/trello%20%281%29.png) Get My Boards

### 📤 Outputs

* Board Names
* Board IDs

## 🃏 Get Cards From a Board

Select a Board

### 📤 Outputs

* Card Names
* Card IDs
* Card Descriptions
* Card Lists

{% hint style="info" %}
This will return up to 1000 of the most-recent cards on your Trello board.
{% endhint %}

## 🌟 Create a New Card

1. Select a Board
2. Select a List

### 📥 Inputs

* Card Name
* Card Description
* Due Date for the Card


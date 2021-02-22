---
description: >-
  Seamlessly integrate Trello with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Trello

![Trello is a team collaboration tool that lets you organize and keep projects on task.](../../.gitbook/assets/trello%20%281%29%20%282%29%20%282%29.png)

{% hint style="info" %}
Check out py-trello on [GitHub](https://github.com/sarumont/py-trello).
{% endhint %}

{% hint style="info" %}
To run your script when changes are made to your Trello boards, lists, and cards, use the [Trello Trigger](../triggers/trello-trigger.md).
{% endhint %}

## 🔗 Link Your Trello Account

When you add a Trello Trigger to your script, you will be prompted to link an account, if you have not done so already.

## ![](../../.gitbook/assets/trello%20%281%29%20%282%29%20%282%29.png) Get My Boards

### 📤 Outputs

```graphql
Boards = [ 
     {
       name : String,
       id   : String
     }, 
]
```

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
* Attachment URL
* Attachment Name

### 📤 Outputs

* Card ID - The ID of the newly created card.

## 🖋 Update a Card

Input the ID of the card you would like to update. \(The ID can be obtained by [searching for a card](trello.md#search-for-a-card), or [getting cards from a board](trello.md#get-cards-from-a-board) in a previous Trello step.\)

### 📥 Inputs

* Card Name
* Card Description
* Attachment URL
* Attachment Name

## 🔎 Search for a Card

1. Select the board you want to search.
2. Input a search term. The card name must start with this term in order to match the query.

### 📤 Outputs

```graphql
Cards = [ 
    {
     name : String,
     id   : String,
     desc : String,
     list : String
    }, 
]
```

{% hint style="info" %}
This will return up to 1000 matching cards.
{% endhint %}

## ➡ Move a Card to Another List

1. Select a Target Board
2. Select a Target List
3. Input the card ID to move

## ⬆ Change a Card's Position in the List

1. Select a Position
2. Input the card ID to move

## ❌ Delete a Card

Input the card ID to delete


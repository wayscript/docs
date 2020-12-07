---
description: >-
  Seamlessly integrate Microsoft Teams with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Microsoft Teams

![More ways to be a team.](../../.gitbook/assets/msteams.png)

{% hint style="info" %}
Check out Microsoft Graph Documentation on [GitHub](https://github.com/microsoftgraph/microsoft-graph-docs).
{% endhint %}

## 🔗 Link Your Microsoft Teams Account

When using Microsoft Teams module for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the 'Select an Account' dropdown in the Microsoft Teams module settings
{% endhint %}

## 💼 Select an Account

Select the team that you would like to work with.

## \#⃣ Work With Channels

### ⚙ Modes

* Create a Channel
* Write to a Channel

### 🌟 Create a Channel

#### 📥 Inputs

* Name _\(required\)_

#### 📤 Output

```graphql
New_Channel_Id : String
```

### ✏ Write to a Channel

Choose any channel in your Workspace.

#### 📥 Inputs

* Message

#### 📤 Output

```graphql
Action_Status : String
```

## 👥 Work with Users

### ⚙ Modes

* Get a User's Member ID

### 🆔 Get a User's Member ID

Choose a User

#### 📤 Output

```graphql
Member_ID : String
```


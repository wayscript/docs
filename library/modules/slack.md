---
description: >-
  Seamlessly integrate Slack with your favorite APIs, databases, and programming
  languages, using WayScript.
---

# Slack

![Slack is where work flows.](../../.gitbook/assets/slack%20%281%29.png)

{% hint style="info" %}
Check out python-slackclient on [GitHub](https://github.com/slackapi/python-slackclient).
{% endhint %}

{% hint style="info" %}
To run your program when Slack events occur, use the [Slack Trigger](../triggers/slack-trigger.md).
{% endhint %}

## 🔗 Link Your Slack Account

When using Slack module for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from 'Select Workspace' dropdown in the Slack module settings
{% endhint %}

## 💼 Select a Slack Workspace

Select the workspace that you would like to work with.

## \#⃣ Work With Channels

### ⚙ Modes

* Create a Channel
* Write to a Channel
* Get a List of Channel Members
* Invite Users to a Channel
* Get Channel's History of Messages

### 🌟 Create a Channel

#### 📥 Inputs

* Name _\(required\)_
* Make Private

#### 📤 Output

```graphql
New_Channels_Id : String
```

### ✏ Write to a Channel

Choose any channel in your Workspace.

#### 📥 Inputs

* Message
* As Bot

#### 📤 Output

```graphql
Action_status : String
```

### 👥 Get a List of Channel Members

Choose any channel in your Workspace.

#### 📤 Output

```graphql
List_Of_Channel_Members : [
    String,
]
```

### 👋 Invite Users to a Channel

Choose any channel in your Workspace.

#### 📥 Inputs

* Users IDs

#### 📤 Output

```graphql
Action_status : String
```

### 💬 Get Channel's History of Messages

Choose any channel in your Workspace

#### 📥 Inputs

* Number of Messages to Retrieve

#### 📤 Output

```graphql
Message_History = [
    {
        username : String, 
        text : String, 
        timestamp : Date, 
        is_bot : Bool,
        attachments : [
            {
                title : String, 
                text : String, 
                author_name : String, 
                fallback : String, 
                color : String, 
                pretext : String, 
                author_link : Url,
                author_icon : Url,
                title_link : Url,
                image_url : Url,
                fields : [
                    {
                        title : String,
                        value : String,
                        short : Bool,
                    },
                ],
                thumb_url : Url,
                footer : String,
                footer_icon : Url,
                timestamp : Date,
            },
        ],
    },
]
```

### ⚡ Run a Slash Command

Choose a channel in your Workspace where the command you would like to run is available.

#### 📥 Inputs

* **Command:** The slash command you would like to run. \(e.g. _/poll "A question" "An answer" "Another Answer"_\) [Click here to learn about Slack slash commands.](https://api.slack.com/interactivity/slash-commands)
* **Legacy Token:** Your Legacy account token. Running slash commands via API requires a legacy account token. You can generate a token for your workspace here: [https://api.slack.com/custom-integrations/legacy-tokens](https://api.slack.com/custom-integrations/legacy-tokens)

#### 📤 Output

```graphql
Action_status : String
```

## 👥 Work with Users

### ⚙ Modes

* Get a User's Member ID
* Lookup a User by their Email
* Send a Direct Message

### 👤 Get a User's Member ID

Choose a User

#### 📤 Output

```graphql
Member_ID : String
```

### 📧 Lookup a User by their Email

#### 📥 Inputs

* Email

#### 📤 Output

```graphql
User = {
    username : String, 
    real_name : String, 
    id : String, 
    is_admin : Bool,
    is_app_user : Bool,
    is_bot : Bool,
    is_owner : Bool,
    is_primary_owner : Bool,
    is_restricted : Bool,
    is_ultra_restricted : Bool,
    profile : {
        display_name : String, 
        email : String, 
        phone : String, 
        skype : String, 
        status_emoji : String, 
        status_text : String, 
        status_expiration : String, 
        title : String, 
        image_192 : Url,
        image_24 : Url,
        image_32 : Url,
        image_48 : Url,
        image_512 : Url,
        image_72 : Url,
    },
    timezone : String,
    tz_label : String, 
}
```

### 💬 Send a Direct Message

#### 📥 Inputs

* Message

#### 📤 Output

```graphql
Action_status : String
```
### 💬 Send a Direct Message to a Group of Users

#### 📥 Inputs

* Message
* Selector Users

#### 📤 Output

```graphql
Action_status : String
```

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

#### 📤 Outputs

* New Channel's ID
* JSON Data

### ✏ Write to a Channel

Choose any channel in your Workspace.

#### 📥 Inputs

* Message
* As Bot

#### 📤 Outputs

* Action status
* JSON Data

### 👥 Get a List of Channel Members

Choose any channel in your Workspace.

#### 📤 Outputs

* List of Channel Members
* JSON Data

### 👋 Invite Users to a Channel

Choose any channel in your Workspace.

#### 📥 Inputs

* Users IDs

#### 📤 Outputs

* Action status
* JSON Data

### 💬 Get Channel's History of Messages

Choose any channel in your Workspace

#### 📥 Inputs

* Number of Messages to Retrieve

#### 📤 Outputs

* Message History
* Messengers
* JSON Data

### ⚡ Run a Slash Command

Choose a channel in your Workspace where the command you would like to run is available.

#### 📥 Inputs

* **Command:** The slash command you would like to run. \(e.g. _/poll "A question" "An answer" "Another Answer"_\) [Click here to learn about Slack slash commands.](https://api.slack.com/interactivity/slash-commands)
* **Legacy Token:** Your Legacy account token. Running slash commands via API requires a legacy account token. You can generate a token for your workspace here: [https://api.slack.com/custom-integrations/legacy-tokens](https://api.slack.com/custom-integrations/legacy-tokens)

#### 📤 Outputs

* Action status
* JSON Data

## 👥 Work with Users

### ⚙ Modes

* Get a User's Member ID
* Lookup a User by their Email
* Send a Direct Message

### 👤 Get a User's Member ID

Choose a User

#### 📤 Outputs

* Member ID
* JSON Data

### 📧 Lookup a User by their Email

#### 📥 Inputs

* Email

#### 📤 Outputs

* Member ID
* Member Name
* JSON Data

### 💬 Send a Direct Message

#### 📥 Inputs

* Message

#### 📤 Outputs

* Action status
* JSON Data


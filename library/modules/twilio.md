---
description: Send Text Messages
---

# Twilio

{% hint style="warning" %}
This module requires that you have a Twilio SMS account. If you don't please set one up before continuing. 
{% endhint %}

{% hint style="info" %}
If you would like to send text messages to yourself, check out the Text Message module.
{% endhint %}

## Setting up your Account

### 1\) Add New Account

Click 'Add New Account' in your Twilio Module Settings.

![Twilio Settings](../../.gitbook/assets/screenshot-2019-07-16-15.36.43.png)

### 2\) Go to your [Twilio Dashboard](https://www.twilio.com/console)

### 3\) Input API Key Data

From your Twilio Dashboard, grab your Account Name, Account SID, and Auth Token. 

![On Twilio Dashboard](../../.gitbook/assets/screenshot-2019-07-16-15.42.17.png)

Copy and paste the data into the WayScript modal.

![](../../.gitbook/assets/screenshot-2019-07-16-15.44.57.png)

Press submit.

## Settings

* **Twilio Phone Number** - Input your Twilio SMS phone number. 
  * Required Format: +12223334567

## Inputs

* **Phone Number** - This is the phone number you are sending a message to.
  * Required Format: +12223334567
* **Text Message** - This is your message.You can [include variable values](../../introduction/modules.md#option-two-hardcode-a-value) in your messages.


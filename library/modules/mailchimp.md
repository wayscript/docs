# Mailchimp

![Marketing automation platform and email marketing service.](../../.gitbook/assets/mailchimp.png)

## Link Your Mailchimp Account

When you drag in a Mailchimp module for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the Mailchimp module settings.
{% endhint %}

## Create a List

### Inputs

* List Name _\(required\)_
* Company Name _\(required\)_
* Address 1_\(required\)_
* Address 2
* City _\(required\)_
* State _\(required\)_
* Zip Code _\(required\)_
* Country Code _\(required\)_
* Phone Number
* Permission Reminder _\(required\)_
* Sender's Name _\(required\)_
* Sender's Email Address _\(required\)_
* Subject _\(required\)_
* Language _\(required\)_
* Email Type Option
  * True
  * False

### Outputs

* JSON Data

## Add a New Member to a List

### Inputs

* List ID _\(required\)_
* Email Address _\(required\)_
* Status
  * Subscribed
  * Unsubscribed
  * Cleaned
  * Pending
* Tags

### Outputs

* JSON Data

## Get Information About All Your Lists

### Outputs

* List ID
* List Name
* JSON Data

## Get All Members in a List

### Inputs

* List ID _\(required\)_

### Outputs

* Member Email Addresses
* Member IDs
* JSON Data


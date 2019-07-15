---
description: Run your program when Gmail messages change.
---

# Gmail Trigger

## Setup

### Link Account

When you drag in a Gmail Trigger for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the Gmail Trigger settings.
{% endhint %}

## Settings

### Modes

1. Run for all emails: All emails are evaluated.
2. Run for emails with specific labels: Only emails containing one of these labels will be evaluated.

### Activation Method

Choose which event\(s\) will activate the trigger.

* [ ] When one or more messages are received.
* [ ] When one or more messages are permanently deleted\( not Trashed \).
* [ ] When labels are added to a message.
* [ ] When labels are removed from a message.

{% hint style="info" %}
The affected message\(s\) will be evaluated to create program variables. 
{% endhint %}

### Outputs

Select the data to retrieve as variables for your program.

* [ ] Event Types
* [ ] Message Ids
* [ ] Thread Ids
* [ ] Labels
* [ ] Labels Added
* [ ] Labels Removed
* [ ] All Email Recipients
* [ ] To Email Recipients
* [ ] Cc Email Recipients
* [ ] Senders
* [ ] Subjects
* [ ] Body Snippets
* [ ] Dates


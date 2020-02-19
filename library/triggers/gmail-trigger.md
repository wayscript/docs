# Gmail Trigger

![Run your script when Gmail messages change.](../../.gitbook/assets/gmail.png)

{% hint style="info" %}
To automate actions with Gmail, use the [Gmail module](../modules/gmail.md).
{% endhint %}

## 🔗 Link Your Gmail Account

When you drag in a Gmail Trigger for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the Gmail Trigger settings.
{% endhint %}

## ⚙ Settings

![](../../.gitbook/assets/screen-shot-2019-07-15-at-12.41.52-pm.png)

### ![](../../.gitbook/assets/gmail.png) Modes

1. **Run for all emails:** All emails are evaluated.
2. **Run for emails with specific labels:** Only emails containing one of these labels will be evaluated.

{% hint style="info" %}
The Gmail Trigger will run your script each time a message is received that matches your specified conditions.
{% endhint %}

### ⚡Activation Method

![](../../.gitbook/assets/screen-shot-2019-07-15-at-12.41.24-pm.png)

If "Run for emails with specific labels" is selected, you will then need to select which labels you want to watch.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-12.42.21-pm.png)

{% hint style="info" %}
If you do not see a label you are looking for, click the refresh button.
{% endhint %}

Choose which event\(s\) will activate the trigger.

* When a message is received
* When a message is permanently deleted \(not Trashed\)
* When labels are added to a message
* When labels are removed from a message

## 📤 Outputs

Select the data to retrieve as variables for your program.

* **Event Type** - Possible values are "Received," "Changed," or "Deleted."
* **Message Id -** The Id of the message.
* **Thread Id** - The Id of the thread this message is a part of.
* **Labels** - The current labels for the message.
* **Labels Added** - The labels that were added to the message. \(Only applicable if the "When labels are added to a message" event is selected.\)
* **Labels Removed** - The labels that were removed from the message. \(Only applicable if the "When labels are removed from a message" event is selected.\)
* **All Email Recipients** - All email addresses that received this message \(includes To and Cc\).
* **To Email Recipients** - Email addresses that were on the "To" line of the message.
* **Cc Email Recipients** - Email addresses that were on the "Cc" line of the message.
* **Sender** - The email address of the person who sent the message.
* **Reply-to Address** - Value of the "Reply-to" email header field.
* **Subject** - The subject of the message.
* **Body Snippet** - A preview of the body of the email.
* **Date** - Date/Time the message was received.


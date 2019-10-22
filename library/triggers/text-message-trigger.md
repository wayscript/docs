# Text Message Trigger

![Run your script with a text message.](../../.gitbook/assets/text_message_128x128.png)

{% hint style="success" %}
You can trigger WayScript programs to run by sending a text message to WayScript at  
**\(415\) WYS-CRPT**   \(+1 415 997 2778\)
{% endhint %}

{% hint style="info" %}
To send text messages to yourself, use the [Text Message module](../modules/text-message.md).
{% endhint %}

## 📱 Phone Number Verification

{% hint style="warning" %}
If you haven't yet verified your phone number with your WayScript account, you will need to do so before using this module. See [Phone Number Verification](../../account-management/phone-number-verification.md) for details.
{% endhint %}

## 📥New Variable Inputs

You can dynamically input new variable data into your program via text message. Specify these variables in the "Variables to Create" section.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-4.27.38-pm.png)

![](../../.gitbook/assets/screen-shot-2019-07-15-at-4.28.50-pm.png)

## 💬 Sending a Text

Send your text message to **\(415\) WYS-CRPT** \(+1 415 997 2778\).

The text message body will be the program name, followed by a colon, then any variable values, all separated by commas.

For example, if you wanted to run your "Stocks" program with the arguments "AAPL" and "MSFT", your message body would be "Stocks:AAPL,MSFT"

![](../../.gitbook/assets/new_conversation.jpg)

{% hint style="info" %}
The "Body" field in the Trigger Settings will also show you how to compose your message
{% endhint %}

![](../../.gitbook/assets/body.png)

{% hint style="warning" %}
Variables must be submitted in the same order as the Outputs defined on the Text Message Trigger.
{% endhint %}

{% hint style="warning" %}
The text must originate from your verified phone number.
{% endhint %}


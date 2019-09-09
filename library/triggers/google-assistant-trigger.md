# Google Assistant Trigger

![Run your program using a Google Assistant voice command.](../../.gitbook/assets/google_assistant.png)

{% hint style="info" %}
To have your Google Assistant speak a phrase, use the [Google Assistant module](../modules/google-assistant.md).‌
{% endhint %}

## ​ ⚙ Setup <a id="setup"></a>

### ​![](../../.gitbook/assets/google_assistant.png) Enable Google Assistant <a id="enable-alexa"></a>

Add the WayScript action to your Google Assistant account. [Get the WayScript Trigger action.](https://assistant.google.com/u/0/services/a/uid/000000dfb9940d69?hl=en-US&source=docs)​

{% hint style="info" %}
WayScript will remind you to do this the first time you use a Google Assistant Trigger.‌
{% endhint %}

### ​ 🕵 Program Alias <a id="program-alias"></a>

You can supply an easy-to-understand alias for your program.

![](../../.gitbook/assets/screen-shot-2019-09-09-at-10.18.02-am.png)

Useful when your program name is long or difficult for the Google Assistant to understand‌

## ​ 🗣 Voice Commands <a id="voice-commands"></a>

### ​➡ Pass in Spoken Input <a id="pass-in-spoken-input"></a>

To pass the input in your voice command, add "with \[Variable Value\]" to your Google Assistant phrase.‌

You can pass an argument to your Google Assistant-Triggered program by enabling the "Spoken Input" variable in the Outputs panel.

![](../../.gitbook/assets/screen-shot-2019-09-09-at-10.22.05-am.png)

Suppose your program is called 'Stocks' and takes a single input called \[Symbol\] as input, you could then speak the following phrase to the Google Assistant:

> "Hey Google, ask WayScript Trigger to run 'Stocks' with AAPL."

![](../../.gitbook/assets/screen-shot-2019-09-09-at-10.24.21-am.png)

### ​💬 Speak a Phrase <a id="speak-a-phrase"></a>

Once you have added the Google Assistant Trigger to a program, you can include the [Google Assistant module](../modules/google-assistant.md), which will allow the Google Assistant to speak to you while your program is running.‌

You can reference variables that were created earlier in the program and insert them into an Google Assistant Phrase. See the [Google Assistant module documentation](../modules/google-assistant.md) for more details.‌

## 🎓 Tutorial

For a brief tutorial on how to use the Google Assistant Trigger, see [Run a Python Script with a Google Assistant Voice Command.](https://wayscript.com/blog_entry/44)


# Microsoft Teams Trigger

---
description: >-
  Seamlessly integrate Microsoft Teams with your favorite APIs, databases, and programming
  languages, using WayScript.
---

# Microsoft Teams Trigger

![Run your script when Microsoft Teams events occur.](../../.gitbook/assets/msteams.png)

{% hint style="info" %}
To work with Microsoft Teams channels and users, use the [Microsoft Teams module](../modules/microsoft-teams.md).
{% endhint %}

## 🔗 Link Your Microsoft Teams Account

When you drag in a Microsoft Teams Trigger for the first time, follow the prompt to authorize access.

## ⚙ Settings

### 💼 Workspace

Select a linked workspace, or add a new one.

### 💡 Mode

Choose which event\(s\) will trigger your program

1. **Channel Events:** Monitor all or specified channels in your workspace.

   1. A message was posted to a channel

2. **User Events:**

   1. A message was posted to a chat


You can scope the trigger to a specific channel and/or user, or allow the notification to fire for any channel and/or user.


## 📤 Outputs

Select what event data you would like to retrieve as a program variable and set default values.

The Microsoft Teams Channel, Slack User, and Raw JSON Data from the Slack event are always available as outputs.

If you chose the "message was posted to a channel" event type, the Microsoft Teams Message Text will also be available.

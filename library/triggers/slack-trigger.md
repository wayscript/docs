# Slack Trigger

![Run your program when Slack events occur.](../../.gitbook/assets/slack.png)

{% hint style="info" %}
To work with Slack channels and users, use the [Slack module](../modules/slack.md).
{% endhint %}

## 🔗Link Your Slack Account

When you drag in a Slack Trigger for the first time, follow the prompt to authorize access.

## ⚙Settings

### 💼Workspace

Select a linked workspace, or add a new one.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-2.57.01-pm.png)

### ⚡Mode

Choose which event\(s\) will trigger your program

1. **Channel Events:** Monitor all or specified channels in your workspace.

   1. A message was posted to a channel
   2. A channel was archived
   3. A channel was unarchived
   4. A channel was created
   5. A channel was deleted
   6. A channel was renamed

   ![](../../.gitbook/assets/screen-shot-2019-07-15-at-2.57.18-pm.png)   

2. **User Events:**

   1. A new user joined
   2. A user's data changed
   3. A user joined a channel
   4. A subteam was created
   5. A subteam was updated

   ![](../../.gitbook/assets/screen-shot-2019-07-15-at-2.57.55-pm.png) 

You can scope the trigger to a specific channel and/or user, or allow the notification to fire for any channel and/or user.

Additionally, you can exclude messages from bots. 

{% hint style="info" %}
Exclude messages from bots if you have a WayScript program that is posting as a bot to a channel that triggers the same WayScript program, so your WayScript program doesn't trigger itself.
{% endhint %}

![](../../.gitbook/assets/screen-shot-2019-07-15-at-3.07.39-pm.png)

## 📤Outputs

Select what event data you would like to retrieve as a program variable and set default values.

The Slack Channel, Slack User, and Raw JSON Data from the Slack event are always available as outputs.

If you chose the "message was posted to a channel" event type, the Slack Message Text will also be available.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-3.10.13-pm.png)


---
description: Run your program via slack message.
---

# Slack Trigger

## Link Your Slack Account

When you drag in a Slack Trigger for the first time, follow the prompt to authorize access.

## Settings

### Workspace

Select a linked workspace, or add a new one.

### Mode

Choose which event\(s\) will trigger your program

1. Channel Events: Monitor all or specified channels in your workspace.

   1. A message was posted to a channel
   2. A channel was archived
   3. A channel was unarchived
   4. A channel was created
   5. A channel was deleted
   6. A channel was renamed

   You can select specific channel\(s\) and/or user\(s\) to monitor

2. User Events:
   1. A new user joined
   2. A user's data changed
   3. A user joined a channel
   4. A subteam was created
   5. A subteam was updated

{% hint style="info" %}
You can also specify users to filter by and whether or not to ignore bots.
{% endhint %}

## Outputs

Select what event data you would like to retrieve as a program variable and set default values.


---
description: >-
  Run your favorite APIs, databases, and programming languages on a schedule,
  using WayScript.
---

# Time Trigger

![Run your script periodically.](../../.gitbook/assets/cron.png)

## ⚡ Activate the Time Trigger

In order to trigger scripts at a particular time, add the Time Trigger module to the triggers section of the script and activate the trigger.

## 🗓 Select a Run Frequency

* Monthly
* Weekly
* Daily
* Hourly
* Every ten minutes \(Premium feature\)
* Every minute \(Premium feature\)
* [Custom \(Crontab syntax\)](time-trigger.md#crontab-syntax)

If you select the **daily frequency**, you will have an option to choose what time your script should run each day.

If you select the **weekly frequency**, you will have an option to choose a day of the week and a time of day for your script to run.

If you select the **monthly frequency**, you will have an option to choose a day of the month and a time of day for your script to run.

{% hint style="info" %}
If you select the 29th, 30th, or 31st, your script will not run on months with fewer than that number of days. **Use the "Last Day" option if you would like your script to run at the end of each month.**
{% endhint %}

### \*\*\*\*✨ **Crontab Syntax**

If you select the "Custom" option for Run Frequency, you will be able to use [Crontab Syntax](https://en.wikipedia.org/wiki/Cron#CRON_expression) to specify the frequency at which you would like your script to run.

#### Examples

1. Schedule your script to run at 5 am and 5 pm: `0 5,17 * * *`
2. Schedule your script to run every Monday at 5am: `0 5 * * mon`
3. Schedule your script to run every 15 minutes: `*/15 * * * *`
4. Schedule your script to run every 4 hours: `0 */4 * * *`

{% hint style="info" %}
Scripts in free accounts are limited to one run per hour. Setting your crontab to a frequency shorter than that will not work. [Contact us](https://wayscript.com/contact) if you'd like to upgrade your account to increase this frequency.
{% endhint %}

## 🕑 Select a Time Zone

In daily, weekly, monthly, or custom/crontab mode, you have the option to select which Time Zone your Time Trigger should run in. This option defaults to UTC.


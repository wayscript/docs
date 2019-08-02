---
description: Coming soon!
---

# Survey Monkey Trigger

![Run your program when Survey Monkey events occur.](../../.gitbook/assets/surveymonkey-logo-300x300.png)

## Settings

### Select an Account

![](../../.gitbook/assets/screen-shot-2019-08-02-at-4.34.08-pm.png)

This is the email of the Survey Monkey account you have authorized. If you want to add another account select **Add an Account** from the drop-down menu.

### Select a Mode

![](../../.gitbook/assets/screen-shot-2019-08-02-at-4.36.03-pm.png)

There are two modes:

1. Response Completed - The program will run whenever a response to the survey is completed.
2. Response Updated - The program will run whenever a response to the survey is updated.

### Select a Survey

![](../../.gitbook/assets/screen-shot-2019-08-02-at-4.38.23-pm.png)

This drop-down menu is automatically populated with the surveys created by the selected Survey Monkey account.

### Survey Response Details

![Check this box if you want survey response details.](../../.gitbook/assets/screen-shot-2019-08-02-at-4.39.49-pm.png)

Check this box if you have a paid Survey Monkey account. By doing so, you will be able to access the answers to your survey as outputs. See the **View Response Details** scope at [https://developer.surveymonkey.com/api/v3/\#scopes](https://developer.surveymonkey.com/api/v3/#scopes) for more details.

## Outputs

* Survey answers
  * Must have a paid Survey Monkey account and have '[Get survey response details](survey-monkey-trigger.md#survey-response-details)' box checked.
* IP Address
  * IP Address the response was taken from.
* Date Created
  * Date the response was created.
* Date Modified
  * Date the response was last modified.
* Analyze URL
  * Weblink to the analyze page to view the response.
* JSON Data
  * Raw JSON data received from the API.


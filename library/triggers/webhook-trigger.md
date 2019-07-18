# Webhook Trigger

![Run your program via a web request.](../../.gitbook/assets/webhook.png)

## Overview

Add the Webhook Trigger to the triggers section of your program and turn it on.

Webhooks require the following data:

1. Your Program ID
2. [Your unique API Key](../../account-management/managing-your-api-key.md)
3. Optional: [New variable inputs](webhook-trigger.md#new-variable-inputs)

This data can be retrieved from the settings within the Webhook Trigger.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-6.06.16-pm.png)

## New Variable Inputs

You can dynamically input new variable data into your WayScript programs from your api call. 

Declare the variables you want your Webhook Trigger to create and pass to your program in the Outputs section.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-6.09.52-pm.png)

## Functions

You can specify which [function](../logic/functions/) you would like to run with your Webhook trigger.

Do this by placing the Webhook Trigger in one or more functions within your WayScript program, then specify which function you would like to run by passing the function name via the "function" parameter in your api call.

![](../../.gitbook/assets/screen-shot-2019-07-15-at-6.18.01-pm.png)

## API Call

Use Python, JavaScript, or [any other programming language ](../../apis/rest.md)to trigger your program.

```python
import requests

url = 'https://wayscript.com/api?'

variables = [ 'new_name', 'www.new_url.com' ]

params = {
    'api_key'   : 'YOUR_API_KEY',  # insert api key
    'program_id': 3726,            # insert program id
    'variables' : variables,       # (optional)
    'function'  : 'My Function'    # insert function name (optional)
}

requests.post( url, params = params )
```

{% hint style="warning" %}
Variables must be submitted in the same order as the Outputs defined on the Trigger Module as displayed above. 
{% endhint %}

{% hint style="info" %}
For information on finding your API Key, see [Managing Your API Key](../../account-management/managing-your-api-key.md).
{% endhint %}

{% hint style="danger" %}
Never share your API Key with anyone else; it is equivalent to giving them your password.
{% endhint %}


---
description: Run WayScript programs via HTTP requests.
---

# REST API

## \*\*\*\*![](../.gitbook/assets/webhook.png) **Add a Webhook Trigger**

In order to trigger WayScript programs with an api call, you must first add a [Webhook Trigger](../library/triggers/webhook-trigger.md) to your program.

![](../.gitbook/assets/webhook_function.png)

{% hint style="info" %}
You can add a different Webhook Trigger to every function if you like, but only one Webhook trigger per function. \(See [Trigger Restrictions](../library/triggers/#trigger-restrictions).\)
{% endhint %}

{% hint style="danger" %}
If you do not specify a function name in your request and your program has multiple functions with Webhook Triggers, you will be asked to specify which function you would like to run.
{% endhint %}

{% api-method method="post" host="https://" path="wayscript.com/api" %}
{% api-method-summary %}
Run Program
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="api\_key" type="string" required=true %}
Your WayScript API Key.
{% endapi-method-parameter %}

{% api-method-parameter name="program\_id" type="integer" required=true %}
The ID of the program you would like to run.
{% endapi-method-parameter %}

{% api-method-parameter name="variables" type="string" required=false %}
Variables that you want to pass to your program. You can append as many of these as your program takes. \(See below.\)
{% endapi-method-parameter %}

{% api-method-parameter name="function" type="string" required=false %}
The name of a specific function that you want to run.
{% endapi-method-parameter %}

{% api-method-parameter name="run\_async" type="boolean" required=false %}
Run this program asynchronously. \(See below.\) Defaults to `False`.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "Success":"Program finished.",
    "Result":[]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% hint style="info" %}
For instructions on finding your WayScript API Key, see [Managing Your API Key](../account-management/managing-your-api-key.md).
{% endhint %}

### 💡 Examples

#### Run a Program

{% tabs %}
{% tab title="Request" %}
```bash
curl -X POST 'https://wayscript.com/api?api_key=YOUR_API_KEY&program_id=1234'
```
{% endtab %}

{% tab title="Response" %}
```bash
{"Success":"Program finished.","Result":[]}
```
{% endtab %}
{% endtabs %}

**Variable Inputs**

You can optionally input new variable data into your WayScript programs from your api call by appending one or more `variables` URL params to your request.

{% tabs %}
{% tab title="Request" %}
```bash
curl -X POST 'https://wayscript.com/api?api_key=YOUR_API_KEY&program_id=1234&variables=Foo&variables=Bar'
```
{% endtab %}

{% tab title="Response" %}
```bash
{"Success":"Program finished.","Result":[]}
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
Variables must be submitted in the same order as the Outputs defined on the Webhook Trigger.
{% endhint %}

**Running a Specific Function**

You can optionally specify which function within your program you would like to run by passing the function name via the `function` ****URL parameter.

{% tabs %}
{% tab title="Request" %}
```bash
curl -X POST 'https://wayscript.com/api?api_key=YOUR_API_KEY&program_id=1234&function=My%20Function'
```
{% endtab %}

{% tab title="Response" %}
```bash
{"Success":"Program finished.","Result":[]}
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
If you do not specify a function name in your request and your program has one function with a Webhook Trigger, the function with the Webhook Trigger will run.
{% endhint %}

{% hint style="warning" %}
The function you specify **MUST** have an _active_ Webhook Trigger.
{% endhint %}

**Running Your Program Asynchronously**

Typically, your program will run synchronously and your request will not return a result until the program has completed. 

However, you can optionally add the `run_async=True` URL param to your request to trigger a non-blocking program run.

{% tabs %}
{% tab title="Request" %}
```bash
curl -X POST 'https://wayscript.com/api?api_key=YOUR_API_KEY&program_id=1234&run_async=True'
```
{% endtab %}

{% tab title="Response" %}
```bash
 {"Success":"Program started."}
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Note that the response in this case is _"Program started"_, as opposed to _"Program finished."_
{% endhint %}


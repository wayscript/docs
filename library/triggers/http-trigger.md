---
description: >-
  Instantly build an HTTP endpoint that connects your favorite APIs, databases,
  and programming languages, using WayScript.
---

# HTTP Trigger

![Trigger a function when a user goes to a URL.](../../.gitbook/assets/http%20%281%29.png)

{% hint style="info" %}
To display a webpage back to the user, use the [HTTP Response](../modules/http-response.md) module.
{% endhint %}

## ⚙ Setup

The HTTP Trigger is used to setup a web request. You can use it to implement a web page endpoint, a JSON post request, or other types of web requests.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.17.39-pm.png)

### ✒ Sample Code

To get you started quickly, the HTTP Trigger provides cURL, Python, and JavaScript sample code, which can simply be pasted into your terminal and run.

This sample code includes some data that demonstrates how to pass query parameters and JSON body parameters with your request.

{% tabs %}
{% tab title="cURL" %}
```bash
curl -d '{"name":"Peter Parker"}' \
    -H "Content-Type: application/json" \
    https://1234.wayscript.com/?hero=Spiderman
```
{% endtab %}

{% tab title="Python" %}
```python
import http.client
data = {"name":"Peter Parker"}
conn = http.client.HTTPSConnection("1234.wayscript.com")
conn.request("POST", "/?hero=Spiderman", str(data), headers={"Content-Type":"application/json"})
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
const data = {"name":"Peter Parker"};
fetch("https://1234.wayscript.com/?hero=Spiderman", {
    method: "POST",
    headers: new Headers({"Content-Type":"application/json"}),
    mode: "cors",
    body: JSON.stringify(data),
})
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Use the WayScript [Python](https://github.com/wayscript/wayscript-python) and [JavaScript](https://github.com/wayscript/wayscript-js) libraries to make calling your HTTP endpoints even easier!
{% endhint %}

### 🔗 Endpoints

When setting up the HTTP Trigger, you can create as many named endpoints as you like. If you don't provide a name for your endpoint, the trigger will match the root URL. All endpoint names must be unique throughout your script to prevent ambiguity.

![](../../.gitbook/assets/screen-shot-2020-03-13-at-1.15.21-pm.png)

To access your endpoints, use the program ID as a subdomain of **wayscript.io**. For example, in the image above, you can trigger your script by hitting either [https://16233.wayscript.io/](https://16233.wayscript.io/) or [https://16233.wayscript.io/custom\_endpoint](https://16233.wayscript.io/custom_endpoint).

Remember to activate your trigger before using the endpoint!

### 🔐 Password-Protect your Endpoints

If you would like the endpoints in your HTTP trigger to require a login to view, enable the "Password Protection" toggle.

A button to "Manage Login Credentials" will appear.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.39.21-pm.png)

Clicking this button will take you to "Login Credentials" section of the "Script Setup" tab, where you can manage the usernames and passwords that will allow people to log in to your endpoints.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.40.18-pm.png)

When you click "Add a credential," a new login will be automatically generated for you, including a username and randomly-generated password. You can choose to use these values, or edit them as you see fit.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.41.50-pm.png)

When a user goes to access your endpoint for the first time, they will now be prompted to login.

![Custom Endpoint Login Prompt](../../.gitbook/assets/screen-shot-2019-11-12-at-7.50.17-pm%20%281%29.png)

### Basic Authentication

If you password-protect your endpoints, you can use the credentials added above to access your endpoints by including an `Authorization: Basic` header in your request.

This header should follow the standard for [HTTP basic access authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). For example, suppose your Username is "**captain@wayscript.com**" and your Password is "**letmein**," you would create the Authorization header by:

1. Joining the Username and Password into a single string, separated by a semicolon: **`captain@wayscript.com:letmein`**
2. Encoding that string in Base64: **`Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=`**
3. Passing that encoded string to your custom endpoint by including the `Authorization: Basic Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=` header in your request.

These headers are also displayed for you under each password in the "Login Credentials" section of the "Script Setup" tab.

### Authenticating Using Your API Key

If your endpoint is not public, you can also use your [WayScript API Key](../../account-management/managing-your-api-key.md) to access your endpoints api call by including an `Authorization: Bearer` header in your request.

For example, if your WayScript API Key is **`fhAEdGT9EbFDh_migcrukZ1Vb28rLFKqt9AxOiq9bdQ`**, you would include the `Authorization: Bearer fhAEdGT9EbFDh_migcrukZ1Vb28rLFKqt9AxOiq9bdQ` header in your request.

## 📤 Outputs

The Outputs section allows you to define variables that you would like the HTTP Trigger to create and make available for use later in your script. You can pass values for these variables within the request to your endpoint.

You can add as many variable outputs as you like, as well as pass any combination of query parameters and JSON body data.

### ❔ Request Query Parameters

This section allows you to define variable outputs whose values you will pass as query parameters to your script. For example, if you define a query parameter output called "_hero_," you would pass its value to your script by appending the query parameter to your endpoint url:  [https://10834.wayscript.com?hero=Spiderman](https://10834.wayscript.com?hero=superman)

### 🗒 Request JSON Body Parameters

If you define an output to be passed as a JSON body parameter, you will include the data as a key-value pair within the body of your request. For example, if you define a JSON body parameter called "_name_," you will pass its value to your script by including the relevant data within your request:

```bash
curl -d '{"name":"Peter Parker"}' \
    -H "Content-Type: application/json" \
    https://10834.wayscript.com
```

### 🔣 Raw Request Data

The raw data sent to the HTTP Trigger endpoint.

### 🗒 Http Metadata 

{% tab title="Python" %}
```python
StructType({
          'accept_encodings'                  : BoolType(),
          'accept_languages'                  : BoolType(),
          'accept_mimetypes'                  : BoolType(),
          'base_url'                          : UrlType(),
          'content_length'                    : IntType(),
          'content_type'                      : StringType(),
          'content_md5'                       : StringType(),
          'data'                              : StringType(),
          'date'                              : DateType(),
          'form'                              : JSONType(),
          'full_path'                         : StringType(),
          'host'                              : StringType(),
          'host_url'                          : UrlType(),
          'if_modified_since'                 : DateType(),
          'if_unmodified_since'               : DateType(),
          'is_json'                           : BoolType(),
          'is_secure'                         : BoolType(),
          'json'                              : JSONType(),
          'mimetype'                          : StringType(),
          'mimetype_params'                   : JSONType(),
          'method'                            : StringType(),
          'path'                              : StringType(),
          'query_string'                      : StringType(),
          'remote_addr'                       : StringType(),
          'remote_user'                       : StringType(),
          'referrer'                          : StringType(),
          'scheme'                            : StringType(),
          'url'                               : UrlType(),
          'url_root'                          : UrlType(),
          'user_agent'                        : StringType()
  })
```
{% endtab %}



## 🎓 Tutorial

{% embed url="https://www.youtube.com/watch?reload=9&v=OrZMjdVhFfA&feature=youtu.be" caption="Standup a Web App on the Cloud in 1 Minute" %}


# HTTP Trigger

![Trigger a function when a user goes to a URL.](../../.gitbook/assets/http%20%281%29.png)

{% hint style="info" %}
To display a webpage back to the user, use the [HTTP Response](../modules/http-response.md) module.
{% endhint %}

## ⚙ Setup

The HTTP Trigger is used to setup a web request. You can use it to implement a web page endpoint, a json post request, or other types of web requests.

![](../../.gitbook/assets/screen-shot-2019-09-09-at-8.57.49-am.png)

### 🔗 Endpoints

To set up the HTTP Trigger, give your endpoint a name. You can also leave the field blank to match the root URL. You can add multiple endpoints.

To access the endpoint, use the program ID as a subdomain of wayscript.com. For example, in the image above, you could access this endpoint using https://8503.wayscript.com/endpoint.

Remember to Activate your trigger before using the endpoint.

### 🔐 Password-Protect your Endpoints

If you would like the endpoints in your HTTP trigger to require a login to view, uncheck the "Publicly Accessible" checkbox.

A button to "Manage Login Credentials" will appear.

![Manage Login Credentials](../../.gitbook/assets/screen-shot-2019-09-09-at-8.59.56-am.png)

Clicking this button will take you to the "Script Setup" tab, where you can manage the usernames and passwords that will allow people to log in to your endpoints.

![Script Setup](../../.gitbook/assets/screen-shot-2019-09-09-at-9.01.25-am.png)

When you click "Add a credential," a new login will be automatically generated for you, including a username and randomly-generated password. You can choose to use these values, or edit them as you see fit.

![Username and randomly-generated password](../../.gitbook/assets/screen-shot-2019-09-09-at-9.04.12-am.png)

When a user goes to access your endpoint for the first time, they will now be prompted to login.

![Custom endpoint login prompt](../../.gitbook/assets/screen-shot-2019-09-09-at-9.07.16-am.png)

### Basic Authentication

If you password-protect your endpoints, you can access them without the login endpoint by including an `Authorization` header in your request.

This header should follow the standard for [HTTP basic access authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). For example, suppose your Username is "**captain@wayscript.com**" and your Password is "**letmein**," you would create the `Authorization` header by:

1. Joining the Username and Password into a single string, separated by a semicolon: **`captain@wayscript.com:letmein`**
2. Encoding that string in Base64: **`Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=`**
3. Passing that encoded string to your custom endpoint by including the `Authorization: Basic` **`Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=`** header in your request.

## 🎓 Tutorial

{% embed url="https://www.youtube.com/watch?reload=9&v=OrZMjdVhFfA&feature=youtu.be" caption="Standup a Web App on the Cloud in 1 Minute" %}


---
description: >-
  Easily build an HTTP endpoint that sends content created from your favorite
  APIs, databases, and programming languages, using WayScript.
---

# HTTP Response

![Stop the program and return the content as an HTTP response](../../.gitbook/assets/http.png)

{% hint style="info" %}
To trigger a function when a user goes to a URL, use the [HTTP Trigger](../triggers/http-trigger.md).
{% endhint %}

## ⚙ Setup

HTTP Response only works if the function was started by a [HTTP Trigger](../triggers/http-trigger.md). It will stop the program execution and return an HTTP response.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-8.16.02-pm.png)

You can set the response code. The default is 200, which indicates that the request was successful. You can also return a redirect code \(301\), which will allow you to redirect to a different endpoint.

Next, set the response type. The default is [HTML](html.md), but you can also return JSON data to implement a REST API.

Finally, set the content that you want to return in the "Response Content" field.


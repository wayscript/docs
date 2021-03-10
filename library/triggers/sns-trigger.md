---
description: >-
  Seamlessly integrate Amazon SNS service with your favorite APIs, databases,
  and programming languages, using WayScript.
---

# SNS Trigger

![ Provides a low-cost infrastructure for the mass delivery of messages](../../.gitbook/assets/download%20%281%29.png)

## ⚙ **Setup**

### 📥 Input your SNS Topic ARN

![](../../.gitbook/assets/screen-shot-2021-03-09-at-5.07.26-pm.png)

**You will need to sign in to your amazon SNS console and copy the ARN string to the input box**

For more information on how to configure Amazon SNS, Check the following link below:

[https://docs.aws.amazon.com/sns/latest/dg/sns-configuring.html](https://docs.aws.amazon.com/sns/latest/dg/sns-configuring.html)

### 📌 **Subscribe to the ARN topic with the endpoint labeled**

* **Get your Wayscript API key**

         Your Wayscript API key can be found by clicking the setting icon from your left panel

![](../../.gitbook/assets/screen-shot-2021-03-09-at-5.12.25-pm.png)

![Replace YOUR-API-KEY with the api copied from above](../../.gitbook/assets/screen-shot-2021-03-09-at-5.07.13-pm.png)

* **Copy your endpoint to a new Amazon SNS subscription**

![](../../.gitbook/assets/screen-shot-2021-03-09-at-7.25.28-pm.png)

## 📤**Output**

```graphql
Topic Notification = { messageID: String,
                       message: String,
                       subject: String,
                       topicArn: String,
                       timestamp: String,
                       signatureVersion: String,
                       signature: String
                       signingCertURL: String,
                       unsubscribeURL: String, }
```


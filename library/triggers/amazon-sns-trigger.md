---
description: >-
  Seamlessly integrate Amazon Simple Notification Service (SNS) with your
  favorite APIs, databases, and programming languages, using WayScript.
---

# Amazon SNS Trigger

![Provides a low-cost infrastructure for the mass delivery of messages](../../.gitbook/assets/sns.jpeg)

## ⚙ **Setup**

### 📥 Input your SNS Topic ARN

![](../../.gitbook/assets/screen-shot-2021-03-12-at-5.04.58-pm.png)

**You will need to sign in to your amazon SNS console and copy the ARN string to the input box**

For more information on how to configure Amazon SNS, refer to the link below:

[https://docs.aws.amazon.com/sns/latest/dg/sns-configuring.html](https://docs.aws.amazon.com/sns/latest/dg/sns-configuring.html)

### 📌 **Subscribe to the ARN topic with the provided endpoint**

![](../../.gitbook/assets/screen-shot-2021-03-12-at-5.07.39-pm.png)

* \*\*\*\*[**Get your WayScript API key**](../../account-management/managing-your-api-key.md)\*\*\*\*

         Your WayScript API key can be found by clicking the settings icon on the left navigation bar.

![](../../.gitbook/assets/screen-shot-2021-03-09-at-5.12.25-pm.png)

* **Copy your endpoint to a new Amazon SNS subscription**

![](../../.gitbook/assets/screen-shot-2021-03-09-at-7.25.28-pm.png)

## 📤**Output**

```graphql
Topic_Notification = { messageID: String,
                       message: String,
                       subject: String,
                       topicArn: String,
                       timestamp: String,
                       signatureVersion: String,
                       signature: String
                       signingCertURL: String,
                       unsubscribeURL: String, }
```


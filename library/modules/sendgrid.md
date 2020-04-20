---
description: Email API
---

# SendGrid



![](../../.gitbook/assets/sendgrid.png)

## Authentication

Click 'Add an Account' and enter a name for your Key and your SendGrid API Key.

## Simple Email

The simple email function allows you to send 'simple emails'. The **Email Body** TextArea accepts HTML. 

#### Advanced

You can change the content type from HTML \(text/html\) to plaintext \(text/plain\)

## Custom Input \(Advanced\)

SendGrid can accept highly custom email inputs. You are able to pass a Struct Variable to SendGrid with any data you want. 

**Sample Input Format:**

```python
{
  "personalizations": [
    {
      "to": [
        {
          "email": "test@example.com"
        }
      ],
      "subject": "Sending with SendGrid is Fun"
    }
  ],
  "from": {
    "email": "test@example.com"
  },
  "content": [
    {
      "type": "text/plain",
      "value": "and easy to do anywhere, even with Python"
    }
  ]
}
```




---
description: Integrate Push Notifications with your WayScript Programs
---

# Pushbullet

![Push Notifications Made Easy](../../.gitbook/assets/pushbullet.png)

## ⚙ **Setup** <a id="setup"></a>

### ​🗝 Input or Select an API Key <a id="input-or-select-an-api-key"></a>

**You will need your account access token to send notifications through the Pushbullet Module**

This key can be found [here](https://app.datadoghq.com/account/settings#api).

### ​  **Modes** <a id="choose-your-organization"></a>

### **Send a Push**

### 📥 Inputs <a id="inputs"></a>

* **Device Identity** - Send the Push to a Specific Device. If left empty all selected.
* **Title -** The title of the push notification
* **Body -** The message of the push notification

### 📤 Outputs <a id="outputs"></a>

```text
Push_response = {
  active         : Bool,
  body           : String,
  created        : Float,
  direction      : String,
  dismissed      : Bool,
  iden           : String,
  modified       : Float,
  receiver_email : String,
  receiver_email_normalized : String,
  receiver_iden  : String,
  sender_email   : String,
  sender_email_normalized   : String,
  sender_iden    : String,
  sender_name    : String,
  title          : String,
  type           : String
}
```


---
description: >-
  Seamlessly integrate Calendly with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Calendly

![Business Scheduling Software](../../.gitbook/assets/calendly%20%281%29.png)

## 🔑 Connecting your Calendly Account

You will need your Calendly API key to connect your account. You can find this key under your [integrations](https://calendly.com/integrations).

## ⚙ Modes

### 📆 Get User Events

#### 📤 Output

```graphql
user_events = [ {
    type: String,
    id: String,
    attributes: {
            name          : String,
            description   : String,
            duration      : Int,
            slug          : String,
            color         : String,
            active        : String,
            created_at    : String,
            updated_at    : String,
            url           : Url,
    }
} ]        
```




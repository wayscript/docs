---
description: 'Pass Calendly events to other modules and functions, all inside of WayScript.'
---

# Calendly

![Business Scheduling Software](../../.gitbook/assets/calendly.png)

## 🔑 Connecting your Calendly Account

You will need your calendly API key to connect your account. You can find this key under your [integrations](https://calendly.com/integrations).

## ⚙ Modes

### 📆 Get User Events

#### 📤 Output

```graphql
user_events = [ {
    type  :   String,
    id    :   String,
    attributes    :   {
            name          :   String,
            description   : String,
            duration      : Int,
            slug          : String,
            color         : String,
            active        : String,
            created_at    : String,
            updated_at    : String,
            url           : Url,
                    }
            }
    ]        
```




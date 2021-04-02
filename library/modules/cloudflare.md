---
description: >-
  Seamlessly integrate Cloudflare web security and external facing applications
  with your favorite APIs, databases, and programming languages, using
  WayScript.
---

# Cloudflare

![Web Infrastructure and Security](../../.gitbook/assets/cloudflare.png)

##   ⚙ **Setup**

**To setup Cloudflare, you'll need your API Token generated from your Cloudflare** [**User Profile 'API Token' Page**](https://dash.cloudflare.com/profile/api-tokens)**.**

## \*\*\*\*⚡ **Modes**

### ❤ Get Health ****check Events for a Load Balancer

####   📤 Output

```graphql
LB_Events = {
  success: Bool,
  errors: [],
  messages: [],
  result: [
    {
      id: Int,
      timestamp: Datetime,
      pool: {
        id: String,
        name: String,
        healthy: Bool,
        changed: Bool,
        minimum_origins: Int
      },
      origins: [
        {
          name: String,
          address: String,
          ip: String,
          enabled: Bool,
          healthy: Bool,
          failure_reason: String,
          changed: Bool
        }
      ]
    }
  ]
}
```

### 💸 Get Billing History

#### 📤 Output

```graphql
Billing_History = {
  success: Bool,
  errors: [],
  messages: [],
  result: [
    {
      id: String,
      type: String,
      action: String,
      description: String,
      occurred_at: Datetime,
      amount: Float,
      currency: String,
      zone: {
        name: String
      }
    }
  ]
}
```

### 📔 Get User Audit Logs

#### 📤 Output

```graphql
User_Audit_Logs = {
  success: Bool,
  errors: String,
  messages: [],
  result: [
    {
      id: String,
      action: {
        type: String,
        result: Bool
      },
      actor: {
        id: String,
        email: String,
        type: String,
        ip: String
      },
      newValue: String,
      oldValue: String,
      owner: {
        id: String
      },
      resource: {
        type: String,
        id: String
      },
      interface: String,
      metadata: {
        zone_name: String,
        type: String,
        name: String,
        value: String
      },
      when: String
    }
  ]
}
```

### 🗺 List All Zones

#### 📤 Output

```graphql
All_Zones = {
  success: true,
  errors: [],
  messages: [],
  result: [
    {
      id: String,
      name: String,
      development_mode: Int,
      original_name_servers: [ String ],
      original_registrar: String,
      original_dnshost: String,
      created_on: Datetime,
      modified_on: Datetime,
      activated_on: Datetime,
      owner: {
        id: { },
        email: { },
        type: String
      },
      account: {
        id: String,
        name: String
      },
      permissions: [ String ],
      plan: {
        id: String,
        name: String,
        price: Float,
        currency: String,
        frequency: String,
        legacy_id: String,
        is_subscribed: Bool,
        can_subscribe: Bool
      },
      plan_pending: {
        id: String,
        name: String,
        price: Float,
        currency: String,
        frequency: String,
        legacy_id: String,
        is_subscribed: Bool,
        can_subscribe: Bool
      },
      status: String,
      paused: Bool,
      type: String,
      name_servers: [ String ]
    }
  ]
}
```

### 🔧 List Workers

#### 📥 Inputs <a id="inputs"></a>

* **Cloudflare Account ID** - Your account Identifier. Needs permissions: com.cloudflare.edge.worker.script.list

####   📤 Output

```graphql
All_Workers = {
  success: Bool,
  errors: [],
  messages: [],
  result: [
    {
      id: String,
      etag: String,
      created_on: Datetime,
      modified_on: Datetime
    }
  ]
}
```


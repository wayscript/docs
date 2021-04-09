---
description: Send SMS Campaigns automatically using wayscript.
---

# Bulk SMS

![Get Your Message Across with BulkSMS](../../.gitbook/assets/bulk_sms_logo_vector.png)

##  **Setup** <a id="setup"></a>

**To setup BulkSMS, you'll need your API Token generated from your BulkSMS account.**  _**Settings &gt; Developer Settings &gt; API Tokens**_

##   **Modes** <a id="modes"></a>

### ​  Send Message <a id="get-health-check-events-for-a-load-balancer"></a>

####  Output <a id="output"></a>

```graphql
SMS_Send_Response = [
  {
    "from": {
      "type": String,
      "address": String
    },
    "to": [
      {
        "type": String,
        "address": String,
        "fields": [ String ]
      }
    ],
    "routingGroup": String,
    "encoding": String,
    "longMessageMaxParts": Int,
    "body": String,
    "userSuppliedId": String,
    "protocolId": String,
    "messageClass": String,
    "deliveryReports": String
  }
]
```


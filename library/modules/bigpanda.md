---
description: Integrate your BigPanda DevOps Automation Tools with WayScript
---

# BigPanda

![Event Correlation and Automation, powered by AIOps](../../.gitbook/assets/bigpanda_logo_vector.png)

##  ⚙  **Setup** <a id="setup"></a>

**To setup BigPanda, you'll need your API Token generated from your BigPanda** [**A**](https://dash.cloudflare.com/profile/api-tokens)**dmin Account.** 

 To find your token in BigPanda, log in as an administrator and then click the **Integrations** tab at the top of screen. Open the instructions for the Alerts API. Your token appears in the example headers

## **​**⚡ **Modes** <a id="modes"></a>

### ​ 🔎 **Retrieve an Incident** <a id="get-health-check-events-for-a-load-balancer"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Incident ID** - System-generated unique identifier for the incident.

####  📤 Output <a id="output"></a>

```graphql
Incident = {
  "id": String,
  "status": String,
  "active": Bool,
  "flapping": Bool,
  "resolved": Bool,
  "snooze": {
    "snoozed": Bool,
    "wake": null,
    "autoCancel": Bool
  },
  "startedOn": String,
  "changedOn": String,
  "updatedOn": String,
  "endedOn": null,
  "alerts": [
    {
      "alertId": String,
      "alertId": String,
      "alertId": String
    }
  ],
  "links": {
    "rel": String,
    "href": Url
  "expandable": [ String ]
}
```



### ✅ **Resolve an Incident** <a id="get-health-check-events-for-a-load-balancer"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Incident ID** - System-generated unique identifier for the incident.

####  📤 Output <a id="output"></a>

```graphql
Incident_Resolve_Response = None
```


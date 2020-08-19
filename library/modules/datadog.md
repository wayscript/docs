---
description: >-
  Seamlessly integrate Datadog with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Datadog

![Monitoring service for cloud-scale applications](../../.gitbook/assets/datadog.png)

## ⚙ **Setup**

**You will need to have access to two keys in order to return data from the Datadog API:**

* **App Key** - Gives access to interacting with the Datadog Agent.
* **API Key** - Unique to your organization

Both of these keys can be found [here](https://app.datadoghq.com/account/settings#api).

## \*\*\*\*🤖 **Modes**

### **Get a Monitor's Details** 

#### 📤 Output

```graphql
Get_Monitor = {
    "created"   : String,
    "creator"   : {
        "email"     : String,
        "handle"    : String,
        "name"      : String
    } ,
    "deleted"   : String,
    "id"        : Int,
    "message"   : String,
    "modified"  : String,
    "multi"     : Bool,
    "name"      : String,
    "options"   : {
        "aggregation"   : {
        "group_by"      : String,
        "metric"        : String,
        "type"          : String
        } ,
    "device_ids"            : [ String ],
    "enable_logs_sample"    : Bool,
    "escalation_message"    : String,
    "evaluation_delay"      : Int,
    "include_tags"          : Bool,
    "locked"                : Bool,
    "min_failure_duration"  : String,
    "min_location_failed"   : Int,
    "new_host_delay"        : Int,
    "no_data_timeframe"     : Int,
    "notify_audit"          : Bool,
    "notify_no_data"        : Bool,
    "renotify_interval"     : Int,
    "require_full_window"   : Bool,
    "synthetics_check_id"   : Int,
    "threshold_windows"     : {
    "recovery_window"   : String,
    "trigger_window"    : String
    } ,
    "thresholds"        : {
        "critical"          : Float,
        "critical_recovery" : Float,
        "ok"                : Float,
        "unknown"           : Float,
        "warning"           : Float,
        "warning_recovery"  : Float
    } ,
    "timeout_h": Int
    } ),
    "overall_state": String,
    "query": String,
    "tags"  : [ String ],
    "type"  : String
    } 
```

### **Get All Monitor Details**

#### 📥 Inputs

* **Group States** - Accepts "all", "alert", "warn" and "no data"
* **Name** - String to filter monitors
* **Tags** - Comma-separated list indicating what tags should be filtered
* **Monitor Tags** - Comma-separated list indicating what service or tags
* **With Downtimes** - If set to True,  then the returned data includes all current downtime
* **ID Offset** - Monitor ID offset
* **Page** - The page to start paginating from
* **Page Size** - Number of pagination results

#### 📤 Output

```graphql
Get_All_Monitors = {
    "created"   : String,
    "creator"   : {
        "email"     : String,
        "handle"    : String,
        "name"      : String
    } ,
    "deleted"   : String,
    "id"        : Int,
    "message"   : String,
    "modified"  : String,
    "multi"     : Bool,
    "name"      : String,
    "options"   : {
        "aggregation"   : {
        "group_by"      : String,
        "metric"        : String,
        "type"          : String
        } ,
    "device_ids"            : [ String ],
    "enable_logs_sample"    : Bool,
    "escalation_message"    : String,
    "evaluation_delay"      : Int,
    "include_tags"          : Bool,
    "locked"                : Bool,
    "min_failure_duration"  : String,
    "min_location_failed"   : Int,
    "new_host_delay"        : Int,
    "no_data_timeframe"     : Int,
    "notify_audit"          : Bool,
    "notify_no_data"        : Bool,
    "renotify_interval"     : Int,
    "require_full_window"   : Bool,
    "synthetics_check_id"   : Int,
    "threshold_windows"     : {
    "recovery_window"   : String,
    "trigger_window"    : String
    } ,
    "thresholds"        : {
        "critical"          : Float,
        "critical_recovery" : Float,
        "ok"                : Float,
        "unknown"           : Float,
        "warning"           : Float,
        "warning_recovery"  : Float
    } ,
    "timeout_h": Int
    } ),
    "overall_state": String,
    "query": String,
    "tags"  : [ String ],
    "type"  : String
    } 
```


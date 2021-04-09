---
description: Integrate Your Site's Errors with WayScript's Rollbar Module
---

# Rollbar

![Proactively discover, predict, and remediate errors with real-time, AI-assisted workflows](../../.gitbook/assets/rollbar_vector_logo.png)

## ⚙️ **Setup** <a id="setup"></a>

**To setup Rollbar, you'll need your API Token generated from your Rollbar Account.**

Operations performed at the level of the account require an account-specific access token. These can be found and managed at {Account name} Settings -&gt; Account Access Tokens. Account access tokens can have the following scopes:

* **Read -** Supports all GET operations at the account level
* **Write** - Supports all POST, PUT, PATCH, and DELETE operations at the account level.

## **​**⚡ **Modes** <a id="modes"></a>

### ​ 📖 List All Items <a id="get-health-check-events-for-a-load-balancer"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Assigned User** - If not empty, only items assigned to the specified user will be returned
* **Environment -** If not empty, only items in the specified environment will be returned
* **Level** - If not empty, only items with the specified level will be returned. Valid values: `debug`, `info`, `warning`, `error`, `critical`
* **Status -**  If not empty, only items with the specified status will be returned. Valid values: `active`, `resolved`, `muted`, `archived`

For full inputs information, please reference Rollbar's [Get Items documentation](https://explorer.docs.rollbar.com/#operation/list-all-items).

####  📤 Output <a id="output"></a>

```graphql
All_Items = {
  "err": Int,
  "result": {
    "page": Int,
    "instances": [
      {
        "id": Int,
        "project_id": Int,
        "item_id": Int,
        "timestamp": Int,
        "version": Int,
        "data": {},
        "billable": Int
      }
    ]
  }
} 
```



### ​ 🆔 List An Item By ID <a id="get-health-check-events-for-a-load-balancer"></a>

#### 📥 Inputs <a id="inputs"></a>

* **ID -** Unique ID of the item

####  📤 Output <a id="output"></a>

```graphql
All_Items = {
  "err": Int,
  "result": {
    "page": Int,
    "instances": [
      {
        "id": Int,
        "project_id": Int,
        "item_id": Int,
        "timestamp": Int,
        "version": Int,
        "data": {},
        "billable": Int
      }
    ]
  }
} 
```



### ➕ List All Occurrences <a id="get-health-check-events-for-a-load-balancer"></a>

####  📤 Output <a id="output"></a>

```graphql
All_Items = {
  "err": Int,
  "result": {
    "page": Int,
    "instances": [
      {
        "id": Int,
        "project_id": Int,
        "item_id": Int,
        "timestamp": Int,
        "version": Int,
        "data": {},
        "billable": Int
      }
    ]
  }
} 
```



### 🔴 Get All Top Items <a id="get-health-check-events-for-a-load-balancer"></a>

####  📤 Output <a id="output"></a>

```graphql
All_Items = {
  "err": Int,
  "result": {
    "page": Int,
    "instances": [
      {
        "id": Int,
        "project_id": Int,
        "item_id": Int,
        "timestamp": Int,
        "version": Int,
        "data": {},
        "billable": Int
      }
    ]
  }
} 
```



### 🔸 Get a Project <a id="get-health-check-events-for-a-load-balancer"></a>

#### 📥 Inputs <a id="inputs"></a>

* **ID -** Project ID

####  📤 Output <a id="output"></a>

```graphql
All_Items = {
  "err": Int,
  "result": {
    "page": Int,
    "instances": [
      {
        "id": Int,
        "project_id": Int,
        "item_id": Int,
        "timestamp": Int,
        "version": Int,
        "data": {},
        "billable": Int
      }
    ]
  }
} 
```


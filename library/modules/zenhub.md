---
description: >-
  Seamlessly integrate the GitHub issue management software, ZenHub, with your
  favorite APIs, databases, and programming languages, using WayScript.
---

# ZenHub

![GitHub Issue Management Software](../../.gitbook/assets/zenhub_100_100.png)

## 🔑 Connecting your ZenHub Account

You will need: 

* Repo ID - The easiest way to find this is to look at your ZenHub dashboard query strings. i.e.                ?repos=129749216
* [ZenHub account access token](https://app.zenhub.com/dashboard/tokens) 

## ⚙ Modes

### 🔢 Get Issues

####   📥 Inputs <a id="inputs"></a>

* Issue \#

\*\*\*\*📤 **Outputs**

```graphql
issue_data = {
    plus_ones :   [ string, ],
    is_epic   :   Bool,
    pipelines :   [ {
        name          :   String,
        pipeline_id   :   String,
        workspace_id  :   String,
    } ],
    pipeline      :   {
        name          :   String,
        pipeline_id   :   String,
        workspace_id  :   String,
    }
}
```

### 🔢 Get Issue Events

#### 📥 Inputs <a id="inputs"></a>

* Issue \#

\*\*\*\*📤 **Outputs**

```graphql
issue_events = [ {
    user_id           :   Int,
    type              :   String,
    created_at        :   String,
    workspace_id      :   String,
    from_estimate     :   {
        value             :   Float,
    },
    to_estimate       :   {
        value             :   Float( ),
    },
    from_pipeline     :   {
        name              :   String,
    },
    to_pipeline       :   {
        name              :   String,
    }
} ]
```

### 🔢 Set Issue Estimate

#### 📥 Inputs <a id="inputs"></a>

* Issue \#
* estimate 

\*\*\*\*📤 **Outputs**

A 444 response code is used for testing and demo modes.  A 200 response code would indicate a successful set estimate. 

```graphql
response_code = int
```

### 🔢 Get Epic Data

#### 📥 Inputs <a id="inputs"></a>

* Epic \#

**📤 Outputs**

```graphql
epic_data = {
    total_epic_estimates  : {
        value                 : Int,
    },
    estimate              : {
        value                 : Int
    },
    pipeline              : {
        workspace_id          : String,
        name                  : String,
        pipeline_id           : String
    },
    pipelines             : [ {
        workspace_id          : String,
        name                  : String,
        pipeline_id           : String
    } ],
    issues                : [ {
        issue_number          : Int,
        is_epic               : String,
        repo_id               : Int,
        estimate: {
        value     : Int
        },
    } ]
}
```



### 🔢 Get Release Reports

#### 📥 Inputs <a id="inputs"></a>

* Release I.D. String

**📤 Outputs**

```graphql
release_report = {
    release_id          : String,
    title               : String,
    description         : String,
    start_date          : String,
    desired_end_date    : String,
    created_at          : String,
    closed_at           : String,
    state               : String,
    repositories        : [ String ]
}
```


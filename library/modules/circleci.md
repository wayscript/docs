---
description: >-
  Seamlessly integrate CircleCI jobs and workflows with your favorite APIs,
  databases, and programming languages, using WayScript.
---

# CircleCI

![Continuous integration and delivery for any platform](../../.gitbook/assets/circleci-128x128.png)

##   ⚙ **Setup**

**You will need two keys to Interact with the CircleCI module:**

* **Circle Token** 
* **API Key** 

Both of these keys can be found [here](https://app.datadoghq.com/account/settings#api).

##  🤖 **Modes** <a id="modes"></a>

### 💎 **Get all Pipelines**  <a id="get-a-monitors-details"></a>

####   📥 Inputs <a id="inputs"></a>

* **Project Path \(Required\)** -  Project slug in the form `vcs-slug/org-name/repo-name`      Example: gh/CircleCI-Public/api-preview-docs
* **Project Branch \( Optional \)** -  The name of a vcs branch.
* **Page Token \( Optional \)** - A token to retrieve the next page of results.

#### ​ 📤 Output <a id="output"></a>

```text
all_pipeline_details = {
    "items": [ {
        "id" : String,
        "errors": [ {
            "type"       : String,
            "message"    : String,
            } ],
        "project_slug"   : String,
        "updated_at"     : Datetime,
        "number"         : Int,
        "state"          : String,
        "created_at"     : Datetime,
        "trigger" : {
        "type"           : String,
        "received_at"    : Datetime,
        "actor"          : {
            "login"      : String,
            "avatar_url" : String
            }
        },
        "vcs": {
            "provider_name": String,
            "target_repository_url": URL,
            "branch": String,
            "review_id": Int,
            "review_url": String,
            "revision": String,
            "tag": String,
            "commit": {
                "subject": String,
                "body": String
        },
        "origin_repository_url": URL
        }
    } ],
    "next_page_token": "string"
}
```

### \*\*\*\*🔨 **Trigger a Pipeline** <a id="get-a-monitors-details"></a>

####  📥 Inputs <a id="inputs"></a>

* **Project Path \(Required\)** -  Project slug in the form `vcs-slug/org-name/repo-name`      Example: gh/CircleCI-Public/api-preview-docs
* **Project Branch \( Optional \)** -  The name of a vcs branch.
* **X Attribution Login** - The login or user-readable identifier for the pipeline's triggerer.
* **X Attribution Actor ID** - The id the integration uses to identify the pipeline's triggerer.

#### ​ 📤 Output <a id="output"></a>

```text
created_pipeline = {
    "id"            : String,
    "state"         : String,
    "number"        : 0,
    "created_at"    : Datetime
}
```

### \*\*\*\*📌 **Approve a Workflow Job** <a id="get-a-monitors-details"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Job Approval Request ID** -  The ID of the job being approved. 
* **Job ID** -  The unique ID of the workflow.

#### ​ 📤 Output <a id="output"></a>

```text
job_approval_response = {
    "message": String
}
```


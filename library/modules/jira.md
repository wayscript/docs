---
description: Business Productivity Software designed to speed up your work tasks.
---

# Jira

![Automate Work Tasks and Issues](../../.gitbook/assets/jira_logo_100_100.png)

## ⚙️ Setup

* Your Jira URL will be space you want to access data in. \(ex:  https://{your\_input}.atlassian.net/ \)
* Then you will need to [create an API token on your Jira account](https://id.atlassian.com/manage-profile/security/api-tokens). 
* Your email address should be the same as the one used to login to Jira. 

### 📘 Get Application Roles

### 📤 Output

```graphql
Application_Roles = [ 
                       {
 groups : [
  String,
   ],
 name :   String,
 default_groups : [
  String, 
  ],
 selected_by_default : Bool,
 defined : Bool,
 number_of_seats : Int,
 remaining_seats : Int,
 user_count : Int,
 user_count_description : String,
 has_unlimited_seats : Bool,
 platform : Bool,
                        } 
                       ]
```

## 📘 Get Audit Records

### 📤 Output

```graphql
Audit_Records = [
                       {
                       
id   :   Float,
summary  :   String,
remote_address   :   String,
author_key   :   String,
author_account_id   :   String,
created   :   String,
category   :   String,
event_source   :   String,
description   :   String,
     }
        ]
```

## 📘 Get All Dashboards

### 📤 Output

```graphql
All_dashboards = [
                         {
id   :   Int,
is_favorite   :   String,
name   :   String,
popularity   :   Float,
self   :   String,
}
    ]
```

## 📘 Create a Dashboard

###  📥 Inputs <a id="inputs"></a>

* Name of Dashboard, string type. 
* Description of Dashboard, string type.

### 📤 Output

```graphql
Created_dashboard = {
id :   Float,
is_favorite :   String,
name :   String,
popularity :   Int,
self :   String,
}
```

## 📘 Search for Filters

### 📤 Output

```graphql
Application_Roles = [
                       {
                       
self   :   String,
id   :   String,
name   :   String,
description   :   String,
owner_self   :   String,
owner_key   :   String,
owner_account_id   :   String,
owner_name   :   String,
owner_avatar_url_48   :   String,
owner_avatar_url_24   :   String,
owner_avatar_url_16   :   String,
owner_avatar_url_32   :   String,
owner_display_name   :   String,
owner_active   :   String,
jql   :   String,
view_url   :   String,
search_url   :   String,
favourite    :   String,
favourited_count   :   Float,
                         }
                         ]
```

## 📘 Working with Issues

### 📥 Inputs <a id="inputs"></a>

* Issue ID, string type.

### 📤 Output - Issue Watchers

```graphql
Issue_Watchers = [
                       {
                       
self          :   Url,
account_id    :   String,
display_name  :   String,
active        :   String,
     }
        ]
```

### 📤 Output - Issue Attachments

```graphql
Issue_Attachments = [
                       {
                       
id            :   String,
self          :   Url,
file_name     :   String,
author        :   Url,
author_key           :   String,
author_account_id    :   String,
author_name          :   String,
avatar_url_48 :   Url,
avatar_url_24 :   Url,
avatar_url_16 :   Url,
avatar_url_32 :   Url,
display_name  :   String,
active        :   String,
created       :   String,
size          :   Float,
mime_type     :   String,
content       :   Url,
thumbnail     :   Url,
                       }
    ]
```



### 📤 Output - Issue Subtasks

```graphql
Issue_Subtasks = [
                       {
                       
id            :   Float,
type_id       :   Float,
type_name     :   String,
type_inward   :   String,
type_outward  :   String,
outward_issue_id      :   Float,
outward_issue_key     :   String,
outward_issue_self    :   Url,
outward_issue_status  :   String,
}
    ]
```



### 📤 Output - Issue Descriptions

```graphql
Issue_Descriptions = [
                       {
                       
type  :   String,
text  :   String,
}
    ]
```



### 📤 Output - Issue Projects

```graphql
Issue_Project = {
                       
self                      :   Url,
id                        :   Float,
key                       :   String,
name                      :   String,
project_avatar_url_48     :   Url,
project_avatar_url_24     :   Url,
project_avatar_url_16     :   Url,
project_avatar_url_32     :   Url,
project_category          :   Url,
project_id                :   Float,
project_name              :   String,
project_description       :   String,
simplified                :   String,
style                     :   String,
total_issue_count         :   Float,
last_issue_update_time    :   String,
}
```



### 📤 Output - Issue Comments

```graphql
Issue_Comments = [
 {
self                  :   String,
id                    :   Float,
author                :   Url,
author_acc_id         :   String,
author_display_name   :   String,
author_active         :   String,
author_text           :   String,
}
                        ]
```



### 📤 Output - Issue Links

```graphql
Issue_Links = [
 {
id                        :   String,
type_id                   :   Float,
type_name                 :   String,
type_inward               :   String,
type_outward              :   String,
outward_issue_id          :   String,
outward_issue_key         :   String,
outward_issue             :   Url,
outward_issue_status      :   String,
inward_issue_id           :   Float,
inward_issue_key          :   String,
inward_issue              :   Url,
inward_issue_status       :   String,
}))))
```


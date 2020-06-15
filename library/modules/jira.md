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
Application_Roles = [
                       {
                       
self          :   Url,
account_id    :   String,
display_name  :   String,
active        :   String,
     }
        ]
```






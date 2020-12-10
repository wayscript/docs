---
description: >-
  Seamlessly integrate GitHub with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# GitHub Trigger

![Run your script when GitHub events occur.](../../.gitbook/assets/github%20%282%29.png)

{% hint style="info" %}
To automate actions with GitHub, use the [GitHub module](../modules/github.md).
{% endhint %}

## 🔗 Link Your GitHub Account

When you drag in a GitHub Trigger for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the GitHub Trigger settings.
{% endhint %}

## ⚙ Settings

![Select the account and repository you want to work with.](../../.gitbook/assets/screen-shot-2019-08-09-at-3.39.02-pm.png)

### ![](../../.gitbook/assets/github%20%282%29.png) Modes

* **Branch Events**
  * Run program when:
    * A branch is created.
    * A branch is deleted.
* **Issue Events**
  * Run program when:
    * An issue is opened.
    * An issue is closed.
    * An issue is commented on.
    * An issue is assigned.
    * An issue is unassigned.
    * An issue is labeled.
    * An issue is unlabeled.
* **Pull Request Events**
  * Run program when:
    * A pull request is opened.
    * A pull request is closed.
    * A pull request review is submitted.
    * A pull request review is modified.
    * A pull request is commented on.
    * A pull request's code is commented on.
* **Push Events**
  * Run program when there is a push to a repository branch.
  * Select a branch
    * If you choose **Any Branch**, the program will run on any push to that repository.

## 📤 Outputs

* **Branch Events**

  ```graphql
  Branch = {
             ref         : String,
             master      : String,
             description : String
  }
  ```

  JSON Data - Raw JSON data received from the API.



* **Issue Events**

  ```graphql
  PR = {
          title    : String,
          url      : String,
          username : String,
          number   : Int  
  }
  ```

  JSON Data - Raw JSON data received from the API.



* **PR Events**

  ```graphql
  PR = {
          title    : String,
          url      : String,
          username : String,
          number   : Int  
  }
  ```

  JSON Data - Raw JSON data received from the API.



* **Push Events**

  ```graphql
  Push = {
           ref             : String,
           head            : String,
           before          : String,
           size            : Int,
           commit_shas     : [ String ],
           commit_messages : [ String ],
           commit_authors  : [ String ]
  }
  ```

  JSON Data - Raw JSON data received from the API.


# GitHub

![A web-based hosting service for version control using Git.](../../.gitbook/assets/github.png)

{% hint style="info" %}
To run your script when GitHub events occur, use the [GitHub Trigger](../triggers/github-trigger.md).
{% endhint %}

## 👤 Search for a User

### 📥 Inputs

Search for metrics on a user account by:

* Username
* Email
* GitHub URL

### 📤 Outputs

Create variables for:

* Name
* Company
* Blog
* Location
* Email
* Bio
* Number of Public Repos
* Number of Public Gists
* Number of Followers
* Number Following
* Names of Public Repos
* Public Repo URLs
* Most Popular Repo Name
* Most Popular Number of Stars
* Most Popular Number of Forks
* Most Popular Number Watches
* Most Popular Repo URL
* Raw JSON Data

## 🔎 Search for a Repo

### 📥 Inputs

Search for metrics on a repository by entering its Github URL.

### 📤 Outputs

Create variables for:

* Repo Name
* Repo Author Username
* Date Created
* Date of Last Update
* Date of Last Push
* Repo Size \(KB\)
* Number of Stars
* Subscriber Count
* Number of Forks
* Repo Language
* Open Issues Count
* Network Count
* Contributor Usernames
* Contributor URLs
* README content
* Raw JSON Data

## 🖊 Create an Issue

### 📥 Inputs

Create an issue for a repository by:

* GitHub Repo URL
* Title
* Content
* Labels
* Assignments 
* Milestone number

### 📤 Outputs

 Create variables for:

* Raw JSON Data

## 🖊 Edit an Issue

### 📥 Inputs

Edit an issue for a repository by:

* GitHub Repo URL
* Status
* Title
* Content
* Labels
* Assignments
* Milestone number

### 📤 Outputs

Create variables for:

* Raw JSON data

## 📓 Retrieve File Contents

### 📥 Inputs

Retrieve contents of a file in a repository by:

* GitHub Repo URL
* Path URL relative to GitHub URL
* Branch name

### 📤 Outputs

Create variables for:

* File Contents
* Raw JSON data




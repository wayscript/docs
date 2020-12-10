---
description: >-
  Seamlessly integrate Wikipedia with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Wikipedia

![Pull information from Wikipedia.](../../.gitbook/assets/wikipedia.png)

{% hint style="info" %}
Check out Wikipedia on [GitHub](https://github.com/goldsmith/Wikipedia).
{% endhint %}

## 🔎 Search for Wikipedia Pages by a Keyword

### 📥 Inputs

* Search Term
* Number of Results to Retrieve

### 📤 Outputs

* Article Titles

## 📖 Get Contents of a Wikipedia Page

### 📥 Inputs

* Wikipedia Page Title

### 📤Outputs

```graphql
Page = {
         contents : String, 
         summaries : String, 
         references : Any, 
         image_urls : [ String ]
}
```


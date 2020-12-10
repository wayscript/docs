---
description: >-
  Easily pull website data and integrate them with your favorite APIs,
  databases, and programming languages, using WayScript.
---

# Website Searcher

![Search a Website for Data. Powered by Beautiful Soup.](../../.gitbook/assets/site_siftter%20%281%29.png)

🔗Retrieve information from a given website and its linked pages.

## 🕵♀ Search Website for Data

### 📥 Inputs

* Website URL to Crawl
* Max Number of Pages to Search

### 📤 Outputs

```graphql
Crawl_Data = {  
               emails          : [ String ],
               twitter_handles : [ String ],
               third_party_urls: [ String ]
}
```

## 🔎 Search Website for Text and URLs

### 📥 Inputs

* Search Terms
* Website URL to Crawl
* Max Number of Pages to Search
* Search Type
  * Find All Instances
  * Stop Upon Discovery

### 📤 Outputs

* URLs

![](../../.gitbook/assets/screen-shot-2019-07-17-at-5.09.56-pm.png)


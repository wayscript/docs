---
description: >-
  Easily pull web articles and integrate them with your favorite APIs,
  databases, and programming languages, using WayScript.
---

# Article Extractor

![Pull text from a website.](../../.gitbook/assets/article_pull.png)

{% hint style="info" %}
Check out goose3 on [GitHub](https://github.com/goose3/goose3).
{% endhint %}

## 📥 Inputs

* **Website URL** - Enter the URL of the article you want to pull.

## 📤 Outputs

```graphql
Article = {
    title : String, 
    authors : [ 
        String, 
    ],
    description : String,
    article_text : String,
    domain : Url,
    keywords : String,
    links : [
        Url,
    ],
    raw_html : Html,
    image : Url,
    publish_date : Date,
    language : String,
}
```


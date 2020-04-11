---
description: >-
  Easily pull RSS feeds and integrate them with your favorite APIs, databases,
  and programming languages, using WayScript.
---

# RSS Feed

![Pull data from an RSS feed.](../../.gitbook/assets/rss_feed.png)

## 📥 Inputs

* **URL** - The URL for the RSS feed you want to pull.

## 📤 Outputs

* **Rss\_Feed** \(structure will vary depending on the content of the feed\)

```graphql
Rss_Feed = {
    feed : {
        language : String,
        title : String,
        title_detail : {
            type : String,
            language : String,
            base : URL,
            value : String
        },
        subtitle : String,
        subtitle_detail : {
            type : String,
            language : String,
            base : URL,
            value : String
        },
        links : [
            {
                rel : String,
                type : String,
                href : URL
            }
        ],
        link : URL,
        authors : [
            email : String
        ],
        author : String,
        author_detail : {
            email : String
        },
        publisher : String,
        publisher_detail : {
            email : String
        },
        docs : URL
    },
    entries : [
        title : String,
        title_detail : {
            type : String,
            language : String,
            base : URL,
            value : String
        },
        links : [
            {
                rel : String,
                type : String,
                href : URL
            }
        ],
        link : URL,
        summary : String,
        summary_detail : {
            type : String,
            language : String,
            base : URL,
            value : String
        },
        id : URL,
        published : Date,
        source : {
            href : URL,
            title : String
        }
    ],
    href : URL,
    status : Number,
    encoding : String,
    version : String
}
```

## 🎓 Tutorial

{% embed url="https://www.youtube.com/watch?v=ky56Z7UyqXU" %}


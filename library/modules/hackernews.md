---
description: >-
  Seamlessly integrate Hacker News with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Hacker News

![A social news website focusing on computer science and entrepreneurship.](../../.gitbook/assets/hacker_news.png)

## ⚙ Settings

### ![](../../.gitbook/assets/hacker_news.png) Mode

* Get Top Stories
* Get New Stories
* Get Best Stories

## 📥 Inputs

* Number of Stories - Input the number of results you would like returned as outputs. 
  * Note - When the program is not running, only 20 results will be returned. 

## 📤 Output

```graphql
Posts = [
    {
        title : String, 
        score : Int, 
        author : String, 
        url : Url, 
        id : Int, 
        descendants : Int, 
        kids : [
            Int,
        ],
        datetime : Date,
    },
]
```




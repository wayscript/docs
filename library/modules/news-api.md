# News API

![Get breaking news headlines, and search for articles from over 5,000 news sources and blogs.](../../.gitbook/assets/news_api.png)

## ⚙ Settings

#### What would you like to search?

* **Article Database** - We index every recent news and blog article published by over 30,000 different sources large and small, and you can search through them with this endpoint. This endpoint is better suited for news analysis and article discovery, but can be used to retrieve articles for display too.
* **Latest Articles** - Returns breaking news headlines for a country and category, or currently running on a single or multiple sources.

## 📥 Inputs

* **Number of Articles** - The number of articles to be returned. 
* **Sort By** 
  * Options - Most Recent, Most Relevant to Search Term, Most Recent
* **Topic To Search** - Enter the search term you want news articles on \(e.g. "Tesla"\)
  * required

## 📤Output

```graphql
Articles = [
    {
        title : String, 
        url : Url, 
        author : String, 
        description : String, 
        source : Url, 
        img_url : Url, 
        published_at : Date,
    },
]
```


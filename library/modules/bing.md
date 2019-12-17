# Bing

![Search the web with Bing.](../../.gitbook/assets/bing%20%281%29.png)

## 🔎 Search Term

Insert your search term into the Search Term input. This is equivalent to what you would enter in search bar in a Bing search. 

## 📤 Outputs

```graphql
Bing_Results = {
    web_results : [
        {
            name : String, 
            snippet : String,
            url : Url,
            date_last_crawled : Date,
        },
    ],
    video_results : [
        {
            name : String,
            description : String,
            date_published : Date,
            url : Url,
            view_count : Int,
            embed_html : Html,
            encoding_format : String,
            publisher : String,
        },
    ],
}
```


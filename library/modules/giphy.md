# Giphy

![GIPHY is your top source for the best &amp; newest GIFs &amp; Animated Stickers online.](../../.gitbook/assets/giphy.png)

{% hint style="info" %}
Check out the GIPHY [website](https://www.developers.giphy.com).
{% endhint %}

## ⚙ Mode

* **Single Random Result** - returns a single random result each time. 
  * This turns the Giphy outputs into [Single Items](../../getting_started/variables.md#single-item)
* **All Results** - All Results returns the top 25 results. 
  * This turns Giphy outputs in [Lists](../../getting_started/variables.md#lists)

## 📥 Inputs

* **Search Term** - This is the search term for the GIF you want. 

## 📤 Output

Single Random Result

```graphql
Gif = {
    title : String, 
    url : Url, 
    img : Html,
    rating : String, 
    id : String, 
}
```

All Results

```graphql
Gifs = [
    {
        title : String, 
        url : Url, 
        img : Html,
        rating : String, 
        id : String,
    },
]
```




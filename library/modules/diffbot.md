# Diffbot

![Turn websites into data in seconds.](../../.gitbook/assets/diffbot.png)

{% hint style="info" %}
Check out Diffbot on [GitHub](https://github.com/diffbot/diffbot-python-client).
{% endhint %}

## 📰 Extract Article Text

### 📥 Inputs

* **URL** - the website link you want to pull text from. \(E.g. wayscript.com\)

### 📤 Output

```graphql
Article = {
    title : String, 
    text : String, 
    date : Date, 
    html : Html, 
    tags : [
        String,
    ],
    icon : Url,
    url : Url, 
    type : String, 
}
```

## 🛒 Data from any Shopping or e-Commerce Product Page

### 📥 Inputs

* **URL** - the e-commerce website link you want to pull text from.

### 📤 Output

```graphql
Product = {
    title : String, 
    brand : String, 
    price : Float, 
    sku : String, 
    description : String, 
    image_url : Url, 
    availability : Bool,
}
```

\*\*\*\*

## 💬 Forum/Discussion/Product Conversations and Reviews

📃 This mode, pulls [lists](../../getting_started/variables.md#lists) of all of the posts on the forum page.

### 📥 Inputs

* **URL** - the forum link you want to pull text from.

### 📤 Output

```graphql
Posts = [
    {
        title : String, 
        author : String, 
        text : String, 
        url : Url, 
        date : Date,
        html : Html, 
        language : String, 
    },
]
```


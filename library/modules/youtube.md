# YouTube

![Work with YouTube data.](../../.gitbook/assets/youtube%20%281%29.png)

## 🔗 Link Your YouTube Account

When using a YouTube module for the first time, follow the prompt to authorize access.

{% hint style="info" %}
You can add additional accounts from the YouTube module settings.
{% endhint %}

## 🔎 Search for Videos by Keyword

### 📥 Inputs

* Search Term
* Maximum Number of Results
* Advanced:
  * Sort Order
  * Filter Results by U.S. Zip Code

### 📤 Output

```graphql
YouTube_Videos = [
    {
        title : String,
        channel : String,
        url : Url,
        description : String,
        published_at : Date,
        channel_id : String, 
        video_id : String,
    },
]
```

## 📺 Get Data About a Video

### 📥 Inputs

* Video URL

### 📤 Output

```graphql
YouTube_Video = {
    title : String, 
    channel : String, 
    description : String, 
    published_at : Date, 
    channel_id : String, 
    tags : [
        String,
    ],
    comment_count : Int,
    dislike_count : Int,
    favorite_count : Int,
    like_count : Int,
    view_count : Int,
}
```

## 💬 Get Comments on a Video

### 📥Inputs

* Video URL
* Maximum Number of Comments
* Advanced: Sort Order
  * Time
  * Relevance

### 📤Output

```graphql
Video_Comments = [
    {
        text : String, 
        author_display_name : String, 
        author_channel_id : String, 
        author_channel_url : String, 
        like_count : String, 
        published_at : Date, 
        reply_count : Int,
    },
]
```

## 👤 Get Data on a Channel \(User Account\)

### 📥Inputs

* Account/Channel Username

### 📤Output

```graphql
YouTube_Channel = {
    description : String, 
    view_count : Int,
    comment_count : Int, 
    subscriber_count : Int, 
    video_count : Int,
    url : Url,
}
```




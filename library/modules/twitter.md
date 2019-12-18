# Twitter

![A social media platform.](../../.gitbook/assets/twitter.png)

{% hint style="info" %}
Check out twython on [GitHub](https://github.com/ryanmcgrath/twython).
{% endhint %}

## 🔎 Search for a Word or \#Hashtag

### ⚙ Settings

* **Number of Tweets** - Enter the number of tweets you want to receive.

#### 💡 Advanced

* **Ignore Retweets** - Ignore retweets of posts. Will only return original tweets.
* **Ignore Replies** - Ignore replies to posts. Will only return original tweets.
* **Result Type** - Specifies what type of search results you would prefer to receive. The default value is "Mixed".
  * Options: Recent, Popular, Mixed

### 📥 Inputs

* **Search Term** - Excepts Keywords, \#hashtags, or @usernames.
  * Max length: 500 characters.

![](../../.gitbook/assets/screenshot-2019-07-16-16.18.16.png)

### 📤 Output

```graphql
Tweets = [
    {
        content : String, 
        username : String, 
        name : String, 
        id : Int,
        retweet_count : Int,
        follower_count : Int, 
        favorite_count : Int,
        date : Date,
        url : String, 
        hashtags : [
            String,
        ],
        user_mentions : [
            String,
        ],
        url_mentions : [
            String,
        ],
    },
]
```

## 🐦 Tweet History of a User

### 📥 Inputs

* **Include Retweets** - Select whether you want to include retweets or not. 
  * Options: Yes, No
* **Username** - Enter the name of the User whose tweet history you want. 
  * Note: @ not required in username

### 📤 Outputs

* **Tweets**
* **Persons Names**
* **Number of Post Retweets**
* **Number of Times Favorites**
* **Date/Time of Posts**
* **Other Usernames Mentioned in Post -** a [List](../../getting_started/variables.md#lists) of lists all usernames in the tweet. 
* **URLs Mentioned in Tweet** - a [List](../../getting_started/variables.md#lists) of lists all urls in the tweet. 
* **Hashtags** - a [List](../../getting_started/variables.md#lists) of lists all hashtags in the tweet. 

## 👥 Get Data on a User by Username

### 📥Inputs

* **Username** - Enter the name of the User whose tweet history you want. 
  * Note: @ not required in username

### 📤 Outputs

* **Profile Description**
* **User Website**
* **Number of Followers**
* **Number Following**
* **Number of Tweets**
* **Number of Likes**
* **User Location**
* **Name**
* **Profile Image URL**
* **Is Verified**
* **Account Created Date**

## 📖 Get User Followers and Following

{% hint style="warning" %}
Due to Twitter's Rate Limiting Policy, this is a slow operation \(takes 1 minute per 200 users in either category... so be selective with this mode\).
{% endhint %}

This mode lets you pull in lists of the usernames of a users followers and friends \(people the user follows\).

### Inputs

* **Username -** Enter the name of the User \(e.g. [WayScriptHQ](https://twitter.com/WayScriptHQ)\)
  * Note: @ not required in username

### Outputs

* **Following** - A list of usernames of everyone the user is following.
* **Followers** - A list of usernames of everyone following the user.

## 💬 Post a Twitter Status

### 📥 Inputs

* **Message** - Enter in the message field what you want your status to be.

![Posting a Twitter Status](../../.gitbook/assets/screenshot-2019-07-16-16.23.32.png)

## ⌛ My Profile Timeline

This mode pulls data from your own timeline.

### 📤 Outputs

* **Tweets**
* **Number of Post Retweets**

## 👍 Like a Tweet

This mode allows you to like a tweet by its tweet id. This ID can be pulled from the [Twitter Search](twitter.md#search-for-a-word-or-hashtag) functionality or from the URL of the tweet.

![Tweet ID of a Tweet from URL](../../.gitbook/assets/screenshot-2019-09-13-16.59.02.png)

### Inputs

* **Tweet ID** - The ID of the tweet from Twitter. 


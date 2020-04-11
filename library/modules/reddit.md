---
description: >-
  Seamlessly integrate Reddit with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Reddit

![The front page of the internet.](../../.gitbook/assets/reddit%20%281%29.png)

## 👤 Data About My Account

### 📤 Output

```graphql
Account = {
    description : String,
    karma : Int,
    comment_karma : Int,
    link_karma : Int,
    subscribers : Int,
    coins : Int,
    created_utc : Date,
    gold_credits : Int,
    icon_img : Url,
    id : String,
    inbox_count : Int,
    is_employee : Bool,
    is_suspended : Bool,
    name : String,
    num_friends : Int,
}
```

## 🔎 Search a Subreddit

### 📥 Inputs

* **Subreddit Name** - The name of the subreddit \(ex - '[programming](https://www.reddit.com/r/programming/)'\)
* **Sort By**
  * **Options** - Hot, Top, New, Controversial, Rising, Random
* **Number of Posts to Return** - How many posts you want to be outputted. 

### 📤 Outputs

```graphql
Subreddit = {
    num_subscribers : Int,
    active_accounts : Int,
    public_description : String,
    description : String,
    advertiser_category : String,
    all_original_content : Bool,
    banner_background_color : String,
    banner_img : Url,
    community_icon : Url,
    created_utc : Date,
    display_name : String,
    display_name_prefixed : String,
    emojis_enabled : Bool,
    header_img : Url,
    hide_ads : Bool,
    icon_img : Url,
    id : String,
    lang : String,
    link_flair_enabled : Bool,
    over18 : Bool,
    spoilers_enabled : Bool,
    url : Url,
    wiki_enabled : Bool,
}
```

```graphql
Subreddit_Posts = [
    {
        title : String, 
        date : Date. 
        author : String, 
        text : String, 
        score : Int, 
        upvotes : Int, 
        downvotes : Int, 
        num_comments : Int, 
        permalink : Url, 
        post_url : Url, 
        gilded : Int, 
        id : String, 
        is_video : Bool, 
        num_crossposts : Int, 
        num_reports : Int, 
        over18 : Bool, 
    },
]
```

## 👥 Data About Other Users

### 📥 Inputs

* **Account Name** - account name of the user. 

### 📤 Output

```graphql
Reddit_User = {
    description : String, 
    comment_karma : Int, 
    link_karma : Int, 
    karma : Int, 
    subscribers : Int, 
    created_utc : String, 
    icon_img : Url, 
    id : String, 
    is_employee : Bool, 
    is_friend : Bool, 
    is_gold : Bool, 
    moderator : Bool, 
    name : String, 
    verified : Bool,
}
```

## 📌 Get Posts from Other Users

Pull in the posts of a user by their username. 

### 📥 Inputs

* **Number of Posts to Return** - How many posts you want to be outputted. 
* **Account Name -** account name of the user. 

### 📤 Output

```graphql
Posts = [
    {
        title : String, 
        author : String, 
        text : String, 
        created_utc : Date, 
        score : Int, 
        upvotes : Int, 
        downvotes : Int, 
        num_comments : Int, 
        permalink : Url, 
        url : Url, 
        subreddit : String, 
        subreddit_subscribers : Int,
        over_18 : Bool,
        num_crossposts : Int,
    },
]
```

## 💬 Get Comments from Other Users

### 📥 Inputs

* **Number of Posts to Return** - How many posts you want to be outputted. 
* **Account Name -** account name of the user. 

### 📤 Output

```graphql
Comments = [
    {
        text : String, 
        author : String, 
        created_utc : Date, 
        score : Int, 
        num_comments : Int, 
        upvotes : Int, 
        downvotes : Int, 
        subreddit : String, 
        permalink : Url, 
        url : Url, 
    },
]
```


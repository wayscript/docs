---
description: Manage your students and courses with wayscript
---

# Udemy Instructors

![Online Education Website](../../.gitbook/assets/udemy_instructor.png)

## 🔑 Connecting your Udemy Instructor Account

To connect, you will need your Udemy Instructor API key. You can generate your api key [here](https://www.udemy.com/instructor/account/api/). Please note this is the instructor API key and not the affiliate api key. 

## ⚙ Modes

### ✏️ Get Course List

#### 📤 Output

```graphql
instructor_courses = [ {
       "_class" : String,
      "id"      : String,
      "title"   : String,
      "url"     : String,
      "is_paid" : Bool,
      "published_title"     : String,
      "visible_instructors" : [ {
          "_class"  : String,
          "id"      : String,
          "title"   : String,
          "name"    : String,
          "locale"  : String
        } ] 
} ]        
```

### 📝 Get Course Questions

#### 📤 Output

```graphql
course_questions = [ {
  "_class"    : String,
  "id"          : String,
  "created"     : String,
  "title"       : String,
  "body"        : String,
  "num_replies" : Int,
  "num_follows" : Int,
  "num_reply_upvotes": Int,
  "modified"    : String,
  "last_activity": String,
  "is_read"     : Bool,
  "course"      : {
    "_class"    : String,
    "id"        : String,
    "title"     : String,
    "url"       : String
  } ,
  "is_instructor"   : Bool,
  "num_upvotes"    : Int
} ]
```


---
description: >-
  Seamlessly integrate Scryfall with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Scryfall

![Search for Magic: The Gathering Cards](../../.gitbook/assets/scryfall%20%282%29.png)

## 🔎 Search for cards

### ⚙ Settings

* **Search Term** - Name of magic card

### 📤 Output

```graphql
Cards = [ 
    {
     name         : String,
     mana_cost    : String,
     cmc          : Number,
     price        : Number,
     text         : String,
     related      : [ String ],
     related_id   : [ String ],
     scryfall_url : Url
    }, 
]
```

## ![](../../.gitbook/assets/scryfall%20%282%29%20%282%29.png)Get Data About All MTG Sets

### 📤 Output

```graphql
Sets = [ 
    {
     name         : String,
     code         : String,
     card_count   : Int,
     release_date : Date
    }, 
]
```


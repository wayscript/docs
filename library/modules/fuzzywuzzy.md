---
description: >-
  Seamlessly integrate FuzzyWuzzy with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# FuzzyWuzzy

![Fuzzy string matching like a boss. ](../../.gitbook/assets/fuzzy_wuzzy.png)

{% hint style="info" %}
Check out FuzzyWuzzy on [GitHub](https://github.com/seatgeek/fuzzywuzzy).
{% endhint %}

## ![](../../.gitbook/assets/fuzzy_wuzzy%20%281%29.png) About

FuzzyWuzzy is a string similarity matching library. In other words, it tells you how similar two pieces of text are \(and some other functionality\).

FuzzyWuzzy uses Levenshtein Distance to calculate the differences between sequences in a simple-to-use package.

## ⚖ Simple Ratio

| **Text\*** | **Text** | **Ratio** |
| :--- | :--- | :--- |
| this is a test | this is a test! | 97 |

### 📥 Inputs

* Text \(Required\)
* Text

### 📤 Outputs

* Ratio -  _\*\*_This number quantifies the similarity of the two pieces of text. 

![Ratio Returned is 97](../../.gitbook/assets/screenshot-2019-07-16-21.51.36.png)

## 💠 Partial Ratio

| **Text\*** | Text | **Ratio** |
| :--- | :--- | :--- |
| this is a test | this is a test! | 100 |

### 📤 Outputs

* **Ratio**

## ↔ Token Sort Ratio

| **Text**\* | Text | Ratio | Token Sort Ratio |
| :--- | :--- | :--- | :--- |
| fuzzy wuzzy was a bear | wuzzy fuzzy was a bear | 91 | 100 |

### 📤 Outputs

* **Ratio**
* **Token Sort Ratio**

## 🏠 Token Set Ratio

| **Text\*** | Text | Token Set Ratio |
| :--- | :--- | :--- |
| fuzzy was a bear | fuzzy fuzzy was a bear | 100 |

### 📤 Outputs

* **Token Set Ratio**

## 💻 Process

| [Text](../../getting_started/variables.md#single-item) | [Choices](../../getting_started/variables.md#lists) | Extract One Choice | Extract One Ratio |
| :--- | :--- | :--- | :--- |
| new york jets | Atlanta Falcons, New York Jets, Dallas Cowboys, New York Giants | New York Jets | 100 |

### 📥 Inputs

* Text - [Single Item Variable](../../getting_started/variables.md#single-item)
* Choices - [List](../../getting_started/variables.md#lists)

### 📤 Outputs

* **Extract One Choice** - The closest matching item from **Choices** is returned
* **Extract One Ratio** - The ratio of the match


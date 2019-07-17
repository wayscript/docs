---
description: >-
  Fuzzy string matching like a boss. It uses Levenshtein Distance to calculate
  the differences between sequences in a simple-to-use package.
---

# FuzzyWuzzy

{% hint style="info" %}
Opensource - Here is a link to the [GitHub Repo](https://github.com/seatgeek/fuzzywuzzy)
{% endhint %}

FuzzyWuzzy is a string similarity matching library. In other words, it tells you how similar two pieces of text are \(and some other functionality\).

## Simple Ratio

| **Text\*** | **Text** | **Ratio** |
| :--- | :--- | :--- |
| this is a test | this is a test! | 97 |

#### Inputs

* Text
  * Required
* Text

#### Outputs

* Ratio -  ****This number quantifies the similarity of the two pieces of text. 

![Ratio Returned is 97](../../.gitbook/assets/screenshot-2019-07-16-21.51.36.png)

## Partial Ratio

| **Text\*** | Text | **Ratio** |
| :--- | :--- | :--- |
| this is a test | this is a test! | 100 |

## Token Sort Ratio

| **Text**\* | Text | Ratio | Token Sort Ratio |
| :--- | :--- | :--- | :--- |
| fuzzy wuzzy was a bear | wuzzy fuzzy was a bear | 91 | 100 |

#### Outputs

* **Ratio**
* **Token Sort Ratio**

## Token Set Ratio

| **Text\*** | Text | Token Set Ratio |
| :--- | :--- | :--- |
| fuzzy was a bear | fuzzy fuzzy was a bear | 100 |

#### Outputs

* **Token Set Ratio**

## Process

| [Text](../../introduction/variables.md#single-item) | [Choices](../../introduction/variables.md#lists) | Extract One Choice | Extract One Ratio |
| :--- | :--- | :--- | :--- |
| new york jets | Atlanta Falcons, New York Jets, Dallas Cowboys, New York Giants | New York Jets | 100 |

#### Inputs

* Text - [Single Item Variable](../../introduction/variables.md#single-item)
* Choices - [List](../../introduction/variables.md#lists)

#### Outputs

* **Extract One Choice** - The closest matching item from **Choices** is returned
* **Extract One Ratio** - The ratio of the match


# RegEx

## 📥 Inputs

* **String** - sequence of characters
* **Pattern** - sequence of characters representing the regular expression
  * Example to match the start of a string: "^Hello"
  * Example to match the end of a string: "Bye$"
  * Example to match an exact word: "word"
  * Example to match an alphanumeric sequence: "\[a-zA-Z0-9\]\*"
  * Example to match 3 to 6 digits: "\[0-9\]{3,6}"
  * Example to match a pattern with an optional preceding letter: "\[c\]?art"
  * Example to match character groups: "\(c\|m\|h\)at"
* **Global** - search for all non-overlapping matches 
* **Multiline** - match on each line separated by the newline character of the string input
* **Case Insensitive** - match on the lowercase version of the string input
* **Match Dot to All Characters** - match the dot character to all characters, including newline character

## 📤 Outputs

Create variables for:

* **Has Match** - boolean indicating whether a match was found with the specified pattern
* **Matches Found** - list of matches found 
* **Indices of Matches Found** - list of indices for each match found
* **Captured Groups** - list of captured groups for each match found


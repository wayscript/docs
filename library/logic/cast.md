# Cast

![Change variable type from one to another.](../../.gitbook/assets/cast.png)

## ⚙ Settings

* **Variable Input** - Accepts WayScript variables created in previous steps of your script.
* **Cast To -** The type of the variable after the cast module step. 

{% hint style="info" %}
 The Python equivalent error of "Could not convert X type to Y type" will return a blank variable of type "Any" within WayScript
{% endhint %}

## ✏ Examples

| Create Variable Input | Cast to Type | Result  |
| :--- | :--- | :--- |
| var = 4 | String | "4" |
| var = 4 | Float | 4.0 |
| var = "4" | Int | 4 |
| var = "4" | Float | 4.0 |
| var = {"key":"value"} | String | "{"key":"value"}" |
| var = {"key":"value"} | Float | No return - Any Type |
| var = {"key":"value"} | Boolean | True |
| var = {} | Boolean | False |

{% hint style="info" %}
 Casting logic resembles that of Python's. \(e.g. Empty dictionaries return false when casted to Bool type and true when the dictionary contains entries. \)
{% endhint %}


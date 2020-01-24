# Python

![Write Python code.](../../../.gitbook/assets/python_128x128.png)

{% hint style="info" %}
See [Code Editors](../../../getting_started/code-editors.md) for more information on composing code in WayScript.
{% endhint %}

## ![](../../../.gitbook/assets/create_var.png) Inputs

WayScript's python editor lets you reference [Variables](../../../getting_started/variables.md) that exist in your program. To do this, you can reference them through the **inputs dictionary**.

As an example, let's create a variable called "Location" and set a value of "Brooklyn, NY"

![](../../../.gitbook/assets/screenshot-2019-07-16-14.03.23.png)

You can reference the Location variable in your python script with this code:

```python
location = inputs[ "Location" ]
```

More abstractly, you reference any variable with the format:

```python
var = inputs[ "<var_name>" ] 
```

## ![](../../../.gitbook/assets/python.png) Outputs

You can also output data from your python scripts and turn these into variables that can be used by other [Modules](../../../getting_started/modules.md) in your program. 

You can do this with the **outputs dictionary** in the following format:

```python
outputs[ "<Var Name>" ] = variable

# example
from datetime import datetime
outputs[ "Date" ] = str( datetime.today() )
```

## ▶ Running Python

While working on your script, you can press the "Run Code" button inside the Python module to run the Python code and see updated results.

## 📦 Adding Additional Requirements

The Python module comes with [many pre-installed Python Libraries](libraries.md). However, if you would like to use a module that isn't already installed, you can declare those requirements in the "Requirements.txt" file.

Declare these requirements as you would in a [pip Requirements File](https://pip.pypa.io/en/stable/user_guide/#requirements-files), using the [Requirements File Format](https://pip.pypa.io/en/stable/reference/pip_install/#requirements-file-format).

![](../../../.gitbook/assets/screen-shot-2020-01-23-at-6.19.16-pm.png)

{% hint style="info" %}
For faster code execution, only add requirements that aren't already [pre-installed](libraries.md) in the Python module.
{% endhint %}


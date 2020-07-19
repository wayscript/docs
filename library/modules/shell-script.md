---
description: >-
  Seamlessly integrate your Bash shell script with your favorite APIs,
  databases, and programming languages, using WayScript.
---

# Shell Script

![Run a shell script.](../../.gitbook/assets/shell_script%20%281%29.png)

{% hint style="info" %}
See [Code Editors](../../getting_started/code-editors.md) for more information on composing code in WayScript.
{% endhint %}

## ![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LjqAStevvF6Z9bkhj6b%2F-Lk-zqgbODOYzqT7c2HW%2F-Lk-za4o3gvO4s5pclGi%2Fcreate_var.png?alt=media&token=85257162-dd84-494a-9ae1-392886209e6e)Working with Variables <a id="working-with-variables"></a>

###  📥 Inputs <a id="inputs"></a>

WayScript's shell script editor lets you reference [Variables](https://docs.wayscript.com/getting_started/variables) that exist in your program. To do this, you can reference them through the **variables** [**associative array**](https://www.gnu.org/software/bash/manual/html_node/Arrays.html).

As an example, let's create a variable called "Location" and set a value of "Brooklyn, NY"

![](../../.gitbook/assets/screen-shot-2020-07-16-at-3.50.52-pm.png)

You can then reference the Location variable in your shell script:

```bash
LOCATION=${variables["Location"]}
```

More abstractly, you reference any variable with the format:

```bash
MY_VAR=${variables[ "<var_name>" ]}
```

![You can also reference a WayScript variable as a shortcut for the associative array syntax.](../../.gitbook/assets/screen-shot-2020-07-19-at-1.00.40-pm.png)

### ​ 📤 Outputs <a id="outputs"></a>

#### ​ ![](../../.gitbook/assets/shell_script%20%281%29.png) Return Data from Your Shell Script <a id="return-data-from-your-javascript"></a>

You can also output data from your shell script and turn these into variables that can be used by other [Modules](https://docs.wayscript.com/getting_started/modules) in your program.

You can do this with the **variables associative array** in the following format:

```bash
variables["<Var Name>"]=value
```

![You can also reference a WayScript variable to simplify assignment to an existing variable. ](../../.gitbook/assets/screen-shot-2020-07-19-at-1.02.37-pm.png)

## ▶ Running a Shell Script <a id="running-javascript"></a>

While working on your script, you can press the "Run Code" button inside the module to run the script and see updated results.

## ↘ Calling Other Scripts

You can add and reference other shell scripts in your File Browser. For example, suppose you have a file called `foo.sh`.

![](../../.gitbook/assets/screen-shot-2020-07-19-at-1.18.52-pm.png)

You can run `foo.sh` from `scratch.sh`:

```bash
./foo.sh
```

![Example of calling another script in your File Browser.](../../.gitbook/assets/screen-shot-2020-07-19-at-1.20.55-pm.png)


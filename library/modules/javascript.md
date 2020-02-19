# JavaScript



![Write JavaScript code.](../../.gitbook/assets/javascript_code.png)

{% hint style="info" %}
See [Code Editors](../../getting_started/code-editors.md) for more information on composing code in WayScript.
{% endhint %}

## ![](../../.gitbook/assets/create_var.png)Working with Variables

###  📥 Inputs

WayScript's JS editor lets you reference [Variables](../../getting_started/variables.md) that exist in your program. To do this, you can reference them through the **variables dictionary**.

As an example, let's create a variable called "Location" and set a value of "Brooklyn, NY"

![](../../.gitbook/assets/screen-shot-2019-08-19-at-1.21.56-pm.png)

You can reference the Location variable in your JavaScript with this code:

```javascript
location = variables[ "Location" ];

// Or, as a JS object
location = variables.Location;
```

More abstractly, you reference any variable with the format:

```javascript
const my_var = variables[ "<var_name>" ];
```

### 📤 Outputs

#### ![](../../.gitbook/assets/javascript_code.png) Return Data from Your JavaScript

You can also output data from your JS code and turn these into variables that can be used by other [Modules](../../getting_started/modules.md) in your program. 

You can do this with the **variables dictionary** in the following format:

```javascript
variables[ "<Var Name>" ] = variable;

// example
const currentTime = new Date();
variables[ "Date" ] = currentTime.toISOString();
```

#### 🖨 Output Raw JavaScript Code

You can output the raw JavaScript code from the code editor by enabling the "JavaScript Code" output. This is useful when [building a website using WayScript](https://www.youtube.com/watch?reload=9&v=OrZMjdVhFfA&feature=youtu.be) and inserting JavaScript into [HTML](html.md).

![Raw JS Code Output as a Variable](../../.gitbook/assets/screen-shot-2019-08-30-at-2.58.48-pm.png)

{% hint style="info" %}
If you are building JS for a webpage, you might _only_ want to output the code as text and not run it at all. This can be achieved by disabling the "Run Code" setting. 
{% endhint %}

## ▶ Running JavaScript

While working on your code, you can press the "Run Code" button inside the module to run the JavaScript and see updated results.

## 📦 Adding Dependencies

If you would like to use an [npm](https://www.npmjs.com/) module in your code, you can declare those dependencies in the "Requirements.txt" file.

Declare these dependencies on separate lines, using the format you would for an [npm-install](https://docs.npmjs.com/cli/install) command.

![](../../.gitbook/assets/screen-shot-2020-01-23-at-6.21.14-pm.png)

You can then consume these packages in your code:

```javascript
const wayscript = require( 'wayscript' );

wayscript.apiKey = 'YOUR_API_KEY';

let programId = 1234;
wayscript.runProgram( programId );
```

## ↘ Importing Code from Other Files

You can import code from the other JavaScript files in your File Browser. For example, suppose you have a file called `foo.js`, which has an exported function `bar`.

![](../../.gitbook/assets/screen-shot-2020-02-18-at-2.11.18-pm.png)

You can import and use the `bar` method in `scratch.js` by using a relative import:

```javascript
const foo = require('./foo');
```

![Example of importing and using the function &quot;bar&quot; from &quot;foo.js&quot;](../../.gitbook/assets/screen-shot-2020-02-18-at-2.11.28-pm.png)


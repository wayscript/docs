---
description: >-
  Easily build forms that integrate with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Form Trigger

![Build a GUI form and run your script when the form data is submitted.](../../.gitbook/assets/form.png)

## ⚙ Setup

### Title and Description

You can add a title and description to your form to create context for your users. 

Once your trigger is activated, you can press the '**View Form**' button to be taken to the live, public endpoint for your form. This form can be shared with others you want to use your form. 

{% hint style="info" %}
Form Descriptions support markdown!
{% endhint %}

### Adding Form Inputs

{% hint style="info" %}
In order to add an input, press **+ Add a Form Element.** You can add as many form elements as you want.
{% endhint %}

There are four input types you can currently choose from:

#### 1\) Text Input

![Sample Text Input](../../.gitbook/assets/screenshot-2020-02-18-11.31.06.png)

**Title** - There are a few different parts of the element to notice. First, you can create a **title** for the input \(in the example image we are asking 'What is your name?'. 

**Required** - You can set required to On/Off - if on, a user is required to enter an answer before they can submit the form. 

**Placeholder** - This is just placeholder text you can enter for the text input. 

![](../../.gitbook/assets/screenshot-2020-02-18-11.35.32.png)



#### **2\) Text Area**

The Text Area element behaves identically to the [Text Input](form-trigger.md#1-text-input) element. The key difference is it provides space for a longer form answer. 

#### **3\) Selector**

The Selector element can be used to give users of the form a set of choices to choose from. In order to add options to your selector, press the **+ Add an Option** button. You can add as many options as you want. 

![Setting up a Selector](../../.gitbook/assets/screenshot-2020-02-18-11.45.23.png)

![Result on the Form](../../.gitbook/assets/screenshot-2020-02-18-11.46.21.png)

#### **4\) Radio Buttons**

The Radio element behaves exactly like the [Selector](form-trigger.md#3-selector) element above. The form will render the options as radio buttons. 

![Radio button example](../../.gitbook/assets/screenshot-2020-02-18-11.49.15.png)

#### 5\) File Upload

The File Upload element allows users to attach and upload a file when submitting your form. You can choose between a pdf filter, or specify a custom list of file extensions you wish to allow users to upload.

![File Upload Example](../../.gitbook/assets/screen-shot-2020-07-29-at-1.40.38-pm.png)

The File Upload element will output a [Struct](../../getting_started/variables.md#structs) of the following form:

```graphql
File = {
    filename  : String, 
    bytes     : Bytes,
    extension : String,
    mimetype  : String,
}
```

### Advanced Inputs

**CSS** - You can customize the CSS of your form for your own look and feel. 

## 👁🗨 View Form

In order to view your live form, make sure your trigger is active and then press the **View Form** button.

![Trigger is On, press View Form](../../.gitbook/assets/screenshot-2020-02-18-11.55.35.png)

## ⚙ Advanced Settings

### 🔗 Endpoints

When setting up the Form Trigger, you can create as many named endpoints as you like. If you don't provide a name for your endpoint, the trigger will match the root URL. All endpoint names must be unique throughout your script to prevent ambiguity.

![](../../.gitbook/assets/screen-shot-2020-03-13-at-1.15.21-pm.png)

To access your endpoints, use the program ID as a subdomain of **wayscript.io**. For example, in the image above, you can trigger your script by hitting either [https://16233.wayscript.io/](https://16233.wayscript.io/) or [https://16233.wayscript.io/custom\_endpoint](https://16233.wayscript.io/custom_endpoint).

Remember to activate your trigger before using the endpoint!

### 🔐 Password-Protect your Form

If you would like your form to require a login to view, enable the "Password Protection" toggle.

A button to "Manage Login Credentials" will appear.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.39.21-pm.png)

Clicking this button will take you to "Login Credentials" section of the "Script Setup" tab, where you can manage the usernames and passwords that will allow people to log in to your endpoints.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.40.18-pm.png)

When you click "Add a credential," a new login will be automatically generated for you, including a username and randomly-generated password. You can choose to use these values, or edit them as you see fit.

![](../../.gitbook/assets/screen-shot-2019-11-12-at-7.41.50-pm.png)

When a user goes to access your form for the first time, they will now be prompted to login.

![Form Login Prompt](../../.gitbook/assets/screen-shot-2019-11-12-at-7.50.17-pm%20%281%29.png)

### Basic Authentication

If you password-protect your endpoints, you can use the credentials added above to access your endpoints by including an `Authorization: Basic` header in your request.

This header should follow the standard for [HTTP basic access authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). For example, suppose your Username is "**captain@wayscript.com**" and your Password is "**letmein**," you would create the Authorization header by:

1. Joining the Username and Password into a single string, separated by a semicolon: **`captain@wayscript.com:letmein`**
2. Encoding that string in Base64: **`Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=`**
3. Passing that encoded string to your custom endpoint by including the `Authorization: Basic Y2FwdGFpbkB3YXlzY3JpcHQuY29tOmxldG1laW4=` header in your request.

These headers are also displayed for you under each password in the "Login Credentials" section of the "Script Setup" tab.

### Authenticating Using Your API Key

If your endpoint is not public, you can also use your [WayScript API Key](../../account-management/managing-your-api-key.md) to access your endpoints api call by including an `Authorization: Bearer` header in your request.

For example, if your WayScript API Key is **`fhAEdGT9EbFDh_migcrukZ1Vb28rLFKqt9AxOiq9bdQ`**, you would include the `Authorization: Bearer fhAEdGT9EbFDh_migcrukZ1Vb28rLFKqt9AxOiq9bdQ` header in your request.

## 📤 Output

The Form Trigger will output a Struct of the responses to your form. 

```graphql
Form = {
    input_1 = 'Answer One',
    input_2 = 'Answer Two',
    ...
}
```

### 🔣 Raw Request Data

The raw form data submitted to the Form Trigger endpoint.

## 🎓 Tutorial

{% embed url="https://www.youtube.com/watch?v=rO4gY4CzW2o" %}


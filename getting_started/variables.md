# Variables

## What is a Variable?

> **"Variables** are used to store information to be referenced and manipulated in a computer program. They also provide a way of labeling data with a descriptive name, so our programs can be understood more clearly by the reader and ourselves. It is helpful to think of variables as containers that hold information. This data can then be used throughout your program."
>
> -[LaunchSchool](https://launchschool.com/books/ruby/read/variables)

## Create Variable Setup

Drag the [Create Variable](../library/logic/variables/create-variable.md) module into your program flow diagram.

![The Create Variable module is in your Logic Panel](../.gitbook/assets/screenshot-2019-07-15-12.28.05.png)

WayScript will automatically display the Settings Panel for your [Create Variable](../library/logic/variables/create-variable.md) step. This is where you are going to set up your variable. 

![](../.gitbook/assets/screenshot-2019-07-15-12.36.06.png)

## Single Item

For this example, we are going to assign a **Variable Name** called "Location" and set the **Variable Value** to "Brooklyn, NY". Feel free to put in your own location instead.

![](../.gitbook/assets/screenshot-2019-07-15-12.41.46.png)

After setup, your new variable will appear in the **Variables Panel.** You can now use this variable in your program. 

![All accessible variables are in your Variables Panel](../.gitbook/assets/screenshot-2019-07-15-13.00.21.png)

{% hint style="info" %}
The green border indicates that this variable is a single item.
{% endhint %}

#### Example of using a Single Item Variable

Your variable is is available for reference at any future step in your program flow. In this example, we can now print a message which contains the Location variable. 

![](../.gitbook/assets/screenshot-2019-07-15-15.40.49.png)

You can begin typing the variable name to select it, or you can drag the variable from the Variable Panel into the Content to Print input.

![Your variable data is printed when the program runs.](../.gitbook/assets/screenshot-2019-07-15-15.36.21.png)

## Lists

### What is a list?

A list \(also called an array\) is a data structure used to store multiple pieces of information in an ordered sequence where each has a unique 'position' \(also called index\) in the list. List variables can even store other variables.

### Creating a List

In your [Create Variable](../library/logic/variables/create-variable.md) Settings, change your mode to a **List of Items.**

![](../.gitbook/assets/screenshot-2019-07-15-15.46.17.png)

In this example, we'll create a list with **Variable Name** "Grocery List" and add items as **Variable Values.** The use cases for lists will be discussed more in the [Looping](looping-iteration.md) ****section of the docs.

![You can add as many items to a list as you want. ](../.gitbook/assets/screenshot-2019-07-15-15.49.28.png)

![](../.gitbook/assets/screenshot-2019-07-15-15.49.50.png)

Your Grocery List is now a variable that can be used in your program.

{% hint style="info" %}
The blue border indicates that this variable is a list and the number badge indicates its length.
{% endhint %}

## Variable Types

Variables currently have the following types:

* Text
* Number
* Date/Time

You explicitly define the type of your variables. Note - if you are building a [List](variables.md#lists) - the variable type defines the type of data in _each_ list item. WayScript performs type validation on each of your items. As an example, if you create a Number Type, but set your variable value to a non-number, the value will be rejected. This is important because many [modules](../library/modules/) often only accept inputs of particular types. 

![](../.gitbook/assets/screenshot-2019-07-16-09.56.45.png)

## Power-User Features

If you know some coding, you can more rapidly build a variable from the module shortcut dropdown by entering the definition directly. 

This power-user features matches the syntax of the Python programming language for strings and arrays. 

![](../.gitbook/assets/screenshot-2019-07-15-15.53.14.png)

![Press Enter to create your variable.](../.gitbook/assets/screenshot-2019-07-15-15.53.32.png)

{% hint style="info" %}
Press tab to open the shortcut dropdown at the end of your program.
{% endhint %}


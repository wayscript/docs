# Looping / Iteration

{% hint style="warning" %}
If you have not read about [WayScript Lists](variables.md#lists), please do so before continuing.
{% endhint %}

## What is a loop?

In programming, a **for-loop** is a control-flow statement directing your program to execute the loop's contents repeatedly. 🔁 

## Looping with WayScript

![](../.gitbook/assets/screenshot-2019-07-15-16.26.19.png)

The power of looping is easiest to demonstrate with an example.

### ![](../.gitbook/assets/create_var.png)Create a List

In this example, we build the same grocery list variable from the [WayScript Lists documentation](variables.md#lists). 

![Varialbes outlined in blue are lists.](../.gitbook/assets/screenshot-2019-07-15-15.49.50.png)

### ![](../.gitbook/assets/loop.png)Create a Loop

Drag in the Loop Module from the **Logic Panel** as the next step in your program flow. 

![](../.gitbook/assets/screenshot-2019-07-15-16.38.47.png)

In the **Loop Settings Panel**, select your Grocery List variable as an input to loop over. 

![You can add more lists to loop over by pressing the + button](../.gitbook/assets/screenshot-2019-07-15-16.42.28.png)

Notice how you now have a variable in your Variable Panel called **Grocery List Item.** In programming, this is known as an 'iterator' and can be used as a variable at any step inside of the loop. 

At each loop iteration, the value of **Grocery List Item** will change to the next item in the list. This loop will iterate four times, once for each item in the list. To make this more clear, let's print the value of **Grocery List Item** for each loop. To do this, we must drag the Print To Log module inside of the loop.

![](../.gitbook/assets/screenshot-2019-07-15-16.47.52.png)

In the Print To Log setup, let's print a sentence and include our **Grocery List Item** variable.

![](../.gitbook/assets/screenshot-2019-07-15-16.51.46.png)

Finally, let's add a print statement **after** the loop that says "I'm done shopping!"

![Notice how the final print is after the loop.](../.gitbook/assets/screenshot-2019-07-15-16.54.17.png)

### ▶Run Your Program

Press the "Run Main" button to run your program. Now, look at the results in the log. Notice how the loop ran four times, each time with the new value for your Grocery List Item variable. At the end, your "I'm done shopping!" line printed. 

![](../.gitbook/assets/screenshot-2019-07-15-17.14.51.png)


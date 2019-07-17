# List Actions

![Perform common programming operations on lists.](../../.gitbook/assets/list_actions%20%281%29.png)

{% hint style="info" %}
For more information on using WayScript Lists, see the [Introduction to Lists](../../getting_started/variables.md#lists).
{% endhint %}

## **Get List Length**

Outputs the number of elements that are in your list.

## **Get List Index by Value**

Searches your list for the given value.

### Outputs

* The index position of the first occurrence of the value. 
* A list of all the index positions where the value was found in the list.

{% hint style="info" %}
WayScript List indexes start at 0, so the first element in the list has an index of 0.
{% endhint %}

## **Get List Value by Index**

Outputs the value of the element at the given index in your list.

## **Extend List**

Adds each element in the selected variable to the end of your list.

**Example:** Adding \[ B, C \] to \[ A \] results in \[ A, B, C \]

## **Append List**

Adds the selected variable to the end of your list as a single element.

**Example:** Adding \[ B, C \] to \[ A \] results in \[ A, \[ B, C \] \]

## **Compare Lists**

Outputs a list of all the matching elements in the two lists selected.

## **Insert Value Into List at a Given Index**

Inserts the given value at the given index, shifting the following elements in your list to the right.

## **Make a Sub List**

Outputs a new list containing the elements from the starting index up to the ending index of the selected list.

**Example:**  
List = \[ A, B, C, D, E \]   
Starting index = 1   
Ending index = 4   
Sub List = \[ B, C, D \]

## **Get Number of Times a Value Occurs in the List**

Outputs the number of times the given value occurs in the selected list.

## **Remove an Element at a Given Index**

Removes the element at the given index in the selected list. 

Outputs the element that was removed from the list.

## **Remove First Occurrence of an Element in the List**

Removes the first occurrence of the given value in the selected list.


# CSV

![Read and Write to CSV files.](../../.gitbook/assets/csv_reader.png)

## Read File

Import columns from a CSV as WayScript variables.

### Select or Upload CSV

CSV files on your account will appear as options. Use the 'Upload File' button to add a new file.

### Create Variables

Once a file is selected to read, A table with the file's contents will appear in the Outputs section. 

#### Ignore Headers

Specify whether or not to ignore the first line of the file when assigning variables.

#### Assigning Variables

Naming a column in the table creates a [List](../../introduction/variables.md#lists) variable with that name containing all entries in that column.

![](../../.gitbook/assets/screen-shot-2019-07-17-at-11.24.14-am.png)

![Note that first row is ignored in creating variables](../../.gitbook/assets/screen-shot-2019-07-17-at-11.25.14-am.png)

## Write File

### Select File

Use the file dropdown to select an existing file on your account or create a new one.

### Include Headers

If checked, the variable name will be written as the first row of each column.

### Write Mode

1. Add to File: Every time the program runs, new rows of data will be added to the bottom of the CSV file.
2. Replace File: Every time the program runs, the file will be cleared before writing new data.

{% hint style="info" %}
Headers will only be written when the file is blank. 

If 'Include Headers' is selected, changing a variable name when adding to an existing and non-empty file will not replace the header row.
{% endhint %}

### Adding variables

Each time the CSV Module executes in Write Mode, one row of data is added.  

![](../../.gitbook/assets/screen-shot-2019-07-17-at-11.49.04-am.png)

{% hint style="info" %}
To write each entry of list to a new row, use a [Loop](../../introduction/looping-iteration.md).
{% endhint %}

### Preview

As variables are added and removed, the Outputs section displays a preview of what will be written.


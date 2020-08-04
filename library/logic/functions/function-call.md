# Function Call

![Call a function.](../../../.gitbook/assets/func_call.png)

## ![](../../../.gitbook/assets/func_call.png) **Select a Function to Call**

The function dropdown will contain the available functions to call in your program.

![Select a function to call](../../../.gitbook/assets/screen-shot-2019-07-16-at-12.54.08-pm.png)

## \*\*\*\*⚙ **Choose Your Inputs and Outputs**

Once you select a function to call, the inputs and outputs for that function will populate in the settings panel. Select your inputs and outputs as you would for any module.

![Function Inputs and Outputs](../../../.gitbook/assets/screen-shot-2019-07-16-at-12.55.52-pm.png)

## 🔀 Running a Function Asynchronously

The **Run Async** setting in the Function Call module allows you to asynchronously call a function that runs an "expensive" or long-running task.  
  
One common use-case for this setting is to immediately return a `200 Success` response from the [HTTP Response](../../modules/http-response.md) module, while performing a long-running task in the background, on another thread.

{% hint style="warning" %}
It is currently not possible to return outputs from an asynchronous function call.
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=1\_GdSYwQZvs" caption="Learn how to Run Asynchronous Tasks in your WayScript Workflows" %}


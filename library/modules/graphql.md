---
description: >-
  Seamlessly integrate GraphQL with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# GraphQL

![Execute queries against a GraphQL API.](../../.gitbook/assets/graphql.png)

## Inputs

1. **API URL** - This is the root url for the API query. 
2. **Headers -** You can create the custom headers that you pass with the API request. 

   1. **Note - Variables use raw syntax here so String Pills need to be wrapped in quotes.**

   \*\*\*\*

3.  **Code -** Enter your GraphQL query here.

#### Advanced:

1. **Use JSON -** Defaults to True.
2. **Fetch Schema from Transport -** Defaults to True.
3. **Number of Retries** - Defaults to 3
   1. **Options:** 0, 1, 2 ,3

## **Output**

1. **Response -** A struct will return with the JSON response from your API query. 

## Example

* Some example GraphQL APIs can be found in this [Github repository](https://github.com/APIs-guru/graphql-apis).

Using the API URL found [here](https://countries-274616.ew.r.appspot.com), we can access country calling codes with a GraphQl like:

```text
query {
      CallingCode {
        name
        countries {
          name
        }
      }
    }
```

Which would return a response like this:

```text
{ "CallingCode": [
    { "name" : Int Type,
    "Countries" : [
     {
    "name" : String Type
    }
   ]
  }
 ]
}
    
```

A public script using this can be found [here](https://wayscript.com/user/derricks/S_qrNUw8).


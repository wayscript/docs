---
description: Integrate Monday Automations seamlessly into your WayScript Workflows.
---

# Monday

![A collaborative Work Management Platform](../../.gitbook/assets/monday-200x200.png)

### 

##  🔗 Link Your Monday Account <a id="link-your-trello-account"></a>

To link your Monday account, you will need:

* Your account name
* Your [API V2 Token](https://monday.com/developers/v2#authentication-section-api-v2-token)

## Inputs

* Monday works similar to the [GraphQL Module](https://docs.wayscript.com/library/modules/graphql) in that it takes GraphQL inputs.

## **Output**

1. **Response -** A struct will return with the JSON response from your API query. 



## Example

```text
query {
  boards (ids:544471285) {
      activity_logs {
          id
          event
          data
      }
  }
}
```

Which would return a response like this:

```text
{ "id" : "....",
"event" : "....",
"data" : "..."
}

```




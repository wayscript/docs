---
description: >-
  Seamlessly integrate Zendesk with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Zendesk

![Create anonymous requests using Zendesk](../../.gitbook/assets/zendesk.png)

## 📥Inputs

* **Recipient's Subdomain** - The Zendesk subdomain of the person/organization that will receive the request
* **Subject -** The subject of the request
* **Body -** The message of the request

### 📤 Outputs <a id="outputs"></a>

* **Request ID -** The ID of the request that was just generated
* **JSON Data \(Advanced\) -** Raw JSON recieved from the endpoint

```text
request = {
    url : Url
    id : Int
    status : String
    priority : String
    type : String
    subject : String
    description : String
    organization_id : Int
    via : Object
    custom_fields : Array
    requester_id : Int
    collaborator_ids : Array
    email_cc_ids : Array
    is_public : Bool
    due_at : String
    can_be_solved_by_me : Bool
    created_at : String
    updated_at : String
    recipient : String
    followup_source_id : Int
    assignee_id : Int
    ticket_form_id : Int
    fields : Array
}
```

{% hint style="info" %}
If an error occurs, the full error message will be displayed as the JSON Data output.
{% endhint %}

Common errors include:

* **No help desk at ... -** Invalid recipient subdomain
* **Couldn't authenticate you -** The recipient does not accept anonymous requests
* **API rate limit exceeded** - Too many requests to the recipient subdomain were made in a given time frame




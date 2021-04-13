---
description: Integrate your Fundraising Campaigns with WayScript
---

# GiveButter

![](../../.gitbook/assets/givebutter.png)



##   ⚙️ **Setup** <a id="setup"></a>

**The Givebutter API uses API Keys to authenticate and perform requests. To authenticate requests, provide your API Key**

##  ⚡**Modes** <a id="modes"></a>

### ​🔔 **Get Transactions** <a id="get-health-check-events-for-a-load-balancer"></a>

####  📤 Output <a id="output"></a>

```text
​{
    "id": String,
    "campaign_id": Int,
    "team_id": String,
    "member_id": String,
    "first_name": String,
    "last_name": String,
    "email": String,
    "phone": String,
    "address": {
        "address_1": String,
        "address_2": String,
        "city": String,
        "state": String,
        "zipcode": String,
        "country": String
    },
    "status": String,
    "method": String,
    "amount": Int,
    "fee": Float,
    "fee_covered": Float,
    "donated": Float,
    "payout": Float,
    "currency": String,
    "created_at": String,
    "giving_space": {
        "id": Float,
        "name": String,
        "amount": Float,
        "message": String
    },
    "transactions": [
        {
            "id": String,
            "plan_id": String,
            "amount": Int,
            "fee": Float,
            "fee_covered": Float,
            "donated": Int,
            "payout": Int,
            "captured": Bool,
            "captured_at": String,
            "refunded": Bool,
            "line_items": [
                {
                    "type": String,
                    "subtype": String,
                    "description": String,
                    "quantity": Int,
                    "price": Float,
                    "discount": Float,
                    "total": Float
                },
                {
                    "type": String,
                    "subtype": String,
                    "description": String,
                    "quantity": Float,
                    "price": Float,
                    "discount": Float,
                    "total": Float
                }
            ]
        }
    ]
}
```

### **​**💸 **Get Payouts** <a id="get-health-check-events-for-a-load-balancer-1"></a>

####  📤 Output <a id="output-1"></a>

```text
{
    "id": String,
    "campaign_id": Int,
    "method": String,
    "status": String,
    "amount": Float,
    "fee": Float,
    "tip": Float,
    "payout": Float,
    "currency": String,
    "address": {
        "address_1": String,
        "address_2": String,
        "city": String,
        "state": String,
        "zipcode": String,
        "country": String
    },
    "memo": String,
    "completed_at": String,
    "created_at": String
}
```



### 🎫 **Get Tickets** <a id="get-health-check-events-for-a-load-balancer-1"></a>

####  📤 Output <a id="output-1"></a>

```text
{
    "id": String,
    "id_suffix": String,
    "name": String,
    "first_name": String,
    "last_name": String,
    "email": String,
    "phone": String,
    "title": String,
    "description": String,
    "price": Float,
    "pdf": String,
    "arrived_at": String,
    "created_at": String
}
```


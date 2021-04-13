---
description: >-
  Integrate your Coupon Campaigns with WayScript and Automatically Target your
  Audiences.
---

# CouponTools

![Digital Coupon Marketing Platform](../../.gitbook/assets/coupontools.png)

## ⚙️ **Setup** <a id="setup"></a>

**To setup CouponTools, you will need your client id and client secret. Both of these keys can be found under your account page.** 

##  ****⚡ **Modes** <a id="modes"></a>

### ​📱**Send Push Notification to All** <a id="get-health-check-events-for-a-load-balancer"></a>

#### ​📥 Inputs <a id="inputs"></a>

* **Campaign ID** - Can be found in the list of all campaigns. Example: cam\_12345
* **Campaign Message -** Your push notification message

####  📤 Output <a id="output"></a>

```text
{
	"status": {
		"status": String
	}
}
```



### 📢 **Send SMS Coupon** <a id="get-health-check-events-for-a-load-balancer"></a>

#### ​📥 Inputs <a id="inputs"></a>

* **Campaign ID** - Can be found in the list of all campaigns. Example: cam\_12345
* **Phone -** Add the mobile phone number in international E.164 notation.
* **Body -** The SMS body text. The unique coupon URL will be added to each message.

####  📤 Output <a id="output"></a>

```text
{
	"status": {
		"status": String
	},
	"campaign": String,
	"message": String,
	"phone": String,
	"single_use_code": String,
	"single_use_url": String,
	"action": String
}
```


---
description: >-
  Manage data from your various rental properties by linking Guesty and other
  services
---

# Guesty

![Guesty Simplifies Rental Management Tools](../../.gitbook/assets/guestyvectorlogo.png)

##   **Setup** <a id="setup"></a>

**To setup Guesty, you'll need your API Token generated from your Guesty.** To get this token, you can follow the [instructions provided by Guesty](https://support.guesty.com/en/article/generating-an-internal-api-token). 



## **​**⚡ **Modes** <a id="modes"></a>

### ​List All Listings <a id="get-health-check-events-for-a-load-balancer"></a>

####  📤 Output <a id="output"></a>

```text
All_Listings = {
    "results": [
        {
            "_id": String,
            "accommodates": Int,
            "bedrooms": Int,
            "beds": Int,
            "bathrooms": Int,
            "defaultCheckInTime": String,
            "defaultCheckOutTime": String,
            "propertyType": String,
            "roomType": String,
            "timezone": String,
            "nickname": String,
            "title": String,
            "accountId": String,
            "occupancyStats": [],
            "preBooking": [],
            "importedAt": String,
            "offeredServices": [],
            "calendarRules": {
                "rentalPeriods": [],
                "seasonalMinNights": []
            },
            "customFields": [],
            "active": Bool,
            "receptionistsService": {},
            "sales": {
                "salesService": {
                    "atPhones": []
                }
            },
            "pms": {
                "active": Bool,
                "cleaningStatus": {},
                "autoPayments": {
                    "policy": []
                },
                "tasks": {
                    "defaultTasks": []
                },
                "automation": {
                    "autoList": {},
                    "autoPricing": {},
                    "autoReviews": {},
                    "homeAutomation": {},
                    "calendarSmartRules": {},
                    "hooks": {},
                    "answeringMachine": {}
                }
            },
            "prices": {
                "currency": String,
                "basePrice": Int,
                "guestsIncludedInRegularFee": Int,
                "weeklyPriceFactor": Float,
                "monthlyPriceFactor": Float,
                "cleaningFee": Int,
                "securityDepositFee": Int,
                "extraPersonFee": Int
            },
            "terms": {
                "minNights": Int,
                "maxNights": Int
            },
            "amenitiesNotIncluded": [],
            "amenities": [],
            "pictures": [],
            "picture": {
                "thumbnail": Url
            },
            "address": {},
            "tags": [ String ],
            "pendingTasks": [],
            "integrations": [],
            "SaaS": {
                "autoRenew": Bool
            },
            "createdAt": String,
            "__v": Int,
            "isListed": Bool,
            "cleaningStatus": {
                "value": String
            },
            "publishedAddress": {},
            "cleaning": {},
            "publicDescription": {}
        }
    ],
    "title": String,
    "count": Int,
    "fields": String,
    "limit": Int,
    "skip": Int
}
```

### ​💸 Retrieve Listing Financials <a id="get-billing-history"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Listing ID** - Guesty Property Listing ID

#### ​📤 Output <a id="output-1"></a>

```text
Listing_Finc = {
    "guestsIncludedInRegularFee": Int,
    "currency": String,
    "basePriceUSD": Int,
    "basePrice": Int,
    "securityDepositFee": null,
    "extraPersonFee": Int,
    "weeklyPriceFactor": Float,
    "monthlyPriceFactor": Float,
    "cleaningFee": {
        "lastUpdated": Datetime,
        "value": {
            "valueType": String,
            "multiplier": String,
            "formula": Int
        },
        "airbnb": {
            "value": {
                "formula": Int,
                "multiplier": String,
                "valueType": String,
                "_id": String
            }
        },
        "rentalsUnited": {
            "status": String,
            "value": {
                "valueType": String,
                "multiplier": String,
                "formula": Int,
                "_id": String
            },
            "homeAway": {
                "value": {
                    "formula": Int,
                    "valueType": String,
                    "multiplier": String,
                    "_id": String
                }
            },
            "expedia": {
                "value": {
                    "formula": Int,
                    "valueType": String,
                    "multiplier": String,
                    "_id": String
                }
            },
            "despegar": {
                "value": {
                    "formula": Int,
                    "valueType": String,
                    "multiplier": String,
                    "_id": String
                }
            },
            "bookingCom": {
                "value": {
                    "formula": Int,
                    "valueType": String,
                    "multiplier": String,
                    "_id": String
                }
            }
        }
    }
}
```



###  Get Listing Calendar <a id="get-billing-history"></a>

#### 📥 Inputs <a id="inputs"></a>

* **Start Date** - Start Date to Query Calendar.  Format: `YYYY-MM-DD`
* End Date -  Ending Date to Query Calendar.  Format: `YYYY-MM-DD`

#### ​📤 Output <a id="output-1"></a>

```text
listing_Cald = {
  "status": Int,
  "data": {
    "days": [
      {
        "date": String,
        "listingId": String,
        "currency": String,
        "price": Int,
        "isBasePrice": Bool,
        "minNights": Int,
        "isBaseMinNights": Bool,
        "status": String,
        "blocks": {
          "m": Bool,
          "r": Bool,
          "b": Bool,
          "bd": Bool,
          "sr": Bool,
          "abl": Bool,
          "a": Bool,
          "bw": Bool,
          "o": Bool,
          "pt": Bool
        },
        "blockRefs": [
          {
            "_id": String,
            "reservation": {
              "listing": {
                "timezone": String,
                "defaultCheckInTime": String
              },
              "money": {
                "currency": String,
                "hostPayout": Float,
                "totalPaid": Int,
                "balanceDue": Float
              },
              "guest": {
                "_id": String
              },
              "integration": {
                "platform": String
              },
              "_id": String,
              "status": String,
              "checkIn": Datetime,
              "checkOut": Datetime,
              "nightsCount": Int,
              "guestsCount": Int,
              "listingId": String,
              "checkInDateLocalized": String,
              "checkOutDateLocalized": String,
              "accountId": String,
              "guestId": String,
              "source": String,
              "confirmationCode": String
            },
            "listingId": String,
            "startDate": String,
            "endDate": String,
            "type": String,
            "reservationId": String
          }
        ],
        "reservationId": String,
        "reservation": {
          "listing": {
            "timezone": String,
            "defaultCheckInTime": String
          },
          "money": {
            "currency": String,
            "hostPayout": Float,
            "totalPaid": float,
            "balanceDue": Float
          },
          "guest": {
            "_id": String
          },
          "integration": {
            "platform": String
          },
          "_id": String,
          "status": String,
          "checkIn": Datetime,
          "checkOut": Datetime,
          "nightsCount": Int,
          "guestsCount": Int,
          "listingId": String,
          "checkInDateLocalized": String,
          "checkOutDateLocalized": String,
          "accountId": String,
          "guestId": String,
          "source": String,
          "confirmationCode": String
        },
        "cta": Bool,
        "ctd": Bool
      },
      {
        "date": String,
        "listingId": String,
        "currency": String,
        "price": Float,
        "isBasePrice": Bool,
        "minNights": Int,
        "isBaseMinNights": Bool,
        "status": String,
        "blocks": {
          "m": Bool,
          "r": Bool,
          "b": Bool,
          "bd": Bool,
          "sr": Bool,
          "abl": Bool,
          "a": Bool,
          "bw": Bool,
          "o": Bool,
          "pt": Bool
        },
        "blockRefs": [],
        "cta": Bool,
        "ctd": Bool
      }
    ]
  },
  "message": String
}

```


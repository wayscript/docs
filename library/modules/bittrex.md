---
description: >-
  Seamlessly integrate Bittrex with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Bittrex

![Realtime and historical data on digital currencies, such as Bitcoin.](../../.gitbook/assets/bittrex.png)

## 📥 Input

Certain modes collect data about the overall market, while others look up individual Tickers.

{% hint style="info" %}
Tickers follow format 'Ticker 1-Ticker 2' where 1 unit of Ticker 2 is converted to Ticker 1.

Ex. Last Price for 'BTC-LTC' of 0.00832 means that 1 LTC = 0.00832 BTC.
{% endhint %}

For ticker queries, you can select an option from the available list, or input your own.

![](../../.gitbook/assets/screen-shot-2019-07-16-at-12.36.53-pm.png)

## ⚙ Modes

The Following modes are available and the listed outputs can be retrieved as variables.

{% hint style="info" %}
_\(Single\)_: variables are single items

_\(List\)_: variables are lists

_Note: '_JSON Data' is available for all modes and is always a single item.
{% endhint %}

### List of All Tickers _\(List\)_

```graphql
Markets = [
    {
        market_name : String,
        min_trade_size : Float,
        created : Date,
        base_currency : String,
        base_currency_name : String,
        is_active : Bool,
        is_restricted : Bool,
        logo_url : Url,
        market_currency : String,
        market_currency_name : String,
    },
]
```

### Current Data for a Ticker _\(Single\)_

```graphql
Ticker = {
    market_name : String,
    ask : Float,
    bid : Float,
    last : Float,
}
```

### Last 24 Hour Summaries of all Active Exchanges _\(List\)_

```graphql
Market_Summaries = [
    {
        market_name : String,
        ask : Float,
        base_volume : Float,
        bid : Float, 
        created : Date,
        high : Float, 
        last : Float, 
        low : Float, 
        open_buy_orders : Float, 
        open_sell_orders: Float, 
        prev_day : Float, 
        timestamp : Date, 
        volume : Float, 
    },
]
```

### Last 24 Hour Summary of a Ticker _\(Single\)_

```graphql
Market_Summary = {
    ask : Float, 
    base_volume : Float, 
    bid : Float, 
    created : Date, 
    high : Float, 
    last : Float, 
    low : Float, 
    market_name : String, 
    open_buy_orders : Int, 
    open_sell_orders : Int, 
    prev_day : Float, 
    timestamp : Date, 
    volume : Float, 
}
```

### Historical Market Data for a Ticker _\(List\)_

```graphql
Historical_Date = [
    {
        fill_type : String, 
        id : Int, 
        order_type : String, 
        price : Float, 
        quantity : Float, 
        timestamp : Date,
        total : Float, 
        uuid : String, 
    },
]
```




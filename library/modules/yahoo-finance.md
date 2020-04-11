---
description: >-
  Seamlessly integrate Yahoo Finance with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Yahoo Finance

![Retrieve stock information from Yahoo Finance.](../../.gitbook/assets/yahoo_finance.png)

{% hint style="info" %}
Check out yfinance on [GitHub](https://github.com/ranaroussi/yfinance).
{% endhint %}

## 📥 Inputs

Enter the stock ticker symbol. As an example, for Microsoft you would enter MSFT.

## 📤 Outputs

```graphql
Stock = {
    bid : Number,
    ask : Number,
    market_cap : Number,
    exchange : String, 
    symbol : String,
    language : String,
    region : String,
    quote_type : String,
    quote_source_name : String,
    currency : String,
    regular_market_price : Number,
    regular_market_time : Number,
    regular_market_change : Number,
    regular_market_open : Number,
    regular_market_day_high : Number,
    regular_market_day_low : Number,
    regular_market_volume : Number,
    exchange_date_delayed_by : Number,
    regular_market_change_percent : Number,
    regular_market_previous_close : Number,
    bid_size : Number,
    ask_size : Number,
    message_board_id : String,
    full_exchange_name : String,
    long_name : String,
    financial_currency : String,
    average_daily_volume_3_month : Number,
    average_daily_volume_10_day : Number,
    fifty_two_week_low_change : Number,
    fifty_two_week_low_change_pct : Number,
    fifty_two_week_high_change : Number,
    fifty_two_week_high_change_pct : Number,
    fifty_two_week_low : Number,
    fifty_two_week_high : Number, 
    dividend_date : Number,
    earnings_timestamp : Number,
    earnings_timestamp_start : Number,
    earnings_timestamp_end : Number,
    trailing_annual_dividend_rate : Number,
    trailing_pe : Number, 
    trailing_annual_dividend_yield : Number, 
    eps_trailing_twelve_months : Number, 
    eps_forward : Number, 
    shares_outstanding : Number, 
    book_value : Number, 
    fifty_day_average : Number, 
    fifty_day_average_change : Number, 
    fifty_day_average_change_pct : Number, 
    two_hundred_day_average : Number, 
    two_hundred_day_average_change : Number, 
    two_hundred_day_average_change_pct : Number, 
    forward_pe : Number, 
    price_to_book : Number, 
    source_interval : Number, 
    exchange_timezone_name : String, 
    exchange_timezone_short_name : String, 
    gmt_offsett_milliseconds : Number, 
    price_hint : Number, 
    short_name : String, 
    market : String,
    market_state : String, 
}
```

{% hint style="warning" %}
Not every field will have a value for any given stock ticker symbol.
{% endhint %}


---
description: >-
  Seamlessly integrate Open Weather Map's current weather and forecasts with
  your favorite APIs, databases, and programming languages, using WayScript.
---

# Weather API

![Current weather and forecasts in your city.](../../.gitbook/assets/open_weather_map.png)

{% hint style="info" %}
You can read a tutorial using this Module [here](../../getting_started/modules.md).
{% endhint %}

{% hint style="info" %}
To run your program at sunrise and/or sunset in a given location, use the [Weather API Trigger](../triggers/weather-api-trigger.md).
{% endhint %}

## ⚙ Settings

* **Temperature Type**: Fahrenheit, Celcius, Kelvin
* **Forecast length** - Next 48 hrs, 5 days, 16 days

## 📥 Inputs

* **Location** - Input a location to search \(e.g. Brooklyn NY, 123 Fifth Street, etc.\) 
  * This is a required input.

## 📤 Output

```graphql
Weather = {
    city_name : String, 
    categories : [
        String,
    ],
    condition_summary : String,
    conditions : [
        String,
    ],
    ids : [
        String,
    ],
    sunrise_time : Date,
    sunset_time : Date,
    temperature : Int,
    min_temperature : Int,
    max_temperature : Int,
    humidity : String,
    pressure : Int,
    visibility : Int,
    wind_speed : Int,
    wind_direction : Int,
    forecast: [{ 
                 dt         : Int,
                 temp       : Int,
                 feels_like : Int,
                 pressure   : Int,
                 humidity   : Int,
                 visibility : Int,
                 wind_speed : Int,
                 wind_deg   : Int,
                 wind_gust  : Int,
                 weather    : String,
                 pop        : Int,
              }],
}
```


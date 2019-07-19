# Zillow

![Real estate data.](../../.gitbook/assets/zillow_data.png)

{% hint style="info" %}
Check out python-zillow on [GitHub](https://github.com/seme0021/python-zillow).
{% endhint %}

## 🔑 Registering for an API Key

{% hint style="warning" %}
The Zillow module requires you to create an API Key on Zillow.
{% endhint %}

### 1\) Go to [Zillow API Signup Dashboard](https://www.zillow.com/user/Register.htm)

### 2\) Click the 'New Account' tab and submit the required information. 

![](../../.gitbook/assets/zillow_auth_1.png)

### 3\) Fill out the API Sign Up

{% hint style="info" %}
CHECK ALL APIs under the select API\(s\) section!
{% endhint %}

![Check all apis under Select API\(s\)](../../.gitbook/assets/zillow_auth_2.png)

### 4\) You will recieve your Zillow Identification Key \(ZWSID\) via email. 

## 📥 Inputs

* **Address** - Format: Street, Town, State
  * Ex: 3400 Pacific Ave., Marina Del Rey, CA
* **Zip Code** - United States Zip \(postal\) Code
  * Ex: 90292

## 📤 Outputs

{% hint style="info" %}
Outputs are [single Items](../../getting_started/variables.md#single-item) if mode is "Get Data on an Address." Outputs are [lists](../../getting_started/variables.md#lists) if mode is "Get Comparables to an Address."
{% endhint %}

* **Zestimate House Value** - Zestimate House Value in US Dollars
* **Zestimate Valuation \(High\)** - Zestimate House Valuation in US Dollars
* **Zestimate Valuation \(Low\)** - Zestimate House Valuation in US Dollars
* **Zestimate Valuation Change** - Zestimate House Valuation Amount Changed in the last 30 days. Denoted in US Dollars.
* **Number of Bathrooms**
* **Number of Bedrooms**
* **House is Completed** - True if house is completed, False if house is under construction.
* **Square Feet**
* **Lost Size Square Feet** - Square Feet of the entire property.
* **Last Sold Date** - Date of the last time the house was sold.
* **Last Sold Price** - Price of house in last sale.
* **Tax Assessment**


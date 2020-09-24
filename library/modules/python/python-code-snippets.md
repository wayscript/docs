---
description: Example code snippets for use in the WayScript Python module.
---

# Python Code Snippets

## ![](../../../.gitbook/assets/selenium_logo_square_green.png) Using [Selenium](https://selenium-python.readthedocs.io)

The [Python module](./) includes the [Chrome headless browser](https://developers.google.com/web/updates/2017/04/headless-chrome), which you can interact with using Selenium. Here is some sample code to do this:

```python
from selenium import webdriver

options = webdriver.ChromeOptions()
options.add_argument('--headless')
options.add_argument('--no-sandbox')
options.add_argument( '--disable-dev-shm-usage' )
options.add_argument('user-agent=Mozilla/5.0 (Macintosh; Intel Mac OS X 10.10; rv:39.0) Gecko/20100101 Firefox/39.0')

browser = webdriver.Chrome(options = options)
browser.set_page_load_timeout(30)

browser.get('https://wayscript.com/')

ps = browser.page_source
print(ps)

browser.close()
```

{% hint style="warning" %}
Be sure to add the following options:

`option.add_argument('--headless')  
option.add_argument('--no-sandbox')  
option.add_argument('--disable-dev-shm-usage')`
{% endhint %}

## ![](../../../.gitbook/assets/sql%20%281%29.png) Connecting to a Microsoft SQL Server Database

Use the following code to connect to a publicly-accessible SQL Server database using Python.

```python
import pyodbc

server = 'sqlservertest.us-east-1.rds.amazonaws.com'
port = '1430'
database = 'WayScriptTest'
username = 'Admin'
password = 'Pa$$word'
conx = pyodbc.connect('Driver={ODBC Driver 17 for SQL Server};SERVER='+server+','+port+';DATABASE='+database+';Uid='+username+';Pwd='+password)
```


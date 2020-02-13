---
description: Updates and improvements to the WayScript platform.
---

# What's new?

## February 12th, 2020

* You can now easily Undo & Redo changes while editing scripts!
  * Use the Undo/Redo buttons in the editor ![](.gitbook/assets/screen-shot-2020-02-12-at-8.43.14-pm%20%281%29.png)
  * On Mac, Undo with `⌘ Command`+`Z` and Redo with `⇧ Shift`+`⌘ Command`+`Z`
  * On Windows, Undo with `Ctrl`+`Z` and Redo with `Ctrl`+`Y`

## February 5th, 2020

* We have added an [RSS Feed module](library/modules/rss-feed.md) for pulling data from your favorite RSS feed. 
* The WayScript blog page is now [WayScript Learn](https://wayscript.com/learn)! We have refreshed the look of the page, added tags, and search functionality. Happy learning! 
* We have added a [Stripe module](library/modules/stripe.md) for getting account info from Stripe. Check out the video below to see it in action!

{% embed url="https://www.youtube.com/watch?v=Upi-Z7E5H20" %}

## January 23rd, 2020

* We have a new and improved fullscreen code editing experience, where you can take advantage of your screen real-estate to more easily add and edit files, run your code, and see output. Refer to [Code Editors](getting_started/code-editors.md) for more details.

![](.gitbook/assets/screen-shot-2020-01-23-at-6.51.52-pm.png)

* We have launched a new [Community Marketplace](https://wayscript.com/marketplace), where you can see, sort, and clone copies of other users' public programs! \(All publicly shared programs appear in the community marketplace by default.\)

![Sort users&apos; programs or search for the exact one you&apos;re looking for.](.gitbook/assets/screen-shot-2020-01-23-at-6.02.22-pm.png)

{% embed url="https://www.youtube.com/watch?v=2ZtXXYCeOTI&feature=youtu.be" %}

## January 15th, 2020

* We have updated the [Create Variable](library/logic/create-variable.md) module so that you can now declare variables using "Pythonic" syntax and create multiple variables of different types in the same step. You can also [edit variable values](library/logic/create-variable.md#updating-the-value-of-a-variable) using the Create Variable module. For a tutorial on creating variables in WayScript, see the ["Variables" section of Getting Started](getting_started/variables.md).

![An example of creating multiple variables of different types using the Create Variable module.](.gitbook/assets/screen-shot-2020-01-15-at-1.55.49-pm.png)

* You can now [Update a Row](library/modules/airtable.md#update-a-row) using the Airtable module. 
* Stop your [Python](library/modules/python/) and [JavaScript](library/modules/javascript.md) code by pressing the "Stop Running" button during code execution. ![](.gitbook/assets/screen-shot-2020-01-15-at-1.42.31-pm-3.png)  
* We have received requests for users who want to contribute modules to the platform. [Here is a link](https://github.com/wayscript/wayscript_modules/blob/master/giphy.py) to an example of our Giphy module that you can use as a template. You can submit your modules back to us and we will publish them. This is our first step toward eventually open-sourcing our modules.   We are happy to work with anyone who tries to build a module! Please [reach out on our Discord channel](https://discord.gg/hRkE7PP) with any questions. 
* The [WayScript Marketplace](https://wayscript.com/marketplace) has been refreshed with a new look and feel!

## December 17th, 2019

* We have added the ability to edit your user profile!
  * You can now update your profile image, add a bio, and set your contact information.
  * You can also [share the URL of your profile](https://wayscript.com/user/captain1217) to allow people to see your page and view your publicly available scripts.

![](.gitbook/assets/screen-shot-2019-12-17-at-9.21.22-pm.png)

* We have added a customizable landing page for your scripts! From this page, you can:
  * Edit the name and description of your script.
  * Add a ReadMe using Markdown.
  * Customize the script logo and banner image.
  * Delete, clone, share, or edit your script.
  * View statistics about your script.

![](.gitbook/assets/screen-shot-2019-12-17-at-9.22.51-pm.png)

* We have added a [Variable Storage](library/logic/variable-storage.md) module, which  allows you to store the values of variables in your WayScript programs.
* The outputs of most modules have been updated to utilize the new, easy-to-use "struct" variable type.
  * Structs allows you to drill down into variables using the `.` operator. For example, you can access the content of a particular [Tweet](library/modules/twitter.md) within a list of Tweets by referencing `Tweets.0.content`.
  * Refer to the documentation for each individual module to see the contents and structure of the output data.

## November 20th, 2019

* We have added a [RegEx module](library/modules/regex.md) that makes it easy to find pattern matches in text.
* The Dashboard has been updated to show a more streamlined view of your scripts.

![Hover over a dashboard tile to manage the script.](.gitbook/assets/screen-shot-2019-11-20-at-11.27.58-am.png)

* You can now run [Slack "Slash Commands"](https://api.slack.com/interactivity/slash-commands) using the [Slack module](library/modules/slack.md). These commands require use of the [Legacy Slack API](https://api.slack.com/custom-integrations/legacy-tokens), so [follow the docs](library/modules/slack.md#run-a-slash-command) for details on setting this up.

![Run a slash command, like /poll, using the WayScript Slack module.](.gitbook/assets/screen-shot-2019-11-20-at-11.16.03-am.png)

* SQL and Spreadsheet column outputs now infer the type of the variable in the column.

![SQL output variables have different types, depending on the content of the column.](.gitbook/assets/screen-shot-2019-11-20-at-11.20.23-am.png)

## November 13th, 2019

* **You can now** [**easily share scripts**](getting_started/sharing.md) **with public links and manage permissions!**
  * [Share with the world](getting_started/sharing.md#sharing-your-script) via a publicly accessible link
  * [Limit access](getting_started/sharing.md#managing-sharing-and-access) by only sharing with a specific person
  * Allow users to run scripts in your account without needing to copy the script to their account
  * Manage permissions by adding, deleting, or changing users' access

![](.gitbook/assets/screen-shot-2019-11-13-at-7.30.41-pm.png)

* **We have revamped the experience in the** [**HTTP Trigger**](library/triggers/http-trigger.md)**!**
  * [Sample code](library/triggers/http-trigger.md#sample-code) makes it easier than ever to quickly run a program from your terminal
  * You can pass [query parameters](library/triggers/http-trigger.md#request-query-parameters) and/or [JSON body parameters](library/triggers/http-trigger.md#request-json-body-parameters) when triggering your program
  * The WayScript [Python](https://pypi.org/project/wayscript/) and [JavaScript](https://www.npmjs.com/package/wayscript) libraries have been updated to take advantage of the new functionality in the HTTP Trigger
  * The Webhook Trigger has been deprecated, as all of its functionality \(and more!\) is available in the HTTP Trigger

## November 4th, 2019

* We have updated the login and signup flows to provide more information and streamline the process.
* We have made it easier to add comments within your scripts.
* Added more consistent styling for variable colors, so it's easer to determine the types of your variables.
* When adding variables, you are now given a preview of the variable's content.
* You can now drill down into variables using the `.` operator. For example, you can access the content of a particular [Tweet](library/modules/twitter.md) within a list of Tweets by referencing `Tweets.0.content`.

![Updated variable styling, content previews, and &apos;.&apos; operator syntax.](.gitbook/assets/screen-shot-2019-11-04-at-11.17.54-am.png)

## October 16th, 2019

* Reply-to addresses are now available as an [output of the Gmail trigger](library/triggers/gmail-trigger.md#outputs).

## October 8th, 2019

* You can now log in with GitHub!

## September 13th, 2019

* [Google Assistant](library/triggers/google-assistant-trigger.md) integration is now available! Trigger your WayScript programs by saying "Hey, Google" and have the Google Assistant [respond back to you](library/modules/google-assistant.md).
* You can now [password-protect your custom HTTP endpoints](library/triggers/http-trigger.md#password-protect-your-endpoints).
* Added [Discord](library/triggers/discord-trigger.md) functionality, so you can trigger WayScript programs to run when various Discord events occur, or interact with Discord channels [using the WayScript bot](library/modules/discord.md).
* New [Twitter](library/modules/twitter.md) functionality:
  * [Pull a list of followers/following for a Twitter username](library/modules/twitter.md#get-user-followers-and-following)
  * [Like Twitter posts](library/modules/twitter.md#like-a-tweet)

## September 6th, 2019

* Now you can preview [templates](https://wayscript.com/library) in "read-only" mode. [Click here for an example!](https://wayscript.com/view_template/Build%20A%20Website)
* WayScript no longer requires a beta key, so anyone can create an account!
* Documentation for each module now appears in a panel on the right side of the script editor, so you don't have to interrupt your flow to look something up!

## August 30th, 2019

* Added functionality for [hosting your own web app in WayScript](https://www.youtube.com/watch?reload=9&v=OrZMjdVhFfA&feature=youtu.be). This includes the following features:
  * [HTTP Trigger](library/triggers/http-trigger.md), which allows you to trigger a function when a user visits a URL.
  * [HTTP Response](library/modules/http-response.md) module, which returns the output of your script as an HTTP response.
  * [HTML module](library/modules/html.md) for composing HTML code to serve as content on your webpage.
  * [CSS module ](library/modules/css.md)for styling your webpage.
  * [Images module](library/modules/images.md) for adding images to your scripts and including them in HTML.
  * Option to [output raw JS code](library/modules/javascript.md#output-raw-javascript-code) from the [JavaScript module](library/modules/javascript.md), to include it in HTML.
  * The [Build a Website](https://wayscript.com/library/Build_A_Website) template is now available in the [Template Library](https://wayscript.com/library).
* The [Python module](library/modules/python/) now includes the [Chrome headless browser](https://developers.google.com/web/updates/2017/04/headless-chrome), which you can interact with [using Selenium](library/modules/python/libraries.md#using-selenium). 
* You can now [add comments to steps within your scripts](getting_started/modules.md#add-comments-to-a-step).

## August 23rd, 2019

* [Python Slackbot](https://wayscript.com/library/Slack_Bot) added to the [Template Library](https://wayscript.com/library).
* Variable pills now work in code editors.
* You can now share scripts that contain modules requiring authentication.
* Added ability to [trust a computer](account-management/two-factor-authentication.md#trust-a-computer) when using Two-Factor Authentication.

## August 20th, 2019

* Added the [JavaScript module](library/modules/javascript.md), where you can compose and run your own custom JavaScript code as part of your scripts. This module also allows you to [define custom npm dependencies](library/modules/javascript.md#adding-dependencies).
* Added [Else-If](library/logic/conditionals.md#if-else-if-else) functionality to the [Conditional](getting_started/conditionals.md#add-branches) logic module.
* Added a [While Loop](library/logic/loop/while-loop.md) module.
* Added the [Pie Chart data visualization module](library/modules/pie-chart.md), allowing you to visualize category proportions in data.

## August 15th, 2019

* Added a [Template Library](https://wayscript.com/library), where you can get started with ready-made scripts. This replaces the Sidekick functionality.
* You can now [define custom requirements](library/modules/python/#adding-additional-requirements) in the Python module and edit your code in an expanded full-screen mode.


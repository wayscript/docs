# Twitch

![Work with Twitch data.](../../.gitbook/assets/twitch.png)

## Get a List of the Current Top Games

![](../../.gitbook/assets/screen-shot-2019-07-16-at-5.56.37-pm.png)

#### Inputs

* Number of Games
  * Default is 20.
  * Maximum is 100.

#### Outputs

* List of Top Games by name
* List of Top Games by ID
* JSON Data

{% hint style="info" %}
A Games ID can be found in the Games by ID list at the same index that it's in this list.
{% endhint %}

## Get a List of the Current Top Streams

![](../../.gitbook/assets/screen-shot-2019-07-16-at-5.57.10-pm.png)

#### Inputs

* Number of Streams
  * Default is 20.
  * Maximum is 100.
* Filter by Game ids
  * Optional
  * Maximum 100
* Filter by User Names
  * Optional
  * Maximum 100
* Filter by Languages
  * Optional
  * Maximum 100

#### Outputs

* List of Top Streamers
* List of Top Streamers Viewer Counts
* JSON Data

{% hint style="info" %}
To match streamer names to viewer counts, look at the same index in each corresponding list.
{% endhint %}

## Get a Games Name from its ID

![](../../.gitbook/assets/screen-shot-2019-07-16-at-5.57.24-pm.png)

#### Inputs

* Game ID
  * Required

#### Outputs

* Game Name
* JSON Data

## Get a Games ID from its Name

![](../../.gitbook/assets/screen-shot-2019-07-16-at-5.57.38-pm.png)

#### Inputs

* Game Name
  * Required

#### Outputs

* Game ID
* JSON Data


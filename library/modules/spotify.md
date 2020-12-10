---
description: >-
  Seamlessly integrate Spotify with your favorite APIs, databases, and
  programming languages, using WayScript.
---

# Spotify

![A Swedish audio streaming platform.](../../.gitbook/assets/spotify%20%282%29.png)

## ⚙ Settings

### ![](../../.gitbook/assets/spotify%20%282%29.png) **Mode**

* **Options -** Lookup Artist

### \*\*\*\*👩🎤 **Lookup Artist By**

* **Options -** Artist Name, Spotify ID, Spotify URI
* **Warning -** Looking up artist by 'Artist Name' will return top search result, correct result is not guaranteed. For full results, use the JSON Output

### 📥 Inputs

* **Artist** - Put in the artist input that fits your **Lookup Artist By** selection

### 📥 Outputs

```graphql
Artist = {
		name          : String,
		num_followers : Int,
		genres        : [ String ],
		image_url     : Url,
		popularity    : Int,
		spotify_id    : String,
		spotify_uri   : String
}
```

* JSON Data
  * Raw JSON data received from the API


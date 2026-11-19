---
description: >-
  Use this to register your Developer ID with AltStore PAL, as well as to
  process and download ADPs for your notarized apps.
---

# 📔 REST API

## Register Developer ID

`POST https://api.altstore.io/register`

Use this endpoint to register your Developer ID with AltStore PAL and receive a security token to add AltStore PAL as an alternative marketplace in App Store Connect.

#### Request Body

```
{
  "developerID": "[Your Apple Developer ID]",
  "email": "[Your Email Address]
}
```

#### Response

```
{
  "token": "[Your Security Token]",
  "expiration": "2025-02-26T20:30:32Z"
}
```

#### Terminal Command

```
curl --header "Content-Type: application/json" \
  -X POST \
  --data '{ 
    "developerID": "[Your Apple Developer ID]", 
    "email": "[Your Email Address]"
  }' \
  https://api.altstore.io/register
```



## Download ADP

{% hint style="warning" %}
This endpoint requires a notarized ADP ID. [Get your ADP ID](https://developer.apple.com/help/app-store-connect/distributing-apps-in-the-european-union/get-an-alternative-distribution-package-id/)
{% endhint %}

`GET https://api.altstore.io/adps/[Your ADP ID]`

Use this endpoint to check the status of an ADP, and optionally download it once it's finished processing.

To download, copy the `downloadURL` from the response and paste it into a web browser. If there is no `downloadURL`, your app is still processing and you can check the status under the `status` key.

#### Example Request

```
curl -X GET https://api.altstore.io/adps/[Your ADP ID] 
```



## Process ADP

{% hint style="warning" %}
This endpoint requires a notarized ADP ID. [Get your ADP ID](https://developer.apple.com/help/app-store-connect/distributing-apps-in-the-european-union/get-an-alternative-distribution-package-id/)
{% endhint %}

`POST https://api.altstore.io/adps`

Use this endpoint if you haven't set up marketplace notifications, or if you don't want to wait for our servers to process your app automatically, or if a previously-processed ADP download has expired. **You must include your ADP ID in the JSON request body under the `adpID` key.**

After it finishes processing, you can use the Download ADP endpoint above to download it.

#### Example Request

```
curl --header "Content-Type: application/json" \
  -X POST \
  --data '{ "adpID": "[Your ADP ID]" }' \
  https://api.altstore.io/adps
```



## Federate Source

`POST https://api.altstore.io/federate`

Use this endpoint to make your source discoverable on explore.alt.store and start federating to the open social web.

#### Request Body

```
{
  "source": "YOUR_SOURCE_URL",
}
```

#### Response

```
HTTP 200 OK
```

#### Terminal Command

```
curl --header "Content-Type: application/json" \
  -X POST \
  --data '{  
    "source": "YOUR_SOURCE_URL"
  }' \
  https://api.altstore.io/federate
```


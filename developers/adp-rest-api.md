---
description: Process and download ADPs for your notarized apps.
---

# 📔 ADP REST API

{% hint style="info" %}
These endpoints require a notarized ADP ID. [Get your ADP ID](https://developer.apple.com/help/app-store-connect/distributing-apps-in-the-european-union/get-an-alternative-distribution-package-id/)
{% endhint %}

## Download ADP

`GET https://api.altstore.io/adps/[Your ADP ID]`

Use this endpoint to check the status of an ADP, and optionally download it once it's finished processing.

To download, copy the `downloadURL` from the response and paste it into a web browser. If there is no `downloadURL`, your app is still processing and you can check the status under the `status` key.

#### Example Request

```
curl -X GET https://api.altstore.io/adps/[Your ADP ID] 
```



## Process ADP

`POST https://api.altstore.io/adps`

Use this endpoint if you haven't set up marketplace notifications, or if you don't want to wait for our servers to process your app automatically. **You must include your ADP ID in the JSON request body under the `adpID` key.**

After it finishes processing, you can use the Download ADP endpoint above to download it.

#### Example Request

```
curl --header "Content-Type: application/json" \
  -X POST \
  --data '{ "adpID": "[Your ADP ID]" }' \
  https://api.altstore.io/adps
```

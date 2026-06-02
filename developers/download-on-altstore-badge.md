# 🏷️ “Download on AltStore” Badge

After you make your app live on AltStore, you can add our download badge to your website to easily link people to your app. This works for both AltStore Classic and AltStore PAL.



{% file src="../.gitbook/assets/Download Badge (1).zip" %}

<div><figure><img src="../.gitbook/assets/DownloadBadge_light (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/DownloadBadge_dark (1).png" alt="" width="188"><figcaption></figcaption></figure></div>

## Instructions

1. Download the "Download Badge.zip" file above
2. Upload the variant of your choice somewhere publicly accessible via URL
3. Create an AltStore deep link using one of the below [Deep Link Formats](download-on-altstore-badge.md#deep-link-formats)
4. Embed the following HTML code on your website, replacing:\
   \- `YOUR_SOURCE_URL`  with the deep link URL from step 3\
   \- `PATH_TO_IMAGE` with the URL to the image you uploaded from step 2

```
<a href="YOUR_SOURCE_URL" style="display: inline-block;">
    <img src="PATH_TO_IMAGE" alt="Download on AltStore" style="width: 245px; height: 82px; vertical-align: middle; object-fit: contain; />
</a>
```

### Deep Link Formats

**Linking to a source**

{% hint style="info" %}
#### https://altstore.io/source/<mark style="background-color:yellow;">**URL/TO/YOUR/SOURCE**</mark><mark style="background-color:yellow;">.json</mark>

Example:



**Source URL:** https://i.cizzuk.net/altstore/source.pal.json<br>

**Deep Link:**

```
https://altstore.io/source/i.cizzuk.net/altstore/source.pal.json
```
{% endhint %}



**Linking to an app in a source**

{% hint style="info" %}
#### https://altstore.io/source/<mark style="background-color:yellow;">**URL/TO/YOUR/SOURCE**</mark><mark style="background-color:yellow;">.json</mark>?app=<mark style="background-color:$warning;">**APP\_BUNDLE\_ID**</mark>

Example:<br>

**Source URL:** https://i.cizzuk.net/altstore/source.pal.json

**App Bundle ID:** net.cizzuk.alare<br>

**Deep Link:**

```
https://altstore.io/source/i.cizzuk.net/altstore/source.pal.json?app=net.cizzuk.alare
```
{% endhint %}



**Linking to a specific app version in a source**

{% hint style="info" %}
#### https://altstore.io/source/<mark style="background-color:yellow;">**URL/TO/YOUR/SOURCE**</mark><mark style="background-color:yellow;">.json</mark>?app=<mark style="background-color:$warning;">**APP\_BUNDLE\_ID**</mark>\&version=<mark style="background-color:pink;">**APP\_VERSION**</mark>

Example:\
\
**Source URL:** https://i.cizzuk.net/altstore/source.pal.json

**App Bundle ID:** net.cizzuk.alare

**App Version:** 3.0<br>

**Deep Link:**

```
https://altstore.io/source/i.cizzuk.net/altstore/source.pal.json?app=net.cizzuk.alare&version=3.0
```
{% endhint %}

# ⬆ Updating Apps

### Overview

To update your app, you'll need to add a new App Versions entry to your Source JSON with a unique `version` and/or `buildVersion`. After uploading your changes, AltStore will automatically detect that an app update is available and notify users.

Specifically, AltStore detects updates by comparing the first version listed in your App Versions array (i.e index = 0) with the user's installed version. If the first version listed is not compatible with the user's device, AltStore iterates through the array until it finds one that is. If this version is different than what the user has installed, AltStore will notify them that an update is available.&#x20;

{% hint style="warning" %}
AltStore **does not** use dates to determine if there's a newer version.
{% endhint %}



### Version Compatibility

AltStore will only show that an app update is available if it's compatible with the user's OS version. By default AltStore considers all versions to be compatible, but if your update only supports certain iOS versions, you can specify this via the `minOSVersion` and `maxOSVersion` keys.

Users can see a list of unsupported updates from the My Apps tab. Additionally, if a user tries to download a new app that is not compatible with their device, they will be asked to download a previous version instead.



### Update Instructions

1. Upload the IPA file to your server and copy the URL.
2. Add a new entry to the beginning of your app's `versions` array in your Source JSON file.
   * Update `downloadURL` to the copied URL
   * Update `version` to match the app's `CFBundleShortVersionString` (e.g "1.2.1")
   * (Optional) Update `buildVersion` to match the app's `CFBundleVersion` (e.g "10")

{% hint style="info" %}
Each entry must have a different `version` or `buildVersion` from the previous version.
{% endhint %}

{% code lineNumbers="true" %}
```json
"versions": [
   {
    "version": "1.1",
    "buildVersion": "2",
    "date": "2024-05-25",
    "localizedDescription": "First AltStore Update!",
    "downloadURL": "https://myapp.com/myapp-1.1.ipa",
    "size": 80925,
    "minOSVersion": "14.0",
    "maxOSVersion": "16.3"
  }
  {
    "version": "1.0",
    "buildVersion": "1",
    "date": "2024-03-30",
    "localizedDescription": "First AltStore release!",
    "downloadURL": "https://myapp.com/myapp-1.0.ipa",
    "size": 79821,
    "minOSVersion": "12.0",
    "maxOSVersion": "16.3"
  },
]
```
{% endcode %}

3\. Upload your Source JSON to your server - that's it!

{% hint style="warning" %}
**Once uploaded, the update is immediately made live.**&#x20;

For this reason, we recommend updating a staging version of your source first to verify that the changes work as expected.
{% endhint %}

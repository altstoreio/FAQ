---
description: Here is an template and details you need to create your own source!
---

# 📂 Make Your Own Source

## Template

The JSON file below is what you can download and fill in with your App's information to get you app available on AltStore today! There are also some notes below on how to properly fill out the source template.&#x20;

{% file src="../.gitbook/assets/altsource-template.json" %}

### <mark style="color:purple;">**Source**</mark>

**Source Identifier ("identifier”)**

Must be unique. Reverse DNS-style recommended.

### <mark style="color:purple;">**Apps Section**</mark>

**App Bundle ID (“bundleIdentifier”)**

Must be unique, and match the app’s bundle identifier exactly. Case sensitive.

**App Version Date (“versionDate”)**

Must be in ISO8601 format.

**App Tint Color (“tintColor”)**

Hexadecimal encoded RGB color.

**App Size (“size”)**

Size of .ipa in bytes.\
**App Screenshot URLs (“screenshotURLs”)**

Each image MUST be 9:16 portrait aspect ratio to avoid breaking AltStore layout.

### <mark style="color:purple;">**News Section**</mark>

**News Item Identifier ("identifier”)**

Must be unique.

**Send Notification (“notify”) (OPTIONAL)**

Boolean. When TRUE, AltStore will send a push notification to the user about this news item.

**Website URL (“url”) (OPTIONAL)**

A website AltStore should open when the news item is tapped.

**App ID (“appID”) (OPTIONAL)**

The bundle ID of an app listed in this source. AltStore shows a banner for this app below the news item.

# 🇪🇺 AltStore PAL

## <mark style="color:blue;">AltStore PAL 2.2</mark>

<mark style="color:blue;">**May 6, 2025**</mark>

### New

Sources

* Supports installing apps from developers registered via our updated [REST API](https://faq.altstore.io/developers/rest-api)
* Supports localized titles, subtitles, and descriptions in sources
* Supports downloading ADPs from Patreon posts
* Supports `assetURLs` to override URLs for individual ADP assets
  * Dictionary of override URLs for files in ADP, keyed by filename (without file extension)
  * Allows for hosting ADPs is other ways besides just a directory structure (e.g. GitHub Releases)

Misc.

* Added Bluesky social media button to Settings

### Improved

UI

* Hides “See All” button in Browse tab for sources with just 1 app
* Sorts apps alphabetically in My Apps

Sources

* Supports using ADP's `manifest.json` URL as `downloadURL`
* Ignores irrelevant `maxOSVersion` AltStore Classic key

Patreon

* Migrates Patreon cookies to shared container on launch (if needed)
* Attempts to re-authenticate if necessary when downloading ADP from Patreon

Misc.

* Includes error message in `AltMarketplace` headers if error occurs
* Ignores “downgrade” updates for AltStore PAL

### Fixed

* Fixed choosing alternate app icon on iPad
* Fixed fetching Patreon post attachments with `nil` mimeType
* Fixed handling source deep link when already viewing source details
* Fixed installing ADPs with case-sensitive download URLs
* Fixed installing apps before adding source via deep link
* Fixed “Join Patreon” sheet appearance in dark mode
* Fixed not showing OPEN for installed apps when previewing source via deep link
* Fixed not showing OPEN for installed apps when previewing already-added Recommended Source
* Fixed accessing deep link Source on background context from main thread



## <mark style="color:blue;">AltStore PAL 2.1.6</mark>

<mark style="color:blue;">**January 22, 2025**</mark>

* Automatically removes apps when deleted from the Home Screen (iOS 18+)
* Adds "Discover More Apps" button to showcase featured apps on [altstore.io](https://altstore.io)
* Includes app bundle ID when logging installation progress
* Fixed apps not appearing in My Apps if installation finishes while in background
* Fixed apps not updating under certain conditions
* Fixed opening source deep links when app is not in background
* Fixed displaying internal version number instead of public version number in settings



## <mark style="color:blue;">AltStore PAL 2.1.5</mark>

<mark style="color:blue;">**November 13, 2024**</mark>

* Delays fetching Friend Zone patrons until user first opens Patreon screen
* Fixed handling Patreon rate limit errors
* Fixed crash updating apps when there is more than 1 update available
* Fixed updating apps with "Auto Manage Installed Apps" enabled
* Fixed crash if fetching MarketplaceKit install token fails



## <mark style="color:blue;">AltStore PAL 2.1.4</mark>

<mark style="color:blue;">**October 31, 2024 🎃**</mark>

* Fixed certificate validation error when redeeming PAL promo&#x20;
* Fixed "Failed to Verify AltStore" error when updating PAL



## <mark style="color:blue;">AltStore PAL 2.1.3</mark>

<mark style="color:blue;">**October 22, 2024**</mark>

### **New**

"Day One" Promo

* New promo to thank our early adopters who paid €1,50 to install AltStore PAL
* Exclusive "Day One" app icon
* 1 free month of access to our "Early Adopter" Patreon tier
* Follow instructions here to redeem: [https://faq.altstore.io/altstore-pal/day-one-promo](https://faq.altstore.io/altstore-pal/day-one-promo)

Misc.

* Added dark mode & tinted variants of primary app icon
* Added new Home Screen quick actions with support info

### **Fixed**

* Fixed crash when fetching source containing app larger than 2GB&#x20;



## <mark style="color:blue;">AltStore PAL 2.1.2</mark>

<mark style="color:blue;">**August 29, 2024**</mark>

### **New**&#x20;

* “Auto Manage Installed Apps” debug setting
* Supports `marketingVersion` source key

### **Improved**

* Verifies downloaded app matches source values
* Handles MarketplaceKit deep links

### **Fixed**

* Fixed incorrect progress when installing multiple apps in single session&#x20;
* Fixed installing apps before adding sources
* Fixed Settings tab bar disappearing on iOS 18



## <mark style="color:blue;">AltStore PAL 2.1.1</mark>

<mark style="color:blue;">**August 8, 2024**</mark>

* Handles "search" and "view app" deep links
  * Search: `altstore-pal://search?q=[query]`
  * View App: `altstore-pal://viewApp?bundleID=[app bundle ID]`
* Fixed duplicate "New Update Available" notifications
* Fixed restoring offloaded apps
* Fixed updating apps under certain conditions
* Fixed not unlocking certain Patreon benefits
* Fixed showing legacy app intents in Shortcuts app



## <mark style="color:blue;">AltStore PAL 2.1</mark>

<mark style="color:blue;">**July 24, 2024**</mark>

* Supports adding "Recommended Sources"
* Added altstore-pal:// URL scheme
* Replaced AppCenter dependency with TelemetryDeck



## <mark style="color:blue;">AltStore PAL 2.0.1</mark>

<mark style="color:blue;">**June 5, 2024**</mark>

* Supports distributing Patreon-exclusive apps to free members
* Adds "Manage Subscription" option in Settings to manage PAL annual subscription
* Shows instructions when updating AltStore PAL

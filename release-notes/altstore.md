# 🛍 AltStore

## <mark style="color:green;">AltStore 1.5.1</mark>

<mark style="color:green;">**July 14, 2022**</mark>

* Fixed signing in with Apple IDs that contain capital letters
* Fixed signing in with Apple IDs that have 2FA enabled but don’t have any registered trusted devices
* Fixed repeatedly asking some users to sign in every time they refresh their apps
* Fixed “Application is missing application-identifier” error when sideloading or (de-)activating certain apps
* Fixed “Incorrect Apple ID or password” error after changing an Apple ID’s primary email address
* Fixed crash when receiving unknown error codes from AltServer

## <mark style="color:green;">AltStore 1.5</mark>&#x20;

<mark style="color:green;">**May 6, 2022**</mark>

### New

#### Trusted Sources&#x20;

* Download and update certain third party apps entirely through AltStore
* Add Trusted Sources directly from the new Sources page
* Trusted Sources are sources we’ve explicitly approved because they meet our safety standards
* Support for adding any source by URL will be coming later

#### AltJIT&#x20;

* Allows sideloaded apps to use Just-in-Time (JIT) compilation
* Long-press an app in My Apps, then choose “Enable JIT” – a few seconds later you should see an AltStore notification saying “Successfully Enabled JIT”
  * Your device must be on the same WiFi network as AltServer or connected to your computer via USB
* JIT will remain enabled until the app is quit from the app switcher or purged from memory in the background
* Requires iOS 14 or later
* Requires AltServer 1.5 or later

### Improved&#x20;

* Supports landscape app screenshots
* Adds Shane to credits and Patreon screen
* Prefetches & caches Friend Zone patrons to offset the Patreon API’s slow response time

### Fixed

* Fixed a potential crash when sideloading certain apps
* Fixed some apps having access to AltStore’s app group after being (de-)activated
* Fixed crash when adding or removing sources that have News items
* Fixed Core Data error when not connected to internet due to saving non-NSSecureEncoding items from NSError’s userInfo

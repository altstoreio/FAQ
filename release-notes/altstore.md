# 🛍 AltStore

## <mark style="color:green;">AltStore 1.5</mark>&#x20;

<mark style="color:green;">**May 5th, 2022**</mark>

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

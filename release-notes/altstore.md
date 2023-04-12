# 🛍 AltStore

## <mark style="color:green;">AltStore 1.6.3</mark>

<mark style="color:green;">**April 12, 2023**</mark>

* Fixed error fetching Friend Zone patrons due to unexpected nil name
* Fixed incorrect cell height for some News items



## <mark style="color:green;">AltStore 1.6.2</mark>

<mark style="color:green;">**March 22, 2023**</mark>

* Fixed “no provisioning profile with the requested identifier…” error when sideloading and refreshing apps



## <mark style="color:green;">AltStore 1.6.1</mark>

<mark style="color:green;">**February 20, 2023**</mark>

* “Clear Cache” button removes temporary files and deleted app backups to free up disk space
* Disable new “Enforce 3-App Limit” setting to sideload more than 3 apps via MacDirtyCow exploit\*
* Fixed crash when viewing Sources on iOS 12

\*Requires iOS 14.0 - 16.1.2 (excluding 15.7.2). **iOS 16.2 or later not supported.**



## <mark style="color:green;">AltStore 1.6</mark>

<mark style="color:green;">**January 30, 2023**</mark>

### New

#### Lock Screen Widget (iOS 16 only)&#x20;

* Counts down days until AltStore expires&#x20;
* Available in 2 different styles: “text” and “icon”

#### Error Log&#x20;

* View past errors in more detail
* Tap an error to copy the error message or error code
* Search for error code directly in AltStore FAQ
* “View More Details” button to view detailed error information
* Access via new “Techy Things” section in AltStore settings

#### iOS Version Compatibility

* Supports app updates with minimum or maximum OS requirements
* Hides app updates if they’re not compatible with current device
* Falls back to downloading last compatible version on older devices
* View all unsupported updates from My Apps tab

#### Revamped Error Handling&#x20;

* Completely revamped error handling to include as much information as possible, which should make debugging certain issues much easier
* Revised error messages to be more descriptive and provide more suggestions
* Revised error domain format to `[Module].[ErrorType]`
* `AltStore.OperationError` codes start at 1000
* `AltServer.ServerError` codes start at 2000
* `AltStore.AppleDeveloperError` codes start at 3000
* Uses underlying error messages (if available) for several `AltServer.ServerError` errors
* Encodes/Decodes all Codable user info values, not just recognized types

#### Misc.&#x20;

* Adds pull-to-refresh to check for updates
* Supports new “versions” key in source JSON
* Supports updating apps from app detail page

### Improved&#x20;

#### Source Validation&#x20;

* Verifies sources don't contain duplicate app bundle identifiers
* Verifies sources don't contain duplicate app versions
* Shows error if a source is configured incorrectly instead of silently failing

#### Misc.

* Updated `LaunchViewController` error alert to display more detailed error messages
* Always displays loading indicator when fetching Friend Zone patrons
* Improves error message when .ipa does not exist at provided downloadURL
* Caches MergeErrors when refreshing sources to view later from Sources page

### Fixed

* Fixed `CollapsingTextView` incorrectly showing “more” button
* Fixed “error migrating persistent store” issue
* Fixed widgets potentially not updating after refreshing apps
* Fixed simultaneous database access from multiple AltStores
* Fixed incorrect app name and iOS version in "Unsupported iOS version" error message
* Fixed refreshing tweaked apps with removed app extensions
* Fixed error encoding CodableError Int/UInt user info values
* Fixed adding failures to NSErrors with nil localizedFailureReasons
* Fixed incorrect error toast view color when sign-in fails



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

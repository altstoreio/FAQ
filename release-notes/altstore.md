# 🛍️ AltStore Classic

## <mark style="color:green;">AltStore 2.0</mark>

<mark style="color:green;">**September 28, 2024**</mark>

### New

**Sources**

* Add any 3rd-party source, in addition to existing Recommended Sources!
* New dedicated Sources tab to easily manage and browse sources
* Separate "Add Source" screen to simplify adding sources
* Preview sources before adding them to AltStore
  * View detailed information as well as any additional links
  * Browse all apps and news for a source
  * "Featured Apps" section showcases a source's best apps
* Supports remote blocking malicious sources

**Redesigned Browse Tab**

* New "card" design for app listings
* View most recently updated apps at a glance
* Browse apps by source or by 8 new categories
* Scroll through featured apps from each source
* Change sort order of apps when browsing by source or category
* Tap category name to easily switch between categories when browsing
* Swipe through all screenshots directly from Browse tab

**Patreon**

* 3rd-party sources can now distribute Patreon-exclusive apps to patrons, including free members
* Donate to developers' Patreons and download Patreon-exclusive apps all within AltStore
* Supports "custom" pledge amounts so patrons can donate what they want
* Shows required pledge amount for Patreon apps (if provided)

**App Icon**

* Brand new app icon
* Choose alternate app icons in Settings

**Detailed App Permissions**

* View all entitlements and privacy permissions for an app from its store page
* Tap any permission to view a detailed description
* Automatically verifies permissions are accurate before installing
* Asks user to review permissions when installing and updating apps
  * When installing a new app, all entitlements will be shown
  * When updating an app, only added entitlements will be shown

**Source JSON**

* Supports JSON5
* `buildVersion` parameter allows distributing multiple builds with same app version
* `sha256` parameter lets AltStore verify downloaded .ipa's have the correct SHA-256 hash
* `appPermissions` parameter declares all permissions used by an app and its extensions
* `marketingVersion` parameter allows customizing the version displayed to the user

**Misc.**

* Added social media follow buttons to Settings
* Handles “search” and “view app” deep links
  * Search: `altstore://search?q=[query]`
  * View App: `altstore://viewApp?bundleID=[app bundle ID]`

### Improved

**Screenshots**

* Supports screenshots of different sizes
* Supports both iPhone and iPad specific screenshots
* Automatically rounds screenshots taken with Face ID iPhone
* Preview screenshots full-screen by tapping them from an app's store page
* Dismiss full-screen screenshots with swipe gesture

**App Verification**

* Verifies downloaded app version matches source
* Verifies downloaded app build version matches source
* Verifies downloaded app’s permissions match source
* Verifies downloaded .ipa matches SHA-256 hash (if provided)

**Source Verification**

* Verifies source's identifier doesn't change after refreshing
* Verifies source’s identifier doesn’t match existing sources when adding
* Verifies all privacy permissions have a valid `usageDescription`
* Throws error when adding marketplace source to non-marketplace AltStore (and vice versa)
* Includes missing last Coding Path value for DecodingError.keyNotFound
* Deprecates `identifier` key

**News Tab**

* Changed image aspect ratio to 3:2
* Updated font to use dynamic text styles
* Uses uniform height for all News Items on source's detail page

**Logging**

* Switched to OSLog.framework for important tasks
* Export detailed logs via Error Log from Settings tab

**Image Caching**

* Increased cache limit to reduce how often AltStore refetches images
* Clear image cache with “Clear Cache…” option in Settings

**Misc.**

* Limits relative dates to "Today" and "Yesterday"
* Changed "WiFi" spelling to "Wi-Fi"
* Displays version # for updates in My Apps tab
* Replaced AppCenter dependency with TelemetryDeck
* Added Privacy manifest
* Updated Patreon sign-out alert message to apply to all pledged apps
* Rethrows Core Data save errors after installing apps
* Captures `#fileID` and `#line` for `OperationError.appNotFound`
* Enforces consistent minimum size for `PillButton`
* Updates `AppViewController` to use `UINavigationBarAppearance` APIs

### Fixed

**Resigning Apps**

* Fixed various issues resigning certain apps
* Fixed app sometimes freezing when installing/refreshing apps
* Fixed resigning apps with entitlements the original app doesn’t have
* Fixed resigning apps without required entitlements
* Fixed resigning apps with wildcard \`keychain-access-groups\` entitlement
* Fixed resigning apps with non-English alphanumeric characters in name

**User Interface**

* Fixed Settings tab bar disappearing on iOS 18
* Fixed squished banners on App IDs screen
* Fixed button titles flashing when scrolling into view
* Fixed incorrect corner radius animation for app + source detail screens
* Fixed "More" button appearing by accident if text height exactly equals collapsed height
* Fixed not showing "more updates" button when there are more than 2 updates
* Fixed erroneously showing “Unsupported Updates Available” message
* Fixed showing “Update” button on app store page when no supported update is available
* Fixed incorrect cell height for some News items
* Fixed missing blur when pushing `AppViewController` onto modal navigation controller

**Misc.**

* Fixed crash when adding source with the same name as another source
* Fixed “Core Data error” if error occurs while parsing Source JSON
* Fixed redundant app update appearing after failing to backup/restore app
* Fixed not showing toast view if error occurs during initial sources fetch
* Fixed incorrectly handling various cancelled operations
* Fixed error fetching Friend Zone patrons due to unexpected nil name
* Fixed incorrectly merging app versions for same app from different sources
* Fixed migration error on launch if AltStore app group does not exist
* Fixed "missing app group" error if AltStore app group is not the first one listed in Info.plist
* Fixed accidentally saving "Operation Cancelled" errors to Error Log
* \[iPad] Fixed crash when removing apps from My Apps tab
* Fixed `CollapsingTextView` “TextKit 1 compatibility mode” runtime warning
* Fixed "transformable properties not using secure transformer" runtime warnings
* Fixed "unsatisfiable constraints" runtime error for `InstalledAppsCollectionFooterView`



## <mark style="color:green;">AltStore 1.7</mark>

<mark style="color:green;">**September 18, 2023**</mark>

### New

**"Active Apps" Widget (iOS 17+)**&#x20;

* View remaining days for ALL active apps from Home Screen
* Refresh apps directly from home screen by tapping countdown timers

### Improved

**Shortcuts Support**

* Converted existing "Refresh Apps" shortcut into App Shortcut
* Available by default in "App Shortcuts" section of Shortcuts app
* Displays accurate progress when refreshing apps via Shortcuts app

**Widgets**

* Updated existing home screen widget to support refreshing apps by tapping countdown (iOS 17+)
* Explicitly reloads widget timelines on app launch

### Fixed

* Fixed updating apps with manually-removed app extensions (e.g. uYou+)
* Fixed not refreshing AltStore last when refreshing via Shortcut
* Fixed race condition causing duplicate background refresh notifications (or none)
* Fixed Error Log not displaying all detailed info for certain errors

##

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

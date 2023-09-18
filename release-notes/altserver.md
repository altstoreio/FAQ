# 🖥 AltServer

## <mark style="color:blue;">AltServer 1.7 (macOS only)</mark>

<mark style="color:blue;">**September 18, 2023**</mark>

### **New**

* Mail Plug-in no longer required!
* Supports macOS 14 Sonoma

**`altjit` CLI**

* Command-line tool to enable JIT on iOS 17 devices
* Used internally by AltServer, but can be run manually via Terminal
* e.g. `AltServer.app/MacOS/altjit enable DolphiniOS --udid [device ID]`
* Requires installing additional dependencies (view [AltJIT page](https://faq.altstore.io/how-to-use-altstore/altjit) for instructions)
* Thanks to [pymobiledevice3](https://github.com/doronz88/pymobiledevice3) for their work on the iOS 17 Developer Disk format!

### Fixed

* Fixed AltJIT on iOS 17
* Fixed "About" panel appearing behind other apps
* Updates Copyright year to 2023

##

## <mark style="color:blue;">AltServer 1.6.1</mark>

<mark style="color:blue;">**February 20, 2023**</mark>

* Supports Apple IDs with Advanced Data Protection (ADP) enabled **(Windows)**



## <mark style="color:blue;">AltServer 1.6</mark>

<mark style="color:blue;">**January 30, 2023**</mark>

### **New**

#### Revamped Error Handling

* Completely revamped error handling to include as much information as possible, which should make debugging certain issues much easier
* Revised error messages to be more descriptive and provide more suggestions
* Adds “View More Details”/”Help” button to error alerts to view detailed error information
* Adds "Search FAQ" button to error alert
* Revised error domain format to `[Module].[ErrorType]`
* AltServer.ServerError codes start at 2000
* AltStore.AppleDeveloperError codes start at 3000
* Uses underlying error messages (if available) for several AltServer.ServerError errors
* Encodes/Decodes all Codable user info values, not just recognized types

#### iOS Version Compatibility

* Checks iOS compatibility before installing AltStore
* Downloads latest compatible AltStore version for your iOS device

### **Improved**

* Uses `CFBundleDisplayName` instead of `CFBundleName` for app name if it exists **(Windows)**
* Revised error messages to match AltServer macOS **(Windows)**

### **Fixed**

* Fixed error encoding CodableError Int/UInt user info values
* Fixed adding failures to NSErrors with nil localizedFailureReasons
* Fixed occasional crash when receiving requests from AltStore **(macOS)**
* Fixed installation alerts saying "iPhone" instead of actual device name **(macOS)**
* Fixed AltServer notification icon not appearing in Windows 11 22H2 taskbar **(Windows)**



## <mark style="color:blue;">AltServer 1.5.1</mark>

<mark style="color:blue;">**July 14, 2022**</mark>

* Fixed signing in with Apple IDs that contain capital letters
* Fixed signing in with Apple IDs that have 2FA enabled but don’t have any registered trusted devices
* Fixed incorrect “Developer Disk incompatible with \[iOS Version]” error when enabling AltJIT
* Fixed installing Mail plug-in after uninstalling it **(macOS)**
* Fixed memory leak when refreshing apps over WiFi **(macOS)**
* Fixed an issue causing wired connections to occasionally stall **(macOS)**
* Fixed an issue causing indefinite high CPU usage after enabling AltJIT **(Windows)**
* Fixed an issue causing indefinite high CPU usage after updating AltStore **(Windows)**



## <mark style="color:blue;">AltServer 1.5</mark>

<mark style="color:blue;">**May 3, 2022**</mark>

### **New**

#### AltJIT

* Allows sideloaded apps to use Just-in-Time (JIT) compilation
* Go to "Enable JIT" > \[Your Device] from the AltServer menu, then choose a sideloaded app
  * Your device must be on the same WiFi network as AltServer or connected to your computer via USB
* JIT will remain enabled until the app is quit from the app switcher or purged from memory in the background
* Requires iOS 14 or later

#### Direct .ipa Sideloading

* Sideload apps (.ipa's) directly to iOS devices without installing AltStore first
* Hold Option (macOS) or Shift (Windows) when clicking the AltServer icon to reveal new "Sideload .ipa…" menu option
* Supports iPhones and iPads running iOS 9.3 or later
* Supports Apple TVs running tvOS 9.3 or later **(macOS)**
  * For now, Apple TVs must be manually paired with Xcode first
* Apps sideloaded with AltServer must be manually re-installed every 7 days
  * Install AltStore to automatically refresh your sideloaded apps in the background

#### Multiple Device Support

* Install AltStore onto multiple iOS devices using the same Apple ID
* You must use the same computer to install AltStore each time

#### Mail Plug-in Improvements (macOS)

* AltPlugin can now be updated independently from AltServer&#x20;
* AltPlugin is no longer required if both System Integrity Protection (SIP) and Apple Mobile File Integrity (AMFI) are disabled

### Improved

* Added “…” to menu items that require additional user input to match macOS HIG **(macOS)**
* Prefers “Individual” paid teams over free teams if there are multiple Apple Developer teams associated with your Apple ID
* Revokes the previous iOS Development certificate created by AltStore (if one exists) instead of revoking a random one
* Updated “Cannot activate more than 3 apps” error alert to list all sideloaded app bundle IDs
* Revised code signing logic to more accurately match Apple’s codesign tool
* Improved error message when authenticating with invalid anisette data
* Improved error messages for libimobiledevice errors
* Improved error messages for various AltServer-specific errors
* Updated libimobiledevice dependency to 1.3.0
* Updated LaunchAtLogin dependency to 4.1.0 **(macOS)**

### Fixed

* Fixed “App Group does not exist” error when sideloading apps
* Fixed a potential crash when disconnecting an iOS device from your computer
* Fixed a potential crash when sideloading certain apps
* Fixed potentially registering an app group twice when sideloading an app containing app extensions
* Fixed “RSTPlaceholderView.nib couldn’t be saved” error when sideloading apps **(macOS)**
* Fixed duplicate “Revoke Development Certificate” alerts when sideloading apps **(macOS)**
* Fixed issue unzipping .ipa’s with unexpected files in Payload directory **(Windows)**
* Fixed ignoring some error responses from Apple’s developer servers **(Windows)**
* Fixed memory leak when parsing responses from Apple’s developer servers **(Windows)**
* Fixed various memory leaks when managing a device’s provisioning profiles **(Windows)**
* Fixed various memory leaks when installing AltStore or sideloading .ipa’s **(Windows)**

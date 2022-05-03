# 🖥 AltServer

## <mark style="color:blue;">AltServer 1.5</mark>

<mark style="color:blue;">**May 3, 2022**</mark>

### **New**

**AltJIT**

* Allows sideloaded apps to use Just-in-Time (JIT) compilation
* Go to "Enable JIT" > \[Your Device] from the AltServer menu, then choose a sideloaded app
  * Your device must be on the same WiFi network as AltServer or connected to your computer via USB
* JIT will remain enabled until the app is quit from the app switcher or purged from memory in the background
* Requires iOS 14 or later

**Direct .ipa Sideloading**

* Sideload apps (.ipa's) directly to iOS devices without installing AltStore first
* Hold Option (macOS) or Start (Windows) when clicking the AltServer icon to reveal new "Sideload .ipa…" menu option
* Supports iPhones and iPads running iOS 9.3 or later
* Supports Apple TVs running tvOS 9.3 or later **(macOS)**
  * For now, Apple TVs must be manually paired with Xcode first
* Apps sideloaded with AltServer must be manually re-installed every 7 days
  * Install AltStore to automatically refresh your sideloaded apps in the background

**Multiple Device Support**

* Install AltStore onto multiple iOS devices using the same Apple ID
* You must use the same computer to install AltStore each time

**Mail Plug-in Improvements (macOS)**

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

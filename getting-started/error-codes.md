---
description: >-
  This page includes a list of various error codes you may receive while using
  AltStore.
---

# ⚠ Error Codes

## AltServer Errors

#### <mark style="color:purple;">**(1) Could not connect to AltServer. / There was an error connecting to the device.**</mark>&#x20;

`com.rileytestut.AltServer`

This means that AltServer is having trouble connecting to your iOS device. Try plugging your device directly into your computer if it is not already.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(2) Lost Connection to AltServer.**</mark>

`com.rileytestut.AltServer`

This means that the connection was dropped between AltServer and your iOS device. Make sure your device and computer are connected to the same WiFi network and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(3) AltServer could not find this device.**</mark>

`com.rileytestut.AltServer`

This means that AltServer had trouble locating your iOS device either over USB or via WiFi. Make sure your device and computer are connected to the same WiFi network and that your device is trusted and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).

<mark style="color:purple;">****</mark>

#### <mark style="color:purple;">**(4) Failed to write app data to device.**</mark>

`com.rileytestut.AltServer`

This means that AltServer tried to write a file to your device and could not or was interrupted. Make sure your device and computer are connected to the same WiFi network and that your device is trusted and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(5) AltServer received an invalid request.**</mark>

`com.rileytestut.AltServer`

This means that AltServer received a request it did not understand. This may be because you are running an outdated AltServer version, so please make sure to update to the latest version.



#### <mark style="color:purple;">**(6) AltServer sent an invalid response.**</mark>

`com.rileytestut.AltServer`

This means that AltStore received a response from AltServer it did not understand. This may be because you are running an outdated AltStore version, so please make sure to update to the latest version.



#### <mark style="color:purple;">**(7) The app is invalid.**</mark>

`com.rileytestut.AltServer`

This means that the app your were attempting to install was found to be in an invalid format. If you continue to have issues, try downloading from alternate source.



#### <mark style="color:purple;">**(8) An error occurred while installing the app.**</mark>

`com.rileytestut.AltServer`

This means that iOS rejected the app you were attempting to install. Make sure to use a version compatible your iOS version.



#### <mark style="color:purple;">**(9) Cannot activate more than 3 apps with a non-developer Apple ID.**</mark>

`com.rileytestut.AltServer`

This means that you do not have enough available App IDs to install the requested App. For more information, refer to our [App IDs page](../how-to-use-altstore/app-ids.md).



#### <mark style="color:purple;">**(10) Your device must be running iOS 12.2 or later to install AltStore.**</mark>

`com.rileytestut.AltServer`

This means that you will need to update your phone to the minimum iOS version required before you can continue to use AltStore.



#### <mark style="color:purple;">**(11) AltServer does not support this request.**</mark>

`com.rileytestut.AltServer`

This means that AltServer received a request it did not recognize. You may be running an outdated AltServer version, so be sure to update.



#### <mark style="color:purple;">**(12) Received an unknown response from AltServer.**</mark>

`com.rileytestut.AltServer`

This means that AltStore received a response from AltServer it did not recognize. You may be running an outdated AltStore version, so be sure to update.



#### <mark style="color:purple;">**(13) The provided anisette data is invalid.**</mark>

`com.rileytestut.AltServer`

This means that the Apple ID information AltStore used to try to sign in was invalid because of an unknown issue. Make sure you are using the latest version of iCloud if you are on Windows and that your date/time are accurate.



#### <mark style="color:purple;">**(14) AltServer could not connect to Mail plug-in. (macOS)**</mark>

`com.rileytestut.AltServer`

This means that AltServer could not find the Mail plug-in either because it is not enable or you are not running the mail app on your Mac. Make sure the mail app is running on your Mac and that the plug-in is enabled. For more help, check the [Mail Plug-In](how-to-install-altstore-macos/enable-mail-plug-in.md) page in the install guide.



#### <mark style="color:purple;">**(15) Could not find provisioning profile.**</mark>

`com.rileytestut.AltServer`

This means that the provisioning profile needed to install this app could not be located. This is most likely a problem with AltStore itself, so please message support or to our Patreon inbox.



#### <mark style="color:purple;">**(16) An error occurred while removing the app.**</mark>

`com.rileytestut.AltServer`

This means that there was an issue while removing an app. There are a number of different issues so make sure to check your error log for a more specific message on your issue.&#x20;

****

#### <mark style="color:purple;">**(100) The Requested app is not currently running on the device.**</mark>

`com.rileytestut.AltServer`

This means that **** you tried to enable JIT without the requested app running in the foreground. Make sure to launch the app and have it running before you enable JIT.



#### <mark style="color:purple;">**(101) The disk is incompatible with \[App].**</mark>

`com.rileytestut.AltServer`

This means that the developer disk being used is not compatible with the app. Try updating to the latest version of AltStore and AltServer to make sure the correct one is enabled.

<mark style="color:purple;">****</mark>

## **Apple Errors**

#### <mark style="color:purple;">**(0) An unknown error occurred.**</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon

****

#### <mark style="color:purple;">**(1)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The provided parameters are invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon



#### <mark style="color:purple;">**(2)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">Incorrect Apple ID or password.</mark>

`com.rileytestut.ALTAppleAPI`

This means that the Apple ID credentials you used were invalid. Make sure the username and password are correct.&#x20;

If you still have issues, you can also try creating a new Apple ID to use with AltStore.

****

#### <mark style="color:purple;">**(3)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">You are not a member of any development teams.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(4) An app-specific password is required. You can create one at appleid.apple.com.**</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(5) T**</mark><mark style="color:purple;">his device's UDID is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(6) T**</mark><mark style="color:purple;">his device's UDID is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(7)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The certificate request is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(8)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The certificate request is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(9)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">There is no certificate with the requested serial number for this team.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">**(10)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The name for this app is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(11) The bundle identifier for this app is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(12) The bundle identifier for this app has already been registered.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(13) There is no App ID with the requested identifier on this team.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(14) You may only register 10 App IDs every 7 days.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(15) The provided app group is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(16) App group does not exist.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(17) The identifier for the requested provisioning profile is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(18) There is no provisioning profile with the requested identifier on this team.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(19) This account requires signing in with two-factor authentication.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(20) Incorrect verification code.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(21) Failed to perform authentication handshake with server.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.



#### <mark style="color:purple;">(22) The provided anisette data is invalid.</mark>

`com.rileytestut.ALTAppleAPI`

Updated information coming soon.

## **Windows Errors**

<mark style="color:purple;">**(1100) Your session has expired. Please log in.**</mark>&#x20;

NSURLErrorDomain

1. Make sure iTunes is closed.&#x20;
2. Go to Program Data -> Apple Computer -> iTunes -> ADI -> delete the files&#x20;
3. Start iTunes&#x20;
4. Retry installing AltStore&#x20;

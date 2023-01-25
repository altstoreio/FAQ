---
description: >-
  This page includes a list of various error codes you may receive while using
  AltStore.
---

# ⚠ Error Codes



## AltStore Errors

#### <mark style="color:purple;">**(1000) An unknown error occurred.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore...

#### <mark style="color:purple;">****</mark>

#### <mark style="color:purple;">**(1001) The operation returned an unknown result.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1002) The operation was cancelled.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore could not complete the requested action because it was stopped by the user.



#### <mark style="color:purple;">**(1003) The operation timed out.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1004) You are not signed in.**</mark>&#x20;

`AltStore.OperationError`

This means that you must enter your Apple ID information in the settings tab to do the requested action.



#### <mark style="color:purple;">**(1005)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">AltStore could not determine this device's UDID.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1006) This app is in an invalid format**</mark><mark style="color:purple;">.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1007) Invalid parameters**</mark><mark style="color:purple;">.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1008)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">You cannot register more than 10 App IDs within a 7 day period.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1009)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">There are no AltStore sources.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1010)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">AltStore's shared app group could not be accessed.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1011) The app**</mark> <mark style="color:purple;">could not be found.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1012)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">AltStore was denied permission to launch the app.</mark>

`AltStore.OperationError`

This means that AltStore...



#### <mark style="color:purple;">**(1200)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">AltServer could not be found.</mark>

`AltStore.OperationError`

This means that AltStore is having trouble connecting to AltServer on your PC/Mac. Make sure you have Wi-Fi sync enabled, and otherwise you may try plugging in your device directly via USB.



#### <mark style="color:purple;">**(1201)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">A connection to AltServer could not be established.</mark>

`AltStore.OperationError`

This means that AltStore is having trouble connecting to AltServer on your PC/Mac. Make sure you have Wi-Fi sync enabled, and otherwise you may try plugging in your device directly via USB.



#### <mark style="color:purple;">**(1202)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The connection to AltServer was dropped.</mark>

`AltStore.OperationError`

This means that AltStore's connection to AltServer on your PC/Mac was interrupted. Make sure you have Wi-Fi sync enabled, and otherwise you may try plugging in your device directly via USB.





## AltServer Errors

#### <mark style="color:purple;">**(1999) Underlying Error**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer ran into an unknown error. We recommend reaching out to our support channels if the issue persists.



#### <mark style="color:purple;">**(20000) Unknown Error**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer ran into an unknown error. We recommend reaching out to our support channels if the issue persists.



#### <mark style="color:purple;">**(2000) Could not connect to AltServer. / There was an error connecting to the device.**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer is having trouble connecting to your iOS device. Try plugging your device directly into your computer if it is not already.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).

#### <mark style="color:purple;">****</mark>

#### <mark style="color:purple;">**(2001) Could not connect to AltServer. / There was an error connecting to the device.**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer is having trouble connecting to your iOS device. Try plugging your device directly into your computer if it is not already.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(2002) Lost Connection to AltServer.**</mark>

`AltServer.ServerError`

This means that the connection was dropped between AltServer and your iOS device. Make sure your device and computer are connected to the same WiFi network and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(2003) AltServer could not find this device.**</mark>

`AltServer.ServerError`

This means that AltServer had trouble locating your iOS device either over USB or via WiFi. Make sure your device and computer are connected to the same WiFi network and that your device is trusted and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).

<mark style="color:purple;">****</mark>

#### <mark style="color:purple;">**(2004) Failed to write app data to device.**</mark>

`AltServer.ServerError`

This means that AltServer tried to write a file to your device and could not or was interrupted. Make sure your device and computer are connected to the same WiFi network and that your device is trusted and try again.

If you still have issues, please refer to the [Troubleshooting Guide](troubleshooting-guide.md).



#### <mark style="color:purple;">**(2005) AltServer received an invalid request.**</mark>

`AltServer.ServerError`

This means that AltServer received a request it did not understand. This may be because you are running an outdated AltServer version, so please make sure to update to the latest version.



#### <mark style="color:purple;">**(2006) AltServer sent an invalid response.**</mark>

`AltServer.ServerError`

This means that AltStore received a response from AltServer it did not understand. This may be because you are running an outdated AltStore version, so please make sure to update to the latest version.



#### <mark style="color:purple;">**(2007) The app is invalid.**</mark>

`AltServer.ServerError`

This means that the app your were attempting to install was found to be in an invalid format. If you continue to have issues, try downloading from alternate source.



#### <mark style="color:purple;">**(2008) An error occurred while installing the app.**</mark>

`AltServer.ServerError`

This means that iOS rejected the app you were attempting to install. Make sure to use a version compatible your iOS version.



#### <mark style="color:purple;">**(2009) Cannot activate more than 3 apps with a non-developer Apple ID.**</mark>

`AltServer.ServerError`

This means that you do not have enough available App IDs to install the requested App. For more information, refer to our [App IDs page](../how-to-use-altstore/app-ids.md).



#### <mark style="color:purple;">**(2010) Your device must be running iOS 12.2 or later to install AltStore.**</mark>

`AltServer.ServerError`

This means that you will need to update your phone to the minimum iOS version required before you can continue to use AltStore.



#### <mark style="color:purple;">**(2011) AltServer does not support this request.**</mark>

`AltServer.ServerError`

This means that AltServer received a request it did not recognize. You may be running an outdated AltServer version, so be sure to update.



#### <mark style="color:purple;">**(2012) Received an unknown response from AltServer.**</mark>

`AltServer.ServerError`

This means that AltStore received a response from AltServer it did not recognize. You may be running an outdated AltStore version, so be sure to update.



#### <mark style="color:purple;">**(2013) The provided anisette data is invalid.**</mark>

`AltServer.ServerError`

This means that the Apple ID information AltStore used to try to sign in was invalid because of an unknown issue. Make sure you are using the latest version of iCloud if you are on Windows and that your date/time are accurate.



#### <mark style="color:purple;">**(2014) AltServer could not connect to Mail plug-in. (macOS)**</mark>

`AltServer.ServerError`

This means that AltServer could not find the Mail plug-in either because it is not enable or you are not running the mail app on your Mac. Make sure the mail app is running on your Mac and that the plug-in is enabled. For more help, check the [Mail Plug-In](how-to-install-altstore-macos/enable-mail-plug-in.md) page in the install guide.



#### <mark style="color:purple;">**(2015) Could not find provisioning profile.**</mark>

`AltServer.ServerError`

This means that the provisioning profile needed to install this app could not be located. This is most likely a problem with AltStore itself, so please message support or to our Patreon inbox.



#### <mark style="color:purple;">**(2016) An error occurred while removing the app.**</mark>

`AltServer.ServerError`

This means that there was an issue while removing an app. There are a number of different issues so make sure to check your error log for a more specific message on your issue.&#x20;

****

#### <mark style="color:purple;">**(2100) The Requested app is not currently running on the device.**</mark>

`AltServer.ServerError`

This means that **** you tried to enable JIT without the requested app running in the foreground. Make sure to launch the app and have it running before you enable JIT.



#### <mark style="color:purple;">**(2101) The disk is incompatible with \[App].**</mark>

`AltServer.ServerError`

This means that the developer disk being used is not compatible with the app. Try updating to the latest version of AltStore and AltServer to make sure the correct one is enabled.

<mark style="color:purple;">****</mark>

## **Apple Developer Errors**

#### <mark style="color:purple;">**(3000) An unknown error occurred.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon

****

#### <mark style="color:purple;">**(3001)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The provided parameters are invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon



#### <mark style="color:purple;">**(3002)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">Incorrect Apple ID or password.</mark>

`AltStore.AppleDeveloperError`

This means that the Apple ID credentials you used were invalid. Make sure the username and password are correct.&#x20;

If you still have issues, you can also try creating a new Apple ID to use with AltStore.

****

#### <mark style="color:purple;">**(3003)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">You are not a member of any development teams.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3004) An app-specific password is required. You can create one at appleid.apple.com.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3005) T**</mark><mark style="color:purple;">his device's UDID is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3006) T**</mark><mark style="color:purple;">his device's UDID is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3007)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The certificate request is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3008)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The certificate request is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3009)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">There is no certificate with the requested serial number for this team.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3010)**</mark> <mark style="color:purple;"></mark><mark style="color:purple;">The name for this app is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">11) The bundle identifier for this app is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">12) The bundle identifier for this app has already been registered.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">13) There is no App ID with the requested identifier on this team.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">14) You may only register 10 App IDs every 7 days.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">15) The provided app group is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">16) App group does not exist.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">17) The identifier for the requested provisioning profile is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">18) There is no provisioning profile with the requested identifier on this team.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">19) This account requires signing in with two-factor authentication.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">20) Incorrect verification code.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">21) Failed to perform authentication handshake with server.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">(</mark><mark style="color:purple;">**30**</mark><mark style="color:purple;">22) The provided anisette data is invalid.</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



## **Connection Errors**

#### <mark style="color:purple;">**(0) Error Unknown.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(1) Device Locked.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(2) Invalid Request.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(3) Invalid Response.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(4) Usbmuxd.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(5) SSL Error.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



#### <mark style="color:purple;">**(6) Timed Out.**</mark>

`AltServer.ConnectionError`

Updated information coming soon



## **Windows Errors**

<mark style="color:purple;">**(1100) Your session has expired. Please log in.**</mark>&#x20;

`NSURLErrorDomain`

1. Make sure iTunes is closed.&#x20;
2. Go to Program Data -> Apple Computer -> iTunes -> ADI -> delete the files&#x20;
3. Start iTunes&#x20;
4. Retry installing AltStore&#x20;

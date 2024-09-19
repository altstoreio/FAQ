---
description: >-
  This page includes a list of various error codes you may receive while using
  AltStore.
---

# ⚠️ Error Codes



## AltStore Errors



#### <mark style="color:purple;">**(1000) An unknown error occurred.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore ran into an unexpected error. Please check our [Troubleshooting Guide](troubleshooting-guide.md), and you can reach out to us directly if the issue persists.

####

#### <mark style="color:purple;">**(1001) The operation returned an unknown result.**</mark>&#x20;

This means that AltStore ran into an unexpected error. Please check our [Troubleshooting Guide](troubleshooting-guide.md), and you can reach out to us directly if the issue persists.



#### <mark style="color:purple;">**(1002) The operation was cancelled.**</mark>&#x20;

`AltStore.OperationError`

This means that the performed action was stopped. Please try again.



#### <mark style="color:purple;">**(1003) The operation timed out.**</mark>&#x20;

`AltStore.OperationError`

This means that AltStore ran into problems trying to complete the requested action. Please try again and check our [Troubleshooting Guide](troubleshooting-guide.md) for additional help. You can reach out to us directly if the issue persists.



#### <mark style="color:purple;">**(1004) You are not signed in.**</mark>&#x20;

`AltStore.OperationError`

This means that you must enter your Apple ID information in the settings tab to do the requested action.



#### <mark style="color:purple;">**(1005) The app**</mark> <mark style="color:purple;">**could not be found.**</mark>

`AltStore.OperationError`

This means that AltStore could not locate the file to download or install, most likely because the file does not exist at the provided URL.



#### <mark style="color:purple;">**(1006) AltStore could not determine this device's UDID.**</mark>

`AltStore.OperationError`

This means that AltStore couldn't read the device UDID embedded by AltServer when installing AltStore. Make sure you're installing AltStore with the latest AltServer version and not via another method.



#### <mark style="color:purple;">**(1007) This app is in an invalid format**</mark><mark style="color:purple;">.</mark>

`AltStore.OperationError`

This means the app you're trying to install is not a standard .ipa. Try downloading the app from another location.



#### <mark style="color:purple;">**(1008) Invalid parameters**</mark><mark style="color:purple;">.</mark>

`AltStore.OperationError`

This means an internal error occured and AltStore couldn't provide the necessary information to perform the requested task. Please try again and check our [Troubleshooting Guide](troubleshooting-guide.md) for additional help. You can reach out to us directly if the issue persists.



#### <mark style="color:purple;">**(1009) You cannot register more than 10 App IDs within a 7 day period**</mark>.

`AltStore.OperationError`

This means that you have reached the maximum amount of App IDs available. Please check the App IDs in the My Apps tab to see when they will expire.



#### <mark style="color:purple;">**(1010) There are no AltStore sources.**</mark>

`AltStore.OperationError`

This means an internal error occured and AltStore is unable to fetch changes for any Sources you've added. Please try again and check our [Troubleshooting Guide](troubleshooting-guide.md) for additional help. You can reach out to us directly if the issue persists.



#### <mark style="color:purple;">**(1011) AltStore was denied permission to launch the app.**</mark>

`AltStore.OperationError`

This means AltStore couldn't launch a sideloaded app because you tapped "Cancel" on the "AltStore wants to open \[app]" alert, or because you still need to trust your Apple ID in Settings.



#### <mark style="color:purple;">**(1012) AltStore's shared app group could not be accessed.**</mark>

`AltStore.OperationError`

This means AltStore was not able to access the directory where app backups are stored. Make sure you're installing AltStore with the latest AltServer version and not via another method.



#### <mark style="color:purple;">**(1200) AltServer could not be found.**</mark>

`AltStore.OperationError`

This means that AltStore is having trouble discovering AltServer on your local network. Make sure you're connected to the same WiFi network as your PC/Mac running AltServer, or try connecting your device to your computer via USB.



#### <mark style="color:purple;">**(1201) A connection to AltServer could not be established.**</mark>

`AltStore.OperationError`

This means that AltStore is having trouble connecting to AltServer on your PC/Mac. Make sure you have Wi-Fi sync enabled, and otherwise you may try plugging in your device directly via USB.



#### <mark style="color:purple;">**(1202) The connection to AltServer was dropped.**</mark>

`AltStore.OperationError`

This means that AltStore's connection to AltServer on your PC/Mac was interrupted. Make sure you have Wi-Fi sync enabled, and otherwise you may try plugging in your device directly via USB.





## AltServer Errors

#### <mark style="color:purple;">**(0) Exception Error**</mark>

`AltServer.ExceptionError`

This error can appear for many reasons, and below are a few that you might see (this is not an exhaustive list).

#### "vector too long"

This means that Windows Defender is blocking your request. You may need to first disable Real-Time Protection on Windows in order for AltStore to work as expected.

####

#### <mark style="color:purple;">**(1999) Underlying Error**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer ran into an unknown error. We recommend reaching out to our support channels if the issue persists.



#### <mark style="color:purple;">**(2000) Unknown Error**</mark>&#x20;

`AltServer.ServerError`

This means that AltServer ran into an unknown error. We recommend reaching out to our support channels if the issue persists.



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

This means that you have reached the maximum amount of sideloaded apps you can have with a Free Developer Account. Apple limits the amount of sideloaded apps you can have with a free account, and to remove the limit you need to sign up for a Paid Developer account at [developer.apple.com](https://developer.apple.com).

You can also remove this limit if you have a device capable of using the [MacDirtyCow](macdirtycow.md) exploit



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

This means that AltServer could not find the Mail plug-in either because it is not enable or you are not running the Mail app on your Mac. Make sure the Mail app is running on your Mac and that the plug-in is enabled. For more help, check the [Mail Plug-In](how-to-install-altstore-macos/enable-mail-plug-in.md) page in the install guide.



#### <mark style="color:purple;">**(2015) Could not find provisioning profile.**</mark>

`AltServer.ServerError`

This means that the provisioning profile needed to install this app could not be located. This is most likely a problem with AltStore itself, so please message support or to our Patreon inbox.



#### <mark style="color:purple;">**(2016) An error occurred while removing the app.**</mark>

`AltServer.ServerError`

This means that there was an issue while removing an app. There are a number of different issues so make sure to check your error log for a more specific message on your issue.&#x20;



#### <mark style="color:purple;">**(2100) The Requested app is not currently running on the device.**</mark>

`AltServer.ServerError`

This means that you tried to enable JIT without the requested app running in the foreground. Make sure to launch the app and have it running before you enable JIT.



#### <mark style="color:purple;">**(2101) The disk is incompatible with \[iOS version].**</mark>

`AltServer.ServerError`

This means that the developer disk required to enable JIT is not compatible with your device's OS version. Make sure you're running the latest version of AltStore and AltServer, and try again later.



## **Apple Developer Errors**

#### <mark style="color:purple;">**(3000) An unknown error occurred.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon



#### <mark style="color:purple;">**(3001) The provided parameters are invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon



#### <mark style="color:purple;">**(3002) Incorrect Apple ID or password.**</mark>

`AltStore.AppleDeveloperError`

This means that the Apple ID credentials you used were invalid. Make sure the username and password are correct.&#x20;

If you still have issues, you can also try creating a new Apple ID to use with AltStore.



#### <mark style="color:purple;">**(3003) An app-specific password is required. You can create one at appleid.apple.com.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3004) You are not a member of any development teams.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3005) This device's UDID is invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3006) This device is already registered with another ID.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3007) The certificate request is invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3008) There is no certificate with the requested serial number for this team.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3009) The name for this app is invalid.**</mark>

`AltStore.AppleDeveloperError`

AltStore couldn’t register an App ID with Apple because the app name contains non-ASCII characters. You can try downloading from another source.



#### <mark style="color:purple;">**(3010) The bundle identifier for this app is invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3011) The bundle identifier for this app has already been registered.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3012) There is no App ID with the requested identifier on this team.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3013) You may only register 10 App IDs every 7 days.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3014) The provided app group is invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3015) App group does not exist.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3016) The identifier for the requested provisioning profile is invalid.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3017) There is no provisioning profile with the requested identifier on this team.**</mark>

`AltStore.AppleDeveloperError`

If you are seeing this error, it's likely due to a recent server-side change made by Apple. Please see the following announcement with more info: [https://twitter.com/altstoreio/status/1638599316762664974?s=20](https://twitter.com/altstoreio/status/1638599316762664974?s=20)



#### <mark style="color:purple;">**(3018) This account requires signing in with two-factor authentication.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3019) Incorrect verification code.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.

####

#### <mark style="color:purple;">**(3020) Failed to perform authentication handshake with server.**</mark>

`AltStore.AppleDeveloperError`

Updated information coming soon.



#### <mark style="color:purple;">**(3021) The provided anisette data is invalid.**</mark>

`AltStore.AppleDeveloperError`

This error means that the information used to authenticate your AppleID information either expired or invalid. Make sure your computer date and time are accurate and that you’ve installed iTunes and iCloud from Apple.



## **Apple API Error**

#### <mark style="color:purple;">(1100) Your session has expired.</mark>

`Apple.APIError`

This error means that the information used to authenticate your Apple ID is either expired or invalid. Make sure your computer's date and time are accurate and try again.



#### <mark style="color:purple;">(1102) Apple ID cannot be used for development.</mark>

`Apple.APIError`

You may need to agree to Apple’s Terms of Service on [developer.apple.com](https://developer.apple.com). If that doesn’t work, you can create a new “throwaway” Apple ID dedicated to sideloading.



#### <mark style="color:purple;">(-20101) Your account information was entered incorrectly.</mark>

`Apple.APIError`

This error means that the username or password used to authenticate your Apple ID is either expired or invalid. Make sure you've entered them both in correctly and that your computer's date and time are accurate.



## **Connection Errors**

#### <mark style="color:purple;">**(0) Error Unknown.**</mark>

`AltServer.ConnectionError`

This means that AltServer ran into an unknown error. We recommend reaching out to our support channels if the issue persists.



#### <mark style="color:purple;">**(1) Device Locked.**</mark>

`AltServer.ConnectionError`

This means that you will need to unlock your device before AltServer can connect.



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



## Other Errors

#### <mark style="color:purple;">(512) Failed to write to disk</mark>

`NSCocoaErrorDomain`

This means that an error occurred while writing files to disk. Make sure your phone and PC both have plenty of available disk space and try again.



#### <mark style="color:purple;">**(1) AltJIT failed with error code 1 (iOS 17)**</mark>

`AltServer.ProcessError`

If you are trying to enable JIT on an iOS 17 device, you may see this error. Make sure to install all dependencies and keep your device connected with the app open until JIT has successfully been enabled. Instructions for this can be found [here](altjit.md#ios-17-instructions-macos-only).

---
description: >-
  Having problems with AltStore or AltServer? Try some of these troubleshooting
  tips!
---

# 🙋 Troubleshooting Guide

### Installation&#x20;

#### <mark style="color:purple;">I followed the instructions, but I still can't install AltStore.</mark>

Please make sure you tried the following:

* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by opening Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) with your device connected to your Mac and seeing if a dialog box pops up asking if you want to trust the device.
* Try using another Apple ID. If necessary, you can [create a new Apple ID](https://appleid.apple.com/account#!\&page=create) specifically for use with AltStore for free.
* Make sure iTunes and/or iCloud are running while using AltServer.
* (Windows) Right-click AltServer and choose “Run as Administrator”&#x20;
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.

### Sign-In

#### <mark style="color:purple;">AltStore freezes/takes forever to sign-in.</mark>

This could happen for a number of reasons. If you’re experiencing this issue, please check the following:

* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting your computer to your phone’s hotspot and trying again. (If you're using an iPad, make sure it's connected to your hotspot as well.)
* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) and seeing if a dialog box pops up asking if you want to trust your phone.
* (Windows) Firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* You may need to make sure iTunes and iCloud are running on your computer as well.
* Finally, try plugging your iPhone or iPad into your computer. This should fix all connectivity problems, but does mean AltStore may not be able to automatically refresh apps for you in the background over WiFi.

### AltServer

#### <mark style="color:purple;">AltStore says “Could not find AltServer” when trying to sideload or refresh apps.</mark>

AltServer must be running on a computer connected to the same WiFi as AltStore in order to sideload or refresh apps. If AltServer is running on the same WiFi network as AltStore and you're still receiving this error, try the following:

* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting your computer to your phone’s hotspot and trying again. (If you're using an iPad, make sure it's connected to your hotspot as well.)
* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) and seeing if a dialog box pops up asking if you want to trust your phone.
* (Windows) Your firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* Finally, try plugging your iPhone or iPad into your computer. This should fix all connectivity problems, but does mean AltStore may not be able to automatically refresh apps for you in the background over WiFi.

#### <mark style="color:purple;">I’m unable to change my network settings to allow devices to communicate with each other (such as on school/work/public WiFi).</mark>

You can always sideload and refresh apps without WiFi by plugging your iPhone or iPad into your computer. However, this means AltStore may not be able to refresh apps for you in the background over WiFi.



### AltJIT

#### <mark style="color:purple;">AltServer says “JIT could not be enabled for \[App]".</mark>

This could happen for a number of reasons. If you’re experiencing this issue, please check the following:

* Make sure the app you are trying to enable JIT for is running in the foreground on your device.
* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting your computer to your phone’s hotspot and trying again. (If you're using an iPad, make sure it's connected to your hotspot as well.)
* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) and seeing if a dialog box pops up asking if you want to trust your phone.
* (Windows) Firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* You may need to make sure iTunes and iCloud are running on your computer as well.
* Finally, try plugging your iPhone or iPad into your computer. This should fix all connectivity problems, but does mean AltStore may not be able to automatically refresh apps for you in the background over WiFi.

{% hint style="info" %}
If you can't find the answer to your question here, you can email [support@altstore.io](mailto:support@altstore.io) and we will try to get back to you as soon as we can.&#x20;
{% endhint %}



### What if I need to use the Windows Store version of iCloud?

AltStore requires that you install iCloud directly from Apple in order to authenticate your Apple ID. If you need to use the Windows Store version instead, you can follow these alternate instructions copied from [this reddit post](https://www.reddit.com/r/jailbreak/comments/rp5buz/tutorial\_how\_to\_use\_altserver\_if\_you\_have\_to\_use/?utm\_source=share\&utm\_medium=ios\_app\&utm\_name=iossmf):

1. Download and install [iTunes](https://www.apple.com/itunes/) from the official Apple website. Make sure to **scroll down** and click on "Windows" next to the "Looking for other versions?" text.
2. Download and install [iCloud](https://support.apple.com/en-us/HT204283) from the official Apple website. Make sure to **scroll down** and click on the link in this text: "\* On Windows 7 and Windows 8, you can _download iCloud for Windows on Apple's website_".
3. Locate your "C:\Program Files (x86)\Common Files\Apple" folder. Copy the "Apple Application Support" and "Internet Services" folders, then create a new folder, name it anyway you want, and paste them in.
4. Remove iCloud from your computer. **DO NOT** remove iTunes! (Also, **NEVER** remove the "Apple Mobile Device Support" or the "Apple Application Support" that are installed alongside iTunes and iCloud.)
5. Install [iCloud](https://www.microsoft.com/store/productId/9PKTQ5699M62) from the Windows Store.
6. Download and install [AltServer](https://altstore.io/). When you open it for the first time, click on "Choose Folder...", and locate the folder you created in the 3rd step.

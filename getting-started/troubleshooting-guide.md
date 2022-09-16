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

<mark style="color:purple;">**AltStore says “Could not find AltServer” when trying to sideload or refresh apps.**</mark>

AltServer must be running on a computer connected to the same WiFi as AltStore in order to sideload or refresh apps. If AltServer is running on the same WiFi network as AltStore and you're still receiving this error, try the following:

* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting your computer to your phone’s hotspot and trying again. (If you're using an iPad, make sure it's connected to your hotspot as well.)
* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) and seeing if a dialog box pops up asking if you want to trust your phone.
* (Windows) Your firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* Finally, try plugging your iPhone or iPad into your computer. This should fix all connectivity problems, but does mean AltStore may not be able to automatically refresh apps for you in the background over WiFi.

#### <mark style="color:purple;">I’m unable to change my network settings to allow devices to communicate with each other (such as on school/work/public WiFi).</mark>

You can always sideload and refresh apps without WiFi by plugging your iPhone or iPad into your computer. However, this means AltStore may not be able to refresh apps for you in the background over WiFi.



### AltJIT

<mark style="color:purple;">**AltServer says “JIT could not be enabled for \[App]".**</mark>

This could happen for a number of reasons. If you’re experiencing this issue, please check the following:

* Make sure the app you are trying to enable JIT for is running in the foreground on your device.
* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting your computer to your phone’s hotspot and trying again. (If you're using an iPad, make sure it's connected to your hotspot as well.)
* Have you said “Trust” on both your Mac and iOS device after connecting your device to your Mac? You can check by Finder (macOS 10.15 Catalina or later) or iTunes (macOS 10.14 Mojave and earlier) and seeing if a dialog box pops up asking if you want to trust your phone.
* (Windows) Firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* You may need to make sure iTunes and iCloud are running on your computer as well.
* Finally, try plugging your iPhone or iPad into your computer. This should fix all connectivity problems, but does mean AltStore may not be able to automatically refresh apps for you in the background over WiFi.



### Common Error Codes

<mark style="color:purple;">**1100 - Your session has expired. Please log in. (Windows Only)**</mark>

1. Make sure iTunes is closed.&#x20;
2. Go to Program Data -> Apple Computer -> iTunes -> ADI -> delete the files&#x20;
3. Start iTunes&#x20;
4. Retry installing AltStore&#x20;

{% hint style="info" %}
If you can't find the answer to your question here, you can email [support@altstore.io](mailto:support@altstore.io) and we will try to get back to you as soon as we can.&#x20;
{% endhint %}

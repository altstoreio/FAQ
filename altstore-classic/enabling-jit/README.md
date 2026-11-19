# 🏎️ Enabling JIT

Just-In-Time Compilation (JIT)  is a technology that allows certain types of apps to run significantly faster, or even at all. iOS does not normally allow apps to use JIT for security reasons, but you can enable JIT for apps sideloaded with AltStore Classic by following the instructions below.

{% hint style="info" %}
Using JIT requires a one-time setup with a computer. For an alternative method of enabling JIT, see [AltJIT](altjit.md).
{% endhint %}

## Set-up Instructions

{% hint style="info" %}
These instructions only need to be done once to set your device up to use JIT.
{% endhint %}

### Install StikDebug&#x20;

<details>

<summary>StikDebug (AltStore Classic)</summary>

1. If you haven't already set up [remote AltServers](altstore-classic/remote-altservers.md), install LocalDevVPN from the [App Store](https://apps.apple.com/us/app/localdevvpn/id6755608044)
2. Add the [StikDebug Source](https://stikdebug.xyz/index.json) to AltStore Classic
3. Sideload StikDebug using AltStore Classic
4. Launch LocalDevVPN and tap 'Connect'
5. Press 'Allow' when prompted to add VPN Configurations and follow the instructions
6. Launch StikDebug

</details>

### Pair StikDebug

To enable JIT, you first need to download a program on your computer that will export information about your device.&#x20;

1. Download `idevice_pair` onto your computer
   1. [macOS](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--macos-universal.dmg)
   2. [Windows](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--windows-x86_64.exe)
   3. [Linux](https://github.com/jkcoxson/idevice_pair/releases/latest/download/idevice_pair--linux-x86_64.AppImage)
2. Plug your iPhone or iPad into your computer
3. Open `idevice_pair` and select your device
4. Click 'Create'
5. Select 'StikDebug (Sideloaded)'
   
## Enabling JIT

<details>

<summary>StikDebug (AltStore Classic)</summary>

1. Connect to Wi-Fi or enable Airplane Mode
2. Open LocalDevVPN and tap 'Connect'
3. Open AltStore Classic
4. Long-press an app in My Apps
5. Tap 'Enable JIT'
6. The chosen app will then launch with JIT enabled

</details>

{% hint style="warning" %}
If you see a 'Device Not Mounted' error alert, force-quit StikDebug and try again.
{% endhint %}


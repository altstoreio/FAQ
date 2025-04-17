# 🏎️ Enabling JIT

Just-In-Time Compilation (JIT)  is a technology that allows certain types of apps to run significantly faster, or even at all. iOS does not normally allow apps to use JIT for security reasons, but you can enable JIT for apps sideloaded with AltStore Classic by following the instructions below.

{% hint style="info" %}
Using JIT requires a one-time setup with a Mac or PC. For an alternative method of enabling JIT, see [AltJIT](altjit.md).
{% endhint %}

## Set-up Instructions

{% hint style="info" %}
These instructions only need to be done once to set your device up to use JIT.
{% endhint %}

#### Jitterbugpair (Mac/PC)

To enable JIT, you first need to download a program on your Mac or PC that will export information about your device.&#x20;

1. Download `jitterbugpair` onto your computer
   1. [macOS](https://cdn.altstore.io/file/altstore/altstore/jitterbugpair.zip)
   2. [Windows](https://github.com/osy/Jitterbug/releases/download/v1.3.1/jitterbugpair-win64.zip)
2. Plug your iPhone or iPad into your computer
3. Open Terminal (Mac) or PowerShell (Windows)
4. Drag `jitterbugpair` into the Terminal/PowerShell window and hit 'Enter'
5. Type `open .` then hit 'Enter' to open the output directory in Finder (Mac) or Explorer (Windows)
6. Locate the `.mobiledevicepairing` file and transfer it to your iOS device

#### Import File into StikDebug/SkitJIT&#x20;

Once you've created the pairing file, you can import it into StikDebug/StikJIT to enable JIT:

<details>

<summary>StikDebug (AltStore PAL)</summary>

1. Install StikDebug from the [StikDebug source](https://altstore-pal/source?url=https://stikdebug.xyz/apps.json)
2. Open StikDebug
3. Press "Allow" when prompted to add VPN Configurations and follow instructions
4. Tap 'Select Pairing File'
5. Select the `.mobiledevicepairing` file you transferred to your device in the above steps

</details>

<details>

<summary> StikJIT (AltStore Classic)</summary>

1. Install StosVPN from the [App Store](https://apps.apple.com/us/app/stosvpn/id6744003051)
2. Download StikJIT .ipa from [GitHub](https://github.com/0-Blu/StikJIT/releases)
3. Sideload StikJIT using AltStore Classic
4. Launch StosVPN and tap "Connect"
5. Press "Allow" when prompted to add VPN Configurations and follow instructions
6. Launch StikJIT
7. Tap 'Select Pairing File'
8. Select the `.mobiledevicepairing` file you transferred to your device in the above steps

</details>

## Enabling JIT

<details>

<summary>StikDebug (AltStore PAL)</summary>

1. Open AltStore Classic
2. Long-press an app in My Apps
3. Tap "Enable JIT"
4. The chosen app will then launch with JIT enabled

</details>

<details>

<summary>StikJIT (AltStore Classic)</summary>

1. Open StosVPN and tap "Connect"
2. Open AltStore Classic
3. Long-press an app in My Apps
4. Tap "Enable JIT"
5. The chosen app will then launch with JIT enabled

</details>

{% hint style="warning" %}
If you see a 'Device Not Mounted' error alert, force-quit StikDebug and try again.
{% endhint %}


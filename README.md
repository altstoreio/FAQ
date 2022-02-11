# FAQ Test

## FAQ Test

## General

#### **How do I install AltStore? (Mac)**

1. Download AltServer for Mac.
2. Copy “AltServer.app” to your Applications folder.
3. Launch AltServer (it will appear as an icon in the menu bar).
4. Connect your iPhone to your computer and make sure it is unlocked.
5. Trust your iPhone with your computer (if needed).
6. (Mojave only) Open iTunes and enable iTunes Wi-Fi sync for your phone.
7. (Catalina only) Open Finder and enable “Show this iPhone when on WiFi” for your phone.
8. Click the AltServer icon in the Mac menu bar, click “Install AltStore”, then choose your phone.
9. Enter your Apple ID email and password (NOTE: both email address and password are case sensitive).
10. (First time only) AltServer will ask you to install a Mail plug-in. Follow the instructions to continue (or see below for more detailed instructions).
11. Wait a few seconds, then AltStore will be installed to your phone.

#### **How do I install AltStore? (Windows)**

**Before Installing:**

1. Download the latest version of iTunes [directly from Apple](https://www.apple.com/itunes/) (**not** the Microsoft Store).
2. Download the latest version of iCloud [directly from Apple](https://support.apple.com/en-us/HT204283) (**not** the Microsoft Store).

**Installing:**

1. Download AltServer for Windows.
2. Extract the downloaded “AltInstaller.zip” file.
3. Double-click “setup.exe”, then follow the installation instructions.
4. Launch AltServer (it will appear as an icon in the Notification Area).
5. Trust your iPhone with your computer (if needed).
6. Open iTunes and enable iTunes Wi-Fi sync for your phone.
7. Click the AltServer icon in the Notification Area, click “Install AltStore”, then choose your phone.
8. Enter your Apple ID email and password (NOTE: both email address and password are case sensitive).
9. Wait a few seconds, then AltStore will be installed to your phone.

#### **How do I install the Mail plug-in? (Mac only)**

1. Click “Install Mail Plug-in” from the AltServer menu.
2. Enter your password to grant AltServer permission to install the plug-in.
3. Open Mail (quit Mail first if it was already running).
4. Open Mail > Preferences.
5. Click “Manage Plug-ins...”
6. Enable “AltPlugin.mailbundle”
7. Click “Apply and Restart Mail” to finish installation.

#### **I followed the instructions, why is AltStore still not installing for me?**

This could happen for a number of reasons, but these solutions have reportedly helped:

* Have you said “Trust” on both your computer and phone after connecting it to your computer? You can check by opening iTunes and seeing if a dialog box pops up asking if you want to trust your phone.
* Try using another Apple ID. If necessary, you can [create a new Apple ID](https://appleid.apple.com/account#!\&page=create) specifically for use with AltStore for free.
* (Windows only) Make sure iTunes and/or iCloud are running while using AltServer.
* (Windows only) Right-click AltServer and choose “Run as Administrator”.
* (Windows only) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.

#### **AltStore freezes/takes forever to sign-in.**

This could happen for a number of reasons. If you’re experiencing this issue, please check the following:

* (Windows only) Your Windows firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows only) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* (Windows only) You may need to make sure iTunes and iCloud are running on your computer as well.
* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting to your phone’s hotspot and trying again.
* Have you said “Trust” on both your computer and phone after connecting it to your computer? You can check by opening iTunes and seeing if a dialog box pops up asking if you want to trust your phone.
* Finally, try plugging your phone into your computer. This will fix almost all connectivity problems, but will mean AltStore most likely won't be able to refresh apps for you in the background over WiFi.

#### **AltStore says “Could not find AltServer” when trying to refresh.**

This means AltStore could not discover a running AltServer on the same WiFi network. If you’re getting this error, try the following:

* Make sure AltServer is running and connected to the same WiFi network as AltStore.
* (Windows only) Your Windows firewall might be blocking incoming network connections to AltServer. You must enable network access for AltServer in your firewall settings for it to receive refreshed apps from AltStore.
* (Windows only) Did you install iTunes or iCloud from the Microsoft Store? If so, you’ll need to uninstall them and download the latest versions directly from Apple.
* (Windows only) You may need to make sure iTunes and iCloud are running on your computer as well.
* Are you on public/work/school WiFi? If so, your WiFi might be preventing devices from discovering each other. Try connecting to your phone’s hotspot and trying again.
* Have you said “Trust” on both your computer and phone after connecting it to your computer? You can check by opening iTunes and seeing if a dialog box pops up asking if you want to trust your phone.
* Finally, try plugging your phone into your computer. This will fix almost all connectivity problems, but will mean AltStore most likely won't be able to refresh apps for you in the background over WiFi.

#### **I’m unable to change my network settings to allow devices to communicate with each other (such as on school/work/public WiFi).**

You can always install and refresh apps without WiFi by plugging your phone in to your computer. However, this means AltStore won't be able to refresh apps for you in the background over WiFi.

#### **What is the recommended way to use AltStore?**

* Set AltServer to launch automatically when turning on/logging in to your computer.
* Leave your computer in sleep mode when not using it, and plugged in if possible (especially at night, since iOS will wake up apps in the background much more frequently when the phone is plugged in and not doing anything).
* Open AltStore once a day/every few days so iOS learns to prioritize it and let it refresh apps in the background as much as possible.
* Don’t stress; AltStore is designed to check several times over the course of the week. Leave your laptop in your bag, leave your desktop off, whatever; just make sure it's active every once in a while so AltStore can refresh 🙂

#### **What apps are available in AltStore?**

Right now, Delta is the only app listed in AltStore. However, you can sideload additional apps from the Files app, and support for 3rd party sources is coming soon!

#### **How do I sideload additional apps (.ipa files) with AltStore?**

From the My Apps tab, tap the "+" button in the top left, then select the .ipa file you want to sideload.

#### **Do I need to worry about “revokes”?**

No. Other alternative app stores use “enterprise certificates” to allow people to install apps. However, this is explicitly disallowed by Apple, resulting in them actively shutting down, or “revoking”, these enterprise certificates used by other app stores. This causes apps to stop opening every once in a while until a new enterprise certificate can be obtained.

Because AltStore doesn’t use enterprise certificates, there is no fear of Apple shutting down AltStore by revoking a single certificate (since each person technically now has their own signing certificate).

#### **Why do you need my Apple ID?**

Apple allows anyone with an Apple ID to install apps they’ve built themselves onto their devices for testing. AltStore uses your Apple ID to communicate with Apple's servers on your behalf and perform the necessary steps to prepare your account for installing apps onto your device.

#### **Do you save or send my Apple ID to anyone besides Apple?**

Your Apple ID is **never** sent to anyone but Apple. AltStore does save your Apple ID so it can refresh apps for you automatically, but it is stored securely in the device’s keychain. AltServer does not save your Apple ID, and requires you to enter your credentials each time.

#### **Why does it say my apps will expire in 7 days?**

Unfortunately, apps that have been installed using non-developer Apple IDs (in other words, Apple IDs not tied to a $99/year Apple developer account) are only valid for 7 days, at which point they will no longer open. To compensate for this, AltStore will periodically attempt to refresh your apps in the background, and you can always manually refresh your apps from within AltStore.

#### **How long before apps installed with a developer Apple ID expire?**

Apps installed with a developer Apple ID expire after a year.

#### **Does AltServer need to be running to install/refresh apps?**

Yes, AltServer must be running and on the same WiFi network as AltStore when installing or refreshing apps.

#### **Does this mean I need to keep AltServer running 24/7?**

No. AltStore periodically checks in the background to see if it’s on the same WiFi network as AltServer, and if so refreshes your apps. This means as long as this check succeeds at least once during the 7 day period, your apps will never expire.

For best results, we recommend setting AltServer to automatically run in the background when turning on your computer, and then just leave your computer in sleep mode every once in a while (Windows users might need to allow network connectivity when the computer is sleeping).

#### **Will letting AltServer run in the background drain my battery or affect my computer’s performance?**

No. When running in the background, AltServer does nothing but wait for incoming connections from AltStore.

#### **How can I increase the frequency AltStore refreshes apps in the background?**

iOS determines how frequently to wake AltStore in the background based on how often you open the app. For this reason, we strongly recommend opening AltStore at least once every few days. Otherwise, iOS might decide you no longer are using the app and stop waking it in the background.

#### **How can I see if AltStore is refreshing apps for me in the background?**

On the Settings tab, swipe up with 3 fingers 3 times to make a "Debug" section appear. You can then press "View Refresh Attempts" to see a log of all the times AltStore attempted to refresh in the background.

## Patreon

#### **How do I download beta versions of Delta and AltStore?**

1. Open the Settings tab in AltStore.
2. Press “Link Patreon account”.
3. Sign in with your Patreon account. After signing in, the message on the Patreon screen will now begin with “Hey \[your name]”. If a different Patreon account than the one you want to use is already logged in via Safari, you may need to sign out in Safari first.
4. Open the Browse tab. Now, the beta versions of AltStore and Delta will be listed alongside their non-beta versions, designated with a “Beta” badge.
5. Download the beta of your choice.

**IMPORTANT:** If you download the AltStore beta, make sure to delete the regular AltStore afterwards. Having two AltStores installed might cause conflicts with each other. Having both Delta and Delta beta installed will not cause any issues, however.

#### **How do I play DS games?**

You need to download the Delta beta play DS games. See “How do I download beta versions of Delta and AltStore?” for how to download the Delta beta.

#### **How do I add 3rd party sources to AltStore?**

You need to download the AltStore beta to add 3rd party sources. See “How do I download beta versions of Delta and AltStore?” for how to download the AltStore beta, then you can add sources from the Browse tab.

#### **How do I access the AltStore Discord? ($5+ tiers only)**

Follow [this very helpful guide from Patreon.](https://support.patreon.com/hc/en-us/articles/212052266-How-do-I-receive-my-Discord-role-)

#### **Where does my name show up in AltStore? ($10 tier only)**

Your name will appear on the Patreon screen in the AltStore settings (same screen where you connect your Patreon account) under the “Special thanks to...” section. And seriously, thank you so much 😊🙏

#### **What happens when if I stop being a patron?**

You’ll still have normal access to everything until the end of the month. At that point, you’ll lose access to beta apps, the AltStore Discord ($5+ patrons), and your name will no longer be listed in AltStore ($10 patrons).

#### **What exactly does it mean when I lose access to beta apps?**

AltStore will no longer list the beta apps in the Browse tab and will also remove them from the My Apps app. This means they can no longer be refreshed by AltStore, and will no longer open once they expire. However, as long as you don’t delete the apps, you can still refresh them in the future and keep all your data if you choose to become a patron again.

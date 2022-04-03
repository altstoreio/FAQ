# 🏎 AltJIT

AltJIT allows apps sideloaded with AltStore to enable just-in-time compilation, more commonly known as JIT. JIT allows some apps to run significantly faster — or even at all — but iOS does not normally allow apps to use JIT for security reasons. AltJIT is an AltStore-specific workaround that allows you to enable JIT for any sideloaded app whenever you're on the same WiFi as AltServer.

To use AltJIT, open the "My Apps" tab then long-press the app you want to use JIT. Press "Enable JIT" to launch the app, and within a few seconds you should see an AltStore notification saying JIT has been enabled. The app can now use any JIT-related features without crashing.

{% hint style="info" %}
Once enabled, an app can continue using JIT until it is force-quit from the app switcher or purged from memory while suspended in the background.
{% endhint %}

If you're experiencing issues getting AltJIT to work, make sure to check our troubleshooting guide for [macOS](../../getting-started-mac/troubleshooting-macos.md) or [Windows](../../getting-started-windows/troubleshooting-windows.md).

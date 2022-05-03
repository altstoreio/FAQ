# 🏎 AltJIT

AltJIT allows apps sideloaded with AltStore to enable just-in-time compilation, more commonly known as JIT. JIT allows some apps to run significantly faster — or even at all — but iOS does not normally allow apps to use JIT for security reasons. AltJIT is an AltStore-specific workaround that allows you to enable JIT for any sideloaded app whenever you're on the same WiFi as AltServer.

To use AltJIT, go to "Enable JIT" > \[Your Device] from the AltServer menu, then choose a sideloaded app. Within a few seconds you should see an AltServer alert saying JIT has been enabled. The app can now use any JIT-related features without crashing.

{% hint style="info" %}
Once enabled, an app can continue using JIT until it is force-quit from the app switcher or purged from memory while suspended in the background.
{% endhint %}

If you're experiencing issues getting AltJIT to work, be sure to check out our [troubleshooting guide](../getting-started/troubleshooting-guide.md).

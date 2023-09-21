# 🏎 AltJIT

AltJIT allows apps sideloaded with AltStore to enable just-in-time compilation, more commonly known as JIT. JIT allows some apps to run significantly faster — or even at all — but iOS does not normally allow apps to use JIT for security reasons. AltJIT is an AltStore-specific workaround that allows you to enable JIT for any sideloaded app whenever you're on the same WiFi as AltServer.

### Enable JIT

{% hint style="info" %}
There are additional requirements for users on iOS 17. Please see the instructions below.
{% endhint %}

#### **AltStore**

1. Open the "My Apps" tab then long-press the app you want to use JIT.&#x20;
2. Press "Enable JIT" to launch the app, and within a few seconds you should see an AltStore notification saying JIT has been enabled.&#x20;

#### **AltServer**

1. First, make sure that the app you want to use JIT with is running in the foreground of your device.&#x20;
2. Go to “Enable JIT” > \[Your Device], then choose an app you want to use with JIT.&#x20;

{% hint style="info" %}
Once enabled, an app can continue using JIT until it is force-quit from the app switcher or purged from memory while suspended in the background.
{% endhint %}

If you're experiencing issues getting AltJIT to work, be sure to check out our [troubleshooting guide](../getting-started/troubleshooting-guide.md).



### iOS 17 Instructions (macOS only)

{% hint style="warning" %}
Using AltJIT on iOS 17 is not yet supported for Windows users.
{% endhint %}

Currently, there are extra steps needed to enable JIT on iOS 17+:

1. Open Terminal on your Mac
2. Install Xcode Command Line Tools with the following command:

```
xcode-select --install
```

{% hint style="warning" %}
If you are running macOS Sonoma and see an error that Command Line Tools aren’t currently available, try the following commands instead:
{% endhint %}

```
sudo mkdir -p /Library/Developer/CommandLineTools   
sudo touch /Library/Developer/CommandLineTools/.beta  
```

3. Install [Homebrew](https://brew.sh/) with the following command:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

4. Install [pymobiledevice3](https://github.com/doronz88/pymobiledevice3) with the following commands:

```
brew install openssl@3 
python3 -m pip install -U pymobiledevice3
```

5. Connect your device to your Mac via lightning/USB-C. **Enabling JIT via WiFi is not yet supported**
6. Open AltStore (or any app that requires JIT)
7. AltServer run Enable JIT

Once everything is installed, you can now enable JIT as usual from AltServer, though you may be asked to enter your password.

{% hint style="info" %}
Enabling JIT on iOS 17 may take up to a minute. To speed up this process, we recommend installing [Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12).
{% endhint %}



### Troubleshooting



#### "pymobiledevice3 not installed"

Make sure you have followed the above instructions and installed pymobiledevice3. If you're still seeing this error after you've installed it, you can try downloading Xcode and using this command to reinstall pymobiledevice3:

```
/Applications/Xcode.app/Contents/Developer/usr/bin/python3 -m pip install -U pymobiledevice3
```



#### "The process 'altjit' failed with code 1. Could not attach debugger to \[app]. \[app] is not running"

This means that you tried to enable JIT without the requested app running in the foreground. Make sure to launch the app and have it running before you enable JIT.



To use AltJIT, you first need the app to be open on your device. You can do this by simply launching the app you want to use and waiting for it to connect automatically. If the app does not connect automatically for any reason, you can either enable it from AltStore by long-pressing the app in the My Apps tab or by launching the app first, then selecting the option to Enable JIT on AltServer.



#### "The process 'altjit' failed with code 1. Could not connect to device \[DeviceID]."

Please make sure to have your device connected to your Mac/PC via USB-C/Lightining until AltJIT has successfully been enabled. Once it's been enabled, you can disconnect and use the app normally as long as it's kept running.

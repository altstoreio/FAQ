# 🤖 AltSource CLI

## Overview

[AltServer for macOS](https://cdn.altstore.io/file/altstore/altserver.zip) comes with a built-in `altsource` tool for easily creating and updating AltStore sources using your apps' .ipa files. You can run this tool from Terminal to automatically populate your source with information from a provided .ipa.

Currently, this tool can do the following tasks:

* Create a new source
* Add an app to an existing source
* Update an app to a new version



## Instructions

This tool is located in AltServer's app bundle: `AltServer.app/Contents/MacOS/altsource`.  In Terminal, you will need to run this tool from wherever AltServer is located (usually your Applications folder) to enter commands, e.g:

<pre><code><strong>/Applications/AltServer.app/Contents/MacOS/altsource new
</strong></code></pre>

There are two main commands, `new` and `update`. You can run either of these commands with any of the [additional arguments](altsource-cli.md#additional-arguments) below to overwrite default values.

```
USAGE: altsource <subcommand>

OPTIONS:
  -h, --help              Show help information.

SUBCOMMANDS:
  new                     Create a new AltStore source, optionally based on a
                          provided .ipa file.
  update                  Update source with new app or version.
```

#### `new`

Generates a new source JSON file either from scratch or based on an existing .ipa file using the `--ipa` argument. Use the `-o` argument to change where the file is saved.

```
USAGE: altsource new [<options>]

OPTIONS:
  -o <o>                  The output destination.
  --ipa <ipa>             An .ipa to add to the source during creation.

```

#### `update`

Adds a new app or app version to an existing source. You can also use this command to edit your source information using the additional arguments below.

```
OVERVIEW: Update an existing AltStore source.

USAGE: altsource update [<options>] <source-url>

ARGUMENTS:
  <source-url>            The source JSON to update.
  
OPTIONS:
  -o <o>                  The output destination.
  --ipa <ipa>             An .ipa to add to the source during creation.
```

###

## Additional Arguments

When creating or updating a source, you can provide these arguments to populate optional values or override default values with your own. For more info on any of these arguments, including examples, see the [Make A Source](make-a-source.md) page.

| Command                | Use                                                                                                                     |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------- |
|   --name               | The name of the source.                                                                                                 |
|   --subtitle           | A short tagline for your source.                                                                                        |
| --description          | A marketing description of your source.                                                                                 |
| --website              | A website with more information about your source.                                                                      |
| --icon                 | A URL pointing to your source's icon.                                                                                   |
| --header               | A URL pointing to your source's header image.                                                                           |
| --tint-color           | A hexadecimal string representing your source's preferred tint color.                                                   |
| --app-name             | The name of the app.                                                                                                    |
| --app-developer        | The name of the app's developer.                                                                                        |
| --app-description      | A marketing description about your app.                                                                                 |
| --app-subtitle         | A short tagline for your app.                                                                                           |
| --app-icon             | A URL pointing to your app's icon.                                                                                      |
| --app-tint-color       | A hexadecimal string representing your app's tint color.                                                                |
| --app-category         | The AltStore category that best represents your app. See [here](make-a-source.md#category-string) for supported values. |
| --version-date         | The release date for this app version.                                                                                  |
| --version-description  | A description of what's changed in this app version.                                                                    |
| --version-download-url | The URL where the provided .ipa will be hosted.                                                                         |

###

### Examples

Create an empty source

```
path/to/altsource new 
```

Create an empty source with name

```
path/to/altsource new --name "my source"
```

Create a new source from .ipa

```
path/to/altsource new --ipa myapp.ipa
```

Create a new source from .ipa with optional app subtitle

```
path/to/altsource new --ipa myapp.ipa --app-subtitle "My Cool Source" 
```

Add app to existing source

<pre><code><strong>path/to/altsource update mysource.json --ipa myapp.ipa
</strong></code></pre>

Add app to existing source with app category and description

{% code overflow="wrap" %}
```
path/to/altsource update --ipa myapp.ipa --category "utilities" --app-description "My New App" 
```
{% endcode %}

Update an existing app to a new version with version description

<pre><code><strong>path/to/altsource update mysource.json --ipa myapp.ipa --version-description "bug fixes"
</strong></code></pre>

{% hint style="info" %}
If the .ipa provided does not exist yet in your source, this command will create a new [app entry](make-a-source.md#apps) in your Source
{% endhint %}

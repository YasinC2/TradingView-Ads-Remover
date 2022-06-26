# TradingView Hide Ads
Chrome/Chromium extension to hide ads from TradingView.

## Installation

1. Download the `crx` file from the latest release (https://github.com/YasinC2/TradingView-Hide-Ads/releases) 
2. Open `chrome://extensions/`
3. Drop the `crx` file into the page
4. Enjoy TradingView without ads :)

## Browser Warning

If after installing the extension file, the browser displays an error with 
`This extension is not listed in the Chrome Web Store and may have been added without your knowledge.`
or
`This extension is not from any known source, and may have been added without your knowledge.`
 content, there are two method you can fix the problem:
 
 #### Method 1: Install as Unpacked Extension
 Extract .crx file to a folder, and then install the extension by using **Load unpacked** option.
 
 #### Method 2: Whitelist the Extension through Policies
 Use [this tutorial](https://techjourney.net/chrome-edge-disables-crx-installed-extensions-workarounds-to-turn-on/)
 or
 Open `chrome://system/` and find extension id in extensions section, then create a .reg file and copy the text below and paste it to the created file and replace `ExtensionID` with id you find from previous step. save the file and run it.
 ```
 Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist]
"999"="ExtensionID"
 ```
 This registry introduces extension to the browser as a trusted extension.

#iOS-splash-maker v0.1 alpha

A Photoshop script to automatically generate properly sized splash screens for iOS devices from a single PSD image.

##Device support:
- iPhone/iPod 1-5

##Usage

1. Open the PSD for your splash screen. The PSD should be as large as the largest splash screen you want to generate (usually iPhone5 @ 640px×1136px)
2. Go to File > Scripts > Browse and select `splash.js`.
3. The script will generate your splash screens as web optimized PNG's, and save them to the same folder as your PSD.

##Configuring which platforms to generate splash screens for

1. Open `splash.js` in your favorite text editor (Notepad, TextEdit, Sublime Text) or Adobe's ExtendScript Toolkit (which comes bundled with Photoshop Extended)
2. At the very beginning of the file you'll see the following:

```javascript
var use = {
	'iPhone': 'yes',
	'iPhone:retina': 'yes',
	'iPad': 'no',
	'iPad:retina': 'no'
};
```

3. To toggle support for a platform, just change the corresponding `yes` to a `no`, or vice-versa.

##To do:

- Proper support for iPad
- Support for Android
- Support for Windows Mobile
- Support for Blackberry
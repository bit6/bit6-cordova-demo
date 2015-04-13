Bit6 Cordova Demo App
---------------------
[![GitHub version](https://badge.fury.io/gh/bit6%2Fbit6-cordova.svg)](https://github.com/bit6/bit6-cordova-demo)

This project demonstrates the full functionality of [Bit6 Cordova Plugin](https://github.com/bit6/bit6-cordova).

### Usage
* Get the API Key at [Bit6 Dashboard](https://dashboard.bit6.com).
* Clone this repo.
* Edit `config.xml` to set your app id - replace `com.bit6.samples.DemoApp` with your app id
  (note: iOS APN requires unique bundle id).
* Set your Bit6 API Key in `www/js/index.js`
  ```js
  {'apikey': 'yourApiKey'}
  ```

* Add Bit6 plugin
  ```bash
  cordova plugin add https://github.com/bit6/bit6-cordova
  # Or if you have the plugin installed locally
  # cordova plugin add<path/to/bit6plugin>
  ```
* Add the platforms you want to support (ios/android/browser)
  ```
  cordova platform add ios
  cordova platform add android
  cordova platform add browser
  ```

* Optional plugin:

  To avoid cordova webview and iOS status bar overlapping you can add [statusbar plugin](https://github.com/apache/cordova-plugin-statusbar).
  ```
  cordova plugin add https://github.com/apache/cordova-plugin-statusbar
  ```

* Run the demo app
  ```
  # Run on iOS device
  cordova run ios --device
  # Run on Android device
  cordova run android --device
  # Run in a browser
  cordova run browser
  ```

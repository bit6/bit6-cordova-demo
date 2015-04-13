Bit6 Cordova Demo App
---------------------
[![GitHub version](https://badge.fury.io/gh/bit6%2Fbit6-cordova.svg)](https://github.com/bit6/bit6-cordova-demo)

This project demonstrates the full functionality of [Bit6 Cordova Plugin](https://github.com/bit6/bit6-cordova).

### Prerequisites
* Get the API Key at [Bit6 Dashboard](https://dashboard.bit6.com).

### Installation
Clone this repo.
``` sh
$ git clone git://github.com/bit6/bit6-cordova-demo.git
```

### Configuration
1. Edit [config.xml](config.xml#L3) to set your app id (iOS APNs requires unique bundle id).

2. Specify your Bit6 API Key in [www/js/index.js](www/js/index.js#L19)
  ```js
  {'apikey': 'yourApiKey'}
  ```

3. Add Bit6 Plugin
  ```sh
  $ cordova plugin add https://github.com/bit6/bit6-cordova
  ```
4. Add the platforms you want to support
  ```sh
  $ cordova platform add ios
  $ cordova platform add android
  $ cordova platform add browser
  ```

5. [Configure](https://github.com/bit6/bit6-cordova#push-notifications) push notification support.

6. Fix WebView overlap on iOS (optional)
  ```sh
  # Add StatusBar plugin
  $ cordova plugin add https://github.com/apache/cordova-plugin-statusbar
  ```

### Running the app
```sh
# Run on iOS device
$ cordova run ios --device
# Run on Android device
$ cordova run android --device
# Run in a browser
$ cordova run browser
```

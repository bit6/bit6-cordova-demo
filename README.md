Bit6 Cordova Plugin
-------------------
[![GitHub version](https://badge.fury.io/gh/bit6%2Fbit6-cordova.svg)](https://github.com/bit6/bit6-cordova-demo)

This cordova demo project demonstrates the full functionality of [Bit6 plugin](https://github.com/bit6/bit6-cordova).

### Usage
* Open config.xml and set your package id - replace id="com.bit6.samples.DemoApp" with your id
  (note: APN certificate requires unique bundle id).
* Get Bit6 API Key by going to [Dashboard](https://dashboard.bit6.com) (if not done yet).
* Clone this repo.
* Set you API key in www/js/index.js
   ```
   {'apikey': 'yourApiKey'}
   ```

* Add plugin
  ```
    cd demo
    cordova plugin add https://github.com/bit6/bit6-cordova
      or if you have the plugin locally
    cordova plugin add  <path/to/bit6plugin>
  ```
* Add needed platforms (ios/android/browser)
```
   cordova platform add <ios | andoroid | browser>
```

* Run the demo app
```
  cordova run ios --device
```
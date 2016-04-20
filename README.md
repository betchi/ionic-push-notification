# ionic Push Notification


## Screenshot

### iOS

| Registration | Receive notificaiton | Show badge |
|:------------:|:------------:|:------------:|
|![Screenshot iOS 01](https://raw.githubusercontent.com/wiki/betchi/ionic-push-notification/images/screenshot_ios_01.png)|![Screenshot iOS 02](https://raw.githubusercontent.com/wiki/betchi/ionic-push-notification/images/screenshot_ios_02.png)|![Screenshot iOS 03](https://raw.githubusercontent.com/wiki/betchi/ionic-push-notification/images/screenshot_ios_03.png)|

## Operation Environment

```
$ ionic info

Your system information:

Cordova CLI: 6.1.1
Gulp version:  CLI version 3.9.1
Gulp local:   Local version 3.9.1
Ionic Version: 1.2.4
Ionic CLI Version: 1.7.14
Ionic App Lib Version: 0.7.0
ios-deploy version: 1.8.6 
ios-sim version: 5.0.8 
OS: Mac OS X El Capitan
Node Version: v0.12.13
Xcode version: Xcode 7.3 Build version 7D175 

$ cordova platform list
Installed platforms:
  ios 4.1.1
```

## Run

You will need to set up an APP_ID.

*config.xml*

```xml:config.xml
<widget id="[APP ID]" version="0.0.1" xmlns="http://www.w3.org/ns/widgets" xmlns:cdv="http://cordova.apache.org/ns/1.0">
```

Install phonegap-plugin-push

```
cordova plugin add phonegap-plugin-push --variable SENDER_ID=dummy
```

### To run in iOS device

phonegap-plugin-push require cordova-ios@4.0.0 over

```
ionic platform update ios
ionic platform add ios
open platforms/ios/ionic-push-notification.xcodeproj
```

Push notification provider 

[ApnsPHP](https://github.com/immobiliare/ApnsPHP)


Registration

![Xcode 01](https://raw.githubusercontent.com/wiki/betchi/ionic-push-notification/images/xcode_log_01.png)

Receive notification

![Xcode 02](https://raw.githubusercontent.com/wiki/betchi/ionic-push-notification/images/xcode_log_02.png)

## Link

**phonegap-plugin-push**

https://github.com/phonegap/phonegap-plugin-push

**ApnsPHP**

https://github.com/immobiliare/ApnsPHP
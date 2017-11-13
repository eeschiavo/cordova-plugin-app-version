# Cordova AppVersion plugin

Reads the version of your app from the target build settings.

## Installation

### With cordova-cli

If you are using [cordova-cli](https://github.com/apache/cordova-cli), install
with:

    cordova plugin add eeschiavo-cordova.plugin-appversion

## Use from Javascript

If you are using jQuery or AngularJS, promise style is supported. Use something like:

    cordova.getAppVersion.getVersionNumber().then(function (version) {
        $('.version').text(version);
    });

If not, pass a callback function:

    cordova.getAppVersion.getVersionNumber(function (version) {
        alert(version);
    });

In addition to the version number you can also retrieve other details about your application:

### getAppName

Returns the name of the app. E.g. "My Awesome App"

### getPackageName

Returns the package name of the app - the reversed domain name app identifier like com.example.myawesomeapp

### getVersionCode

Returns the build identifier of the app

### getVersionNumber

Returns the version number of the app

### Credits

This is a fork modified under MIT license.

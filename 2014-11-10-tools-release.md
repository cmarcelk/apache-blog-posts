---
layout: post
author:
    name: Mark Koudritsky
    url: https://github.com/kamrik
title:  "Tools Release: November 10, 2014"
categories: news
tags: release tools
---
New versions of cordova tools are now live!

* [cordova-lib@4.1.0](https://www.npmjs.org/package/cordova-lib)
* [cordova@4.1.0](https://www.npmjs.org/package/cordova)
* [plugman@0.22.14](https://www.npmjs.org/package/plugman)
* [cordova-js@3.7.2](https://www.npmjs.org/package/cordova-js)

To update your tools:

    npm install -g cordova
    npm install -g plugman

Changes include:
<!--more-->

## Platform updates
When adding these platforms to your project, the following versions are now used by default. These platform versions were released recently, and the tools' defaults were updated.
* [Cordova iOS 3.7.0](http://cordova.apache.org/announcements/2014/11/06/cordova-ios-3.7.0.html)
* [Cordova Windows & WP8 3.7.0](http://cordova.apache.org/announcements/2014/11/06/cordova-wp-windows-3.7.0.html)

## cordova-lib
* [CB-7988](https://issues.apache.org/jira/browse/CB-7988) Update platform versions for **iOS**, **WP8** & **Windows** to 3.7.0
* [CB-7846](https://issues.apache.org/jira/browse/CB-7846) Fix plugin deletion when dependency plugin does not exist
* [CB-6992](https://issues.apache.org/jira/browse/CB-6992) Fix build issue on iOS when app name contains accented characters
* [CB-7884](https://issues.apache.org/jira/browse/CB-7884) moved platform metadata to platformsConfig.json
* Amazon Specific changes: Added support for SdkVersion
* Expose PluginInfo from cordova-lib
* [CB-7839](https://issues.apache.org/jira/browse/CB-7839) android: Fix versionCode logic when version is less than 3 digits
* [CB-7033](https://issues.apache.org/jira/browse/CB-7033) Improve cordova platform check
* [CB-7311](https://issues.apache.org/jira/browse/CB-7311) Fix xcode project manipulation on Windows host
* [CB-7820](https://issues.apache.org/jira/browse/CB-7820) Make cordova platfrom restore not stop if a platforms fails to restore
* Enable platform-specific id for android and ios
* Check for a CORDOVA_HOME environment variable to create a global config path

## cordova
* Expose cordova-lib and the cli from cordova-cli
* [CB-7636](https://issues.apache.org/jira/browse/CB-7636) Allow using --nobuild flag without screaning

## cordova-js
* [CB-7868](https://issues.apache.org/jira/browse/CB-7868) Make <clobbers> on navigator not break on some versions of Android
* [CB-7868](https://issues.apache.org/jira/browse/CB-7868) Use utils.defineGetterSetter instead of Object.defineProperty
* Upleveled amazon-fireos bridge.
* [CB-7735](https://issues.apache.org/jira/browse/CB-7735) Fix **iOS** bridge race condition when using innerHTML on <body>
* [CB-2520](https://issues.apache.org/jira/browse/CB-2520) - User agent-related changes for custom user agents in **iOS**


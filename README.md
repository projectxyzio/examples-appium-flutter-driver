# appium_flutter_webinar

This repository is sample code in https://www.headspin.io/events/appium-for-flutter-app/

## Setup

```
$ flutter pub get
```

## Run appium test

1. Get Appium server (It requires NodeJS environment)
    ```
    # A Flutter driver versions in appium 1.21.0 has a few issues. Please try out the latest beta.
    # Or newer than Appium 1.22.0 (It is in beta on Jun 30, 2021)
    $ npm install -g appium@beta

    # start your local appium server
    $ appium
    ```
2. Runs this test code against the appium server
    ```
    # Please update capabilities in appium-test/main_test.dart for your environment
    $ dart appium-test/main_test.dart
    ```

## About Appium client

This repository uses Appium client in Dart so that you can try out this repository only Flutter and Appium environment.
https://pub.dev/packages/appium_driver.

## Other appium client libraries to support `finder` in appium-flutter-appium

- https://github.com/truongsinh/appium-flutter-driver/tree/master/example


## When you want to modify the sample code and build them

```
# debug build
$ flutter apk --debug

# release build
$ flutter apk --release
```

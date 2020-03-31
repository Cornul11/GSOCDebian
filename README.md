# GSOCDebian
This is the task I've fulfilled for the "Android SDK Tools in Debian" project for GSoC'20.

I've created a basic app containing an empty activity. It does not contain any functional since that is not relevant. The goal of this task was to try to build an Android app using only the following Debian packages: `android-sdk android-sdk-platform-23 android-sdk-helper`. 

I had some troubles with the `ANDROID_HOME` and `JAVA_HOME` environment variables that needed to be changed to the right directories. Moreover, I had to change the `build.gradle` file to contain Google's Maven repository so as to find all the necessary dependencies. After this i just had to use `./gradlew installDebug` in order to install the app on my connected device.
<br/>
<br/>
<br/>
Moreover, I played a bit with `adb` from the `platform-tools` package and couldn't find any bug in the completion part.


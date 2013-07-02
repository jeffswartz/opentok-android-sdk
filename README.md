OpenTok Android SDK
===================

This package contains what you need to get you started using the OpenTok Android SDK.

This is a beta version of the OpenTok Android SDK. The Samsung Galaxy S3 is the only supported device for use with this SDK.

The OpenTok Android SDK lets you use OpenTok video sessions in apps you build for Android devices.
This means you can use OpenTok video sessions that connect Android users with each other and with web clients and apps built using
the OpenTok iOS SDK.

For information on OpenTok, see [http://www.tokbox.com/opentok](http://www.tokbox.com/opentok).

Apps written with the OpenTok Android SDK can interact with OpenTok apps written with the following OpenTok SDKs:

* The OpenTok JavaScript library v1.1
* The OpenTok iOS SDK
* The OpenTok ActionScript library v1.1

In the browser, these sessions use Adobe Flash. This version of the OpenTok Android SDK does *not* interact with apps that use
WebRTC video (such as browser-based apps that use version 2.0 of the OpenTok JavaScript library).

Support is available at the [OpenTok forums](http://www.tokbox.com/forums/android).

Release Notes
-------------

#### v1.0 beta -- July 3, 2013

This is a beta version of the OpenTok Android SDK. The Samsung Galaxy S3 is the only supported device for use with this SDK.
This version of the SDK replaces the previous version of the OpenTok Android SDK, which is no longer supported.
  
Known issues
------------

* Some features available in the OpenTok SDK for other platforms (such as JavaScript) are not supported in the OpenTok Android SDK. These unsupported features include peer-to-peer streaming and archiving.

* The OpenTok Android SDK requires Android 4.1 (Jelly Bean). The Samsung Galaxy S3 is the only supported device for use with this SDK.

* You cannot publish streams in the ADT Simulator. Build and deploy to a supported device.

Developer and client requirements
---------------------------------

* You need to test OpenTok apps on a supported device. Currently, the only supported device is the Samsung Galaxy S3.
* You need an [OpenTok developer account](https://dashboard.tokbox.com/). 

Using the sample apps
---------------------

Download the [OpenTok Android SDK demo app](https://github.com/opentok/opentok-android-sdk-demo). This app shows the most basic
functionality of the OpenTok Android SDK: connecting to sessions, publishing streams, and subscribing to streams. It also shows
how to add user interface controls for muting audio and selecting the camera used.

Creating your own app using the OpenTok Android SDK
---------------------------------------------------

Add the opentok-android-sdk.jar file to your project's build path.

Also, you need to add the following permissions and features to your app manifest:

* android.permission.CAMERA
* android.permission.INTERNET
* android.permission.WAKE_LOCK
* android.permission.RECORD_AUDIO
* android.hardware.camera
* android.hardware.camera.autofocus

Your app needs to use a session ID and token generated with your OpenTok API key, which you can get at
[the OpenTok developer dashboard](https://dashboard.tokbox.com).

For test purposes, you can generate a session ID and token at [the projects page](https://dashboard.tokbox.com/projects)
of the OpenTok developer dashboard. For a production app, generate unique tokens (and session IDs, if you need to support
multiple sessions) using the [OpenTok server-side libraries](http://www.tokbox.com/opentok/docs/server/server_side_libraries.html).

Connect with TokBox and with other OpenTok developers
-----------------------------------------------------

Your comments and questions are welcome. Come join the conversation at the
[OpenTok Android SDK forum](http://www.tokbox.com/forums/android).

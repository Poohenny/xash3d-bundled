# Xash3D FWGS Engine, but you can bundle games in the APK! <img align="right" width="128" height="128" src="https://github.com/FWGS/xash3d-fwgs/raw/master/game_launch/icon-xash-material.png" alt="Xash3D FWGS icon" />

## Fork features
* Games can be built in to the APK.
* This allows for an easy, one-click install!
* Consequentially, the game's directory is inaccessible without root.
* To work around this, saves are initially kept in /data, and on every start, are copied to /sdcard/xash/saves.
* If no saves are available in /data, the app copies the external save location, back to /sdcard.

## Building
* Install [Android Studio](https://developer.android.com/studio) (or the command line tools).
* Install [Python](https://python.org) (at least 2.7, latest is better).
* Install [Git](https://git-scm.com/download/win).
* Install [Ninja](https://ninja-build.org/).
* Install [CMake](https://cmake.org/) (for some dependencies).
* Clone this repostory: `$ git clone --recursive https://github.com/FWGS/xash3d-fwgs`.

To build you should clone [SDL](https://github.com/libsdl-org/SDL) from `SDL2` branch and [HLSDK-portable](https://github.com/FWGS/hlsdk-portable) `mobile-hacks` branch repositories to 3rdparty folder, after that you should be able to open the project in Android Studio from `android` directory or manually call Gradle to build the APK.

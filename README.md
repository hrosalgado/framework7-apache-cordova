# framework7-apache-cordova
Create hybrid mobile applications with Apache Cordova & Framework7

# Requirements
## General
- npm (https://nodejs.org/)

## Android app
- Gradle (https://gradle.org/)
- Android Studio (https://developer.android.com/studio)

* You can install it from source, using a package manager like ChocolateY on Windows or whatever package manager on Linux

Once Android Studio is installed, you need to setup some configurations:
- Tools -> AVD Manager
	It's necessary to create a virtual android device. On Android Studio, click on Tools and then click con AVD Manager. This shows a list of virtual devices manager.
	Click on + Create Virtual Device and choose one, download a system image (your preferred, last Android version) and finish the steps.
- Tools -> SDK Manager
	If you haven't downloaded any sdk, choose one and download it

## iOS app
- Xcode

# Apache Cordova + Framework7
https://framework7.io/cli/

## Step by step
1. Install Apache Cordova
	$ npm install -g cordova

2. Install framework7
	$ npm install -g framework7-cli

3. Create a project
	* Follow step by step choosing the options that your project app requires
	$ framework7 create --ui

4. Compile a project
	At root project, choose one of this options to compile your project:
	* Web application on development mode
	$ npm run build-dev
	* Web application on release mode
	$ npm run build-prod
	* Compile all platforms on development mode
	$ npm run build-dev-cordova
	* Compile all platforms on release mode
	$ npm run build-prod-cordova
	* Compile ios application on development mode
	$ npm run build-dev-cordova-ios
	* Compile ios application on release mode
	$ npm run build-prod-cordova-ios
	* Compile android application on development mode
	$ npm run build-dev-cordova-android
	* Compile android application on release mode
	$ npm run build-prod-cordova-android

5. Run
	At root project, choose one:
	* This actions launch the application on your web browser
	$ npm run start
	$ npm run dev

### Apache Cordova functions on Framework7
To use Apache Cordova functions on Framework7, you can do it like that:
$ framework7 cordova ...
Example: framework7 cordova plugin add cordova-plugin-statusbar
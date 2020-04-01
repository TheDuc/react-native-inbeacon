
# react-native-inbeacon
This module is developed because I needed to make use of the Native Inbeacon SDKs in react-native. There were no bridge libraries yet so I thought why not write it myself and publish it for others.

Inbeacon Android SDK: https://github.com/inbeacon/InbeaconSdk-android \
Inbeacon iOS SDK: https://github.com/inbeacon/InbeaconSdk-ios

## Installation
`$ npm install react-native-inbeacon --save`

For react-native versions 0.60 and higher the installation will take place through autolinking.

For react-native versions lower than 0.60, please take a look at the manual installation.

### Manual installation

#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-inbeacon` and add `RNInbeacon.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNInbeacon.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNInbeaconPackage;` to the imports at the top of the file
  - Add `new RNInbeaconPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-inbeacon'
  	project(':react-native-inbeacon').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-inbeacon/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-inbeacon')
  	```

## Usage
```javascript
import RNInbeacon from 'react-native-inbeacon';

// API docs are in development
RNInbeacon;
```

# Expo CLI Build Errors: Native Module Integration Issues

This repository demonstrates a common issue encountered when integrating native modules into React Native projects managed by Expo CLI.  The problem arises from improper configuration or missing steps during the linking process for Android or iOS.

## Problem Description

The `bug.js` file contains a simplified example of attempting to use a native module (`MyNativeModule`) without the necessary setup in the Expo project.  Building the project results in errors related to missing headers, undefined symbols, or incorrect linking.  These errors commonly arise when the native module is not correctly configured to work with the Expo build system.

## Solution

The `bugSolution.js` file offers a potential solution.  In this solution, the native module is correctly integrated and configured (in reality, this would entail steps outlined below). 

## Steps to reproduce the bug:

1.  Create an Expo managed workflow project.
2. Install the problematic native module (`npm install --save my-native-module`)
3. Attempt to run the app with the buggy code.

## Steps to solve the bug:

1.  Ensure all native dependencies are installed, particularly those required by the native module.
2.  Follow the specific instructions provided by the native module's documentation for integration into Expo.
3.  For bare workflows, correctly link the native modules with expo prebuild.
4. For managed workflows, consult documentation on integration for native modules with expo.
5. Double-check your Android and iOS build configurations, ensuring that the required native module is correctly integrated into both platforms.
6. Clean and rebuild the project.

## Additional Notes

This example focuses on the core issue.  The exact errors and solutions may vary depending on the specific native module being used and the Expo version you are on.

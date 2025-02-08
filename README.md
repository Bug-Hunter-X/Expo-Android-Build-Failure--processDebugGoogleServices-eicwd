# Expo Android Build Failure: processDebugGoogleServices

This repository demonstrates a common issue encountered when building Android APKs using the Expo CLI. The build process fails with the error message: "Execution failed for task ':app:processDebugGoogleServices". This usually stems from inconsistencies between the Google Services JSON file and the project's configuration.

## Problem Description

The `bug.js` file showcases a scenario where the Google Services JSON file is incorrectly configured or missing, leading to the build failure.

## Solution

The `bugSolution.js` file provides a solution to resolve the issue. This involves verifying the correctness of the `google-services.json` file and ensuring its proper integration into the project.  Specific steps might include:

1. **Verify Google Services JSON:** Double-check the contents of your `google-services.json` file for any errors or missing information. Ensure the package name matches your app's package name.
2. **Correct Placement:** Make sure that `google-services.json` is placed in the correct directory (usually `android/app`).
3. **Clean and Rebuild:**  Try cleaning your project and rebuilding it to resolve any cached build issues.
4. **Check Expo SDK Version:** Ensure that your Expo SDK version is compatible with the latest Google Play services.
5. **Check for updates:**  Update to the newest Expo CLI version to ensure no conflicts with the build process.

This example should help understand how to address this prevalent build error.
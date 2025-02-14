# React Native Dimensions.get('window') Inconsistency on Android

This repository demonstrates a common issue encountered when using `Dimensions.get('window')` in React Native to obtain screen dimensions, particularly on Android devices. The problem lies in the potential for inconsistent or inaccurate dimension values, primarily during the initial render or following screen rotation.

## Problem

The `Dimensions` API's `get('window')` method sometimes returns incorrect width and height values, leading to layout problems where components are rendered with improper sizing or positioning.

## Solution

The provided solution uses the `onLayout` prop to reliably capture accurate dimensions *after* the component has been fully rendered and laid out.  This ensures consistent and correct measurements, resolving the layout inconsistencies.

## Usage

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` (or iOS equivalent) to start the app.
# Expo Camera: onBarCodeScanned Not Firing

This repository demonstrates a common issue when using the Expo Camera API's `onBarCodeScanned` prop.  The prop might not function correctly if accessed before the camera component has fully initialized. 

The `bug.js` file showcases the problem, and `bugSolution.js` provides a solution using asynchronous operations and the camera's `isCameraReady` state to ensure functionality.

## How to Reproduce

1. Clone the repo.
2. Navigate to the directory.
3. Run `npm install`.
4. Run `expo start`.
5. Observe the console logs in `bug.js` and compare it to the functionality in `bugSolution.js`

## Solution

The solution involves ensuring that the camera has finished initializing and is ready before attempting to use features like `onBarCodeScanned`.
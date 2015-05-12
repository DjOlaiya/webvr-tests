# webvr-tests
A set of simple tests for testing WebVR functionality. See https://developer.mozilla.org/en-US/docs/Web/API/WebVR_API for the latest on the documentation. The tests included here are:

* [VRDevice test](http://mdn.github.io/webvr-tests/vrdevice/): Uses [navigator.getVRDevices()](https://developer.mozilla.org/en-US/docs/Web/API/Navigator/getVRDevices) to retrieve the VR devices attached to the computer, and prints out some information about each one, retrieved from the properties of each one.
* [PositionSensorVRDevice test](http://mdn.github.io/webvr-tests/positionsensorvrdevice/): Here [HTML5 canvas 2D](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D) is used to fake a simple VR scene - a Firefox logo projected onto a white background, drawn twice for the left and right eyes. PositionSensorVRDevice.getState() is used to retrieve a VRPositionState object (stored in the PosState variable) from which position and orientation data is derived and used to update the position of the drawn scene. The scene is updated every frame using [requestAnimationFrame()](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame).
* [Velocity/Acceleration test](http://mdn.github.io/webvr-tests/velocity-acceleration/): The demo is the same as the PositionSensorVRDevice test, except that the information output at the bottom of the display is the linearVelocity, linearAcceleration, angularVelocity and angularAcceleration.
* [Simple 3D position/orientation](http://mdn.github.io/webvr-tests/3Dpositionorientation/): A very simple 3D scene that uses very similar calculations to the PositionSensorVR device demo listed above to work out scene rendering updates in reaction to VR headset movements. This scene however uses [Three.js](http://threejs.org/) for rendering, with the Mozilla VR team's [threejs-vr-boilerplate](https://github.com/MozVR/vr-web-examples/tree/master/threejs-vr-boilerplate) code for adding the VR view effect. 
* [VREyeParameters test](http://mdn.github.io/webvr-tests/vreyeparameters-test/): A version of the simple 3D scene that includes buttons that output the VREyeParameters for each eye.

 



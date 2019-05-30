# SphereSense

This library will allow you to control anything just by moving your hands in front of the screen.
It uses an image recognition engine to track your hands translating their postion to spherical coordinates.

One hand is used as an anchor to determine the relative position in 3D space of the other hand.
Aditionaly is detected if the hands are open or closed rather than just the postion of the hands.

SphereSense is intended to be used like it has been descrived avobe but it will also provide 2D tracking features of the hands relative to the screen top left corner of the imaged captured.

## Output

The API will provide the hand state and 3D coordintes of the hands.

* **RIGHT_HAND_STATE** : boolean
* **LEFT_HAND_STATE** : boolean
* **COORDINATES** : {x : float, y : float, z : float}
* **RIGHT_HAND** : {x : float, y : float}
* **LEFT_HAND** : {x : float, y : float}

## Input

* The refresh rate of the system can be adjust.
* NN that tracks the hands will be open for others to train it with its own data.

## Requirements

* SphereSense is built with JavaScript
* The API will be able to run from any browser.
* You will need a web cam from which to get the image used to feed the hand tracking algorithm.
* Camera input will be obtined with [getUserMedia()](https://webrtc.github.io/samples/src/content/getusermedia/gum/)

## Image recognition engine

Has been created with [ml5](https://ml5js.org).
In order to get a deeper understanding on neural networks and image and also to learn the first steps to use the libray we recomend [The Coding Traing](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6YPSwT06y_AEYTqIwbeam3y)

## Demo

* Demos will be created with [Babylon.js](https://www.babylonjs.com).

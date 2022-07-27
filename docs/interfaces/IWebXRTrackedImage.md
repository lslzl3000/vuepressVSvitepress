[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRTrackedImage

# Interface: IWebXRTrackedImage

An object representing an image tracked by the system

## Table of contents

### Properties

- [emulated](IWebXRTrackedImage.md#emulated)
- [id](IWebXRTrackedImage.md#id)
- [originalBitmap](IWebXRTrackedImage.md#originalbitmap)
- [ratio](IWebXRTrackedImage.md#ratio)
- [realWorldWidth](IWebXRTrackedImage.md#realworldwidth)
- [transformationMatrix](IWebXRTrackedImage.md#transformationmatrix)
- [xrTrackingResult](IWebXRTrackedImage.md#xrtrackingresult)

## Properties

### emulated

• `Optional` **emulated**: `boolean`

Is the transformation provided emulated. If it is, the system "guesses" its real position. Otherwise it can be considered as exact position.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:39

___

### id

• **id**: `number`

The ID of this image (which is the same as the position in the array that was used to initialize the feature)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:35

___

### originalBitmap

• **originalBitmap**: `ImageBitmap`

Just in case it is needed - the image bitmap that is being tracked

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:43

___

### ratio

• `Optional` **ratio**: `number`

The width/height ratio of this image. can be used to calculate the size of the detected object/image

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:59

___

### realWorldWidth

• `Optional` **realWorldWidth**: `number`

Width in real world (meters)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:51

___

### transformationMatrix

• **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

A transformation matrix of this current image in the current reference space.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:55

___

### xrTrackingResult

• `Optional` **xrTrackingResult**: `XRImageTrackingResult`

The native XR result image tracking result, untouched

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRImageTracking.ts:47

[@dev/core](../README.md) / [Exports](../modules.md) / VRCameraMetrics

# Class: VRCameraMetrics

This represents all the required metrics to create a VR camera.

**`See`**

https://doc.babylonjs.com/babylon101/cameras#device-orientation-camera

## Table of contents

### Constructors

- [constructor](VRCameraMetrics.md#constructor)

### Properties

- [chromaAbCorrection](VRCameraMetrics.md#chromaabcorrection)
- [compensateDistortion](VRCameraMetrics.md#compensatedistortion)
- [distortionK](VRCameraMetrics.md#distortionk)
- [eyeToScreenDistance](VRCameraMetrics.md#eyetoscreendistance)
- [hResolution](VRCameraMetrics.md#hresolution)
- [hScreenSize](VRCameraMetrics.md#hscreensize)
- [interpupillaryDistance](VRCameraMetrics.md#interpupillarydistance)
- [lensCenterOffset](VRCameraMetrics.md#lenscenteroffset)
- [lensSeparationDistance](VRCameraMetrics.md#lensseparationdistance)
- [multiviewEnabled](VRCameraMetrics.md#multiviewenabled)
- [postProcessScaleFactor](VRCameraMetrics.md#postprocessscalefactor)
- [vResolution](VRCameraMetrics.md#vresolution)
- [vScreenCenter](VRCameraMetrics.md#vscreencenter)
- [vScreenSize](VRCameraMetrics.md#vscreensize)

### Accessors

- [aspectRatio](VRCameraMetrics.md#aspectratio)
- [aspectRatioFov](VRCameraMetrics.md#aspectratiofov)

### Methods

- [GetDefault](VRCameraMetrics.md#getdefault)

## Constructors

### constructor

• **new VRCameraMetrics**()

## Properties

### chromaAbCorrection

• **chromaAbCorrection**: `number`[]

Define the chromatic aberration correction factors for the VR post process.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:47

___

### compensateDistortion

• **compensateDistortion**: `boolean` = `true`

Define if the current vr camera should compensate the distortion of the lens or not.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:60

___

### distortionK

• **distortionK**: `number`[]

Define the distortion factor of the VR postprocess.
Please, touch with care.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:43

___

### eyeToScreenDistance

• **eyeToScreenDistance**: `number`

Define the distance of the eyes to the screen.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:30

___

### hResolution

• **hResolution**: `number`

Define the horizontal resolution off the screen.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:10

___

### hScreenSize

• **hScreenSize**: `number`

Define the horizontal screen size.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:18

___

### interpupillaryDistance

• **interpupillaryDistance**: `number`

Define the distance between both viewer's eyes.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:38

___

### lensCenterOffset

• **lensCenterOffset**: `number`

Define an offset for the lens center.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:56

___

### lensSeparationDistance

• **lensSeparationDistance**: `number`

Define the distance between both lenses

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:34

___

### multiviewEnabled

• **multiviewEnabled**: `boolean` = `false`

Defines if multiview should be enabled when rendering (Default: false)

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:65

___

### postProcessScaleFactor

• **postProcessScaleFactor**: `number`

Define the scale factor of the post process.
The smaller the better but the slower.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:52

___

### vResolution

• **vResolution**: `number`

Define the vertical resolution off the screen.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:14

___

### vScreenCenter

• **vScreenCenter**: `number`

Define the vertical screen center position.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:26

___

### vScreenSize

• **vScreenSize**: `number`

Define the vertical screen size.

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:22

## Accessors

### aspectRatio

• `get` **aspectRatio**(): `number`

Gets the rendering aspect ratio based on the provided resolutions.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:70

___

### aspectRatioFov

• `get` **aspectRatioFov**(): `number`

Gets the aspect ratio based on the FOV, scale factors, and real screen sizes.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:77

## Methods

### GetDefault

▸ `Static` **GetDefault**(): [`VRCameraMetrics`](VRCameraMetrics.md)

Get the default VRMetrics based on the most generic setup.

#### Returns

[`VRCameraMetrics`](VRCameraMetrics.md)

the default vr metrics

#### Defined in

packages/dev/core/src/Cameras/VR/vrCameraMetrics.ts:119

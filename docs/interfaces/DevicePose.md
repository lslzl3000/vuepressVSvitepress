[@dev/core](../README.md) / [Exports](../modules.md) / DevicePose

# Interface: DevicePose

This is a copy of VRPose. See https://developer.mozilla.org/en-US/docs/Web/API/VRPose
IMPORTANT!! The data is right-hand data.

**`Export`**

**`Interface`**

DevicePose

## Table of contents

### Properties

- [angularAcceleration](DevicePose.md#angularacceleration)
- [angularVelocity](DevicePose.md#angularvelocity)
- [linearAcceleration](DevicePose.md#linearacceleration)
- [linearVelocity](DevicePose.md#linearvelocity)
- [orientation](DevicePose.md#orientation)
- [position](DevicePose.md#position)

## Properties

### angularAcceleration

• `Readonly` **angularAcceleration**: [`Nullable`](../modules.md#nullable)`Float32Array`

The angularAcceleration of the device, values in array are [x,y,z].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:64

___

### angularVelocity

• `Readonly` **angularVelocity**: [`Nullable`](../modules.md#nullable)`Float32Array`

The angularVelocity of the device, values in array are [x,y,z].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:60

___

### linearAcceleration

• `Readonly` **linearAcceleration**: [`Nullable`](../modules.md#nullable)`Float32Array`

The linearAcceleration of the device, values in array are [x,y,z].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:51

___

### linearVelocity

• `Readonly` **linearVelocity**: [`Nullable`](../modules.md#nullable)`Float32Array`

The linearVelocity of the device, values in array are [x,y,z].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:47

___

### orientation

• `Readonly` **orientation**: [`Nullable`](../modules.md#nullable)`Float32Array`

The orientation of the device in a quaternion array, values in array are [x,y,z,w].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:56

___

### position

• `Readonly` **position**: [`Nullable`](../modules.md#nullable)`Float32Array`

The position of the device, values in array are [x,y,z].

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:43

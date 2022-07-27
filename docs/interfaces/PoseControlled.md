[@dev/core](../README.md) / [Exports](../modules.md) / PoseControlled

# Interface: PoseControlled

Interface representing a pose controlled object in Babylon.
A pose controlled object has both regular pose values as well as pose values
from an external device such as a VR head mounted display

## Implemented by

- [`PoseEnabledController`](../classes/PoseEnabledController.md)
- [`WebVRFreeCamera`](../classes/WebVRFreeCamera.md)

## Table of contents

### Properties

- [devicePosition](PoseControlled.md#deviceposition)
- [deviceRotationQuaternion](PoseControlled.md#devicerotationquaternion)
- [deviceScaleFactor](PoseControlled.md#devicescalefactor)
- [position](PoseControlled.md#position)
- [rawPose](PoseControlled.md#rawpose)
- [rotationQuaternion](PoseControlled.md#rotationquaternion)

### Methods

- [updateFromDevice](PoseControlled.md#updatefromdevice)

## Properties

### devicePosition

• `Optional` **devicePosition**: [`Vector3`](../classes/Vector3.md)

The position of the device in babylon space.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:84

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](../classes/Quaternion.md)

The rotation quaternion of the device in babylon space.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:88

___

### deviceScaleFactor

• **deviceScaleFactor**: `number`

The scale of the device to be used when translating from device space to babylon space.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:96

___

### position

• **position**: [`Vector3`](../classes/Vector3.md)

The position of the object in babylon space.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:76

___

### rawPose

• **rawPose**: [`Nullable`](../modules.md#nullable)[`DevicePose`](DevicePose.md)

The raw pose coming from the device.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:92

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](../classes/Quaternion.md)

The rotation quaternion of the object in babylon space.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:80

## Methods

### updateFromDevice

▸ **updateFromDevice**(`poseData`): `void`

Updates the poseControlled values based on the input device pose.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poseData` | [`DevicePose`](DevicePose.md) | the pose data to update the object with |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:101

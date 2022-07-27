[@dev/core](../README.md) / [Exports](../modules.md) / PoseEnabledController

# Class: PoseEnabledController

Defines the PoseEnabledController object that contains state of a vr capable controller

## Hierarchy

- [`Gamepad`](Gamepad.md)

  ↳ **`PoseEnabledController`**

  ↳↳ [`WebVRController`](WebVRController.md)

## Implements

- [`PoseControlled`](../interfaces/PoseControlled.md)

## Table of contents

### Constructors

- [constructor](PoseEnabledController.md#constructor)

### Properties

- [\_calculatedPosition](PoseEnabledController.md#_calculatedposition)
- [\_calculatedRotation](PoseEnabledController.md#_calculatedrotation)
- [\_deviceRoomPosition](PoseEnabledController.md#_deviceroomposition)
- [\_deviceRoomRotationQuaternion](PoseEnabledController.md#_deviceroomrotationquaternion)
- [\_draggedRoomRotation](PoseEnabledController.md#_draggedroomrotation)
- [\_invertLeftStickY](PoseEnabledController.md#_invertleftsticky)
- [\_leftHandSystemQuaternion](PoseEnabledController.md#_lefthandsystemquaternion)
- [\_maxRotationDistFromHeadset](PoseEnabledController.md#_maxrotationdistfromheadset)
- [\_poseControlledCamera](PoseEnabledController.md#_posecontrolledcamera)
- [\_trackPosition](PoseEnabledController.md#_trackposition)
- [\_workingMatrix](PoseEnabledController.md#_workingmatrix)
- [browserGamepad](PoseEnabledController.md#browsergamepad)
- [controllerType](PoseEnabledController.md#controllertype)
- [devicePosition](PoseEnabledController.md#deviceposition)
- [deviceRotationQuaternion](PoseEnabledController.md#devicerotationquaternion)
- [deviceScaleFactor](PoseEnabledController.md#devicescalefactor)
- [id](PoseEnabledController.md#id)
- [index](PoseEnabledController.md#index)
- [isXR](PoseEnabledController.md#isxr)
- [position](PoseEnabledController.md#position)
- [rawPose](PoseEnabledController.md#rawpose)
- [rotationQuaternion](PoseEnabledController.md#rotationquaternion)
- [type](PoseEnabledController.md#type)
- [DUALSHOCK](PoseEnabledController.md#dualshock)
- [GAMEPAD](PoseEnabledController.md#gamepad)
- [GENERIC](PoseEnabledController.md#generic)
- [POINTING\_POSE](PoseEnabledController.md#pointing_pose)
- [POSE\_ENABLED](PoseEnabledController.md#pose_enabled)
- [XBOX](PoseEnabledController.md#xbox)

### Accessors

- [isConnected](PoseEnabledController.md#isconnected)
- [leftStick](PoseEnabledController.md#leftstick)
- [mesh](PoseEnabledController.md#mesh)
- [rightStick](PoseEnabledController.md#rightstick)

### Methods

- [\_updatePoseAndMesh](PoseEnabledController.md#_updateposeandmesh)
- [attachToMesh](PoseEnabledController.md#attachtomesh)
- [attachToPoseControlledCamera](PoseEnabledController.md#attachtoposecontrolledcamera)
- [dispose](PoseEnabledController.md#dispose)
- [getForwardRay](PoseEnabledController.md#getforwardray)
- [onleftstickchanged](PoseEnabledController.md#onleftstickchanged)
- [onrightstickchanged](PoseEnabledController.md#onrightstickchanged)
- [update](PoseEnabledController.md#update)
- [updateFromDevice](PoseEnabledController.md#updatefromdevice)

## Constructors

### constructor

• **new PoseEnabledController**(`browserGamepad`)

Creates a new PoseEnabledController from a gamepad

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `browserGamepad` | `any` | the gamepad that the PoseEnabledController should be created from |

#### Overrides

[Gamepad](Gamepad.md).[constructor](Gamepad.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:218

## Properties

### \_calculatedPosition

• `Protected` **\_calculatedPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:167

___

### \_calculatedRotation

• `Private` **\_calculatedRotation**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:168

___

### \_deviceRoomPosition

• `Private` **\_deviceRoomPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:138

___

### \_deviceRoomRotationQuaternion

• `Private` **\_deviceRoomRotationQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:139

___

### \_draggedRoomRotation

• `Private` **\_draggedRoomRotation**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:178

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[Gamepad](Gamepad.md).[_invertLeftStickY](Gamepad.md#_invertleftsticky)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:100

___

### \_leftHandSystemQuaternion

• `Private` **\_leftHandSystemQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:197

___

### \_maxRotationDistFromHeadset

• `Private` **\_maxRotationDistFromHeadset**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:177

___

### \_poseControlledCamera

• `Private` **\_poseControlledCamera**: [`TargetCamera`](TargetCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:195

___

### \_trackPosition

• `Private` **\_trackPosition**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:176

___

### \_workingMatrix

• `Private` **\_workingMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:230

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[Gamepad](Gamepad.md).[browserGamepad](Gamepad.md#browsergamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:131

___

### controllerType

• **controllerType**: [`PoseEnabledControllerType`](../enums/PoseEnabledControllerType.md)

The type of controller (Eg. Windows mixed reality)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:165

___

### devicePosition

• **devicePosition**: [`Vector3`](Vector3.md)

The device position in babylon space

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[devicePosition](../interfaces/PoseControlled.md#deviceposition)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:144

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](Quaternion.md)

The device rotation in babylon space

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[deviceRotationQuaternion](../interfaces/PoseControlled.md#devicerotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:148

___

### deviceScaleFactor

• **deviceScaleFactor**: `number` = `1`

The scale factor of the device in babylon space

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[deviceScaleFactor](../interfaces/PoseControlled.md#devicescalefactor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:152

___

### id

• **id**: `string`

#### Inherited from

[Gamepad](Gamepad.md).[id](Gamepad.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[Gamepad](Gamepad.md).[index](Gamepad.md#index)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:127

___

### isXR

• **isXR**: `boolean` = `false`

If the controller is used in a webXR session

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:136

___

### position

• **position**: [`Vector3`](Vector3.md)

(Likely devicePosition should be used instead) The device position in its room space

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[position](../interfaces/PoseControlled.md#position)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:157

___

### rawPose

• **rawPose**: [`DevicePose`](../interfaces/DevicePose.md)

The raw pose from the device

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[rawPose](../interfaces/PoseControlled.md#rawpose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:173

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

(Likely deviceRotationQuaternion should be used instead) The device rotation in its room space

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[rotationQuaternion](../interfaces/PoseControlled.md#rotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:161

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[Gamepad](Gamepad.md).[type](Gamepad.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[Gamepad](Gamepad.md).[DUALSHOCK](Gamepad.md#dualshock)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[Gamepad](Gamepad.md).[GAMEPAD](Gamepad.md#gamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[Gamepad](Gamepad.md).[GENERIC](Gamepad.md#generic)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:83

___

### POINTING\_POSE

▪ `Static` `Readonly` **POINTING\_POSE**: ``"POINTING_POSE"``

Name of the child mesh that can be used to cast a ray from the controller

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:213

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[Gamepad](Gamepad.md).[POSE_ENABLED](Gamepad.md#pose_enabled)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[Gamepad](Gamepad.md).[XBOX](Gamepad.md#xbox)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:87

## Accessors

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

Gamepad.isConnected

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.leftStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:169

• `set` **leftStick**(`newValues`): `void`

Sets the left joystick values

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

Gamepad.leftStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:175

___

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is attached to the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:396

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.rightStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:184

• `set` **rightStick**(`newValues`): `void`

Sets the right joystick value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

Gamepad.rightStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:190

## Methods

### \_updatePoseAndMesh

▸ `Protected` **_updatePoseAndMesh**(): `void`

Updates only the pose device and mesh without doing any button event checking

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:242

___

### attachToMesh

▸ **attachToMesh**(`mesh`): `void`

Attaches a mesh to the controller

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh to be attached |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:339

___

### attachToPoseControlledCamera

▸ **attachToPoseControlledCamera**(`camera`): `void`

Attaches the controllers mesh to a camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`TargetCamera`](TargetCamera.md) | the camera the mesh should be attached to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:374

___

### dispose

▸ **dispose**(): `void`

Disposes of the controller

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[dispose](Gamepad.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:384

___

### getForwardRay

▸ **getForwardRay**(`length?`): [`Ray`](Ray.md)

Gets the ray of the controller in the direction the controller is pointing

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `length` | `number` | `100` | the length the resulting ray should be |

#### Returns

[`Ray`](Ray.md)

a ray in the direction the controller is pointing

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:405

___

### onleftstickchanged

▸ **onleftstickchanged**(`callback`): `void`

Callback triggered when the left joystick has changed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`values`: [`StickValues`](StickValues.md)) => `void` |

#### Returns

`void`

#### Inherited from

[Gamepad](Gamepad.md).[onleftstickchanged](Gamepad.md#onleftstickchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:154

___

### onrightstickchanged

▸ **onrightstickchanged**(`callback`): `void`

Callback triggered when the right joystick has changed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`values`: [`StickValues`](StickValues.md)) => `void` |

#### Returns

`void`

#### Inherited from

[Gamepad](Gamepad.md).[onrightstickchanged](Gamepad.md#onrightstickchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Updates the state of the pose enabled controller and mesh based on the current position and rotation of the controller

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[update](Gamepad.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:234

___

### updateFromDevice

▸ **updateFromDevice**(`poseData`): `void`

Updates the state of the pose enbaled controller based on the raw pose data from the device

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `poseData` | [`DevicePose`](../interfaces/DevicePose.md) | raw pose fromthe device |

#### Returns

`void`

#### Implementation of

[PoseControlled](../interfaces/PoseControlled.md).[updateFromDevice](../interfaces/PoseControlled.md#updatefromdevice)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:296

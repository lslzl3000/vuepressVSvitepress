[@dev/core](../README.md) / [Exports](../modules.md) / WebVRController

# Class: WebVRController

Defines the WebVRController object that represents controllers tracked in 3D space

**`Deprecated`**

Use WebXR instead

## Hierarchy

- [`PoseEnabledController`](PoseEnabledController.md)

  ↳ **`WebVRController`**

  ↳↳ [`DaydreamController`](DaydreamController.md)

  ↳↳ [`GearVRController`](GearVRController.md)

  ↳↳ [`GenericController`](GenericController.md)

  ↳↳ [`OculusTouchController`](OculusTouchController.md)

  ↳↳ [`ViveController`](ViveController.md)

  ↳↳ [`WindowsMotionController`](WindowsMotionController.md)

## Table of contents

### Constructors

- [constructor](WebVRController.md#constructor)

### Properties

- [\_buttons](WebVRController.md#_buttons)
- [\_calculatedPosition](WebVRController.md#_calculatedposition)
- [\_changes](WebVRController.md#_changes)
- [\_defaultModel](WebVRController.md#_defaultmodel)
- [\_invertLeftStickY](WebVRController.md#_invertleftsticky)
- [\_onButtonStateChange](WebVRController.md#_onbuttonstatechange)
- [browserGamepad](WebVRController.md#browsergamepad)
- [controllerType](WebVRController.md#controllertype)
- [devicePosition](WebVRController.md#deviceposition)
- [deviceRotationQuaternion](WebVRController.md#devicerotationquaternion)
- [deviceScaleFactor](WebVRController.md#devicescalefactor)
- [hand](WebVRController.md#hand)
- [id](WebVRController.md#id)
- [index](WebVRController.md#index)
- [isXR](WebVRController.md#isxr)
- [onMainButtonStateChangedObservable](WebVRController.md#onmainbuttonstatechangedobservable)
- [onPadStateChangedObservable](WebVRController.md#onpadstatechangedobservable)
- [onPadValuesChangedObservable](WebVRController.md#onpadvalueschangedobservable)
- [onSecondaryButtonStateChangedObservable](WebVRController.md#onsecondarybuttonstatechangedobservable)
- [onTriggerStateChangedObservable](WebVRController.md#ontriggerstatechangedobservable)
- [pad](WebVRController.md#pad)
- [position](WebVRController.md#position)
- [rawPose](WebVRController.md#rawpose)
- [rotationQuaternion](WebVRController.md#rotationquaternion)
- [type](WebVRController.md#type)
- [DUALSHOCK](WebVRController.md#dualshock)
- [GAMEPAD](WebVRController.md#gamepad)
- [GENERIC](WebVRController.md#generic)
- [POINTING\_POSE](WebVRController.md#pointing_pose)
- [POSE\_ENABLED](WebVRController.md#pose_enabled)
- [XBOX](WebVRController.md#xbox)

### Accessors

- [defaultModel](WebVRController.md#defaultmodel)
- [isConnected](WebVRController.md#isconnected)
- [leftStick](WebVRController.md#leftstick)
- [mesh](WebVRController.md#mesh)
- [rightStick](WebVRController.md#rightstick)

### Methods

- [\_checkChanges](WebVRController.md#_checkchanges)
- [\_handleButtonChange](WebVRController.md#_handlebuttonchange)
- [\_setButtonValue](WebVRController.md#_setbuttonvalue)
- [\_updatePoseAndMesh](WebVRController.md#_updateposeandmesh)
- [attachToMesh](WebVRController.md#attachtomesh)
- [attachToPoseControlledCamera](WebVRController.md#attachtoposecontrolledcamera)
- [dispose](WebVRController.md#dispose)
- [getForwardRay](WebVRController.md#getforwardray)
- [initControllerMesh](WebVRController.md#initcontrollermesh)
- [onButtonStateChange](WebVRController.md#onbuttonstatechange)
- [onleftstickchanged](WebVRController.md#onleftstickchanged)
- [onrightstickchanged](WebVRController.md#onrightstickchanged)
- [update](WebVRController.md#update)
- [updateFromDevice](WebVRController.md#updatefromdevice)

## Constructors

### constructor

• **new WebVRController**(`vrGamepad`)

Creates a new WebVRController from a gamepad

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vrGamepad` | `any` | the gamepad that the WebVRController should be created from |

#### Overrides

[PoseEnabledController](PoseEnabledController.md).[constructor](PoseEnabledController.md#constructor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:77

## Properties

### \_buttons

• `Protected` **\_buttons**: [`MutableGamepadButton`](../interfaces/MutableGamepadButton.md)[]

Array of button available on the controller

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:44

___

### \_calculatedPosition

• `Protected` **\_calculatedPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[_calculatedPosition](PoseEnabledController.md#_calculatedposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:167

___

### \_changes

• `Private` **\_changes**: [`GamepadButtonChanges`](../interfaces/GamepadButtonChanges.md)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:139

___

### \_defaultModel

• `Protected` **\_defaultModel**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Internal, the default controller model for the controller

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:17

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[_invertLeftStickY](PoseEnabledController.md#_invertleftsticky)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:100

___

### \_onButtonStateChange

• `Private` **\_onButtonStateChange**: (`controlledIndex`: `number`, `buttonIndex`: `number`, `state`: `ExtendedGamepadButton`) => `void`

#### Type declaration

▸ (`controlledIndex`, `buttonIndex`, `state`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `controlledIndex` | `number` |
| `buttonIndex` | `number` |
| `state` | `ExtendedGamepadButton` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:46

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[browserGamepad](PoseEnabledController.md#browsergamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:131

___

### controllerType

• **controllerType**: [`PoseEnabledControllerType`](../enums/PoseEnabledControllerType.md)

The type of controller (Eg. Windows mixed reality)

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[controllerType](PoseEnabledController.md#controllertype)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:165

___

### devicePosition

• **devicePosition**: [`Vector3`](Vector3.md)

The device position in babylon space

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[devicePosition](PoseEnabledController.md#deviceposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:144

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](Quaternion.md)

The device rotation in babylon space

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[deviceRotationQuaternion](PoseEnabledController.md#devicerotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:148

___

### deviceScaleFactor

• **deviceScaleFactor**: `number` = `1`

The scale factor of the device in babylon space

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[deviceScaleFactor](PoseEnabledController.md#devicescalefactor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:152

___

### hand

• **hand**: `string`

'left' or 'right', see https://w3c.github.io/gamepad/extensions.html#gamepadhand-enum

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:64

___

### id

• **id**: `string`

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[id](PoseEnabledController.md#id)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[index](PoseEnabledController.md#index)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:127

___

### isXR

• **isXR**: `boolean` = `false`

If the controller is used in a webXR session

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[isXR](PoseEnabledController.md#isxr)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:136

___

### onMainButtonStateChangedObservable

• **onMainButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the main button state has changed

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:27

___

### onPadStateChangedObservable

• **onPadStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the pad state has changed

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:35

___

### onPadValuesChangedObservable

• **onPadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when controllers stick values have changed

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:39

___

### onSecondaryButtonStateChangedObservable

• **onSecondaryButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the secondary button state has changed

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:31

___

### onTriggerStateChangedObservable

• **onTriggerStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger state has changed

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:23

___

### pad

• **pad**: [`StickValues`](StickValues.md)

X and Y axis corresponding to the controllers joystick

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:59

___

### position

• **position**: [`Vector3`](Vector3.md)

(Likely devicePosition should be used instead) The device position in its room space

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[position](PoseEnabledController.md#position)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:157

___

### rawPose

• **rawPose**: [`DevicePose`](../interfaces/DevicePose.md)

The raw pose from the device

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[rawPose](PoseEnabledController.md#rawpose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:173

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

(Likely deviceRotationQuaternion should be used instead) The device rotation in its room space

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[rotationQuaternion](PoseEnabledController.md#rotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:161

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[type](PoseEnabledController.md#type)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[DUALSHOCK](PoseEnabledController.md#dualshock)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[GAMEPAD](PoseEnabledController.md#gamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[GENERIC](PoseEnabledController.md#generic)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:83

___

### POINTING\_POSE

▪ `Static` `Readonly` **POINTING\_POSE**: ``"POINTING_POSE"``

Name of the child mesh that can be used to cast a ray from the controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[POINTING_POSE](PoseEnabledController.md#pointing_pose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:213

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[POSE_ENABLED](PoseEnabledController.md#pose_enabled)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[XBOX](PoseEnabledController.md#xbox)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:87

## Accessors

### defaultModel

• `get` **defaultModel**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The default controller model for the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:69

___

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

PoseEnabledController.isConnected

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

PoseEnabledController.leftStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:169

• `set` **leftStick**(`newValues`): `void`

Sets the left joystick values

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

PoseEnabledController.leftStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:175

___

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is attached to the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

PoseEnabledController.mesh

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:396

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

PoseEnabledController.rightStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:184

• `set` **rightStick**(`newValues`): `void`

Sets the right joystick value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

PoseEnabledController.rightStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:190

## Methods

### \_checkChanges

▸ `Private` **_checkChanges**(`newState`, `currentState`): [`GamepadButtonChanges`](../interfaces/GamepadButtonChanges.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `newState` | `ExtendedGamepadButton` |
| `currentState` | `ExtendedGamepadButton` |

#### Returns

[`GamepadButtonChanges`](../interfaces/GamepadButtonChanges.md)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:146

___

### \_handleButtonChange

▸ `Protected` `Abstract` **_handleButtonChange**(`buttonIdx`, `value`, `changes`): `void`

Function to be called when a button is modified

#### Parameters

| Name | Type |
| :------ | :------ |
| `buttonIdx` | `number` |
| `value` | `ExtendedGamepadButton` |
| `changes` | [`GamepadButtonChanges`](../interfaces/GamepadButtonChanges.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:101

___

### \_setButtonValue

▸ `Private` **_setButtonValue**(`newState`, `currentState`, `buttonIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newState` | `ExtendedGamepadButton` |
| `currentState` | `ExtendedGamepadButton` |
| `buttonIndex` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:110

___

### \_updatePoseAndMesh

▸ `Protected` **_updatePoseAndMesh**(): `void`

Updates only the pose device and mesh without doing any button event checking

#### Returns

`void`

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[_updatePoseAndMesh](PoseEnabledController.md#_updateposeandmesh)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:242

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

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[attachToMesh](PoseEnabledController.md#attachtomesh)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:339

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

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[attachToPoseControlledCamera](PoseEnabledController.md#attachtoposecontrolledcamera)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:374

___

### dispose

▸ **dispose**(): `void`

Disposes of th webVRController

#### Returns

`void`

#### Overrides

[PoseEnabledController](PoseEnabledController.md).[dispose](PoseEnabledController.md#dispose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:157

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

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[getForwardRay](PoseEnabledController.md#getforwardray)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:405

___

### initControllerMesh

▸ `Abstract` **initControllerMesh**(`scene`, `meshLoaded?`): `void`

Loads a mesh and attaches it to the controller

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | the scene the mesh should be added to |
| `meshLoaded?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | callback for when the mesh has been loaded |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:108

___

### onButtonStateChange

▸ **onButtonStateChange**(`callback`): `void`

Fired when a controller button's state has changed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`controlledIndex`: `number`, `buttonIndex`: `number`, `state`: `ExtendedGamepadButton`) => `void` | the callback containing the button that was modified |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:52

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

[PoseEnabledController](PoseEnabledController.md).[onleftstickchanged](PoseEnabledController.md#onleftstickchanged)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:154

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

[PoseEnabledController](PoseEnabledController.md).[onrightstickchanged](PoseEnabledController.md#onrightstickchanged)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Updates the state of the controller and mesh based on the current position and rotation of the controller

#### Returns

`void`

#### Overrides

[PoseEnabledController](PoseEnabledController.md).[update](PoseEnabledController.md#update)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:86

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

#### Inherited from

[PoseEnabledController](PoseEnabledController.md).[updateFromDevice](PoseEnabledController.md#updatefromdevice)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:296

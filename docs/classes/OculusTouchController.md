[@dev/core](../README.md) / [Exports](../modules.md) / OculusTouchController

# Class: OculusTouchController

Oculus Touch Controller

## Hierarchy

- [`WebVRController`](WebVRController.md)

  ↳ **`OculusTouchController`**

## Table of contents

### Constructors

- [constructor](OculusTouchController.md#constructor)

### Properties

- [\_buttons](OculusTouchController.md#_buttons)
- [\_calculatedPosition](OculusTouchController.md#_calculatedposition)
- [\_defaultModel](OculusTouchController.md#_defaultmodel)
- [\_invertLeftStickY](OculusTouchController.md#_invertleftsticky)
- [browserGamepad](OculusTouchController.md#browsergamepad)
- [controllerType](OculusTouchController.md#controllertype)
- [devicePosition](OculusTouchController.md#deviceposition)
- [deviceRotationQuaternion](OculusTouchController.md#devicerotationquaternion)
- [deviceScaleFactor](OculusTouchController.md#devicescalefactor)
- [hand](OculusTouchController.md#hand)
- [id](OculusTouchController.md#id)
- [index](OculusTouchController.md#index)
- [isXR](OculusTouchController.md#isxr)
- [onMainButtonStateChangedObservable](OculusTouchController.md#onmainbuttonstatechangedobservable)
- [onPadStateChangedObservable](OculusTouchController.md#onpadstatechangedobservable)
- [onPadValuesChangedObservable](OculusTouchController.md#onpadvalueschangedobservable)
- [onSecondaryButtonStateChangedObservable](OculusTouchController.md#onsecondarybuttonstatechangedobservable)
- [onSecondaryTriggerStateChangedObservable](OculusTouchController.md#onsecondarytriggerstatechangedobservable)
- [onThumbRestChangedObservable](OculusTouchController.md#onthumbrestchangedobservable)
- [onTriggerStateChangedObservable](OculusTouchController.md#ontriggerstatechangedobservable)
- [pad](OculusTouchController.md#pad)
- [position](OculusTouchController.md#position)
- [rawPose](OculusTouchController.md#rawpose)
- [rotationQuaternion](OculusTouchController.md#rotationquaternion)
- [type](OculusTouchController.md#type)
- [DUALSHOCK](OculusTouchController.md#dualshock)
- [GAMEPAD](OculusTouchController.md#gamepad)
- [GENERIC](OculusTouchController.md#generic)
- [MODEL\_BASE\_URL](OculusTouchController.md#model_base_url)
- [MODEL\_LEFT\_FILENAME](OculusTouchController.md#model_left_filename)
- [MODEL\_RIGHT\_FILENAME](OculusTouchController.md#model_right_filename)
- [POINTING\_POSE](OculusTouchController.md#pointing_pose)
- [POSE\_ENABLED](OculusTouchController.md#pose_enabled)
- [QUEST\_MODEL\_BASE\_URL](OculusTouchController.md#quest_model_base_url)
- [XBOX](OculusTouchController.md#xbox)

### Accessors

- [defaultModel](OculusTouchController.md#defaultmodel)
- [isConnected](OculusTouchController.md#isconnected)
- [leftStick](OculusTouchController.md#leftstick)
- [mesh](OculusTouchController.md#mesh)
- [onAButtonStateChangedObservable](OculusTouchController.md#onabuttonstatechangedobservable)
- [onBButtonStateChangedObservable](OculusTouchController.md#onbbuttonstatechangedobservable)
- [onXButtonStateChangedObservable](OculusTouchController.md#onxbuttonstatechangedobservable)
- [onYButtonStateChangedObservable](OculusTouchController.md#onybuttonstatechangedobservable)
- [rightStick](OculusTouchController.md#rightstick)

### Methods

- [\_handleButtonChange](OculusTouchController.md#_handlebuttonchange)
- [\_updatePoseAndMesh](OculusTouchController.md#_updateposeandmesh)
- [attachToMesh](OculusTouchController.md#attachtomesh)
- [attachToPoseControlledCamera](OculusTouchController.md#attachtoposecontrolledcamera)
- [dispose](OculusTouchController.md#dispose)
- [getForwardRay](OculusTouchController.md#getforwardray)
- [initControllerMesh](OculusTouchController.md#initcontrollermesh)
- [onButtonStateChange](OculusTouchController.md#onbuttonstatechange)
- [onleftstickchanged](OculusTouchController.md#onleftstickchanged)
- [onrightstickchanged](OculusTouchController.md#onrightstickchanged)
- [update](OculusTouchController.md#update)
- [updateFromDevice](OculusTouchController.md#updatefromdevice)

## Constructors

### constructor

• **new OculusTouchController**(`vrGamepad`)

Creates a new OculusTouchController from a gamepad

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vrGamepad` | `any` | the gamepad that the controller should be created from |

#### Overrides

[WebVRController](WebVRController.md).[constructor](WebVRController.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:51

## Properties

### \_buttons

• `Protected` **\_buttons**: [`MutableGamepadButton`](../interfaces/MutableGamepadButton.md)[]

Array of button available on the controller

#### Inherited from

[WebVRController](WebVRController.md).[_buttons](WebVRController.md#_buttons)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:44

___

### \_calculatedPosition

• `Protected` **\_calculatedPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[WebVRController](WebVRController.md).[_calculatedPosition](WebVRController.md#_calculatedposition)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:167

___

### \_defaultModel

• `Protected` **\_defaultModel**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Internal, the default controller model for the controller

#### Inherited from

[WebVRController](WebVRController.md).[_defaultModel](WebVRController.md#_defaultmodel)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:17

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[WebVRController](WebVRController.md).[_invertLeftStickY](WebVRController.md#_invertleftsticky)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:100

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[WebVRController](WebVRController.md).[browserGamepad](WebVRController.md#browsergamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:131

___

### controllerType

• **controllerType**: [`PoseEnabledControllerType`](../enums/PoseEnabledControllerType.md)

The type of controller (Eg. Windows mixed reality)

#### Inherited from

[WebVRController](WebVRController.md).[controllerType](WebVRController.md#controllertype)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:165

___

### devicePosition

• **devicePosition**: [`Vector3`](Vector3.md)

The device position in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[devicePosition](WebVRController.md#deviceposition)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:144

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](Quaternion.md)

The device rotation in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[deviceRotationQuaternion](WebVRController.md#devicerotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:148

___

### deviceScaleFactor

• **deviceScaleFactor**: `number` = `1`

The scale factor of the device in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[deviceScaleFactor](WebVRController.md#devicescalefactor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:152

___

### hand

• **hand**: `string`

'left' or 'right', see https://w3c.github.io/gamepad/extensions.html#gamepadhand-enum

#### Inherited from

[WebVRController](WebVRController.md).[hand](WebVRController.md#hand)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:64

___

### id

• **id**: `string`

#### Inherited from

[WebVRController](WebVRController.md).[id](WebVRController.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[WebVRController](WebVRController.md).[index](WebVRController.md#index)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:127

___

### isXR

• **isXR**: `boolean` = `false`

If the controller is used in a webXR session

#### Inherited from

[WebVRController](WebVRController.md).[isXR](WebVRController.md#isxr)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:136

___

### onMainButtonStateChangedObservable

• **onMainButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the main button state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onMainButtonStateChangedObservable](WebVRController.md#onmainbuttonstatechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:27

___

### onPadStateChangedObservable

• **onPadStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the pad state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onPadStateChangedObservable](WebVRController.md#onpadstatechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:35

___

### onPadValuesChangedObservable

• **onPadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when controllers stick values have changed

#### Inherited from

[WebVRController](WebVRController.md).[onPadValuesChangedObservable](WebVRController.md#onpadvalueschangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:39

___

### onSecondaryButtonStateChangedObservable

• **onSecondaryButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the secondary button state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onSecondaryButtonStateChangedObservable](WebVRController.md#onsecondarybuttonstatechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:31

___

### onSecondaryTriggerStateChangedObservable

• **onSecondaryTriggerStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the secondary trigger on this controller is modified

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:40

___

### onThumbRestChangedObservable

• **onThumbRestChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the thumb rest on this controller is modified

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:45

___

### onTriggerStateChangedObservable

• **onTriggerStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onTriggerStateChangedObservable](WebVRController.md#ontriggerstatechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:23

___

### pad

• **pad**: [`StickValues`](StickValues.md)

X and Y axis corresponding to the controllers joystick

#### Inherited from

[WebVRController](WebVRController.md).[pad](WebVRController.md#pad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:59

___

### position

• **position**: [`Vector3`](Vector3.md)

(Likely devicePosition should be used instead) The device position in its room space

#### Inherited from

[WebVRController](WebVRController.md).[position](WebVRController.md#position)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:157

___

### rawPose

• **rawPose**: [`DevicePose`](../interfaces/DevicePose.md)

The raw pose from the device

#### Inherited from

[WebVRController](WebVRController.md).[rawPose](WebVRController.md#rawpose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:173

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

(Likely deviceRotationQuaternion should be used instead) The device rotation in its room space

#### Inherited from

[WebVRController](WebVRController.md).[rotationQuaternion](WebVRController.md#rotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:161

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[WebVRController](WebVRController.md).[type](WebVRController.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[WebVRController](WebVRController.md).[DUALSHOCK](WebVRController.md#dualshock)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[WebVRController](WebVRController.md).[GAMEPAD](WebVRController.md#gamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[WebVRController](WebVRController.md).[GENERIC](WebVRController.md#generic)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:83

___

### MODEL\_BASE\_URL

▪ `Static` **MODEL\_BASE\_URL**: `string` = `"https://controllers.babylonjs.com/oculus/"`

Base Url for the controller model.

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:16

___

### MODEL\_LEFT\_FILENAME

▪ `Static` **MODEL\_LEFT\_FILENAME**: `string` = `"left.babylon"`

File name for the left controller model.

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:20

___

### MODEL\_RIGHT\_FILENAME

▪ `Static` **MODEL\_RIGHT\_FILENAME**: `string` = `"right.babylon"`

File name for the right controller model.

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:24

___

### POINTING\_POSE

▪ `Static` `Readonly` **POINTING\_POSE**: ``"POINTING_POSE"``

Name of the child mesh that can be used to cast a ray from the controller

#### Inherited from

[WebVRController](WebVRController.md).[POINTING_POSE](WebVRController.md#pointing_pose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:213

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[WebVRController](WebVRController.md).[POSE_ENABLED](WebVRController.md#pose_enabled)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:91

___

### QUEST\_MODEL\_BASE\_URL

▪ `Static` **QUEST\_MODEL\_BASE\_URL**: `string` = `"https://controllers.babylonjs.com/oculusQuest/"`

Base Url for the Quest controller model.

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:29

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[WebVRController](WebVRController.md).[XBOX](WebVRController.md#xbox)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:87

## Accessors

### defaultModel

• `get` **defaultModel**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The default controller model for the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WebVRController.defaultModel

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:69

___

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

WebVRController.isConnected

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WebVRController.leftStick

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

WebVRController.leftStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:175

___

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is attached to the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WebVRController.mesh

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:396

___

### onAButtonStateChangedObservable

• `get` **onAButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the A button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:101

___

### onBButtonStateChangedObservable

• `get` **onBButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the B button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:112

___

### onXButtonStateChangedObservable

• `get` **onXButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the X button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:123

___

### onYButtonStateChangedObservable

• `get` **onYButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the Y button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:134

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WebVRController.rightStick

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

WebVRController.rightStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:190

## Methods

### \_handleButtonChange

▸ `Protected` **_handleButtonChange**(`buttonIdx`, `state`): `void`

Called once for each button that changed state since the last frame
0) thumb stick (touch, press, value = pressed (0,1)). value is in this.leftStick
1) index trigger (touch (?), press (only when value > 0.1), value 0 to 1)
2) secondary trigger (same)
3) A (right) X (left), touch, pressed = value
4) B / Y
5) thumb rest

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buttonIdx` | `number` | Which button index changed |
| `state` | `ExtendedGamepadButton` | New state of the button |

#### Returns

`void`

#### Overrides

[WebVRController](WebVRController.md).[_handleButtonChange](WebVRController.md#_handlebuttonchange)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:153

___

### \_updatePoseAndMesh

▸ `Protected` **_updatePoseAndMesh**(): `void`

Updates only the pose device and mesh without doing any button event checking

#### Returns

`void`

#### Inherited from

[WebVRController](WebVRController.md).[_updatePoseAndMesh](WebVRController.md#_updateposeandmesh)

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

#### Inherited from

[WebVRController](WebVRController.md).[attachToMesh](WebVRController.md#attachtomesh)

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

#### Inherited from

[WebVRController](WebVRController.md).[attachToPoseControlledCamera](WebVRController.md#attachtoposecontrolledcamera)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:374

___

### dispose

▸ **dispose**(): `void`

Disposes of th webVRController

#### Returns

`void`

#### Inherited from

[WebVRController](WebVRController.md).[dispose](WebVRController.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:157

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

[WebVRController](WebVRController.md).[getForwardRay](WebVRController.md#getforwardray)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:405

___

### initControllerMesh

▸ **initControllerMesh**(`scene`, `meshLoaded?`): `void`

Implements abstract method on WebVRController class, loading controller meshes and calling this.attachToMesh if successful.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | scene in which to add meshes |
| `meshLoaded?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | optional callback function that will be called if the mesh loads successfully. |

#### Returns

`void`

#### Overrides

[WebVRController](WebVRController.md).[initControllerMesh](WebVRController.md#initcontrollermesh)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/oculusTouchController.ts:61

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

#### Inherited from

[WebVRController](WebVRController.md).[onButtonStateChange](WebVRController.md#onbuttonstatechange)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:52

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

[WebVRController](WebVRController.md).[onleftstickchanged](WebVRController.md#onleftstickchanged)

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

[WebVRController](WebVRController.md).[onrightstickchanged](WebVRController.md#onrightstickchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Updates the state of the controller and mesh based on the current position and rotation of the controller

#### Returns

`void`

#### Inherited from

[WebVRController](WebVRController.md).[update](WebVRController.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/webVRController.ts:86

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

[WebVRController](WebVRController.md).[updateFromDevice](WebVRController.md#updatefromdevice)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/Controllers/poseEnabledController.ts:296

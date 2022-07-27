[@dev/core](../README.md) / [Exports](../modules.md) / WindowsMotionController

# Class: WindowsMotionController

Defines the WindowsMotionController object that the state of the windows motion controller

## Hierarchy

- [`WebVRController`](WebVRController.md)

  ↳ **`WindowsMotionController`**

  ↳↳ [`XRWindowsMotionController`](XRWindowsMotionController.md)

## Table of contents

### Constructors

- [constructor](WindowsMotionController.md#constructor)

### Properties

- [\_buttons](WindowsMotionController.md#_buttons)
- [\_calculatedPosition](WindowsMotionController.md#_calculatedposition)
- [\_defaultModel](WindowsMotionController.md#_defaultmodel)
- [\_invertLeftStickY](WindowsMotionController.md#_invertleftsticky)
- [\_loadedMeshInfo](WindowsMotionController.md#_loadedmeshinfo)
- [\_mapping](WindowsMotionController.md#_mapping)
- [browserGamepad](WindowsMotionController.md#browsergamepad)
- [controllerType](WindowsMotionController.md#controllertype)
- [devicePosition](WindowsMotionController.md#deviceposition)
- [deviceRotationQuaternion](WindowsMotionController.md#devicerotationquaternion)
- [deviceScaleFactor](WindowsMotionController.md#devicescalefactor)
- [hand](WindowsMotionController.md#hand)
- [id](WindowsMotionController.md#id)
- [index](WindowsMotionController.md#index)
- [isXR](WindowsMotionController.md#isxr)
- [onMainButtonStateChangedObservable](WindowsMotionController.md#onmainbuttonstatechangedobservable)
- [onPadStateChangedObservable](WindowsMotionController.md#onpadstatechangedobservable)
- [onPadValuesChangedObservable](WindowsMotionController.md#onpadvalueschangedobservable)
- [onSecondaryButtonStateChangedObservable](WindowsMotionController.md#onsecondarybuttonstatechangedobservable)
- [onTrackpadChangedObservable](WindowsMotionController.md#ontrackpadchangedobservable)
- [onTrackpadValuesChangedObservable](WindowsMotionController.md#ontrackpadvalueschangedobservable)
- [onTriggerStateChangedObservable](WindowsMotionController.md#ontriggerstatechangedobservable)
- [pad](WindowsMotionController.md#pad)
- [position](WindowsMotionController.md#position)
- [rawPose](WindowsMotionController.md#rawpose)
- [rotationQuaternion](WindowsMotionController.md#rotationquaternion)
- [trackpad](WindowsMotionController.md#trackpad)
- [type](WindowsMotionController.md#type)
- [DUALSHOCK](WindowsMotionController.md#dualshock)
- [GAMEPAD](WindowsMotionController.md#gamepad)
- [GAMEPAD\_ID\_PATTERN](WindowsMotionController.md#gamepad_id_pattern)
- [GAMEPAD\_ID\_PREFIX](WindowsMotionController.md#gamepad_id_prefix)
- [GENERIC](WindowsMotionController.md#generic)
- [MODEL\_BASE\_URL](WindowsMotionController.md#model_base_url)
- [MODEL\_LEFT\_FILENAME](WindowsMotionController.md#model_left_filename)
- [MODEL\_RIGHT\_FILENAME](WindowsMotionController.md#model_right_filename)
- [POINTING\_POSE](WindowsMotionController.md#pointing_pose)
- [POSE\_ENABLED](WindowsMotionController.md#pose_enabled)
- [XBOX](WindowsMotionController.md#xbox)

### Accessors

- [defaultModel](WindowsMotionController.md#defaultmodel)
- [isConnected](WindowsMotionController.md#isconnected)
- [leftStick](WindowsMotionController.md#leftstick)
- [mesh](WindowsMotionController.md#mesh)
- [onGripButtonStateChangedObservable](WindowsMotionController.md#ongripbuttonstatechangedobservable)
- [onMenuButtonStateChangedObservable](WindowsMotionController.md#onmenubuttonstatechangedobservable)
- [onThumbstickButtonStateChangedObservable](WindowsMotionController.md#onthumbstickbuttonstatechangedobservable)
- [onTouchpadButtonStateChangedObservable](WindowsMotionController.md#ontouchpadbuttonstatechangedobservable)
- [onTouchpadValuesChangedObservable](WindowsMotionController.md#ontouchpadvalueschangedobservable)
- [onTriggerButtonStateChangedObservable](WindowsMotionController.md#ontriggerbuttonstatechangedobservable)
- [rightStick](WindowsMotionController.md#rightstick)

### Methods

- [\_createMeshInfo](WindowsMotionController.md#_createmeshinfo)
- [\_handleButtonChange](WindowsMotionController.md#_handlebuttonchange)
- [\_lerpButtonTransform](WindowsMotionController.md#_lerpbuttontransform)
- [\_processModel](WindowsMotionController.md#_processmodel)
- [\_updatePoseAndMesh](WindowsMotionController.md#_updateposeandmesh)
- [\_updateTrackpad](WindowsMotionController.md#_updatetrackpad)
- [attachToMesh](WindowsMotionController.md#attachtomesh)
- [attachToPoseControlledCamera](WindowsMotionController.md#attachtoposecontrolledcamera)
- [dispose](WindowsMotionController.md#dispose)
- [getForwardRay](WindowsMotionController.md#getforwardray)
- [initControllerMesh](WindowsMotionController.md#initcontrollermesh)
- [onButtonStateChange](WindowsMotionController.md#onbuttonstatechange)
- [onleftstickchanged](WindowsMotionController.md#onleftstickchanged)
- [onrightstickchanged](WindowsMotionController.md#onrightstickchanged)
- [update](WindowsMotionController.md#update)
- [updateFromDevice](WindowsMotionController.md#updatefromdevice)

## Constructors

### constructor

• **new WindowsMotionController**(`vrGamepad`)

Creates a new WindowsMotionController from a gamepad

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vrGamepad` | `any` | the gamepad that the controller should be created from |

#### Overrides

[WebVRController](WebVRController.md).[constructor](WebVRController.md#constructor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:158

## Properties

### \_buttons

• `Protected` **\_buttons**: [`MutableGamepadButton`](../interfaces/MutableGamepadButton.md)[]

Array of button available on the controller

#### Inherited from

[WebVRController](WebVRController.md).[_buttons](WebVRController.md#_buttons)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:44

___

### \_calculatedPosition

• `Protected` **\_calculatedPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[WebVRController](WebVRController.md).[_calculatedPosition](WebVRController.md#_calculatedposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:167

___

### \_defaultModel

• `Protected` **\_defaultModel**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Internal, the default controller model for the controller

#### Inherited from

[WebVRController](WebVRController.md).[_defaultModel](WebVRController.md#_defaultmodel)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:17

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[WebVRController](WebVRController.md).[_invertLeftStickY](WebVRController.md#_invertleftsticky)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:100

___

### \_loadedMeshInfo

• `Private` **\_loadedMeshInfo**: [`Nullable`](../modules.md#nullable)`LoadedMeshInfo`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:109

___

### \_mapping

• `Protected` `Readonly` **\_mapping**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `axisMeshNames` | `string`[] |
| `buttonMeshNames` | { `grip`: `string` = "GRASP"; `menu`: `string` = "MENU"; `thumbstick`: `string` = "THUMBSTICK\_PRESS"; `trackpad`: `string` = "TOUCHPAD\_PRESS"; `trigger`: `string` = "SELECT" } |
| `buttonMeshNames.grip` | `string` |
| `buttonMeshNames.menu` | `string` |
| `buttonMeshNames.thumbstick` | `string` |
| `buttonMeshNames.trackpad` | `string` |
| `buttonMeshNames.trigger` | `string` |
| `buttonObservableNames` | { `grip`: `string` = "onMainButtonStateChangedObservable"; `menu`: `string` = "onSecondaryButtonStateChangedObservable"; `thumbstick`: `string` = "onPadStateChangedObservable"; `trackpad`: `string` = "onTrackpadChangedObservable"; `trigger`: `string` = "onTriggerStateChangedObservable" } |
| `buttonObservableNames.grip` | `string` |
| `buttonObservableNames.menu` | `string` |
| `buttonObservableNames.thumbstick` | `string` |
| `buttonObservableNames.trackpad` | `string` |
| `buttonObservableNames.trigger` | `string` |
| `buttons` | `string`[] |
| `pointingPoseMeshName` | `string` |

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:110

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[WebVRController](WebVRController.md).[browserGamepad](WebVRController.md#browsergamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:131

___

### controllerType

• **controllerType**: [`PoseEnabledControllerType`](../enums/PoseEnabledControllerType.md)

The type of controller (Eg. Windows mixed reality)

#### Inherited from

[WebVRController](WebVRController.md).[controllerType](WebVRController.md#controllertype)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:165

___

### devicePosition

• **devicePosition**: [`Vector3`](Vector3.md)

The device position in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[devicePosition](WebVRController.md#deviceposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:144

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](Quaternion.md)

The device rotation in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[deviceRotationQuaternion](WebVRController.md#devicerotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:148

___

### deviceScaleFactor

• **deviceScaleFactor**: `number` = `1`

The scale factor of the device in babylon space

#### Inherited from

[WebVRController](WebVRController.md).[deviceScaleFactor](WebVRController.md#devicescalefactor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:152

___

### hand

• **hand**: `string`

'left' or 'right', see https://w3c.github.io/gamepad/extensions.html#gamepadhand-enum

#### Inherited from

[WebVRController](WebVRController.md).[hand](WebVRController.md#hand)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:64

___

### id

• **id**: `string`

#### Inherited from

[WebVRController](WebVRController.md).[id](WebVRController.md#id)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[WebVRController](WebVRController.md).[index](WebVRController.md#index)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:127

___

### isXR

• **isXR**: `boolean` = `false`

If the controller is used in a webXR session

#### Inherited from

[WebVRController](WebVRController.md).[isXR](WebVRController.md#isxr)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:136

___

### onMainButtonStateChangedObservable

• **onMainButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the main button state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onMainButtonStateChangedObservable](WebVRController.md#onmainbuttonstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:27

___

### onPadStateChangedObservable

• **onPadStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the pad state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onPadStateChangedObservable](WebVRController.md#onpadstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:35

___

### onPadValuesChangedObservable

• **onPadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when controllers stick values have changed

#### Inherited from

[WebVRController](WebVRController.md).[onPadValuesChangedObservable](WebVRController.md#onpadvalueschangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:39

___

### onSecondaryButtonStateChangedObservable

• **onSecondaryButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the secondary button state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onSecondaryButtonStateChangedObservable](WebVRController.md#onsecondarybuttonstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:31

___

### onTrackpadChangedObservable

• **onTrackpadChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trackpad on this controller is clicked

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:144

___

### onTrackpadValuesChangedObservable

• **onTrackpadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when the trackpad on this controller is modified

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:148

___

### onTriggerStateChangedObservable

• **onTriggerStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger state has changed

#### Inherited from

[WebVRController](WebVRController.md).[onTriggerStateChangedObservable](WebVRController.md#ontriggerstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:23

___

### pad

• **pad**: [`StickValues`](StickValues.md)

X and Y axis corresponding to the controllers joystick

#### Inherited from

[WebVRController](WebVRController.md).[pad](WebVRController.md#pad)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:59

___

### position

• **position**: [`Vector3`](Vector3.md)

(Likely devicePosition should be used instead) The device position in its room space

#### Inherited from

[WebVRController](WebVRController.md).[position](WebVRController.md#position)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:157

___

### rawPose

• **rawPose**: [`DevicePose`](../interfaces/DevicePose.md)

The raw pose from the device

#### Inherited from

[WebVRController](WebVRController.md).[rawPose](WebVRController.md#rawpose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:173

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

(Likely deviceRotationQuaternion should be used instead) The device rotation in its room space

#### Inherited from

[WebVRController](WebVRController.md).[rotationQuaternion](WebVRController.md#rotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:161

___

### trackpad

• **trackpad**: [`StickValues`](StickValues.md)

The current x and y values of this controller's trackpad

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:152

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[WebVRController](WebVRController.md).[type](WebVRController.md#type)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[WebVRController](WebVRController.md).[DUALSHOCK](WebVRController.md#dualshock)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[WebVRController](WebVRController.md).[GAMEPAD](WebVRController.md#gamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:79

___

### GAMEPAD\_ID\_PATTERN

▪ `Static` `Private` `Readonly` **GAMEPAD\_ID\_PATTERN**: `RegExp`

The controller id pattern for this controller type

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:107

___

### GAMEPAD\_ID\_PREFIX

▪ `Static` `Readonly` **GAMEPAD\_ID\_PREFIX**: `string` = `"Spatial Controller (Spatial Interaction Source) "`

The controller name prefix for this controller type

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:102

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[WebVRController](WebVRController.md).[GENERIC](WebVRController.md#generic)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:83

___

### MODEL\_BASE\_URL

▪ `Static` **MODEL\_BASE\_URL**: `string` = `"https://controllers.babylonjs.com/microsoft/"`

The base url used to load the left and right controller models

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:89

___

### MODEL\_LEFT\_FILENAME

▪ `Static` **MODEL\_LEFT\_FILENAME**: `string` = `"left.glb"`

The name of the left controller model file

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:93

___

### MODEL\_RIGHT\_FILENAME

▪ `Static` **MODEL\_RIGHT\_FILENAME**: `string` = `"right.glb"`

The name of the right controller model file

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:97

___

### POINTING\_POSE

▪ `Static` `Readonly` **POINTING\_POSE**: ``"POINTING_POSE"``

Name of the child mesh that can be used to cast a ray from the controller

#### Inherited from

[WebVRController](WebVRController.md).[POINTING_POSE](WebVRController.md#pointing_pose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:213

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[WebVRController](WebVRController.md).[POSE_ENABLED](WebVRController.md#pose_enabled)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[WebVRController](WebVRController.md).[XBOX](WebVRController.md#xbox)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:87

## Accessors

### defaultModel

• `get` **defaultModel**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The default controller model for the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WebVRController.defaultModel

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:69

___

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

WebVRController.isConnected

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WebVRController.leftStick

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

WebVRController.leftStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:175

___

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is attached to the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WebVRController.mesh

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:396

___

### onGripButtonStateChangedObservable

• `get` **onGripButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the grip button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:181

___

### onMenuButtonStateChangedObservable

• `get` **onMenuButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the menu button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:174

___

### onThumbstickButtonStateChangedObservable

• `get` **onThumbstickButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the thumbstick button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:188

___

### onTouchpadButtonStateChangedObservable

• `get` **onTouchpadButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the touchpad button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:195

___

### onTouchpadValuesChangedObservable

• `get` **onTouchpadValuesChangedObservable**(): [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when the touchpad values on this controller are modified

#### Returns

[`Observable`](Observable.md)[`StickValues`](StickValues.md)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:202

___

### onTriggerButtonStateChangedObservable

• `get` **onTriggerButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:167

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WebVRController.rightStick

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

WebVRController.rightStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:190

## Methods

### \_createMeshInfo

▸ `Private` **_createMeshInfo**(`rootNode`): `LoadedMeshInfo`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rootNode` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`LoadedMeshInfo`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:406

___

### \_handleButtonChange

▸ `Protected` **_handleButtonChange**(`buttonIdx`, `state`): `void`

Called once for each button that changed state since the last frame

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

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:235

___

### \_lerpButtonTransform

▸ `Protected` **_lerpButtonTransform**(`buttonName`, `buttonValue`): `void`

Moves the buttons on the controller mesh based on their current state

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buttonName` | `string` | the name of the button to move |
| `buttonValue` | `number` | the value of the button which determines the buttons new position |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:258

___

### \_processModel

▸ `Private` **_processModel**(`scene`, `meshes`): [`Nullable`](../modules.md#nullable)`LoadedMeshInfo`

Takes a list of meshes (as loaded from the glTF file) and finds the root node, as well as nodes that
can be transformed by button presses and axes values, based on this._mapping.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | scene in which the meshes exist |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | list of meshes that make up the controller model to process |

#### Returns

[`Nullable`](../modules.md#nullable)`LoadedMeshInfo`

structured view of the given meshes, with mapping of buttons and axes to meshes that can be transformed.

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:373

___

### \_updatePoseAndMesh

▸ `Protected` **_updatePoseAndMesh**(): `void`

Updates only the pose device and mesh without doing any button event checking

#### Returns

`void`

#### Inherited from

[WebVRController](WebVRController.md).[_updatePoseAndMesh](WebVRController.md#_updateposeandmesh)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:242

___

### \_updateTrackpad

▸ `Protected` **_updateTrackpad**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:206

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

[WebVRController](WebVRController.md).[attachToPoseControlledCamera](WebVRController.md#attachtoposecontrolledcamera)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:374

___

### dispose

▸ **dispose**(): `void`

Disposes of the controller

#### Returns

`void`

#### Overrides

[WebVRController](WebVRController.md).[dispose](WebVRController.md#dispose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:535

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

#### Overrides

[WebVRController](WebVRController.md).[getForwardRay](WebVRController.md#getforwardray)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:516

___

### initControllerMesh

▸ **initControllerMesh**(`scene`, `meshLoaded?`, `forceDefault?`): `void`

Implements abstract method on WebVRController class, loading controller meshes and calling this.attachToMesh if successful.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | scene in which to add meshes |
| `meshLoaded?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | `undefined` | optional callback function that will be called if the mesh loads successfully. |
| `forceDefault` | `boolean` | `false` |  |

#### Returns

`void`

#### Overrides

[WebVRController](WebVRController.md).[initControllerMesh](WebVRController.md#initcontrollermesh)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:306

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

[WebVRController](WebVRController.md).[onleftstickchanged](WebVRController.md#onleftstickchanged)

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

[WebVRController](WebVRController.md).[onrightstickchanged](WebVRController.md#onrightstickchanged)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Called once per frame by the engine.

#### Returns

`void`

#### Overrides

[WebVRController](WebVRController.md).[update](WebVRController.md#update)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:217

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

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:296

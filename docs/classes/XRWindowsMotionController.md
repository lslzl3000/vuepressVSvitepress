[@dev/core](../README.md) / [Exports](../modules.md) / XRWindowsMotionController

# Class: XRWindowsMotionController

This class represents a new windows motion controller in XR.

## Hierarchy

- [`WindowsMotionController`](WindowsMotionController.md)

  ↳ **`XRWindowsMotionController`**

## Table of contents

### Constructors

- [constructor](XRWindowsMotionController.md#constructor)

### Properties

- [\_buttons](XRWindowsMotionController.md#_buttons)
- [\_calculatedPosition](XRWindowsMotionController.md#_calculatedposition)
- [\_defaultModel](XRWindowsMotionController.md#_defaultmodel)
- [\_invertLeftStickY](XRWindowsMotionController.md#_invertleftsticky)
- [\_mapping](XRWindowsMotionController.md#_mapping)
- [browserGamepad](XRWindowsMotionController.md#browsergamepad)
- [controllerType](XRWindowsMotionController.md#controllertype)
- [devicePosition](XRWindowsMotionController.md#deviceposition)
- [deviceRotationQuaternion](XRWindowsMotionController.md#devicerotationquaternion)
- [deviceScaleFactor](XRWindowsMotionController.md#devicescalefactor)
- [hand](XRWindowsMotionController.md#hand)
- [id](XRWindowsMotionController.md#id)
- [index](XRWindowsMotionController.md#index)
- [isXR](XRWindowsMotionController.md#isxr)
- [onMainButtonStateChangedObservable](XRWindowsMotionController.md#onmainbuttonstatechangedobservable)
- [onPadStateChangedObservable](XRWindowsMotionController.md#onpadstatechangedobservable)
- [onPadValuesChangedObservable](XRWindowsMotionController.md#onpadvalueschangedobservable)
- [onSecondaryButtonStateChangedObservable](XRWindowsMotionController.md#onsecondarybuttonstatechangedobservable)
- [onThumbstickStateChangedObservable](XRWindowsMotionController.md#onthumbstickstatechangedobservable)
- [onThumbstickValuesChangedObservable](XRWindowsMotionController.md#onthumbstickvalueschangedobservable)
- [onTrackpadChangedObservable](XRWindowsMotionController.md#ontrackpadchangedobservable)
- [onTrackpadValuesChangedObservable](XRWindowsMotionController.md#ontrackpadvalueschangedobservable)
- [onTriggerStateChangedObservable](XRWindowsMotionController.md#ontriggerstatechangedobservable)
- [pad](XRWindowsMotionController.md#pad)
- [position](XRWindowsMotionController.md#position)
- [rawPose](XRWindowsMotionController.md#rawpose)
- [rotationQuaternion](XRWindowsMotionController.md#rotationquaternion)
- [thumbstickValues](XRWindowsMotionController.md#thumbstickvalues)
- [trackpad](XRWindowsMotionController.md#trackpad)
- [type](XRWindowsMotionController.md#type)
- [DUALSHOCK](XRWindowsMotionController.md#dualshock)
- [GAMEPAD](XRWindowsMotionController.md#gamepad)
- [GAMEPAD\_ID\_PREFIX](XRWindowsMotionController.md#gamepad_id_prefix)
- [GENERIC](XRWindowsMotionController.md#generic)
- [MODEL\_BASE\_URL](XRWindowsMotionController.md#model_base_url)
- [MODEL\_LEFT\_FILENAME](XRWindowsMotionController.md#model_left_filename)
- [MODEL\_RIGHT\_FILENAME](XRWindowsMotionController.md#model_right_filename)
- [POINTING\_POSE](XRWindowsMotionController.md#pointing_pose)
- [POSE\_ENABLED](XRWindowsMotionController.md#pose_enabled)
- [XBOX](XRWindowsMotionController.md#xbox)

### Accessors

- [defaultModel](XRWindowsMotionController.md#defaultmodel)
- [isConnected](XRWindowsMotionController.md#isconnected)
- [leftStick](XRWindowsMotionController.md#leftstick)
- [mesh](XRWindowsMotionController.md#mesh)
- [onGripButtonStateChangedObservable](XRWindowsMotionController.md#ongripbuttonstatechangedobservable)
- [onMenuButtonStateChangedObservable](XRWindowsMotionController.md#onmenubuttonstatechangedobservable)
- [onThumbstickButtonStateChangedObservable](XRWindowsMotionController.md#onthumbstickbuttonstatechangedobservable)
- [onTouchpadButtonStateChangedObservable](XRWindowsMotionController.md#ontouchpadbuttonstatechangedobservable)
- [onTouchpadValuesChangedObservable](XRWindowsMotionController.md#ontouchpadvalueschangedobservable)
- [onTriggerButtonStateChangedObservable](XRWindowsMotionController.md#ontriggerbuttonstatechangedobservable)
- [rightStick](XRWindowsMotionController.md#rightstick)

### Methods

- [\_handleButtonChange](XRWindowsMotionController.md#_handlebuttonchange)
- [\_lerpButtonTransform](XRWindowsMotionController.md#_lerpbuttontransform)
- [\_updatePoseAndMesh](XRWindowsMotionController.md#_updateposeandmesh)
- [\_updateTrackpad](XRWindowsMotionController.md#_updatetrackpad)
- [attachToMesh](XRWindowsMotionController.md#attachtomesh)
- [attachToPoseControlledCamera](XRWindowsMotionController.md#attachtoposecontrolledcamera)
- [dispose](XRWindowsMotionController.md#dispose)
- [getForwardRay](XRWindowsMotionController.md#getforwardray)
- [initControllerMesh](XRWindowsMotionController.md#initcontrollermesh)
- [onButtonStateChange](XRWindowsMotionController.md#onbuttonstatechange)
- [onleftstickchanged](XRWindowsMotionController.md#onleftstickchanged)
- [onrightstickchanged](XRWindowsMotionController.md#onrightstickchanged)
- [update](XRWindowsMotionController.md#update)
- [updateFromDevice](XRWindowsMotionController.md#updatefromdevice)

## Constructors

### constructor

• **new XRWindowsMotionController**(`gamepadInfo`)

Construct a new XR-Based windows motion controller

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gamepadInfo` | `any` | the gamepad object from the browser |

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[constructor](WindowsMotionController.md#constructor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:586

## Properties

### \_buttons

• `Protected` **\_buttons**: [`MutableGamepadButton`](../interfaces/MutableGamepadButton.md)[]

Array of button available on the controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_buttons](WindowsMotionController.md#_buttons)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:44

___

### \_calculatedPosition

• `Protected` **\_calculatedPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_calculatedPosition](WindowsMotionController.md#_calculatedposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:167

___

### \_defaultModel

• `Protected` **\_defaultModel**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Internal, the default controller model for the controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_defaultModel](WindowsMotionController.md#_defaultmodel)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:17

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_invertLeftStickY](WindowsMotionController.md#_invertleftsticky)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:100

___

### \_mapping

• `Protected` `Readonly` **\_mapping**: `Object`

Changing the original WIndowsMotionController mapping to fir the new mapping

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
| `buttonObservableNames` | { `grip`: `string` = "onMainButtonStateChangedObservable"; `menu`: `string` = "onSecondaryButtonStateChangedObservable"; `thumbstick`: `string` = "onThumbstickStateChangedObservable"; `trackpad`: `string` = "onTrackpadChangedObservable"; `trigger`: `string` = "onTriggerStateChangedObservable" } |
| `buttonObservableNames.grip` | `string` |
| `buttonObservableNames.menu` | `string` |
| `buttonObservableNames.thumbstick` | `string` |
| `buttonObservableNames.trackpad` | `string` |
| `buttonObservableNames.trigger` | `string` |
| `buttons` | `string`[] |
| `pointingPoseMeshName` | `string` |

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[_mapping](WindowsMotionController.md#_mapping)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:550

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[browserGamepad](WindowsMotionController.md#browsergamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:131

___

### controllerType

• **controllerType**: [`PoseEnabledControllerType`](../enums/PoseEnabledControllerType.md)

The type of controller (Eg. Windows mixed reality)

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[controllerType](WindowsMotionController.md#controllertype)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:165

___

### devicePosition

• **devicePosition**: [`Vector3`](Vector3.md)

The device position in babylon space

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[devicePosition](WindowsMotionController.md#deviceposition)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:144

___

### deviceRotationQuaternion

• **deviceRotationQuaternion**: [`Quaternion`](Quaternion.md)

The device rotation in babylon space

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[deviceRotationQuaternion](WindowsMotionController.md#devicerotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:148

___

### deviceScaleFactor

• **deviceScaleFactor**: `number` = `1`

The scale factor of the device in babylon space

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[deviceScaleFactor](WindowsMotionController.md#devicescalefactor)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:152

___

### hand

• **hand**: `string`

'left' or 'right', see https://w3c.github.io/gamepad/extensions.html#gamepadhand-enum

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[hand](WindowsMotionController.md#hand)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:64

___

### id

• **id**: `string`

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[id](WindowsMotionController.md#id)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[index](WindowsMotionController.md#index)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:127

___

### isXR

• **isXR**: `boolean` = `false`

If the controller is used in a webXR session

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[isXR](WindowsMotionController.md#isxr)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:136

___

### onMainButtonStateChangedObservable

• **onMainButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the main button state has changed

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[onMainButtonStateChangedObservable](WindowsMotionController.md#onmainbuttonstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:27

___

### onPadStateChangedObservable

• **onPadStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the pad state has changed

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[onPadStateChangedObservable](WindowsMotionController.md#onpadstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:35

___

### onPadValuesChangedObservable

• **onPadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when controllers stick values have changed

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[onPadValuesChangedObservable](WindowsMotionController.md#onpadvalueschangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:39

___

### onSecondaryButtonStateChangedObservable

• **onSecondaryButtonStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the secondary button state has changed

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[onSecondaryButtonStateChangedObservable](WindowsMotionController.md#onsecondarybuttonstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:31

___

### onThumbstickStateChangedObservable

• **onThumbstickStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the thumbstick on this controller is clicked

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:598

___

### onThumbstickValuesChangedObservable

• **onThumbstickValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when the thumbstick on this controller is modified

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:602

___

### onTrackpadChangedObservable

• **onTrackpadChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the touchpad button on this controller is modified

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[onTrackpadChangedObservable](WindowsMotionController.md#ontrackpadchangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:607

___

### onTrackpadValuesChangedObservable

• **onTrackpadValuesChangedObservable**: [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when the touchpad values on this controller are modified

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[onTrackpadValuesChangedObservable](WindowsMotionController.md#ontrackpadvalueschangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:612

___

### onTriggerStateChangedObservable

• **onTriggerStateChangedObservable**: [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger state has changed

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[onTriggerStateChangedObservable](WindowsMotionController.md#ontriggerstatechangedobservable)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:23

___

### pad

• **pad**: [`StickValues`](StickValues.md)

X and Y axis corresponding to the controllers joystick

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[pad](WindowsMotionController.md#pad)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:59

___

### position

• **position**: [`Vector3`](Vector3.md)

(Likely devicePosition should be used instead) The device position in its room space

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[position](WindowsMotionController.md#position)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:157

___

### rawPose

• **rawPose**: [`DevicePose`](../interfaces/DevicePose.md)

The raw pose from the device

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[rawPose](WindowsMotionController.md#rawpose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:173

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

(Likely deviceRotationQuaternion should be used instead) The device rotation in its room space

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[rotationQuaternion](WindowsMotionController.md#rotationquaternion)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:161

___

### thumbstickValues

• **thumbstickValues**: [`StickValues`](StickValues.md)

holds the thumbstick values (X,Y)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:593

___

### trackpad

• **trackpad**: [`StickValues`](StickValues.md)

The current x and y values of this controller's trackpad

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[trackpad](WindowsMotionController.md#trackpad)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:152

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[type](WindowsMotionController.md#type)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[DUALSHOCK](WindowsMotionController.md#dualshock)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[GAMEPAD](WindowsMotionController.md#gamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:79

___

### GAMEPAD\_ID\_PREFIX

▪ `Static` `Readonly` **GAMEPAD\_ID\_PREFIX**: `string` = `"Spatial Controller (Spatial Interaction Source) "`

The controller name prefix for this controller type

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[GAMEPAD_ID_PREFIX](WindowsMotionController.md#gamepad_id_prefix)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:102

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[GENERIC](WindowsMotionController.md#generic)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:83

___

### MODEL\_BASE\_URL

▪ `Static` **MODEL\_BASE\_URL**: `string` = `"https://controllers.babylonjs.com/microsoft/"`

The base url used to load the left and right controller models

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[MODEL_BASE_URL](WindowsMotionController.md#model_base_url)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:89

___

### MODEL\_LEFT\_FILENAME

▪ `Static` **MODEL\_LEFT\_FILENAME**: `string` = `"left.glb"`

The name of the left controller model file

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[MODEL_LEFT_FILENAME](WindowsMotionController.md#model_left_filename)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:93

___

### MODEL\_RIGHT\_FILENAME

▪ `Static` **MODEL\_RIGHT\_FILENAME**: `string` = `"right.glb"`

The name of the right controller model file

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[MODEL_RIGHT_FILENAME](WindowsMotionController.md#model_right_filename)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:97

___

### POINTING\_POSE

▪ `Static` `Readonly` **POINTING\_POSE**: ``"POINTING_POSE"``

Name of the child mesh that can be used to cast a ray from the controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[POINTING_POSE](WindowsMotionController.md#pointing_pose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:213

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[POSE_ENABLED](WindowsMotionController.md#pose_enabled)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[XBOX](WindowsMotionController.md#xbox)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:87

## Accessors

### defaultModel

• `get` **defaultModel**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The default controller model for the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WindowsMotionController.defaultModel

#### Defined in

packages/dev/core/src/Gamepads/Controllers/webVRController.ts:69

___

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

WindowsMotionController.isConnected

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WindowsMotionController.leftStick

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

WindowsMotionController.leftStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:175

___

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is attached to the controller

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

WindowsMotionController.mesh

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:396

___

### onGripButtonStateChangedObservable

• `get` **onGripButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the grip button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Inherited from

WindowsMotionController.onGripButtonStateChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:181

___

### onMenuButtonStateChangedObservable

• `get` **onMenuButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the menu button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Inherited from

WindowsMotionController.onMenuButtonStateChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:174

___

### onThumbstickButtonStateChangedObservable

• `get` **onThumbstickButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the thumbstick button on this controller is modified
here to prevent breaking changes

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Overrides

WindowsMotionController.onThumbstickButtonStateChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:618

___

### onTouchpadButtonStateChangedObservable

• `get` **onTouchpadButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the touchpad button on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Inherited from

WindowsMotionController.onTouchpadButtonStateChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:195

___

### onTouchpadValuesChangedObservable

• `get` **onTouchpadValuesChangedObservable**(): [`Observable`](Observable.md)[`StickValues`](StickValues.md)

Fired when the touchpad values on this controller are modified

#### Returns

[`Observable`](Observable.md)[`StickValues`](StickValues.md)

#### Inherited from

WindowsMotionController.onTouchpadValuesChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:202

___

### onTriggerButtonStateChangedObservable

• `get` **onTriggerButtonStateChangedObservable**(): [`Observable`](Observable.md)`ExtendedGamepadButton`

Fired when the trigger on this controller is modified

#### Returns

[`Observable`](Observable.md)`ExtendedGamepadButton`

#### Inherited from

WindowsMotionController.onTriggerButtonStateChangedObservable

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:167

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

WindowsMotionController.rightStick

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

WindowsMotionController.rightStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:190

## Methods

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

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_handleButtonChange](WindowsMotionController.md#_handlebuttonchange)

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

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_lerpButtonTransform](WindowsMotionController.md#_lerpbuttontransform)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:258

___

### \_updatePoseAndMesh

▸ `Protected` **_updatePoseAndMesh**(): `void`

Updates only the pose device and mesh without doing any button event checking

#### Returns

`void`

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[_updatePoseAndMesh](WindowsMotionController.md#_updateposeandmesh)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:242

___

### \_updateTrackpad

▸ `Protected` **_updateTrackpad**(): `void`

updating the thumbstick(!) and not the trackpad.
This is named this way due to the difference between WebVR and XR and to avoid
changing the parent class.

#### Returns

`void`

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[_updateTrackpad](WindowsMotionController.md#_updatetrackpad)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:627

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

[WindowsMotionController](WindowsMotionController.md).[attachToMesh](WindowsMotionController.md#attachtomesh)

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

[WindowsMotionController](WindowsMotionController.md).[attachToPoseControlledCamera](WindowsMotionController.md#attachtoposecontrolledcamera)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:374

___

### dispose

▸ **dispose**(): `void`

Disposes the class with joy

#### Returns

`void`

#### Overrides

[WindowsMotionController](WindowsMotionController.md).[dispose](WindowsMotionController.md#dispose)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/windowsMotionController.ts:638

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

[WindowsMotionController](WindowsMotionController.md).[getForwardRay](WindowsMotionController.md#getforwardray)

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

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[initControllerMesh](WindowsMotionController.md#initcontrollermesh)

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

[WindowsMotionController](WindowsMotionController.md).[onButtonStateChange](WindowsMotionController.md#onbuttonstatechange)

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

[WindowsMotionController](WindowsMotionController.md).[onleftstickchanged](WindowsMotionController.md#onleftstickchanged)

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

[WindowsMotionController](WindowsMotionController.md).[onrightstickchanged](WindowsMotionController.md#onrightstickchanged)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Called once per frame by the engine.

#### Returns

`void`

#### Inherited from

[WindowsMotionController](WindowsMotionController.md).[update](WindowsMotionController.md#update)

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

[WindowsMotionController](WindowsMotionController.md).[updateFromDevice](WindowsMotionController.md#updatefromdevice)

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:296

[@dev/core](../README.md) / [Exports](../modules.md) / FollowCameraKeyboardMoveInput

# Class: FollowCameraKeyboardMoveInput

Manage the keyboard inputs to control the movement of a follow camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FollowCamera`](FollowCamera.md)

## Table of contents

### Constructors

- [constructor](FollowCameraKeyboardMoveInput.md#constructor)

### Properties

- [\_altPressed](FollowCameraKeyboardMoveInput.md#_altpressed)
- [\_ctrlPressed](FollowCameraKeyboardMoveInput.md#_ctrlpressed)
- [\_engine](FollowCameraKeyboardMoveInput.md#_engine)
- [\_keys](FollowCameraKeyboardMoveInput.md#_keys)
- [\_onCanvasBlurObserver](FollowCameraKeyboardMoveInput.md#_oncanvasblurobserver)
- [\_onKeyboardObserver](FollowCameraKeyboardMoveInput.md#_onkeyboardobserver)
- [\_scene](FollowCameraKeyboardMoveInput.md#_scene)
- [\_shiftPressed](FollowCameraKeyboardMoveInput.md#_shiftpressed)
- [camera](FollowCameraKeyboardMoveInput.md#camera)
- [heightSensibility](FollowCameraKeyboardMoveInput.md#heightsensibility)
- [keysHeightOffsetDecr](FollowCameraKeyboardMoveInput.md#keysheightoffsetdecr)
- [keysHeightOffsetIncr](FollowCameraKeyboardMoveInput.md#keysheightoffsetincr)
- [keysHeightOffsetModifierAlt](FollowCameraKeyboardMoveInput.md#keysheightoffsetmodifieralt)
- [keysHeightOffsetModifierCtrl](FollowCameraKeyboardMoveInput.md#keysheightoffsetmodifierctrl)
- [keysHeightOffsetModifierShift](FollowCameraKeyboardMoveInput.md#keysheightoffsetmodifiershift)
- [keysRadiusDecr](FollowCameraKeyboardMoveInput.md#keysradiusdecr)
- [keysRadiusIncr](FollowCameraKeyboardMoveInput.md#keysradiusincr)
- [keysRadiusModifierAlt](FollowCameraKeyboardMoveInput.md#keysradiusmodifieralt)
- [keysRadiusModifierCtrl](FollowCameraKeyboardMoveInput.md#keysradiusmodifierctrl)
- [keysRadiusModifierShift](FollowCameraKeyboardMoveInput.md#keysradiusmodifiershift)
- [keysRotationOffsetDecr](FollowCameraKeyboardMoveInput.md#keysrotationoffsetdecr)
- [keysRotationOffsetIncr](FollowCameraKeyboardMoveInput.md#keysrotationoffsetincr)
- [keysRotationOffsetModifierAlt](FollowCameraKeyboardMoveInput.md#keysrotationoffsetmodifieralt)
- [keysRotationOffsetModifierCtrl](FollowCameraKeyboardMoveInput.md#keysrotationoffsetmodifierctrl)
- [keysRotationOffsetModifierShift](FollowCameraKeyboardMoveInput.md#keysrotationoffsetmodifiershift)
- [radiusSensibility](FollowCameraKeyboardMoveInput.md#radiussensibility)
- [rotationSensibility](FollowCameraKeyboardMoveInput.md#rotationsensibility)

### Methods

- [\_modifierHeightOffset](FollowCameraKeyboardMoveInput.md#_modifierheightoffset)
- [\_modifierRadius](FollowCameraKeyboardMoveInput.md#_modifierradius)
- [\_modifierRotationOffset](FollowCameraKeyboardMoveInput.md#_modifierrotationoffset)
- [attachControl](FollowCameraKeyboardMoveInput.md#attachcontrol)
- [checkInputs](FollowCameraKeyboardMoveInput.md#checkinputs)
- [detachControl](FollowCameraKeyboardMoveInput.md#detachcontrol)
- [getClassName](FollowCameraKeyboardMoveInput.md#getclassname)
- [getSimpleName](FollowCameraKeyboardMoveInput.md#getsimplename)

## Constructors

### constructor

• **new FollowCameraKeyboardMoveInput**()

## Properties

### \_altPressed

• `Private` **\_altPressed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:133

___

### \_ctrlPressed

• `Private` **\_ctrlPressed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:132

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:137

___

### \_keys

• `Private` **\_keys**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:131

___

### \_onCanvasBlurObserver

• `Private` **\_onCanvasBlurObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:135

___

### \_onKeyboardObserver

• `Private` **\_onKeyboardObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`KeyboardInfo`](KeyboardInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:136

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:138

___

### \_shiftPressed

• `Private` **\_shiftPressed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:134

___

### camera

• **camera**: [`FollowCamera`](FollowCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:21

___

### heightSensibility

• **heightSensibility**: `number` = `1`

Defines the rate of change of heightOffset.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:117

___

### keysHeightOffsetDecr

• **keysHeightOffsetDecr**: `number`[]

Defines the list of key codes associated with the down action (decrease heightOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:33

___

### keysHeightOffsetIncr

• **keysHeightOffsetIncr**: `number`[]

Defines the list of key codes associated with the up action (increase heightOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:27

___

### keysHeightOffsetModifierAlt

• **keysHeightOffsetModifierAlt**: `boolean` = `false`

Defines whether the Alt modifier key is required to move up/down (alter heightOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:39

___

### keysHeightOffsetModifierCtrl

• **keysHeightOffsetModifierCtrl**: `boolean` = `false`

Defines whether the Ctrl modifier key is required to move up/down (alter heightOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:45

___

### keysHeightOffsetModifierShift

• **keysHeightOffsetModifierShift**: `boolean` = `false`

Defines whether the Shift modifier key is required to move up/down (alter heightOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:51

___

### keysRadiusDecr

• **keysRadiusDecr**: `number`[]

Defines the list of key codes associated with the zoom-out action (increase radius)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:93

___

### keysRadiusIncr

• **keysRadiusIncr**: `number`[]

Defines the list of key codes associated with the zoom-in action (decrease radius)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:87

___

### keysRadiusModifierAlt

• **keysRadiusModifierAlt**: `boolean` = `true`

Defines whether the Alt modifier key is required to zoom in/out (alter radius value)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:99

___

### keysRadiusModifierCtrl

• **keysRadiusModifierCtrl**: `boolean` = `false`

Defines whether the Ctrl modifier key is required to zoom in/out (alter radius value)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:105

___

### keysRadiusModifierShift

• **keysRadiusModifierShift**: `boolean` = `false`

Defines whether the Shift modifier key is required to zoom in/out (alter radius value)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:111

___

### keysRotationOffsetDecr

• **keysRotationOffsetDecr**: `number`[]

Defines the list of key codes associated with the right action (decrease rotationOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:63

___

### keysRotationOffsetIncr

• **keysRotationOffsetIncr**: `number`[]

Defines the list of key codes associated with the left action (increase rotationOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:57

___

### keysRotationOffsetModifierAlt

• **keysRotationOffsetModifierAlt**: `boolean` = `false`

Defines whether the Alt modifier key is required to move left/right (alter rotationOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:69

___

### keysRotationOffsetModifierCtrl

• **keysRotationOffsetModifierCtrl**: `boolean` = `false`

Defines whether the Ctrl modifier key is required to move left/right (alter rotationOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:75

___

### keysRotationOffsetModifierShift

• **keysRotationOffsetModifierShift**: `boolean` = `false`

Defines whether the Shift modifier key is required to move left/right (alter rotationOffset)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:81

___

### radiusSensibility

• **radiusSensibility**: `number` = `1`

Defines the rate of change of radius.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:129

___

### rotationSensibility

• **rotationSensibility**: `number` = `1`

Defines the rate of change of rotationOffset.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:123

## Methods

### \_modifierHeightOffset

▸ `Private` **_modifierHeightOffset**(): `boolean`

Check if the pressed modifier keys (Alt/Ctrl/Shift) match those configured to
allow modification of the heightOffset value.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:276

___

### \_modifierRadius

▸ `Private` **_modifierRadius**(): `boolean`

Check if the pressed modifier keys (Alt/Ctrl/Shift) match those configured to
allow modification of the radius value.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:300

___

### \_modifierRotationOffset

▸ `Private` **_modifierRotationOffset**(): `boolean`

Check if the pressed modifier keys (Alt/Ctrl/Shift) match those configured to
allow modification of the rotationOffset value.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:288

___

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:144

___

### checkInputs

▸ **checkInputs**(): `void`

Update the current camera state depending on the inputs that have been used this frame.
This is a dynamically created lambda to avoid the performance penalty of looping for inputs in the render loop.

#### Returns

`void`

#### Implementation of

ICameraInput.checkInputs

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:234

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:215

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getClassName](../interfaces/ICameraInput.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:260

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getSimpleName](../interfaces/ICameraInput.md#getsimplename)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraKeyboardMoveInput.ts:268

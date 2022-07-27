[@dev/core](../README.md) / [Exports](../modules.md) / FollowCameraPointersInput

# Class: FollowCameraPointersInput

Manage the pointers inputs to control an follow camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`BaseCameraPointersInput`](BaseCameraPointersInput.md)

  ↳ **`FollowCameraPointersInput`**

## Table of contents

### Constructors

- [constructor](FollowCameraPointersInput.md#constructor)

### Properties

- [\_altKey](FollowCameraPointersInput.md#_altkey)
- [\_buttonsPressed](FollowCameraPointersInput.md#_buttonspressed)
- [\_ctrlKey](FollowCameraPointersInput.md#_ctrlkey)
- [\_metaKey](FollowCameraPointersInput.md#_metakey)
- [\_shiftKey](FollowCameraPointersInput.md#_shiftkey)
- [\_warningCounter](FollowCameraPointersInput.md#_warningcounter)
- [angularSensibilityX](FollowCameraPointersInput.md#angularsensibilityx)
- [angularSensibilityY](FollowCameraPointersInput.md#angularsensibilityy)
- [axisPinchControlHeight](FollowCameraPointersInput.md#axispinchcontrolheight)
- [axisPinchControlRadius](FollowCameraPointersInput.md#axispinchcontrolradius)
- [axisPinchControlRotation](FollowCameraPointersInput.md#axispinchcontrolrotation)
- [axisXControlHeight](FollowCameraPointersInput.md#axisxcontrolheight)
- [axisXControlRadius](FollowCameraPointersInput.md#axisxcontrolradius)
- [axisXControlRotation](FollowCameraPointersInput.md#axisxcontrolrotation)
- [axisYControlHeight](FollowCameraPointersInput.md#axisycontrolheight)
- [axisYControlRadius](FollowCameraPointersInput.md#axisycontrolradius)
- [axisYControlRotation](FollowCameraPointersInput.md#axisycontrolrotation)
- [buttons](FollowCameraPointersInput.md#buttons)
- [camera](FollowCameraPointersInput.md#camera)
- [pinchDeltaPercentage](FollowCameraPointersInput.md#pinchdeltapercentage)
- [pinchPrecision](FollowCameraPointersInput.md#pinchprecision)
- [warningEnable](FollowCameraPointersInput.md#warningenable)

### Methods

- [\_warning](FollowCameraPointersInput.md#_warning)
- [attachControl](FollowCameraPointersInput.md#attachcontrol)
- [detachControl](FollowCameraPointersInput.md#detachcontrol)
- [getClassName](FollowCameraPointersInput.md#getclassname)
- [getSimpleName](FollowCameraPointersInput.md#getsimplename)
- [onButtonDown](FollowCameraPointersInput.md#onbuttondown)
- [onButtonUp](FollowCameraPointersInput.md#onbuttonup)
- [onContextMenu](FollowCameraPointersInput.md#oncontextmenu)
- [onDoubleTap](FollowCameraPointersInput.md#ondoubletap)
- [onLostFocus](FollowCameraPointersInput.md#onlostfocus)
- [onMultiTouch](FollowCameraPointersInput.md#onmultitouch)
- [onTouch](FollowCameraPointersInput.md#ontouch)

## Constructors

### constructor

• **new FollowCameraPointersInput**()

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[constructor](BaseCameraPointersInput.md#constructor)

## Properties

### \_altKey

• `Protected` **\_altKey**: `boolean`

Whether keyboard modifier keys are pressed at time of last mouse event.

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_altKey](BaseCameraPointersInput.md#_altkey)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:26

___

### \_buttonsPressed

• `Protected` **\_buttonsPressed**: `number`

Which mouse buttons were pressed at time of last mouse event.
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/buttons

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_buttonsPressed](BaseCameraPointersInput.md#_buttonspressed)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:35

___

### \_ctrlKey

• `Protected` **\_ctrlKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_ctrlKey](BaseCameraPointersInput.md#_ctrlkey)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:27

___

### \_metaKey

• `Protected` **\_metaKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_metaKey](BaseCameraPointersInput.md#_metakey)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:28

___

### \_shiftKey

• `Protected` **\_shiftKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_shiftKey](BaseCameraPointersInput.md#_shiftkey)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:29

___

### \_warningCounter

• `Private` **\_warningCounter**: `number` = `0`

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:186

___

### angularSensibilityX

• **angularSensibilityX**: `number` = `1`

Defines the pointer angular sensibility along the X axis or how fast is
the camera rotating.
A negative number will reverse the axis direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:32

___

### angularSensibilityY

• **angularSensibilityY**: `number` = `1`

Defines the pointer angular sensibility along the Y axis or how fast is
the camera rotating.
A negative number will reverse the axis direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:40

___

### axisPinchControlHeight

• **axisPinchControlHeight**: `boolean` = `false`

Pinch controls height. (Pinch modifies camera.heightOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:104

___

### axisPinchControlRadius

• **axisPinchControlRadius**: `boolean` = `true`

Pinch controls zoom. (Pinch modifies camera.radius value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:98

___

### axisPinchControlRotation

• **axisPinchControlRotation**: `boolean` = `false`

Pinch controls angle. (Pinch modifies camera.rotationOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:110

___

### axisXControlHeight

• **axisXControlHeight**: `boolean` = `false`

Pointer X axis controls height. (X axis modifies camera.heightOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:68

___

### axisXControlRadius

• **axisXControlRadius**: `boolean` = `false`

Pointer X axis controls zoom. (X axis modifies camera.radius value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:62

___

### axisXControlRotation

• **axisXControlRotation**: `boolean` = `true`

Pointer X axis controls angle. (X axis modifies camera.rotationOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:74

___

### axisYControlHeight

• **axisYControlHeight**: `boolean` = `true`

Pointer Y axis controls height. (Y axis modifies camera.heightOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:86

___

### axisYControlRadius

• **axisYControlRadius**: `boolean` = `false`

Pointer Y axis controls zoom. (Y axis modifies camera.radius value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:80

___

### axisYControlRotation

• **axisYControlRotation**: `boolean` = `false`

Pointer Y axis controls angle. (Y axis modifies camera.rotationOffset value.)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:92

___

### buttons

• **buttons**: `number`[]

Defines the buttons associated with the input to handle camera move.

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[buttons](BaseCameraPointersInput.md#buttons)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:44

___

### camera

• **camera**: [`FollowCamera`](FollowCamera.md)

Defines the camera the input is attached to.

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[camera](BaseCameraPointersInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:16

___

### pinchDeltaPercentage

• **pinchDeltaPercentage**: `number` = `0`

pinchDeltaPercentage will be used instead of pinchPrecision if different
from 0.
It defines the percentage of current camera.radius to use as delta when
pinch zoom is used.

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:56

___

### pinchPrecision

• **pinchPrecision**: `number` = `10000.0`

Defines the pointer pinch precision or how fast is the camera zooming.
A negative number will reverse the axis direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:47

___

### warningEnable

• **warningEnable**: `boolean` = `true`

Log error messages if basic misconfiguration has occurred.

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:115

## Methods

### \_warning

▸ `Private` **_warning**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:187

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

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[attachControl](BaseCameraPointersInput.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:50

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[detachControl](BaseCameraPointersInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:245

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[getClassName](BaseCameraPointersInput.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:22

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[getSimpleName](BaseCameraPointersInput.md#getsimplename)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:285

___

### onButtonDown

▸ **onButtonDown**(`evt`): `void`

Called each time a new POINTERDOWN event occurs. Ie, for each button
press.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onButtonDown](BaseCameraPointersInput.md#onbuttondown)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:343

___

### onButtonUp

▸ **onButtonUp**(`evt`): `void`

Called each time a new POINTERUP event occurs. Ie, for each button
release.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onButtonUp](BaseCameraPointersInput.md#onbuttonup)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:352

___

### onContextMenu

▸ **onContextMenu**(`evt`): `void`

Called on JS contextmenu event.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `PointerEvent` |

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onContextMenu](BaseCameraPointersInput.md#oncontextmenu)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:332

___

### onDoubleTap

▸ **onDoubleTap**(`type`): `void`

Called on pointer POINTERDOUBLETAP event.
Override this method to provide functionality on POINTERDOUBLETAP event.

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | `string` |

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onDoubleTap](BaseCameraPointersInput.md#ondoubletap)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:295

___

### onLostFocus

▸ **onLostFocus**(): `void`

Called when window becomes inactive.
Override this method to provide functionality.

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onLostFocus](BaseCameraPointersInput.md#onlostfocus)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:358

___

### onMultiTouch

▸ **onMultiTouch**(`pointA`, `pointB`, `previousPinchSquaredDistance`, `pinchSquaredDistance`, `previousMultiTouchPanPosition`, `multiTouchPanPosition`): `void`

Called on pointer POINTERMOVE event if multiple touches are active.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointA` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `pointB` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `previousPinchSquaredDistance` | `number` |
| `pinchSquaredDistance` | `number` |
| `previousMultiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `multiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onMultiTouch](BaseCameraPointersInput.md#onmultitouch)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:139

___

### onTouch

▸ **onTouch**(`pointA`, `offsetX`, `offsetY`): `void`

Called on pointer POINTERMOVE event if only a single touch is active.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointA` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `offsetX` | `number` |
| `offsetY` | `number` |

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onTouch](BaseCameraPointersInput.md#ontouch)

#### Defined in

packages/dev/core/src/Cameras/Inputs/followCameraPointersInput.ts:117

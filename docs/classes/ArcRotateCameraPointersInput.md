[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraPointersInput

# Class: ArcRotateCameraPointersInput

Manage the pointers inputs to control an arc rotate camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`BaseCameraPointersInput`](BaseCameraPointersInput.md)

  ↳ **`ArcRotateCameraPointersInput`**

## Table of contents

### Constructors

- [constructor](ArcRotateCameraPointersInput.md#constructor)

### Properties

- [\_altKey](ArcRotateCameraPointersInput.md#_altkey)
- [\_buttonsPressed](ArcRotateCameraPointersInput.md#_buttonspressed)
- [\_ctrlKey](ArcRotateCameraPointersInput.md#_ctrlkey)
- [\_isPanClick](ArcRotateCameraPointersInput.md#_ispanclick)
- [\_isPinching](ArcRotateCameraPointersInput.md#_ispinching)
- [\_metaKey](ArcRotateCameraPointersInput.md#_metakey)
- [\_shiftKey](ArcRotateCameraPointersInput.md#_shiftkey)
- [\_twoFingerActivityCount](ArcRotateCameraPointersInput.md#_twofingeractivitycount)
- [angularSensibilityX](ArcRotateCameraPointersInput.md#angularsensibilityx)
- [angularSensibilityY](ArcRotateCameraPointersInput.md#angularsensibilityy)
- [buttons](ArcRotateCameraPointersInput.md#buttons)
- [camera](ArcRotateCameraPointersInput.md#camera)
- [multiTouchPanAndZoom](ArcRotateCameraPointersInput.md#multitouchpanandzoom)
- [multiTouchPanning](ArcRotateCameraPointersInput.md#multitouchpanning)
- [panningSensibility](ArcRotateCameraPointersInput.md#panningsensibility)
- [pinchDeltaPercentage](ArcRotateCameraPointersInput.md#pinchdeltapercentage)
- [pinchInwards](ArcRotateCameraPointersInput.md#pinchinwards)
- [pinchPrecision](ArcRotateCameraPointersInput.md#pinchprecision)
- [pinchZoom](ArcRotateCameraPointersInput.md#pinchzoom)
- [useNaturalPinchZoom](ArcRotateCameraPointersInput.md#usenaturalpinchzoom)
- [MinimumRadiusForPinch](ArcRotateCameraPointersInput.md#minimumradiusforpinch)

### Methods

- [\_computeMultiTouchPanning](ArcRotateCameraPointersInput.md#_computemultitouchpanning)
- [\_computePinchZoom](ArcRotateCameraPointersInput.md#_computepinchzoom)
- [attachControl](ArcRotateCameraPointersInput.md#attachcontrol)
- [detachControl](ArcRotateCameraPointersInput.md#detachcontrol)
- [getClassName](ArcRotateCameraPointersInput.md#getclassname)
- [getSimpleName](ArcRotateCameraPointersInput.md#getsimplename)
- [onButtonDown](ArcRotateCameraPointersInput.md#onbuttondown)
- [onButtonUp](ArcRotateCameraPointersInput.md#onbuttonup)
- [onContextMenu](ArcRotateCameraPointersInput.md#oncontextmenu)
- [onDoubleTap](ArcRotateCameraPointersInput.md#ondoubletap)
- [onLostFocus](ArcRotateCameraPointersInput.md#onlostfocus)
- [onMultiTouch](ArcRotateCameraPointersInput.md#onmultitouch)
- [onTouch](ArcRotateCameraPointersInput.md#ontouch)

## Constructors

### constructor

• **new ArcRotateCameraPointersInput**()

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[constructor](BaseCameraPointersInput.md#constructor)

## Properties

### \_altKey

• `Protected` **\_altKey**: `boolean`

Whether keyboard modifier keys are pressed at time of last mouse event.

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_altKey](BaseCameraPointersInput.md#_altkey)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:26

___

### \_buttonsPressed

• `Protected` **\_buttonsPressed**: `number`

Which mouse buttons were pressed at time of last mouse event.
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/buttons

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_buttonsPressed](BaseCameraPointersInput.md#_buttonspressed)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:35

___

### \_ctrlKey

• `Protected` **\_ctrlKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_ctrlKey](BaseCameraPointersInput.md#_ctrlkey)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:27

___

### \_isPanClick

• `Private` **\_isPanClick**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:106

___

### \_isPinching

• `Private` **\_isPinching**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:108

___

### \_metaKey

• `Protected` **\_metaKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_metaKey](BaseCameraPointersInput.md#_metakey)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:28

___

### \_shiftKey

• `Protected` **\_shiftKey**: `boolean`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[_shiftKey](BaseCameraPointersInput.md#_shiftkey)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:29

___

### \_twoFingerActivityCount

• `Private` **\_twoFingerActivityCount**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:107

___

### angularSensibilityX

• **angularSensibilityX**: `number` = `1000.0`

Defines the pointer angular sensibility  along the X axis or how fast is
the camera rotating.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:43

___

### angularSensibilityY

• **angularSensibilityY**: `number` = `1000.0`

Defines the pointer angular sensibility along the Y axis or how fast is
the camera rotating.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:50

___

### buttons

• **buttons**: `number`[]

Defines the buttons associated with the input to handle camera move.

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[buttons](BaseCameraPointersInput.md#buttons)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:36

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defines the camera the input is attached to.

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[camera](BaseCameraPointersInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:17

___

### multiTouchPanAndZoom

• **multiTouchPanAndZoom**: `boolean` = `true`

Defines whether panning is enabled for both pan (2 fingers swipe) and
zoom (pinch) through multitouch.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:99

___

### multiTouchPanning

• **multiTouchPanning**: `boolean` = `true`

Defines whether panning (2 fingers swipe) is enabled through multitouch.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:92

___

### panningSensibility

• **panningSensibility**: `number` = `1000.0`

Defines the pointer panning sensibility or how fast is the camera moving.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:86

___

### pinchDeltaPercentage

• **pinchDeltaPercentage**: `number` = `0`

pinchDeltaPercentage will be used instead of pinchPrecision if different
from 0.
It defines the percentage of current camera.radius to use as delta when
pinch zoom is used.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:65

___

### pinchInwards

• **pinchInwards**: `boolean` = `true`

Revers pinch action direction.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:104

___

### pinchPrecision

• **pinchPrecision**: `number` = `12.0`

Defines the pointer pinch precision or how fast is the camera zooming.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:56

___

### pinchZoom

• **pinchZoom**: `boolean` = `true`

Defines whether zoom (2 fingers pinch) is enabled through multitouch

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:80

___

### useNaturalPinchZoom

• **useNaturalPinchZoom**: `boolean` = `false`

When useNaturalPinchZoom is true, multi touch zoom will zoom in such
that any object in the plane at the camera's target point will scale
perfectly with finger motion.
Overrides pinchDeltaPercentage and pinchPrecision.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:74

___

### MinimumRadiusForPinch

▪ `Static` **MinimumRadiusForPinch**: `number` = `0.001`

The minimum radius used for pinch, to avoid radius lock at 0

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:22

## Methods

### \_computeMultiTouchPanning

▸ `Private` **_computeMultiTouchPanning**(`previousMultiTouchPanPosition`, `multiTouchPanPosition`): `void`

Move camera from multi touch panning positions.

#### Parameters

| Name | Type |
| :------ | :------ |
| `previousMultiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `multiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:115

___

### \_computePinchZoom

▸ `Private` **_computePinchZoom**(`previousPinchSquaredDistance`, `pinchSquaredDistance`): `void`

Move camera from pinch zoom distances.

#### Parameters

| Name | Type |
| :------ | :------ |
| `previousPinchSquaredDistance` | `number` |
| `pinchSquaredDistance` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:129

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

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:50

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Inherited from

[BaseCameraPointersInput](BaseCameraPointersInput.md).[detachControl](BaseCameraPointersInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:245

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:28

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

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:285

___

### onButtonDown

▸ **onButtonDown**(`evt`): `void`

Called each time a new POINTERDOWN event occurs. Ie, for each button
press.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onButtonDown](BaseCameraPointersInput.md#onbuttondown)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:233

___

### onButtonUp

▸ **onButtonUp**(): `void`

Called each time a new POINTERUP event occurs. Ie, for each button
release.

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onButtonUp](BaseCameraPointersInput.md#onbuttonup)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:241

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

https://github.com/babylon.js/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:332

___

### onDoubleTap

▸ **onDoubleTap**(): `void`

Called on pointer POINTERDOUBLETAP event.

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onDoubleTap](BaseCameraPointersInput.md#ondoubletap)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:161

___

### onLostFocus

▸ **onLostFocus**(): `void`

Called when window becomes inactive.

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onLostFocus](BaseCameraPointersInput.md#onlostfocus)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:249

___

### onMultiTouch

▸ **onMultiTouch**(`pointA`, `pointB`, `previousPinchSquaredDistance`, `pinchSquaredDistance`, `previousMultiTouchPanPosition`, `multiTouchPanPosition`): `void`

Called on pointer POINTERMOVE event if multiple touches are active.

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:176

___

### onTouch

▸ **onTouch**(`point`, `offsetX`, `offsetY`): `void`

Called on pointer POINTERMOVE event if only a single touch is active.

#### Parameters

| Name | Type |
| :------ | :------ |
| `point` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `offsetX` | `number` |
| `offsetY` | `number` |

#### Returns

`void`

#### Overrides

[BaseCameraPointersInput](BaseCameraPointersInput.md).[onTouch](BaseCameraPointersInput.md#ontouch)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraPointersInput.ts:148

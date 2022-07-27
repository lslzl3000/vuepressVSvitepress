[@dev/core](../README.md) / [Exports](../modules.md) / BaseCameraPointersInput

# Class: BaseCameraPointersInput

Base class for Camera Pointer Inputs.
See FollowCameraPointersInput in src/Cameras/Inputs/followCameraPointersInput.ts
for example usage.

## Hierarchy

- **`BaseCameraPointersInput`**

  ↳ [`ArcRotateCameraPointersInput`](ArcRotateCameraPointersInput.md)

  ↳ [`FollowCameraPointersInput`](FollowCameraPointersInput.md)

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`Camera`](Camera.md)

## Table of contents

### Constructors

- [constructor](BaseCameraPointersInput.md#constructor)

### Properties

- [\_altKey](BaseCameraPointersInput.md#_altkey)
- [\_buttonsPressed](BaseCameraPointersInput.md#_buttonspressed)
- [\_contextMenuBind](BaseCameraPointersInput.md#_contextmenubind)
- [\_ctrlKey](BaseCameraPointersInput.md#_ctrlkey)
- [\_currentActiveButton](BaseCameraPointersInput.md#_currentactivebutton)
- [\_metaKey](BaseCameraPointersInput.md#_metakey)
- [\_observer](BaseCameraPointersInput.md#_observer)
- [\_onLostFocus](BaseCameraPointersInput.md#_onlostfocus)
- [\_pointA](BaseCameraPointersInput.md#_pointa)
- [\_pointB](BaseCameraPointersInput.md#_pointb)
- [\_pointerInput](BaseCameraPointersInput.md#_pointerinput)
- [\_shiftKey](BaseCameraPointersInput.md#_shiftkey)
- [buttons](BaseCameraPointersInput.md#buttons)
- [camera](BaseCameraPointersInput.md#camera)

### Methods

- [attachControl](BaseCameraPointersInput.md#attachcontrol)
- [detachControl](BaseCameraPointersInput.md#detachcontrol)
- [getClassName](BaseCameraPointersInput.md#getclassname)
- [getSimpleName](BaseCameraPointersInput.md#getsimplename)
- [onButtonDown](BaseCameraPointersInput.md#onbuttondown)
- [onButtonUp](BaseCameraPointersInput.md#onbuttonup)
- [onContextMenu](BaseCameraPointersInput.md#oncontextmenu)
- [onDoubleTap](BaseCameraPointersInput.md#ondoubletap)
- [onLostFocus](BaseCameraPointersInput.md#onlostfocus)
- [onMultiTouch](BaseCameraPointersInput.md#onmultitouch)
- [onTouch](BaseCameraPointersInput.md#ontouch)

## Constructors

### constructor

• **new BaseCameraPointersInput**()

## Properties

### \_altKey

• `Protected` **\_altKey**: `boolean`

Whether keyboard modifier keys are pressed at time of last mouse event.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:26

___

### \_buttonsPressed

• `Protected` **\_buttonsPressed**: `number`

Which mouse buttons were pressed at time of last mouse event.
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/buttons

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:35

___

### \_contextMenuBind

• `Private` **\_contextMenuBind**: `EventListener`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:38

___

### \_ctrlKey

• `Protected` **\_ctrlKey**: `boolean`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:27

___

### \_currentActiveButton

• `Private` **\_currentActiveButton**: `number` = `-1`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:37

___

### \_metaKey

• `Protected` **\_metaKey**: `boolean`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:28

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:361

___

### \_onLostFocus

• `Private` **\_onLostFocus**: [`Nullable`](../modules.md#nullable)(`e`: `FocusEvent`) => `any`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:362

___

### \_pointA

• `Private` **\_pointA**: [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:363

___

### \_pointB

• `Private` **\_pointB**: [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:364

___

### \_pointerInput

• `Private` **\_pointerInput**: (`p`: [`PointerInfo`](PointerInfo.md), `s`: [`EventState`](EventState.md)) => `void`

#### Type declaration

▸ (`p`, `s`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `p` | [`PointerInfo`](PointerInfo.md) |
| `s` | [`EventState`](EventState.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:360

___

### \_shiftKey

• `Protected` **\_shiftKey**: `boolean`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:29

___

### buttons

• **buttons**: `number`[]

Defines the buttons associated with the input to handle camera move.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:44

___

### camera

• `Abstract` **camera**: [`Camera`](Camera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:21

## Methods

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

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:50

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:245

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

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:277

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

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:295

___

### onLostFocus

▸ **onLostFocus**(): `void`

Called when window becomes inactive.
Override this method to provide functionality.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:358

___

### onMultiTouch

▸ **onMultiTouch**(`_pointA`, `_pointB`, `previousPinchSquaredDistance`, `pinchSquaredDistance`, `previousMultiTouchPanPosition`, `multiTouchPanPosition`): `void`

Called on pointer POINTERMOVE event if multiple touches are active.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `_pointA` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `_pointB` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `previousPinchSquaredDistance` | `number` |
| `pinchSquaredDistance` | `number` |
| `previousMultiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `multiTouchPanPosition` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:318

___

### onTouch

▸ **onTouch**(`point`, `offsetX`, `offsetY`): `void`

Called on pointer POINTERMOVE event if only a single touch is active.
Override this method to provide functionality.

#### Parameters

| Name | Type |
| :------ | :------ |
| `point` | [`Nullable`](../modules.md#nullable)[`PointerTouch`](../interfaces/PointerTouch.md) |
| `offsetX` | `number` |
| `offsetY` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraPointersInput.ts:305

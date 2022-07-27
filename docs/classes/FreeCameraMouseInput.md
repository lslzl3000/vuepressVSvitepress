[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraMouseInput

# Class: FreeCameraMouseInput

Manage the mouse inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraMouseInput.md#constructor)

### Properties

- [\_contextMenuBind](FreeCameraMouseInput.md#_contextmenubind)
- [\_currentActiveButton](FreeCameraMouseInput.md#_currentactivebutton)
- [\_observer](FreeCameraMouseInput.md#_observer)
- [\_onMouseMove](FreeCameraMouseInput.md#_onmousemove)
- [\_pointerInput](FreeCameraMouseInput.md#_pointerinput)
- [\_previousPosition](FreeCameraMouseInput.md#_previousposition)
- [angularSensibility](FreeCameraMouseInput.md#angularsensibility)
- [buttons](FreeCameraMouseInput.md#buttons)
- [camera](FreeCameraMouseInput.md#camera)
- [onPointerMovedObservable](FreeCameraMouseInput.md#onpointermovedobservable)
- [touchEnabled](FreeCameraMouseInput.md#touchenabled)

### Methods

- [attachControl](FreeCameraMouseInput.md#attachcontrol)
- [detachControl](FreeCameraMouseInput.md#detachcontrol)
- [getClassName](FreeCameraMouseInput.md#getclassname)
- [getSimpleName](FreeCameraMouseInput.md#getsimplename)
- [onContextMenu](FreeCameraMouseInput.md#oncontextmenu)

## Constructors

### constructor

• **new FreeCameraMouseInput**(`touchEnabled?`)

Manage the mouse inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `touchEnabled` | `boolean` | `true` | Defines if touch is enabled or not |

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:58

## Properties

### \_contextMenuBind

• `Private` **\_contextMenuBind**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:51

___

### \_currentActiveButton

• `Private` **\_currentActiveButton**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:49

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:36

___

### \_onMouseMove

• `Private` **\_onMouseMove**: [`Nullable`](../modules.md#nullable)(`e`: [`IMouseEvent`](../interfaces/IMouseEvent.md)) => `any`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:35

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:34

___

### \_previousPosition

• `Private` **\_previousPosition**: [`Nullable`](../modules.md#nullable){ `x`: `number` ; `y`: `number`  } = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:37

___

### angularSensibility

• **angularSensibility**: `number` = `2000.0`

Defines the pointer angular sensibility  along the X and Y axis or how fast is the camera rotating.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:32

___

### buttons

• **buttons**: `number`[]

Defines the buttons associated with the input to handle camera move.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:26

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:20

___

### onPointerMovedObservable

• **onPointerMovedObservable**: [`Observable`](Observable.md){ `offsetX`: `number` ; `offsetY`: `number`  }

Observable for when a pointer move event occurs containing the move offset

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:42

___

### touchEnabled

• **touchEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:62

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:69

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:213

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:239

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:247

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraMouseInput.ts:206

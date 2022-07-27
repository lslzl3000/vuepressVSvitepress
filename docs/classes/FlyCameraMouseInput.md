[@dev/core](../README.md) / [Exports](../modules.md) / FlyCameraMouseInput

# Class: FlyCameraMouseInput

Listen to mouse events to control the camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FlyCamera`](FlyCamera.md)

## Table of contents

### Constructors

- [constructor](FlyCameraMouseInput.md#constructor)

### Properties

- [\_element](FlyCameraMouseInput.md#_element)
- [\_noPreventDefault](FlyCameraMouseInput.md#_nopreventdefault)
- [\_observer](FlyCameraMouseInput.md#_observer)
- [\_previousPosition](FlyCameraMouseInput.md#_previousposition)
- [\_rollObserver](FlyCameraMouseInput.md#_rollobserver)
- [activeButton](FlyCameraMouseInput.md#activebutton)
- [angularSensibility](FlyCameraMouseInput.md#angularsensibility)
- [buttons](FlyCameraMouseInput.md#buttons)
- [buttonsPitch](FlyCameraMouseInput.md#buttonspitch)
- [buttonsRoll](FlyCameraMouseInput.md#buttonsroll)
- [buttonsYaw](FlyCameraMouseInput.md#buttonsyaw)
- [camera](FlyCameraMouseInput.md#camera)
- [touchEnabled](FlyCameraMouseInput.md#touchenabled)

### Methods

- [\_onMouseMove](FlyCameraMouseInput.md#_onmousemove)
- [\_pointerInput](FlyCameraMouseInput.md#_pointerinput)
- [\_rotateCamera](FlyCameraMouseInput.md#_rotatecamera)
- [attachControl](FlyCameraMouseInput.md#attachcontrol)
- [detachControl](FlyCameraMouseInput.md#detachcontrol)
- [getClassName](FlyCameraMouseInput.md#getclassname)
- [getSimpleName](FlyCameraMouseInput.md#getsimplename)

## Constructors

### constructor

• **new FlyCameraMouseInput**()

Listen to mouse events to control the camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:76

## Properties

### \_element

• `Private` **\_element**: `HTMLElement`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:70

___

### \_noPreventDefault

• `Private` **\_noPreventDefault**: `undefined` \| `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:69

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:66

___

### \_previousPosition

• `Private` **\_previousPosition**: [`Nullable`](../modules.md#nullable){ `x`: `number` ; `y`: `number`  } = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:68

___

### \_rollObserver

• `Private` **\_rollObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:67

___

### activeButton

• **activeButton**: `number` = `-1`

Detect if any button is being pressed while mouse is moved.
-1 = Mouse locked.
0 = Left button.
1 = Middle Button.
2 = Right Button.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:57

___

### angularSensibility

• **angularSensibility**: `number` = `1000.0`

Defines the pointer's angular sensibility, to control the camera rotation speed.
Higher values reduce its sensitivity.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:64

___

### buttons

• **buttons**: `number`[]

Defines the buttons associated with the input to handle camera rotation.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:33

___

### buttonsPitch

• **buttonsPitch**: `number`[]

Assign buttons for Pitch control.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:43

___

### buttonsRoll

• **buttonsRoll**: `number`[]

Assign buttons for Roll control.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:48

___

### buttonsYaw

• **buttonsYaw**: `number`[]

Assign buttons for Yaw control.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:38

___

### camera

• **camera**: [`FlyCamera`](FlyCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:22

___

### touchEnabled

• **touchEnabled**: `boolean`

Defines if touch is enabled. (Default is true.)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:27

## Methods

### \_onMouseMove

▸ `Private` **_onMouseMove**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:220

___

### \_pointerInput

▸ `Private` **_pointerInput**(`p`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `p` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:132

___

### \_rotateCamera

▸ `Private` **_rotateCamera**(`offsetX`, `offsetY`): `void`

Rotate camera by mouse offset.

#### Parameters

| Name | Type |
| :------ | :------ |
| `offsetX` | `number` |
| `offsetY` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:245

___

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the mouse control to the HTML DOM element.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether events caught by the controls should call preventdefault(). |

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:82

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:102

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getClassName](../interfaces/ICameraInput.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:119

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input's friendly name.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getSimpleName](../interfaces/ICameraInput.md#getsimplename)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraMouseInput.ts:127

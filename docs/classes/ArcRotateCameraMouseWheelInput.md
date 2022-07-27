[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraMouseWheelInput

# Class: ArcRotateCameraMouseWheelInput

Manage the mouse wheel inputs to control an arc rotate camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](ArcRotateCameraMouseWheelInput.md#constructor)

### Properties

- [\_hitPlane](ArcRotateCameraMouseWheelInput.md#_hitplane)
- [\_inertialPanning](ArcRotateCameraMouseWheelInput.md#_inertialpanning)
- [\_observer](ArcRotateCameraMouseWheelInput.md#_observer)
- [\_wheel](ArcRotateCameraMouseWheelInput.md#_wheel)
- [camera](ArcRotateCameraMouseWheelInput.md#camera)
- [customComputeDeltaFromMouseWheel](ArcRotateCameraMouseWheelInput.md#customcomputedeltafrommousewheel)
- [wheelDeltaPercentage](ArcRotateCameraMouseWheelInput.md#wheeldeltapercentage)
- [wheelPrecision](ArcRotateCameraMouseWheelInput.md#wheelprecision)
- [zoomToMouseLocation](ArcRotateCameraMouseWheelInput.md#zoomtomouselocation)

### Methods

- [\_computeDeltaFromMouseWheelLegacyEvent](ArcRotateCameraMouseWheelInput.md#_computedeltafrommousewheellegacyevent)
- [\_getPosition](ArcRotateCameraMouseWheelInput.md#_getposition)
- [\_updateHitPlane](ArcRotateCameraMouseWheelInput.md#_updatehitplane)
- [\_zeroIfClose](ArcRotateCameraMouseWheelInput.md#_zeroifclose)
- [\_zoomToMouse](ArcRotateCameraMouseWheelInput.md#_zoomtomouse)
- [attachControl](ArcRotateCameraMouseWheelInput.md#attachcontrol)
- [checkInputs](ArcRotateCameraMouseWheelInput.md#checkinputs)
- [detachControl](ArcRotateCameraMouseWheelInput.md#detachcontrol)
- [getClassName](ArcRotateCameraMouseWheelInput.md#getclassname)
- [getSimpleName](ArcRotateCameraMouseWheelInput.md#getsimplename)

## Constructors

### constructor

• **new ArcRotateCameraMouseWheelInput**()

## Properties

### \_hitPlane

• `Private` **\_hitPlane**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:63

___

### \_inertialPanning

• `Private` **\_inertialPanning**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:223

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:62

___

### \_wheel

• `Private` **\_wheel**: [`Nullable`](../modules.md#nullable)(`p`: [`PointerInfo`](PointerInfo.md), `s`: [`EventState`](EventState.md)) => `void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:61

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:34

___

### customComputeDeltaFromMouseWheel

• **customComputeDeltaFromMouseWheel**: [`Nullable`](../modules.md#nullable)(`wheelDelta`: `number`, `input`: [`ArcRotateCameraMouseWheelInput`](ArcRotateCameraMouseWheelInput.md), `event`: [`IWheelEvent`](../interfaces/IWheelEvent.md)) => `number` = `null`

If set, this function will be used to set the radius delta that will be added to the current camera radius

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:59

___

### wheelDeltaPercentage

• **wheelDeltaPercentage**: `number` = `0`

wheelDeltaPercentage will be used instead of wheelPrecision if different from 0.
It defines the percentage of current camera.radius to use as delta when wheel is used.

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:54

___

### wheelPrecision

• **wheelPrecision**: `number` = `3.0`

Gets or Set the mouse wheel precision or how fast is the camera zooming.

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:40

___

### zoomToMouseLocation

• **zoomToMouseLocation**: `boolean` = `false`

Gets or Set the boolean value that controls whether or not the mouse wheel
zooms to the location of the mouse pointer or not.  The default is false.

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:47

## Methods

### \_computeDeltaFromMouseWheelLegacyEvent

▸ `Protected` **_computeDeltaFromMouseWheelLegacyEvent**(`mouseWheelDelta`, `radius`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mouseWheelDelta` | `number` |
| `radius` | `number` |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:65

___

### \_getPosition

▸ `Private` **_getPosition**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:206

___

### \_updateHitPlane

▸ `Private` **_updateHitPlane**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:199

___

### \_zeroIfClose

▸ `Private` **_zeroIfClose**(`vec`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vec` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:258

___

### \_zoomToMouse

▸ `Private` **_zoomToMouse**(`delta`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `delta` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:225

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

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:80

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

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:162

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:150

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

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:187

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

packages/dev/core/src/Cameras/Inputs/arcRotateCameraMouseWheelInput.ts:195

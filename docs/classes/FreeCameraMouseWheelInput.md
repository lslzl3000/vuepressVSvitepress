[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraMouseWheelInput

# Class: FreeCameraMouseWheelInput

Manage the mouse wheel inputs to control a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`BaseCameraMouseWheelInput`](BaseCameraMouseWheelInput.md)

  ↳ **`FreeCameraMouseWheelInput`**

## Table of contents

### Constructors

- [constructor](FreeCameraMouseWheelInput.md#constructor)

### Properties

- [\_moveRelative](FreeCameraMouseWheelInput.md#_moverelative)
- [\_moveScene](FreeCameraMouseWheelInput.md#_movescene)
- [\_rotateRelative](FreeCameraMouseWheelInput.md#_rotaterelative)
- [\_wheelDeltaX](FreeCameraMouseWheelInput.md#_wheeldeltax)
- [\_wheelDeltaY](FreeCameraMouseWheelInput.md#_wheeldeltay)
- [\_wheelDeltaZ](FreeCameraMouseWheelInput.md#_wheeldeltaz)
- [\_wheelXAction](FreeCameraMouseWheelInput.md#_wheelxaction)
- [\_wheelXActionCoordinate](FreeCameraMouseWheelInput.md#_wheelxactioncoordinate)
- [\_wheelYAction](FreeCameraMouseWheelInput.md#_wheelyaction)
- [\_wheelYActionCoordinate](FreeCameraMouseWheelInput.md#_wheelyactioncoordinate)
- [\_wheelZAction](FreeCameraMouseWheelInput.md#_wheelzaction)
- [\_wheelZActionCoordinate](FreeCameraMouseWheelInput.md#_wheelzactioncoordinate)
- [camera](FreeCameraMouseWheelInput.md#camera)
- [onChangedObservable](FreeCameraMouseWheelInput.md#onchangedobservable)
- [wheelPrecisionX](FreeCameraMouseWheelInput.md#wheelprecisionx)
- [wheelPrecisionY](FreeCameraMouseWheelInput.md#wheelprecisiony)
- [wheelPrecisionZ](FreeCameraMouseWheelInput.md#wheelprecisionz)

### Accessors

- [wheelXMoveRelative](FreeCameraMouseWheelInput.md#wheelxmoverelative)
- [wheelXMoveScene](FreeCameraMouseWheelInput.md#wheelxmovescene)
- [wheelXRotateRelative](FreeCameraMouseWheelInput.md#wheelxrotaterelative)
- [wheelYMoveRelative](FreeCameraMouseWheelInput.md#wheelymoverelative)
- [wheelYMoveScene](FreeCameraMouseWheelInput.md#wheelymovescene)
- [wheelYRotateRelative](FreeCameraMouseWheelInput.md#wheelyrotaterelative)
- [wheelZMoveRelative](FreeCameraMouseWheelInput.md#wheelzmoverelative)
- [wheelZMoveScene](FreeCameraMouseWheelInput.md#wheelzmovescene)
- [wheelZRotateRelative](FreeCameraMouseWheelInput.md#wheelzrotaterelative)

### Methods

- [\_updateCamera](FreeCameraMouseWheelInput.md#_updatecamera)
- [\_updateCameraProperty](FreeCameraMouseWheelInput.md#_updatecameraproperty)
- [attachControl](FreeCameraMouseWheelInput.md#attachcontrol)
- [checkInputs](FreeCameraMouseWheelInput.md#checkinputs)
- [detachControl](FreeCameraMouseWheelInput.md#detachcontrol)
- [getClassName](FreeCameraMouseWheelInput.md#getclassname)
- [getSimpleName](FreeCameraMouseWheelInput.md#getsimplename)

## Constructors

### constructor

• **new FreeCameraMouseWheelInput**()

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[constructor](BaseCameraMouseWheelInput.md#constructor)

## Properties

### \_moveRelative

• `Private` **\_moveRelative**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:315

___

### \_moveScene

• `Private` **\_moveScene**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:317

___

### \_rotateRelative

• `Private` **\_rotateRelative**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:316

___

### \_wheelDeltaX

• `Protected` **\_wheelDeltaX**: `number` = `0`

Incremental value of multiple mouse wheel movements of the X axis.
Should be zero-ed when read.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[_wheelDeltaX](BaseCameraMouseWheelInput.md#_wheeldeltax)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:153

___

### \_wheelDeltaY

• `Protected` **\_wheelDeltaY**: `number` = `0`

Incremental value of multiple mouse wheel movements of the Y axis.
Should be zero-ed when read.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[_wheelDeltaY](BaseCameraMouseWheelInput.md#_wheeldeltay)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:159

___

### \_wheelDeltaZ

• `Protected` **\_wheelDeltaZ**: `number` = `0`

Incremental value of multiple mouse wheel movements of the Z axis.
Should be zero-ed when read.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[_wheelDeltaZ](BaseCameraMouseWheelInput.md#_wheeldeltaz)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:165

___

### \_wheelXAction

• `Private` **\_wheelXAction**: [`Nullable`](../modules.md#nullable)`_CameraProperty` = `_CameraProperty.MoveRelative`

These are set to the desired default behaviour.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:322

___

### \_wheelXActionCoordinate

• `Private` **\_wheelXActionCoordinate**: [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) = `Coordinate.X`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:323

___

### \_wheelYAction

• `Private` **\_wheelYAction**: [`Nullable`](../modules.md#nullable)`_CameraProperty` = `_CameraProperty.MoveRelative`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:324

___

### \_wheelYActionCoordinate

• `Private` **\_wheelYActionCoordinate**: [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) = `Coordinate.Z`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:325

___

### \_wheelZAction

• `Private` **\_wheelZAction**: [`Nullable`](../modules.md#nullable)`_CameraProperty` = `null`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:326

___

### \_wheelZActionCoordinate

• `Private` **\_wheelZActionCoordinate**: [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) = `null`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:327

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defines the camera the input is attached to.

#### Overrides

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[camera](BaseCameraMouseWheelInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:24

___

### onChangedObservable

• **onChangedObservable**: [`Observable`](Observable.md){ `wheelDeltaX`: `number` ; `wheelDeltaY`: `number` ; `wheelDeltaZ`: `number`  }

Observable for when a mouse wheel move event occurs.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[onChangedObservable](BaseCameraMouseWheelInput.md#onchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:48

___

### wheelPrecisionX

• **wheelPrecisionX**: `number` = `3.0`

How fast is the camera moves in relation to X axis mouseWheel events.
Use negative value to reverse direction.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[wheelPrecisionX](BaseCameraMouseWheelInput.md#wheelprecisionx)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:29

___

### wheelPrecisionY

• **wheelPrecisionY**: `number` = `3.0`

How fast is the camera moves in relation to Y axis mouseWheel events.
Use negative value to reverse direction.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[wheelPrecisionY](BaseCameraMouseWheelInput.md#wheelprecisiony)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:36

___

### wheelPrecisionZ

• **wheelPrecisionZ**: `number` = `3.0`

How fast is the camera moves in relation to Z axis mouseWheel events.
Use negative value to reverse direction.

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[wheelPrecisionZ](BaseCameraMouseWheelInput.md#wheelprecisionz)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:43

## Accessors

### wheelXMoveRelative

• `get` **wheelXMoveRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to camera's orientation) the
mouse wheel's X axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:54

• `set` **wheelXMoveRelative**(`axis`): `void`

Set which movement axis (relative to camera's orientation) the mouse
wheel's X axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:39

___

### wheelXMoveScene

• `get` **wheelXMoveScene**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to the scene) the mouse wheel's
X axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:216

• `set` **wheelXMoveScene**(`axis`): `void`

Set which movement axis (relative to the scene) the mouse wheel's X axis
controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:201

___

### wheelXRotateRelative

• `get` **wheelXRotateRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured rotation axis (relative to camera's orientation) the
mouse wheel's X axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:135

• `set` **wheelXRotateRelative**(`axis`): `void`

Set which rotation axis (relative to camera's orientation) the mouse
wheel's X axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:120

___

### wheelYMoveRelative

• `get` **wheelYMoveRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to camera's orientation) the
mouse wheel's Y axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:81

• `set` **wheelYMoveRelative**(`axis`): `void`

Set which movement axis (relative to camera's orientation) the mouse
wheel's Y axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:66

___

### wheelYMoveScene

• `get` **wheelYMoveScene**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to the scene) the mouse wheel's
Y axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:243

• `set` **wheelYMoveScene**(`axis`): `void`

Set which movement axis (relative to the scene) the mouse wheel's Y axis
controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:228

___

### wheelYRotateRelative

• `get` **wheelYRotateRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured rotation axis (relative to camera's orientation) the
mouse wheel's Y axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:162

• `set` **wheelYRotateRelative**(`axis`): `void`

Set which rotation axis (relative to camera's orientation) the mouse
wheel's Y axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:147

___

### wheelZMoveRelative

• `get` **wheelZMoveRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to camera's orientation) the
mouse wheel's Z axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:108

• `set` **wheelZMoveRelative**(`axis`): `void`

Set which movement axis (relative to camera's orientation) the mouse
wheel's Z axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:93

___

### wheelZMoveScene

• `get` **wheelZMoveScene**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured movement axis (relative to the scene) the mouse wheel's
Z axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:270

• `set` **wheelZMoveScene**(`axis`): `void`

Set which movement axis (relative to the scene) the mouse wheel's Z axis
controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:255

___

### wheelZRotateRelative

• `get` **wheelZRotateRelative**(): [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

Get the configured rotation axis (relative to camera's orientation) the
mouse wheel's Z axis controls.

#### Returns

[`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md)

The configured axis or null if none.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:189

• `set` **wheelZRotateRelative**(`axis`): `void`

Set which rotation axis (relative to camera's orientation) the mouse
wheel's Z axis controls.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) | The axis to be moved. Set null to clear. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:174

## Methods

### \_updateCamera

▸ `Private` **_updateCamera**(): `void`

Update the camera according to any configured properties for the 3
mouse-wheel axis.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:333

___

### \_updateCameraProperty

▸ `Private` **_updateCameraProperty**(`value`, `cameraProperty`, `coordinate`): `void`

Update one property of the camera.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |
| `cameraProperty` | [`Nullable`](../modules.md#nullable)`_CameraProperty` |
| `coordinate` | [`Nullable`](../modules.md#nullable)[`Coordinate`](../enums/Coordinate.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:346

___

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls    should call preventdefault().    (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[attachControl](BaseCameraMouseWheelInput.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:59

___

### checkInputs

▸ **checkInputs**(): `void`

Called for each rendered frame.

#### Returns

`void`

#### Overrides

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[checkInputs](BaseCameraMouseWheelInput.md#checkinputs)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:280

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[detachControl](BaseCameraMouseWheelInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:106

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Overrides

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[getClassName](BaseCameraMouseWheelInput.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraMouseWheelInput.ts:30

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Inherited from

[BaseCameraMouseWheelInput](BaseCameraMouseWheelInput.md).[getSimpleName](BaseCameraMouseWheelInput.md#getsimplename)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:145

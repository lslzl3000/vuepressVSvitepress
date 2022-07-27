[@dev/core](../README.md) / [Exports](../modules.md) / BaseCameraMouseWheelInput

# Class: BaseCameraMouseWheelInput

Base class for mouse wheel input..
See FollowCameraMouseWheelInput in src/Cameras/Inputs/freeCameraMouseWheelInput.ts
for example usage.

## Hierarchy

- **`BaseCameraMouseWheelInput`**

  ↳ [`FreeCameraMouseWheelInput`](FreeCameraMouseWheelInput.md)

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`Camera`](Camera.md)

## Table of contents

### Constructors

- [constructor](BaseCameraMouseWheelInput.md#constructor)

### Properties

- [\_ffMultiplier](BaseCameraMouseWheelInput.md#_ffmultiplier)
- [\_normalize](BaseCameraMouseWheelInput.md#_normalize)
- [\_observer](BaseCameraMouseWheelInput.md#_observer)
- [\_wheel](BaseCameraMouseWheelInput.md#_wheel)
- [\_wheelDeltaX](BaseCameraMouseWheelInput.md#_wheeldeltax)
- [\_wheelDeltaY](BaseCameraMouseWheelInput.md#_wheeldeltay)
- [\_wheelDeltaZ](BaseCameraMouseWheelInput.md#_wheeldeltaz)
- [camera](BaseCameraMouseWheelInput.md#camera)
- [onChangedObservable](BaseCameraMouseWheelInput.md#onchangedobservable)
- [wheelPrecisionX](BaseCameraMouseWheelInput.md#wheelprecisionx)
- [wheelPrecisionY](BaseCameraMouseWheelInput.md#wheelprecisiony)
- [wheelPrecisionZ](BaseCameraMouseWheelInput.md#wheelprecisionz)

### Methods

- [attachControl](BaseCameraMouseWheelInput.md#attachcontrol)
- [checkInputs](BaseCameraMouseWheelInput.md#checkinputs)
- [detachControl](BaseCameraMouseWheelInput.md#detachcontrol)
- [getClassName](BaseCameraMouseWheelInput.md#getclassname)
- [getSimpleName](BaseCameraMouseWheelInput.md#getsimplename)

## Constructors

### constructor

• **new BaseCameraMouseWheelInput**()

## Properties

### \_ffMultiplier

• `Private` `Readonly` **\_ffMultiplier**: ``12``

Firefox uses a different scheme to report scroll distances to other
browsers. Rather than use complicated methods to calculate the exact
multiple we need to apply, let's just cheat and use a constant.
https://developer.mozilla.org/en-US/docs/Web/API/WheelEvent/deltaMode
https://stackoverflow.com/questions/20110224/what-is-the-height-of-a-line-in-a-wheel-event-deltamode-dom-delta-line

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:174

___

### \_normalize

• `Private` `Readonly` **\_normalize**: ``120``

Different event attributes for wheel data fall into a few set ranges.
Some relevant but dated date here:
https://stackoverflow.com/questions/5527601/normalizing-mousewheel-speed-across-browsers

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:181

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:51

___

### \_wheel

• `Private` **\_wheel**: [`Nullable`](../modules.md#nullable)(`pointer`: [`PointerInfo`](PointerInfo.md)) => `void`

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:50

___

### \_wheelDeltaX

• `Protected` **\_wheelDeltaX**: `number` = `0`

Incremental value of multiple mouse wheel movements of the X axis.
Should be zero-ed when read.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:153

___

### \_wheelDeltaY

• `Protected` **\_wheelDeltaY**: `number` = `0`

Incremental value of multiple mouse wheel movements of the Y axis.
Should be zero-ed when read.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:159

___

### \_wheelDeltaZ

• `Protected` **\_wheelDeltaZ**: `number` = `0`

Incremental value of multiple mouse wheel movements of the Z axis.
Should be zero-ed when read.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:165

___

### camera

• `Abstract` **camera**: [`Camera`](Camera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:22

___

### onChangedObservable

• **onChangedObservable**: [`Observable`](Observable.md){ `wheelDeltaX`: `number` ; `wheelDeltaY`: `number` ; `wheelDeltaZ`: `number`  }

Observable for when a mouse wheel move event occurs.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:48

___

### wheelPrecisionX

• **wheelPrecisionX**: `number` = `3.0`

How fast is the camera moves in relation to X axis mouseWheel events.
Use negative value to reverse direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:29

___

### wheelPrecisionY

• **wheelPrecisionY**: `number` = `3.0`

How fast is the camera moves in relation to Y axis mouseWheel events.
Use negative value to reverse direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:36

___

### wheelPrecisionZ

• **wheelPrecisionZ**: `number` = `3.0`

How fast is the camera moves in relation to Z axis mouseWheel events.
Use negative value to reverse direction.

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:43

## Methods

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls    should call preventdefault().    (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:59

___

### checkInputs

▸ **checkInputs**(): `void`

Called for each rendered frame.

#### Returns

`void`

#### Implementation of

ICameraInput.checkInputs

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:120

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:106

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

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:137

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

packages/dev/core/src/Cameras/Inputs/BaseCameraMouseWheelInput.ts:145

[@dev/core](../README.md) / [Exports](../modules.md) / EasingFunction

# Class: EasingFunction

Base class used for every default easing function.

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Hierarchy

- **`EasingFunction`**

  ↳ [`CircleEase`](CircleEase.md)

  ↳ [`BackEase`](BackEase.md)

  ↳ [`BounceEase`](BounceEase.md)

  ↳ [`CubicEase`](CubicEase.md)

  ↳ [`ElasticEase`](ElasticEase.md)

  ↳ [`ExponentialEase`](ExponentialEase.md)

  ↳ [`PowerEase`](PowerEase.md)

  ↳ [`QuadraticEase`](QuadraticEase.md)

  ↳ [`QuarticEase`](QuarticEase.md)

  ↳ [`QuinticEase`](QuinticEase.md)

  ↳ [`SineEase`](SineEase.md)

  ↳ [`BezierCurveEase`](BezierCurveEase.md)

## Implements

- [`IEasingFunction`](../interfaces/IEasingFunction.md)

## Table of contents

### Constructors

- [constructor](EasingFunction.md#constructor)

### Properties

- [\_easingMode](EasingFunction.md#_easingmode)
- [EASINGMODE\_EASEIN](EasingFunction.md#easingmode_easein)
- [EASINGMODE\_EASEINOUT](EasingFunction.md#easingmode_easeinout)
- [EASINGMODE\_EASEOUT](EasingFunction.md#easingmode_easeout)

### Methods

- [ease](EasingFunction.md#ease)
- [getEasingMode](EasingFunction.md#geteasingmode)
- [setEasingMode](EasingFunction.md#seteasingmode)

## Constructors

### constructor

• **new EasingFunction**()

## Properties

### \_easingMode

• `Private` **\_easingMode**: `number` = `EasingFunction.EASINGMODE_EASEIN`

#### Defined in

packages/dev/core/src/Animations/easing.ts:40

___

### EASINGMODE\_EASEIN

▪ `Static` `Readonly` **EASINGMODE\_EASEIN**: ``0``

Interpolation follows the mathematical formula associated with the easing function.

#### Defined in

packages/dev/core/src/Animations/easing.ts:28

___

### EASINGMODE\_EASEINOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEINOUT**: ``2``

Interpolation uses EaseIn for the first half of the animation and EaseOut for the second half.

#### Defined in

packages/dev/core/src/Animations/easing.ts:38

___

### EASINGMODE\_EASEOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEOUT**: ``1``

Interpolation follows 100% interpolation minus the output of the formula associated with the easing function.

#### Defined in

packages/dev/core/src/Animations/easing.ts:33

## Methods

### ease

▸ **ease**(`gradient`): `number`

Given an input gradient between 0 and 1, this returns the corresponding value
of the easing function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | Defines the value between 0 and 1 we want the easing value for |

#### Returns

`number`

the corresponding value on the curve defined by the easing function

#### Implementation of

[IEasingFunction](../interfaces/IEasingFunction.md).[ease](../interfaces/IEasingFunction.md#ease)

#### Defined in

packages/dev/core/src/Animations/easing.ts:73

___

### getEasingMode

▸ **getEasingMode**(): `number`

Gets the current easing mode.

#### Returns

`number`

the easing mode

#### Defined in

packages/dev/core/src/Animations/easing.ts:54

___

### setEasingMode

▸ **setEasingMode**(`easingMode`): `void`

Sets the easing mode of the current function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `easingMode` | `number` | Defines the willing mode (EASINGMODE_EASEIN, EASINGMODE_EASEOUT or EASINGMODE_EASEINOUT) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/easing.ts:46

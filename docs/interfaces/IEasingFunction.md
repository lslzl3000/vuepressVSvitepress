[@dev/core](../README.md) / [Exports](../modules.md) / IEasingFunction

# Interface: IEasingFunction

This represents the main contract an easing function should follow.
Easing functions are used throughout the animation system.

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Implemented by

- [`BackEase`](../classes/BackEase.md)
- [`BezierCurveEase`](../classes/BezierCurveEase.md)
- [`BounceEase`](../classes/BounceEase.md)
- [`CircleEase`](../classes/CircleEase.md)
- [`CubicEase`](../classes/CubicEase.md)
- [`EasingFunction`](../classes/EasingFunction.md)
- [`ElasticEase`](../classes/ElasticEase.md)
- [`ExponentialEase`](../classes/ExponentialEase.md)
- [`PowerEase`](../classes/PowerEase.md)
- [`QuadraticEase`](../classes/QuadraticEase.md)
- [`QuarticEase`](../classes/QuarticEase.md)
- [`QuinticEase`](../classes/QuinticEase.md)
- [`SineEase`](../classes/SineEase.md)

## Table of contents

### Methods

- [ease](IEasingFunction.md#ease)

## Methods

### ease

▸ **ease**(`gradient`): `number`

Given an input gradient between 0 and 1, this returns the corresponding value
of the easing function.
The link below provides some of the most common examples of easing functions.

**`See`**

https://easings.net/

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | Defines the value between 0 and 1 we want the easing value for |

#### Returns

`number`

the corresponding value on the curve defined by the easing function

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:17

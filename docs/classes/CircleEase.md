[@dev/core](../README.md) / [Exports](../modules.md) / CircleEase

# Class: CircleEase

Easing function with a circle shape (see link below).

**`See`**

 - https://easings.net/#easeInCirc
 - https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Hierarchy

- [`EasingFunction`](EasingFunction.md)

  ↳ **`CircleEase`**

## Implements

- [`IEasingFunction`](../interfaces/IEasingFunction.md)

## Table of contents

### Constructors

- [constructor](CircleEase.md#constructor)

### Properties

- [EASINGMODE\_EASEIN](CircleEase.md#easingmode_easein)
- [EASINGMODE\_EASEINOUT](CircleEase.md#easingmode_easeinout)
- [EASINGMODE\_EASEOUT](CircleEase.md#easingmode_easeout)

### Methods

- [ease](CircleEase.md#ease)
- [getEasingMode](CircleEase.md#geteasingmode)
- [setEasingMode](CircleEase.md#seteasingmode)

## Constructors

### constructor

• **new CircleEase**()

#### Inherited from

[EasingFunction](EasingFunction.md).[constructor](EasingFunction.md#constructor)

## Properties

### EASINGMODE\_EASEIN

▪ `Static` `Readonly` **EASINGMODE\_EASEIN**: ``0``

Interpolation follows the mathematical formula associated with the easing function.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEIN](EasingFunction.md#easingmode_easein)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:28

___

### EASINGMODE\_EASEINOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEINOUT**: ``2``

Interpolation uses EaseIn for the first half of the animation and EaseOut for the second half.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEINOUT](EasingFunction.md#easingmode_easeinout)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:38

___

### EASINGMODE\_EASEOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEOUT**: ``1``

Interpolation follows 100% interpolation minus the output of the formula associated with the easing function.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEOUT](EasingFunction.md#easingmode_easeout)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:33

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

#### Inherited from

[EasingFunction](EasingFunction.md).[ease](EasingFunction.md#ease)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:73

___

### getEasingMode

▸ **getEasingMode**(): `number`

Gets the current easing mode.

#### Returns

`number`

the easing mode

#### Inherited from

[EasingFunction](EasingFunction.md).[getEasingMode](EasingFunction.md#geteasingmode)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:54

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

#### Inherited from

[EasingFunction](EasingFunction.md).[setEasingMode](EasingFunction.md#seteasingmode)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:46

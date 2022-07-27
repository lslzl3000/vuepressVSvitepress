[@dev/core](../README.md) / [Exports](../modules.md) / BounceEase

# Class: BounceEase

Easing function with a bouncing shape (see link below).

**`See`**

 - https://easings.net/#easeInBounce
 - https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Hierarchy

- [`EasingFunction`](EasingFunction.md)

  ↳ **`BounceEase`**

## Implements

- [`IEasingFunction`](../interfaces/IEasingFunction.md)

## Table of contents

### Constructors

- [constructor](BounceEase.md#constructor)

### Properties

- [bounces](BounceEase.md#bounces)
- [bounciness](BounceEase.md#bounciness)
- [EASINGMODE\_EASEIN](BounceEase.md#easingmode_easein)
- [EASINGMODE\_EASEINOUT](BounceEase.md#easingmode_easeinout)
- [EASINGMODE\_EASEOUT](BounceEase.md#easingmode_easeout)

### Methods

- [ease](BounceEase.md#ease)
- [getEasingMode](BounceEase.md#geteasingmode)
- [setEasingMode](BounceEase.md#seteasingmode)

## Constructors

### constructor

• **new BounceEase**(`bounces?`, `bounciness?`)

Instantiates a bounce easing

**`See`**

https://easings.net/#easeInBounce

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `bounces` | `number` | `3` | Defines the number of bounces |
| `bounciness` | `number` | `2` | Defines the amplitude of the bounce |

#### Overrides

[EasingFunction](EasingFunction.md).[constructor](EasingFunction.md#constructor)

#### Defined in

packages/dev/core/src/Animations/easing.ts:145

## Properties

### bounces

• **bounces**: `number` = `3`

#### Defined in

packages/dev/core/src/Animations/easing.ts:147

___

### bounciness

• **bounciness**: `number` = `2`

#### Defined in

packages/dev/core/src/Animations/easing.ts:149

___

### EASINGMODE\_EASEIN

▪ `Static` `Readonly` **EASINGMODE\_EASEIN**: ``0``

Interpolation follows the mathematical formula associated with the easing function.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEIN](EasingFunction.md#easingmode_easein)

#### Defined in

packages/dev/core/src/Animations/easing.ts:28

___

### EASINGMODE\_EASEINOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEINOUT**: ``2``

Interpolation uses EaseIn for the first half of the animation and EaseOut for the second half.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEINOUT](EasingFunction.md#easingmode_easeinout)

#### Defined in

packages/dev/core/src/Animations/easing.ts:38

___

### EASINGMODE\_EASEOUT

▪ `Static` `Readonly` **EASINGMODE\_EASEOUT**: ``1``

Interpolation follows 100% interpolation minus the output of the formula associated with the easing function.

#### Inherited from

[EasingFunction](EasingFunction.md).[EASINGMODE_EASEOUT](EasingFunction.md#easingmode_easeout)

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

#### Inherited from

[EasingFunction](EasingFunction.md).[ease](EasingFunction.md#ease)

#### Defined in

packages/dev/core/src/Animations/easing.ts:73

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

#### Inherited from

[EasingFunction](EasingFunction.md).[setEasingMode](EasingFunction.md#seteasingmode)

#### Defined in

packages/dev/core/src/Animations/easing.ts:46

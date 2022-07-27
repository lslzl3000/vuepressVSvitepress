[@dev/core](../README.md) / [Exports](../modules.md) / PowerEase

# Class: PowerEase

Easing function with a power shape (see link below).

**`See`**

 - https://easings.net/#easeInQuad
 - https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Hierarchy

- [`EasingFunction`](EasingFunction.md)

  ↳ **`PowerEase`**

## Implements

- [`IEasingFunction`](../interfaces/IEasingFunction.md)

## Table of contents

### Constructors

- [constructor](PowerEase.md#constructor)

### Properties

- [power](PowerEase.md#power)
- [EASINGMODE\_EASEIN](PowerEase.md#easingmode_easein)
- [EASINGMODE\_EASEINOUT](PowerEase.md#easingmode_easeinout)
- [EASINGMODE\_EASEOUT](PowerEase.md#easingmode_easeout)

### Methods

- [ease](PowerEase.md#ease)
- [getEasingMode](PowerEase.md#geteasingmode)
- [setEasingMode](PowerEase.md#seteasingmode)

## Constructors

### constructor

• **new PowerEase**(`power?`)

Instantiates an power base easing function

**`See`**

https://easings.net/#easeInQuad

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `power` | `number` | `2` | Defines the power of the function |

#### Overrides

[EasingFunction](EasingFunction.md).[constructor](EasingFunction.md#constructor)

#### Defined in

packages/dev/core/src/Animations/easing.ts:276

## Properties

### power

• **power**: `number` = `2`

#### Defined in

packages/dev/core/src/Animations/easing.ts:278

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

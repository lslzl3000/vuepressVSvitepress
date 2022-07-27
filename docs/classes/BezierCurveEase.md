[@dev/core](../README.md) / [Exports](../modules.md) / BezierCurveEase

# Class: BezierCurveEase

Easing function with a bezier shape (see link below).

**`See`**

 - http://cubic-bezier.com/#.17,.67,.83,.67
 - https://doc.babylonjs.com/divingDeeper/animation/advanced_animations#easing-functions

## Hierarchy

- [`EasingFunction`](EasingFunction.md)

  ↳ **`BezierCurveEase`**

## Implements

- [`IEasingFunction`](../interfaces/IEasingFunction.md)

## Table of contents

### Constructors

- [constructor](BezierCurveEase.md#constructor)

### Properties

- [x1](BezierCurveEase.md#x1)
- [x2](BezierCurveEase.md#x2)
- [y1](BezierCurveEase.md#y1)
- [y2](BezierCurveEase.md#y2)
- [EASINGMODE\_EASEIN](BezierCurveEase.md#easingmode_easein)
- [EASINGMODE\_EASEINOUT](BezierCurveEase.md#easingmode_easeinout)
- [EASINGMODE\_EASEOUT](BezierCurveEase.md#easingmode_easeout)

### Methods

- [ease](BezierCurveEase.md#ease)
- [getEasingMode](BezierCurveEase.md#geteasingmode)
- [setEasingMode](BezierCurveEase.md#seteasingmode)

## Constructors

### constructor

• **new BezierCurveEase**(`x1?`, `y1?`, `x2?`, `y2?`)

Instantiates a bezier function

**`See`**

http://cubic-bezier.com/#.17,.67,.83,.67

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x1` | `number` | `0` | Defines the x component of the start tangent in the bezier curve |
| `y1` | `number` | `0` | Defines the y component of the start tangent in the bezier curve |
| `x2` | `number` | `1` | Defines the x component of the end tangent in the bezier curve |
| `y2` | `number` | `1` | Defines the y component of the end tangent in the bezier curve |

#### Overrides

[EasingFunction](EasingFunction.md).[constructor](EasingFunction.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:367

## Properties

### x1

• **x1**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:369

___

### x2

• **x2**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:373

___

### y1

• **y1**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:371

___

### y2

• **y2**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Animations/easing.ts:375

___

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

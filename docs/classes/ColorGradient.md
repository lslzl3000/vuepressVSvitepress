[@dev/core](../README.md) / [Exports](../modules.md) / ColorGradient

# Class: ColorGradient

Class used to store color4 gradient

## Implements

- [`IValueGradient`](../interfaces/IValueGradient.md)

## Table of contents

### Constructors

- [constructor](ColorGradient.md#constructor)

### Properties

- [color1](ColorGradient.md#color1)
- [color2](ColorGradient.md#color2)
- [gradient](ColorGradient.md#gradient)

### Methods

- [getColorToRef](ColorGradient.md#getcolortoref)

## Constructors

### constructor

• **new ColorGradient**(`gradient`, `color1`, `color2?`)

Creates a new color4 gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | gets or sets the gradient value (between 0 and 1) |
| `color1` | [`Color4`](Color4.md) | gets or sets first associated color |
| `color2?` | [`Color4`](Color4.md) | gets or sets first second color |

#### Defined in

https://github.com/babylon.js/core/src/Misc/gradients.ts:20

## Properties

### color1

• **color1**: [`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/gradients.ts:28

___

### color2

• `Optional` **color2**: [`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/gradients.ts:32

___

### gradient

• **gradient**: `number`

Gets or sets the gradient value (between 0 and 1)

#### Implementation of

[IValueGradient](../interfaces/IValueGradient.md).[gradient](../interfaces/IValueGradient.md#gradient)

#### Defined in

https://github.com/babylon.js/core/src/Misc/gradients.ts:24

## Methods

### getColorToRef

▸ **getColorToRef**(`result`): `void`

Will get a color picked randomly between color1 and color2.
If color2 is undefined then color1 will be used

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Color4`](Color4.md) | defines the target Color4 to store the result in |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/gradients.ts:40

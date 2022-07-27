[@dev/core](../README.md) / [Exports](../modules.md) / GradientBlockColorStep

# Class: GradientBlockColorStep

Class used to store a color step for the GradientBlock

## Table of contents

### Constructors

- [constructor](GradientBlockColorStep.md#constructor)

### Properties

- [\_color](GradientBlockColorStep.md#_color)
- [\_step](GradientBlockColorStep.md#_step)

### Accessors

- [color](GradientBlockColorStep.md#color)
- [step](GradientBlockColorStep.md#step)

## Constructors

### constructor

• **new GradientBlockColorStep**(`step`, `color`)

Creates a new GradientBlockColorStep

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `step` | `number` | defines a value indicating which step this color is associated with (between 0 and 1) |
| `color` | [`Color3`](Color3.md) | defines the color associated with this step |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:51

## Properties

### \_color

• `Private` **\_color**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:30

___

### \_step

• `Private` **\_step**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:15

## Accessors

### color

• `get` **color**(): [`Color3`](Color3.md)

Gets the color associated with this step

#### Returns

[`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:35

• `set` **color**(`val`): `void`

Sets the color associated with this step

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | [`Color3`](Color3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:42

___

### step

• `get` **step**(): `number`

Gets value indicating which step this color is associated with (between 0 and 1)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:19

• `set` **step**(`val`): `void`

Sets a value indicating which step this color is associated with (between 0 and 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/gradientBlock.ts:26

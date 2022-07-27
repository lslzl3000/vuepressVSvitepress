[@dev/core](../README.md) / [Exports](../modules.md) / FactorGradient

# Class: FactorGradient

Class used to store factor gradient

## Implements

- [`IValueGradient`](../interfaces/IValueGradient.md)

## Table of contents

### Constructors

- [constructor](FactorGradient.md#constructor)

### Properties

- [factor1](FactorGradient.md#factor1)
- [factor2](FactorGradient.md#factor2)
- [gradient](FactorGradient.md#gradient)

### Methods

- [getFactor](FactorGradient.md#getfactor)

## Constructors

### constructor

• **new FactorGradient**(`gradient`, `factor1`, `factor2?`)

Creates a new factor gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | gets or sets the gradient value (between 0 and 1) |
| `factor1` | `number` | gets or sets first associated factor |
| `factor2?` | `number` | gets or sets second associated factor |

#### Defined in

packages/dev/core/src/Misc/gradients.ts:77

## Properties

### factor1

• **factor1**: `number`

#### Defined in

packages/dev/core/src/Misc/gradients.ts:85

___

### factor2

• `Optional` **factor2**: `number`

#### Defined in

packages/dev/core/src/Misc/gradients.ts:89

___

### gradient

• **gradient**: `number`

Gets or sets the gradient value (between 0 and 1)

#### Implementation of

[IValueGradient](../interfaces/IValueGradient.md).[gradient](../interfaces/IValueGradient.md#gradient)

#### Defined in

packages/dev/core/src/Misc/gradients.ts:81

## Methods

### getFactor

▸ **getFactor**(): `number`

Will get a number picked randomly between factor1 and factor2.
If factor2 is undefined then factor1 will be used

#### Returns

`number`

the picked number

#### Defined in

packages/dev/core/src/Misc/gradients.ts:97

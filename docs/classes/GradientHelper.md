[@dev/core](../README.md) / [Exports](../modules.md) / GradientHelper

# Class: GradientHelper

Helper used to simplify some generic gradient tasks

## Table of contents

### Constructors

- [constructor](GradientHelper.md#constructor)

### Methods

- [GetCurrentGradient](GradientHelper.md#getcurrentgradient)

## Constructors

### constructor

• **new GradientHelper**()

## Methods

### GetCurrentGradient

▸ `Static` **GetCurrentGradient**(`ratio`, `gradients`, `updateFunc`): `void`

Gets the current gradient from an array of IValueGradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ratio` | `number` | defines the current ratio to get |
| `gradients` | [`IValueGradient`](../interfaces/IValueGradient.md)[] | defines the array of IValueGradient |
| `updateFunc` | (`current`: [`IValueGradient`](../interfaces/IValueGradient.md), `next`: [`IValueGradient`](../interfaces/IValueGradient.md), `scale`: `number`) => `void` | defines the callback function used to get the final value from the selected gradients |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/gradients.ts:116

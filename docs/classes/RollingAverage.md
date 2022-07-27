[@dev/core](../README.md) / [Exports](../modules.md) / RollingAverage

# Class: RollingAverage

RollingAverage

Utility to efficiently compute the rolling average and variance over a sliding window of samples

## Table of contents

### Constructors

- [constructor](RollingAverage.md#constructor)

### Properties

- [\_m2](RollingAverage.md#_m2)
- [\_pos](RollingAverage.md#_pos)
- [\_sampleCount](RollingAverage.md#_samplecount)
- [\_samples](RollingAverage.md#_samples)
- [average](RollingAverage.md#average)
- [variance](RollingAverage.md#variance)

### Methods

- [\_wrapPosition](RollingAverage.md#_wrapposition)
- [add](RollingAverage.md#add)
- [history](RollingAverage.md#history)
- [isSaturated](RollingAverage.md#issaturated)
- [reset](RollingAverage.md#reset)

## Constructors

### constructor

• **new RollingAverage**(`length`)

constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `length` | `number` | The number of samples required to saturate the sliding window |

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:144

## Properties

### \_m2

• `Protected` **\_m2**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:138

___

### \_pos

• `Protected` **\_pos**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:137

___

### \_sampleCount

• `Protected` **\_sampleCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:136

___

### \_samples

• `Protected` **\_samples**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:135

___

### average

• **average**: `number`

Current average

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:129

___

### variance

• **variance**: `number`

Current variance

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:133

## Methods

### \_wrapPosition

▸ `Protected` **_wrapPosition**(`i`): `number`

Wraps a value around the sample range boundaries

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | Position in sample range, for example if the sample length is 5, and i is -3, then 2 will be returned. |

#### Returns

`number`

Wrapped position in sample range

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:220

___

### add

▸ **add**(`v`): `void`

Adds a sample to the sample set

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v` | `number` | The sample value |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:153

___

### history

▸ **history**(`i`): `number`

Returns previously added values or null if outside of history or outside the sliding window domain

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | Index in history. For example, pass 0 for the most recent value and 1 for the value before that |

#### Returns

`number`

Value previously recorded with add() or null if outside of range

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:187

___

### isSaturated

▸ **isSaturated**(): `boolean`

Returns true if enough samples have been taken to completely fill the sliding window

#### Returns

`boolean`

true if sample-set saturated

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:200

___

### reset

▸ **reset**(): `void`

Resets the rolling average (equivalent to 0 samples taken so far)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/performanceMonitor.ts:207

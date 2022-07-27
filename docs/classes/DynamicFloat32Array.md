[@dev/core](../README.md) / [Exports](../modules.md) / DynamicFloat32Array

# Class: DynamicFloat32Array

A class acting as a dynamic float32array used in the performance viewer

## Table of contents

### Constructors

- [constructor](DynamicFloat32Array.md#constructor)

### Properties

- [\_itemLength](DynamicFloat32Array.md#_itemlength)
- [\_view](DynamicFloat32Array.md#_view)

### Accessors

- [itemLength](DynamicFloat32Array.md#itemlength)

### Methods

- [\_growArray](DynamicFloat32Array.md#_growarray)
- [at](DynamicFloat32Array.md#at)
- [push](DynamicFloat32Array.md#push)
- [subarray](DynamicFloat32Array.md#subarray)

## Constructors

### constructor

• **new DynamicFloat32Array**(`itemCapacity`)

Creates a new DynamicFloat32Array with the desired item capacity.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemCapacity` | `number` | The initial item capacity you would like to set for the array. |

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:14

## Properties

### \_itemLength

• `Private` **\_itemLength**: `number`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:8

___

### \_view

• `Private` **\_view**: `Float32Array`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:7

## Accessors

### itemLength

• `get` **itemLength**(): `number`

The number of items currently in the array.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:22

## Methods

### \_growArray

▸ `Private` **_growArray**(): `void`

Grows the array by the growth factor when necessary.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:72

___

### at

▸ **at**(`index`): `number`

Gets value at index, NaN if no such index exists.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | the index to get the value at. |

#### Returns

`number`

the value at the index provided.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:31

___

### push

▸ **push**(`item`): `void`

Pushes items to the end of the array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `number` | The item to push into the array. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:61

___

### subarray

▸ **subarray**(`start`, `end`): `Float32Array`

Gets a view of the original array from start to end (exclusive of end).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | starting index. |
| `end` | `number` | ending index. |

#### Returns

`Float32Array`

a subarray of the original array.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/dynamicFloat32Array.ts:45

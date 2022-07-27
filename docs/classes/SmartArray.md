[@dev/core](../README.md) / [Exports](../modules.md) / SmartArray

# Class: SmartArrayT

Defines an GC Friendly array where the backfield array do not shrink to prevent over allocations.

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- **`SmartArray`**

  ↳ [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)

## Implements

- [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)`T`

## Table of contents

### Constructors

- [constructor](SmartArray.md#constructor)

### Properties

- [\_id](SmartArray.md#_id)
- [data](SmartArray.md#data)
- [length](SmartArray.md#length)
- [\_GlobalId](SmartArray.md#_globalid)

### Methods

- [concat](SmartArray.md#concat)
- [contains](SmartArray.md#contains)
- [dispose](SmartArray.md#dispose)
- [forEach](SmartArray.md#foreach)
- [indexOf](SmartArray.md#indexof)
- [push](SmartArray.md#push)
- [reset](SmartArray.md#reset)
- [sort](SmartArray.md#sort)

## Constructors

### constructor

• **new SmartArray**`T`(`capacity`)

Instantiates a Smart Array.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `capacity` | `number` | defines the default capacity of the array. |

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:36

## Properties

### \_id

• `Protected` **\_id**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:30

___

### data

• **data**: `T`[]

The full set of data from the array.

#### Implementation of

[ISmartArrayLike](../interfaces/ISmartArrayLike.md).[data](../interfaces/ISmartArrayLike.md#data)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:23

___

### length

• **length**: `number` = `0`

The active length of the array.

#### Implementation of

[ISmartArrayLike](../interfaces/ISmartArrayLike.md).[length](../interfaces/ISmartArrayLike.md#length)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:28

___

### \_GlobalId

▪ `Static` `Private` **\_GlobalId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:132

## Methods

### concat

▸ **concat**(`array`): `void`

Concats the active data with a given array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | `any` | defines the data to concatenate with. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:94

___

### contains

▸ **contains**(`value`): `boolean`

Returns whether an element is part of the active data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | defines the value to look for |

#### Returns

`boolean`

true if found in the active data otherwise false

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:127

___

### dispose

▸ **dispose**(): `void`

Releases all the data from the array as well as the array.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:81

___

### forEach

▸ **forEach**(`func`): `void`

Iterates over the active data and apply the lambda to them.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`content`: `T`) => `void` | defines the action to apply on each value. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:57

___

### indexOf

▸ **indexOf**(`value`): `number`

Returns the position of a value in the active data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | defines the value to find the index for |

#### Returns

`number`

the index if found in the active data otherwise -1

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:112

___

### push

▸ **push**(`value`): `void`

Pushes a value at the end of the active data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | defines the object to push in the array. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:45

___

### reset

▸ **reset**(): `void`

Resets the active data to an empty array.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:74

___

### sort

▸ **sort**(`compareFn`): `void`

Sorts the full sets of data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `compareFn` | (`a`: `T`, `b`: `T`) => `number` | defines the comparison function to apply. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:67

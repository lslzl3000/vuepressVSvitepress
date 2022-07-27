[@dev/core](../README.md) / [Exports](../modules.md) / SmartArrayNoDuplicate

# Class: SmartArrayNoDuplicateT

Defines an GC Friendly array where the backfield array do not shrink to prevent over allocations.
The data in this array can only be present once

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`SmartArray`](SmartArray.md)`T`

  ↳ **`SmartArrayNoDuplicate`**

## Table of contents

### Constructors

- [constructor](SmartArrayNoDuplicate.md#constructor)

### Properties

- [\_duplicateId](SmartArrayNoDuplicate.md#_duplicateid)
- [\_id](SmartArrayNoDuplicate.md#_id)
- [data](SmartArrayNoDuplicate.md#data)
- [length](SmartArrayNoDuplicate.md#length)

### Methods

- [concat](SmartArrayNoDuplicate.md#concat)
- [concatWithNoDuplicate](SmartArrayNoDuplicate.md#concatwithnoduplicate)
- [contains](SmartArrayNoDuplicate.md#contains)
- [dispose](SmartArrayNoDuplicate.md#dispose)
- [forEach](SmartArrayNoDuplicate.md#foreach)
- [indexOf](SmartArrayNoDuplicate.md#indexof)
- [push](SmartArrayNoDuplicate.md#push)
- [pushNoDuplicate](SmartArrayNoDuplicate.md#pushnoduplicate)
- [reset](SmartArrayNoDuplicate.md#reset)
- [sort](SmartArrayNoDuplicate.md#sort)

## Constructors

### constructor

• **new SmartArrayNoDuplicate**`T`(`capacity`)

Instantiates a Smart Array.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `capacity` | `number` | defines the default capacity of the array. |

#### Inherited from

[SmartArray](SmartArray.md).[constructor](SmartArray.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:36

## Properties

### \_duplicateId

• `Private` **\_duplicateId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:140

___

### \_id

• `Protected` **\_id**: `number`

#### Inherited from

[SmartArray](SmartArray.md).[_id](SmartArray.md#_id)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:30

___

### data

• **data**: `T`[]

The full set of data from the array.

#### Inherited from

[SmartArray](SmartArray.md).[data](SmartArray.md#data)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:23

___

### length

• **length**: `number` = `0`

The active length of the array.

#### Inherited from

[SmartArray](SmartArray.md).[length](SmartArray.md#length)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:28

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

#### Inherited from

[SmartArray](SmartArray.md).[concat](SmartArray.md#concat)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:94

___

### concatWithNoDuplicate

▸ **concatWithNoDuplicate**(`array`): `void`

Concats the active data with a given array.
This ensures no duplicate will be present in the result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | `any` | defines the data to concatenate with. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:184

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

#### Inherited from

[SmartArray](SmartArray.md).[contains](SmartArray.md#contains)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:127

___

### dispose

▸ **dispose**(): `void`

Releases all the data from the array as well as the array.

#### Returns

`void`

#### Inherited from

[SmartArray](SmartArray.md).[dispose](SmartArray.md#dispose)

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

#### Inherited from

[SmartArray](SmartArray.md).[forEach](SmartArray.md#foreach)

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

#### Inherited from

[SmartArray](SmartArray.md).[indexOf](SmartArray.md#indexof)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:112

___

### push

▸ **push**(`value`): `void`

Pushes a value at the end of the active data.
THIS DOES NOT PREVENT DUPPLICATE DATA

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | defines the object to push in the array. |

#### Returns

`void`

#### Overrides

[SmartArray](SmartArray.md).[push](SmartArray.md#push)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:147

___

### pushNoDuplicate

▸ **pushNoDuplicate**(`value`): `boolean`

Pushes a value at the end of the active data.
If the data is already present, it won t be added again

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | defines the object to push in the array. |

#### Returns

`boolean`

true if added false if it was already present

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:163

___

### reset

▸ **reset**(): `void`

Resets the active data to an empty array.

#### Returns

`void`

#### Overrides

[SmartArray](SmartArray.md).[reset](SmartArray.md#reset)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:174

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

#### Inherited from

[SmartArray](SmartArray.md).[sort](SmartArray.md#sort)

#### Defined in

https://github.com/babylon.js/core/src/Misc/smartArray.ts:67

[@dev/core](../README.md) / [Exports](../modules.md) / StringDictionary

# Class: StringDictionaryT

This class implement a typical dictionary using a string as key and the generic type T as value.
The underlying implementation relies on an associative array to ensure the best performances.
The value can be anything including 'null' but except 'undefined'

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](StringDictionary.md#constructor)

### Properties

- [\_count](StringDictionary.md#_count)
- [\_data](StringDictionary.md#_data)

### Accessors

- [count](StringDictionary.md#count)

### Methods

- [add](StringDictionary.md#add)
- [clear](StringDictionary.md#clear)
- [contains](StringDictionary.md#contains)
- [copyFrom](StringDictionary.md#copyfrom)
- [first](StringDictionary.md#first)
- [forEach](StringDictionary.md#foreach)
- [get](StringDictionary.md#get)
- [getAndRemove](StringDictionary.md#getandremove)
- [getOrAdd](StringDictionary.md#getoradd)
- [getOrAddWithFactory](StringDictionary.md#getoraddwithfactory)
- [remove](StringDictionary.md#remove)
- [set](StringDictionary.md#set)

## Constructors

### constructor

• **new StringDictionary**`T`()

#### Type parameters

| Name |
| :------ |
| `T` |

## Properties

### \_count

• `Private` **\_count**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:182

___

### \_data

• `Private` **\_data**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `T`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:183

## Accessors

### count

• `get` **count**(): `number`

Gets the current count

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:148

## Methods

### add

▸ **add**(`key`, `value`): `boolean`

Add a new key and its corresponding value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the key to add |
| `value` | `T` | the value corresponding to the key |

#### Returns

`boolean`

true if the operation completed successfully, false if we couldn't insert the key/value because there was already this key in the dictionary

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:85

___

### clear

▸ **clear**(): `void`

Clear the whole content of the dictionary

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:140

___

### contains

▸ **contains**(`key`): `boolean`

Check if there's a given key in the dictionary

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the key to check for |

#### Returns

`boolean`

true if the key is present, false otherwise

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:75

___

### copyFrom

▸ **copyFrom**(`source`): `void`

This will clear this dictionary and copy the content from the 'source' one.
If the T value is a custom object, it won't be copied/cloned, the same object will be used

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`StringDictionary`](StringDictionary.md)`T` | the dictionary to take the content from and copy to this dictionary |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:14

___

### first

▸ **first**`TRes`(`callback`): ``null`` \| `TRes`

Execute a callback on every occurrence of the dictionary until it returns a valid TRes object.
If the callback returns null or undefined the method will iterate to the next key/value pair
Note that you can remove any element in this dictionary in the callback implementation

#### Type parameters

| Name |
| :------ |
| `TRes` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`key`: `string`, `val`: `T`) => `TRes` | the callback to execute, if it return a valid T instanced object the enumeration will stop and the object will be returned |

#### Returns

``null`` \| `TRes`

the first item

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:171

___

### forEach

▸ **forEach**(`callback`): `void`

Execute a callback on each key/val of the dictionary.
Note that you can remove any element in this dictionary in the callback implementation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`key`: `string`, `val`: `T`) => `void` | the callback to execute on a given key/value pair |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:157

___

### get

▸ **get**(`key`): `undefined` \| `T`

Get a value based from its key

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the given key to get the matching value from |

#### Returns

`undefined` \| `T`

the value if found, otherwise undefined is returned

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:24

___

### getAndRemove

▸ **getAndRemove**(`key`): [`Nullable`](../modules.md#nullable)`T`

Get the element of the given key and remove it from the dictionary

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | defines the key to search |

#### Returns

[`Nullable`](../modules.md#nullable)`T`

the value associated with the key or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:113

___

### getOrAdd

▸ **getOrAdd**(`key`, `val`): `T`

Get a value from its key if present in the dictionary otherwise add it

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the key to get the value from |
| `val` | `T` | if there's no such key/value pair in the dictionary add it with this value |

#### Returns

`T`

the value corresponding to the key

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:60

___

### getOrAddWithFactory

▸ **getOrAddWithFactory**(`key`, `factory`): `T`

Get a value from its key or add it if it doesn't exist.
This method will ensure you that a given key/data will be present in the dictionary.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the given key to get the matching value from |
| `factory` | (`key`: `string`) => `T` | the factory that will create the value if the key is not present in the dictionary.  The factory will only be invoked if there's no data for the given key. |

#### Returns

`T`

the value corresponding to the key.

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:40

___

### remove

▸ **remove**(`key`): `boolean`

Remove a key/value from the dictionary.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the key to remove |

#### Returns

`boolean`

true if the item was successfully deleted, false if no item with such key exist in the dictionary

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:128

___

### set

▸ **set**(`key`, `value`): `boolean`

Update a specific value associated to a key

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | defines the key to use |
| `value` | `T` | defines the value to store |

#### Returns

`boolean`

true if the value was updated (or false if the key was not found)

#### Defined in

https://github.com/babylon.js/core/src/Misc/stringDictionary.ts:100

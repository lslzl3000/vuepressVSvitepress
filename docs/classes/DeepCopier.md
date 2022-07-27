[@dev/core](../README.md) / [Exports](../modules.md) / DeepCopier

# Class: DeepCopier

Class containing a set of static utilities functions for deep copy.

## Table of contents

### Constructors

- [constructor](DeepCopier.md#constructor)

### Methods

- [DeepCopy](DeepCopier.md#deepcopy)

## Constructors

### constructor

• **new DeepCopier**()

## Methods

### DeepCopy

▸ `Static` **DeepCopy**(`source`, `destination`, `doNotCopyList?`, `mustCopyList?`): `void`

Tries to copy an object by duplicating every property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | defines the source object |
| `destination` | `any` | defines the target object |
| `doNotCopyList?` | `string`[] | defines a list of properties to avoid |
| `mustCopyList?` | `string`[] | defines a list of properties to copy (even if they start with _) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/deepCopier.ts:45

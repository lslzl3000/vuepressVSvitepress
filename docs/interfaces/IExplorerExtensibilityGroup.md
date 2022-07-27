[@dev/core](../README.md) / [Exports](../modules.md) / IExplorerExtensibilityGroup

# Interface: IExplorerExtensibilityGroup

Defines a group of actions associated with a predicate to use when extending the Inspector scene explorer

## Table of contents

### Properties

- [entries](IExplorerExtensibilityGroup.md#entries)
- [predicate](IExplorerExtensibilityGroup.md#predicate)

## Properties

### entries

• **entries**: [`IExplorerExtensibilityOption`](IExplorerExtensibilityOption.md)[]

Gets the list of options added to a type

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:37

___

### predicate

• **predicate**: (`entity`: `any`) => `boolean`

#### Type declaration

▸ (`entity`): `boolean`

Defines a predicate to test if a given type mut be extended

##### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | `any` |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:33

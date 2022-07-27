[@dev/core](../README.md) / [Exports](../modules.md) / IBehaviorAware

# Interface: IBehaviorAwareT

Interface implemented by classes supporting behaviors

## Type parameters

| Name |
| :------ |
| `T` |

## Implemented by

- [`Node`](../classes/Node.md)

## Table of contents

### Methods

- [addBehavior](IBehaviorAware.md#addbehavior)
- [getBehaviorByName](IBehaviorAware.md#getbehaviorbyname)
- [removeBehavior](IBehaviorAware.md#removebehavior)

## Methods

### addBehavior

▸ **addBehavior**(`behavior`): `T`

Attach a behavior

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `behavior` | [`Behavior`](Behavior.md)`T` | defines the behavior to attach |

#### Returns

`T`

the current host

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:34

___

### getBehaviorByName

▸ **getBehaviorByName**(`name`): [`Nullable`](../modules.md#nullable)[`Behavior`](Behavior.md)`T`

Gets a behavior using its name to search

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search |

#### Returns

[`Nullable`](../modules.md#nullable)[`Behavior`](Behavior.md)`T`

the behavior or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:46

___

### removeBehavior

▸ **removeBehavior**(`behavior`): `T`

Remove a behavior from the current object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `behavior` | [`Behavior`](Behavior.md)`T` | defines the behavior to detach |

#### Returns

`T`

the current host

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:40

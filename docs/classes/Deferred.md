[@dev/core](../README.md) / [Exports](../modules.md) / Deferred

# Class: DeferredT

Wrapper class for promise with external resolve and reject.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](Deferred.md#constructor)

### Properties

- [\_reject](Deferred.md#_reject)
- [\_resolve](Deferred.md#_resolve)
- [promise](Deferred.md#promise)

### Accessors

- [reject](Deferred.md#reject)
- [resolve](Deferred.md#resolve)

## Constructors

### constructor

• **new Deferred**`T`()

Constructor for this deferred object.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Defined in

packages/dev/core/src/Misc/deferred.ts:30

## Properties

### \_reject

• `Private` **\_reject**: (`reason?`: `any`) => `void`

#### Type declaration

▸ (`reason?`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/deferred.ts:11

___

### \_resolve

• `Private` **\_resolve**: (`value`: `T` \| `PromiseLike``T`) => `void`

#### Type declaration

▸ (`value`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `T` \| `PromiseLike``T` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/deferred.ts:10

___

### promise

• `Readonly` **promise**: `Promise``T`

The promise associated with this deferred object.

#### Defined in

packages/dev/core/src/Misc/deferred.ts:8

## Accessors

### reject

• `get` **reject**(): (`reason?`: `any`) => `void`

The reject method of the promise associated with this deferred object.

#### Returns

`fn`

▸ (`reason?`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `reason?` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/deferred.ts:23

___

### resolve

• `get` **resolve**(): (`value`: `T` \| `PromiseLike``T`) => `void`

The resolve method of the promise associated with this deferred object.

#### Returns

`fn`

▸ (`value`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `T` \| `PromiseLike``T` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/deferred.ts:16

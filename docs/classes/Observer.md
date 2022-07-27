[@dev/core](../README.md) / [Exports](../modules.md) / Observer

# Class: ObserverT

Represent an Observer registered to a given Observable object.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](Observer.md#constructor)

### Properties

- [callback](Observer.md#callback)
- [mask](Observer.md#mask)
- [scope](Observer.md#scope)
- [unregisterOnNextCall](Observer.md#unregisteronnextcall)

## Constructors

### constructor

• **new Observer**`T`(`callback`, `mask`, `scope?`)

Creates a new observer

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | `undefined` | defines the callback to call when the observer is notified |
| `mask` | `number` | `undefined` | defines the mask of the observer (used to filter notifications) |
| `scope` | `any` | `null` | defines the current scope used to restore the JS context |

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:83

## Properties

### callback

• **callback**: (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void`

#### Type declaration

▸ (`eventData`, `eventState`): `void`

Defines the callback to call when the observer is notified

##### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `T` |
| `eventState` | [`EventState`](EventState.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:87

___

### mask

• **mask**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:91

___

### scope

• **scope**: `any` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:95

___

### unregisterOnNextCall

• **unregisterOnNextCall**: `boolean` = `false`

Gets or sets a property defining that the observer as to be unregistered after the next notification

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:75

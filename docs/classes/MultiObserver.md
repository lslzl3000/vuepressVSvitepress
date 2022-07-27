[@dev/core](../README.md) / [Exports](../modules.md) / MultiObserver

# Class: MultiObserverT

Represent a list of observers registered to multiple Observables object.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](MultiObserver.md#constructor)

### Properties

- [\_observables](MultiObserver.md#_observables)
- [\_observers](MultiObserver.md#_observers)

### Methods

- [dispose](MultiObserver.md#dispose)
- [Watch](MultiObserver.md#watch)

## Constructors

### constructor

• **new MultiObserver**`T`()

#### Type parameters

| Name |
| :------ |
| `T` |

## Properties

### \_observables

• `Private` **\_observables**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md)`T`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:104

___

### \_observers

• `Private` **\_observers**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:103

## Methods

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:109

___

### Watch

▸ `Static` **Watch**`T`(`observables`, `callback`, `mask?`, `scope?`): [`MultiObserver`](MultiObserver.md)`T`

Raise a callback when one of the observable will notify

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `observables` | [`Observable`](Observable.md)`T`[] | `undefined` | defines a list of observables to watch |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | `undefined` | defines the callback to call on notification |
| `mask` | `number` | `-1` | defines the mask used to filter notifications |
| `scope` | `any` | `null` | defines the current scope used to restore the JS context |

#### Returns

[`MultiObserver`](MultiObserver.md)`T`

the new MultiObserver

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:128

[@dev/core](../README.md) / [Exports](../modules.md) / EventState

# Class: EventState

A class serves as a medium between the observable and its observers

## Table of contents

### Constructors

- [constructor](EventState.md#constructor)

### Properties

- [currentTarget](EventState.md#currenttarget)
- [lastReturnValue](EventState.md#lastreturnvalue)
- [mask](EventState.md#mask)
- [skipNextObservers](EventState.md#skipnextobservers)
- [target](EventState.md#target)
- [userInfo](EventState.md#userinfo)

### Methods

- [initialize](EventState.md#initialize)

## Constructors

### constructor

• **new EventState**(`mask`, `skipNextObservers?`, `target?`, `currentTarget?`)

Create a new EventState

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mask` | `number` | `undefined` | defines the mask associated with this state |
| `skipNextObservers` | `boolean` | `false` | defines a flag which will instruct the observable to skip following observers when set to true |
| `target?` | `any` | `undefined` | defines the original target of the state |
| `currentTarget?` | `any` | `undefined` | defines the current target of the state |

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:14

## Properties

### currentTarget

• `Optional` **currentTarget**: `any`

The current object in the bubbling phase

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:52

___

### lastReturnValue

• `Optional` **lastReturnValue**: `any`

This will be populated with the return value of the last function that was executed.
If it is the first function in the callback chain it will be the event data.

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:58

___

### mask

• **mask**: `number`

Get the mask value that were used to trigger the event corresponding to this EventState object

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:42

___

### skipNextObservers

• **skipNextObservers**: `boolean`

An Observer can set this property to true to prevent subsequent observers of being notified

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:37

___

### target

• `Optional` **target**: `any`

The object that originally notified the event

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:47

___

### userInfo

• `Optional` **userInfo**: `any`

User defined information that will be sent to observers

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:63

## Methods

### initialize

▸ **initialize**(`mask`, `skipNextObservers?`, `target?`, `currentTarget?`): [`EventState`](EventState.md)

Initialize the current event state

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mask` | `number` | `undefined` | defines the mask associated with this state |
| `skipNextObservers` | `boolean` | `false` | defines a flag which will instruct the observable to skip following observers when set to true |
| `target?` | `any` | `undefined` | defines the original target of the state |
| `currentTarget?` | `any` | `undefined` | defines the current target of the state |

#### Returns

[`EventState`](EventState.md)

the current event state

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:26

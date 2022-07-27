[@dev/core](../README.md) / [Exports](../modules.md) / AsyncLoop

# Class: AsyncLoop

An implementation of a loop for asynchronous functions.

## Table of contents

### Constructors

- [constructor](AsyncLoop.md#constructor)

### Properties

- [\_done](AsyncLoop.md#_done)
- [\_fn](AsyncLoop.md#_fn)
- [\_successCallback](AsyncLoop.md#_successcallback)
- [index](AsyncLoop.md#index)
- [iterations](AsyncLoop.md#iterations)

### Methods

- [breakLoop](AsyncLoop.md#breakloop)
- [executeNext](AsyncLoop.md#executenext)
- [Run](AsyncLoop.md#run)
- [SyncAsyncForLoop](AsyncLoop.md#syncasyncforloop)

## Constructors

### constructor

• **new AsyncLoop**(`iterations`, `func`, `successCallback`, `offset?`)

Constructor.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `iterations` | `number` | `undefined` | the number of iterations. |
| `func` | (`asyncLoop`: [`AsyncLoop`](AsyncLoop.md)) => `void` | `undefined` | the function to run each iteration |
| `successCallback` | () => `void` | `undefined` | the callback that will be called upon successful execution |
| `offset` | `number` | `0` | starting offset. |

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1367

## Properties

### \_done

• `Private` **\_done**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1356

___

### \_fn

• `Private` **\_fn**: (`asyncLoop`: [`AsyncLoop`](AsyncLoop.md)) => `void`

#### Type declaration

▸ (`asyncLoop`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `asyncLoop` | [`AsyncLoop`](AsyncLoop.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1357

___

### \_successCallback

• `Private` **\_successCallback**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1358

___

### index

• **index**: `number`

Defines the current index of the loop.

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1355

___

### iterations

• **iterations**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1371

## Methods

### breakLoop

▸ **breakLoop**(): `void`

Break the loop and run the success callback.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1399

___

### executeNext

▸ **executeNext**(): `void`

Execute the next iteration. Must be called after the last iteration was finished.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1385

___

### Run

▸ `Static` **Run**(`iterations`, `fn`, `successCallback`, `offset?`): [`AsyncLoop`](AsyncLoop.md)

Create and run an async loop.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `iterations` | `number` | `undefined` | the number of iterations. |
| `fn` | (`asyncLoop`: [`AsyncLoop`](AsyncLoop.md)) => `void` | `undefined` | the function to run each iteration |
| `successCallback` | () => `void` | `undefined` | the callback that will be called upon successful execution |
| `offset` | `number` | `0` | starting offset. |

#### Returns

[`AsyncLoop`](AsyncLoop.md)

the created async loop object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1412

___

### SyncAsyncForLoop

▸ `Static` **SyncAsyncForLoop**(`iterations`, `syncedIterations`, `fn`, `callback`, `breakFunction?`, `timeout?`): [`AsyncLoop`](AsyncLoop.md)

A for-loop that will run a given number of iterations synchronous and the rest async.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `iterations` | `number` | `undefined` | total number of iterations |
| `syncedIterations` | `number` | `undefined` | number of synchronous iterations in each async iteration. |
| `fn` | (`iteration`: `number`) => `void` | `undefined` | the function to call each iteration. |
| `callback` | () => `void` | `undefined` | a success call back that will be called when iterating stops. |
| `breakFunction?` | () => `boolean` | `undefined` | a break condition (optional) |
| `timeout` | `number` | `0` | timeout settings for the setTimeout function. default - 0. |

#### Returns

[`AsyncLoop`](AsyncLoop.md)

the created async loop object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1430

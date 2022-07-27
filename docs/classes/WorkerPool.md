[@dev/core](../README.md) / [Exports](../modules.md) / WorkerPool

# Class: WorkerPool

Helper class to push actions to a pool of workers.

## Hierarchy

- **`WorkerPool`**

  ↳ [`AutoReleaseWorkerPool`](AutoReleaseWorkerPool.md)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WorkerPool.md#constructor)

### Properties

- [\_pendingActions](WorkerPool.md#_pendingactions)
- [\_workerInfos](WorkerPool.md#_workerinfos)

### Methods

- [\_execute](WorkerPool.md#_execute)
- [\_executeOnIdleWorker](WorkerPool.md#_executeonidleworker)
- [dispose](WorkerPool.md#dispose)
- [push](WorkerPool.md#push)

## Constructors

### constructor

• **new WorkerPool**(`workers`)

Constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workers` | `Worker`[] | Array of workers to use for actions |

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:21

## Properties

### \_pendingActions

• `Protected` **\_pendingActions**: (`worker`: `Worker`, `onComplete`: () => `void`) => `void`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:15

___

### \_workerInfos

• `Protected` **\_workerInfos**: `WorkerInfo`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:14

## Methods

### \_execute

▸ `Protected` **_execute**(`workerInfo`, `action`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `workerInfo` | `WorkerInfo` |
| `action` | (`worker`: `Worker`, `onComplete`: () => `void`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:64

___

### \_executeOnIdleWorker

▸ `Protected` **_executeOnIdleWorker**(`action`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `action` | (`worker`: `Worker`, `onComplete`: () => `void`) => `void` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:53

___

### dispose

▸ **dispose**(): `void`

Terminates all workers and clears any pending actions.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:31

___

### push

▸ **push**(`action`): `void`

Pushes an action to the worker pool. If all the workers are active, the action will be
pended until a worker has completed its action.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | (`worker`: `Worker`, `onComplete`: () => `void`) => `void` | The action to perform. Call onComplete when the action is complete. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/workerPool.ts:47

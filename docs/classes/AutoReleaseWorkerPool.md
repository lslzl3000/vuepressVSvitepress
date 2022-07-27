[@dev/core](../README.md) / [Exports](../modules.md) / AutoReleaseWorkerPool

# Class: AutoReleaseWorkerPool

Similar to the WorkerPool class except it creates and destroys workers automatically with a maximum of `maxWorkers` workers.
Workers are terminated when it is idle for at least `idleTimeElapsedBeforeRelease` milliseconds.

## Hierarchy

- [`WorkerPool`](WorkerPool.md)

  ↳ **`AutoReleaseWorkerPool`**

## Table of contents

### Constructors

- [constructor](AutoReleaseWorkerPool.md#constructor)

### Properties

- [\_createWorkerAsync](AutoReleaseWorkerPool.md#_createworkerasync)
- [\_maxWorkers](AutoReleaseWorkerPool.md#_maxworkers)
- [\_options](AutoReleaseWorkerPool.md#_options)
- [\_pendingActions](AutoReleaseWorkerPool.md#_pendingactions)
- [\_workerInfos](AutoReleaseWorkerPool.md#_workerinfos)
- [DefaultOptions](AutoReleaseWorkerPool.md#defaultoptions)

### Methods

- [\_execute](AutoReleaseWorkerPool.md#_execute)
- [\_executeOnIdleWorker](AutoReleaseWorkerPool.md#_executeonidleworker)
- [dispose](AutoReleaseWorkerPool.md#dispose)
- [push](AutoReleaseWorkerPool.md#push)

## Constructors

### constructor

• **new AutoReleaseWorkerPool**(`maxWorkers`, `createWorkerAsync`, `options?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `maxWorkers` | `number` | `undefined` |
| `createWorkerAsync` | () => `Promise``Worker` | `undefined` |
| `options` | [`AutoReleaseWorkerPoolOptions`](../interfaces/AutoReleaseWorkerPoolOptions.md) | `AutoReleaseWorkerPool.DefaultOptions` |

#### Overrides

[WorkerPool](WorkerPool.md).[constructor](WorkerPool.md#constructor)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:106

## Properties

### \_createWorkerAsync

• `Private` `Readonly` **\_createWorkerAsync**: () => `Promise``Worker`

#### Type declaration

▸ (): `Promise``Worker`

##### Returns

`Promise``Worker`

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:103

___

### \_maxWorkers

• `Private` `Readonly` **\_maxWorkers**: `number`

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:102

___

### \_options

• `Private` `Readonly` **\_options**: [`AutoReleaseWorkerPoolOptions`](../interfaces/AutoReleaseWorkerPoolOptions.md)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:104

___

### \_pendingActions

• `Protected` **\_pendingActions**: (`worker`: `Worker`, `onComplete`: () => `void`) => `void`[]

#### Inherited from

[WorkerPool](WorkerPool.md).[_pendingActions](WorkerPool.md#_pendingactions)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:15

___

### \_workerInfos

• `Protected` **\_workerInfos**: `WorkerInfo`[]

#### Inherited from

[WorkerPool](WorkerPool.md).[_workerInfos](WorkerPool.md#_workerinfos)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:14

___

### DefaultOptions

▪ `Static` **DefaultOptions**: [`AutoReleaseWorkerPoolOptions`](../interfaces/AutoReleaseWorkerPoolOptions.md)

Default options for the constructor.
Override to change the defaults.

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:98

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

#### Overrides

[WorkerPool](WorkerPool.md).[_execute](WorkerPool.md#_execute)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:129

___

### \_executeOnIdleWorker

▸ `Protected` **_executeOnIdleWorker**(`action`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `action` | (`worker`: `Worker`, `onComplete`: () => `void`) => `void` |

#### Returns

`boolean`

#### Inherited from

[WorkerPool](WorkerPool.md).[_executeOnIdleWorker](WorkerPool.md#_executeonidleworker)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:53

___

### dispose

▸ **dispose**(): `void`

Terminates all workers and clears any pending actions.

#### Returns

`void`

#### Inherited from

[WorkerPool](WorkerPool.md).[dispose](WorkerPool.md#dispose)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:31

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

#### Overrides

[WorkerPool](WorkerPool.md).[push](WorkerPool.md#push)

#### Defined in

packages/dev/core/src/Misc/workerPool.ts:114

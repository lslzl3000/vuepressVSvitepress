[@dev/core](../README.md) / [Exports](../modules.md) / BinaryFileAssetTask

# Class: BinaryFileAssetTask

Define a task used by AssetsManager to load binary data

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`BinaryFileAssetTask`**

## Table of contents

### Constructors

- [constructor](BinaryFileAssetTask.md#constructor)

### Properties

- [data](BinaryFileAssetTask.md#data)
- [name](BinaryFileAssetTask.md#name)
- [onError](BinaryFileAssetTask.md#onerror)
- [onSuccess](BinaryFileAssetTask.md#onsuccess)
- [url](BinaryFileAssetTask.md#url)

### Accessors

- [errorObject](BinaryFileAssetTask.md#errorobject)
- [isCompleted](BinaryFileAssetTask.md#iscompleted)
- [taskState](BinaryFileAssetTask.md#taskstate)

### Methods

- [reset](BinaryFileAssetTask.md#reset)
- [run](BinaryFileAssetTask.md#run)
- [runTask](BinaryFileAssetTask.md#runtask)

## Constructors

### constructor

• **new BinaryFileAssetTask**(`name`, `url`)

Creates a new BinaryFileAssetTask object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the new task |
| `url` | `string` | defines the location of the file to load |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:484

## Properties

### data

• **data**: `ArrayBuffer`

Gets the loaded data (as an array buffer)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:468

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:488

___

### onError

• **onError**: (`task`: [`BinaryFileAssetTask`](BinaryFileAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`BinaryFileAssetTask`](BinaryFileAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:477

___

### onSuccess

• **onSuccess**: (`task`: [`BinaryFileAssetTask`](BinaryFileAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`BinaryFileAssetTask`](BinaryFileAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:473

___

### url

• **url**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:492

## Accessors

### errorObject

• `get` **errorObject**(): `Object`

Gets the current error object (if task is in error)

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `exception?` | `any` |
| `message?` | `string` |

#### Inherited from

AbstractAssetTask.errorObject

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:85

___

### isCompleted

• `get` **isCompleted**(): `boolean`

Get if the task is completed

#### Returns

`boolean`

#### Inherited from

AbstractAssetTask.isCompleted

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:71

___

### taskState

• `get` **taskState**(): [`AssetTaskState`](../enums/AssetTaskState.md)

Gets the current state of the task

#### Returns

[`AssetTaskState`](../enums/AssetTaskState.md)

#### Inherited from

AbstractAssetTask.taskState

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:78

## Methods

### reset

▸ **reset**(): `void`

Reset will set the task state back to INIT, so the next load call of the assets manager will execute this task again.
This can be used with failed tasks that have the reason for failure fixed.

#### Returns

`void`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[reset](AbstractAssetTask.md#reset)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:140

___

### run

▸ **run**(`scene`, `onSuccess`, `onError`): `void`

Execute the current task

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene where you want your assets to be loaded |
| `onSuccess` | () => `void` | is a callback called when the task is successfully executed |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` | is a callback called if an error occurs |

#### Returns

`void`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[run](AbstractAssetTask.md#run)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:112

___

### runTask

▸ **runTask**(`scene`, `onSuccess`, `onError`): `void`

Execute the current task

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene where you want your assets to be loaded |
| `onSuccess` | () => `void` | is a callback called when the task is successfully executed |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` | is a callback called if an error occurs |

#### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[runTask](AbstractAssetTask.md#runtask)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:503

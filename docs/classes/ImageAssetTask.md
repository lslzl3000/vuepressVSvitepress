[@dev/core](../README.md) / [Exports](../modules.md) / ImageAssetTask

# Class: ImageAssetTask

Define a task used by AssetsManager to load images

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`ImageAssetTask`**

## Table of contents

### Constructors

- [constructor](ImageAssetTask.md#constructor)

### Properties

- [image](ImageAssetTask.md#image)
- [name](ImageAssetTask.md#name)
- [onError](ImageAssetTask.md#onerror)
- [onSuccess](ImageAssetTask.md#onsuccess)
- [url](ImageAssetTask.md#url)

### Accessors

- [errorObject](ImageAssetTask.md#errorobject)
- [isCompleted](ImageAssetTask.md#iscompleted)
- [taskState](ImageAssetTask.md#taskstate)

### Methods

- [reset](ImageAssetTask.md#reset)
- [run](ImageAssetTask.md#run)
- [runTask](ImageAssetTask.md#runtask)

## Constructors

### constructor

• **new ImageAssetTask**(`name`, `url`)

Creates a new ImageAssetTask

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the task |
| `url` | `string` | defines the location of the image to load |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:545

## Properties

### image

• **image**: `HTMLImageElement`

Gets the loaded images

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:529

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:549

___

### onError

• **onError**: (`task`: [`ImageAssetTask`](ImageAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`ImageAssetTask`](ImageAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:538

___

### onSuccess

• **onSuccess**: (`task`: [`ImageAssetTask`](ImageAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`ImageAssetTask`](ImageAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:534

___

### url

• **url**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:553

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

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:564

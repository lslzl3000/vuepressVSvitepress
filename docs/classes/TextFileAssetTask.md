[@dev/core](../README.md) / [Exports](../modules.md) / TextFileAssetTask

# Class: TextFileAssetTask

Define a task used by AssetsManager to load text content

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`TextFileAssetTask`**

## Table of contents

### Constructors

- [constructor](TextFileAssetTask.md#constructor)

### Properties

- [name](TextFileAssetTask.md#name)
- [onError](TextFileAssetTask.md#onerror)
- [onSuccess](TextFileAssetTask.md#onsuccess)
- [text](TextFileAssetTask.md#text)
- [url](TextFileAssetTask.md#url)

### Accessors

- [errorObject](TextFileAssetTask.md#errorobject)
- [isCompleted](TextFileAssetTask.md#iscompleted)
- [taskState](TextFileAssetTask.md#taskstate)

### Methods

- [reset](TextFileAssetTask.md#reset)
- [run](TextFileAssetTask.md#run)
- [runTask](TextFileAssetTask.md#runtask)

## Constructors

### constructor

• **new TextFileAssetTask**(`name`, `url`)

Creates a new TextFileAssetTask object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the task |
| `url` | `string` | defines the location of the file to load |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:423

## Properties

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:427

___

### onError

• **onError**: (`task`: [`TextFileAssetTask`](TextFileAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`TextFileAssetTask`](TextFileAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:416

___

### onSuccess

• **onSuccess**: (`task`: [`TextFileAssetTask`](TextFileAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`TextFileAssetTask`](TextFileAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:411

___

### text

• **text**: `string`

Gets the loaded text string

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:406

___

### url

• **url**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:431

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

packages/dev/core/src/Misc/assetsManager.ts:85

___

### isCompleted

• `get` **isCompleted**(): `boolean`

Get if the task is completed

#### Returns

`boolean`

#### Inherited from

AbstractAssetTask.isCompleted

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:71

___

### taskState

• `get` **taskState**(): [`AssetTaskState`](../enums/AssetTaskState.md)

Gets the current state of the task

#### Returns

[`AssetTaskState`](../enums/AssetTaskState.md)

#### Inherited from

AbstractAssetTask.taskState

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:78

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

packages/dev/core/src/Misc/assetsManager.ts:140

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

packages/dev/core/src/Misc/assetsManager.ts:112

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

packages/dev/core/src/Misc/assetsManager.ts:442

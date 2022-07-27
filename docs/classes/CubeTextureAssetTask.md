[@dev/core](../README.md) / [Exports](../modules.md) / CubeTextureAssetTask

# Class: CubeTextureAssetTask

Define a task used by AssetsManager to load cube textures

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`CubeTextureAssetTask`**

## Implements

- [`ITextureAssetTask`](../interfaces/ITextureAssetTask.md)[`CubeTexture`](CubeTexture.md)

## Table of contents

### Constructors

- [constructor](CubeTextureAssetTask.md#constructor)

### Properties

- [extensions](CubeTextureAssetTask.md#extensions)
- [files](CubeTextureAssetTask.md#files)
- [name](CubeTextureAssetTask.md#name)
- [noMipmap](CubeTextureAssetTask.md#nomipmap)
- [onError](CubeTextureAssetTask.md#onerror)
- [onSuccess](CubeTextureAssetTask.md#onsuccess)
- [prefiltered](CubeTextureAssetTask.md#prefiltered)
- [texture](CubeTextureAssetTask.md#texture)
- [url](CubeTextureAssetTask.md#url)

### Accessors

- [errorObject](CubeTextureAssetTask.md#errorobject)
- [isCompleted](CubeTextureAssetTask.md#iscompleted)
- [taskState](CubeTextureAssetTask.md#taskstate)

### Methods

- [reset](CubeTextureAssetTask.md#reset)
- [run](CubeTextureAssetTask.md#run)
- [runTask](CubeTextureAssetTask.md#runtask)

## Constructors

### constructor

• **new CubeTextureAssetTask**(`name`, `url`, `extensions?`, `noMipmap?`, `files?`, `prefiltered?`)

Creates a new CubeTextureAssetTask

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the task |
| `url` | `string` | defines the location of the files to load (You have to specify the folder where the files are + filename with no extension) |
| `extensions?` | `string`[] | defines the extensions to use to load files (["_px", "_py", "_pz", "_nx", "_ny", "_nz"] by default) |
| `noMipmap?` | `boolean` | defines if mipmaps should not be generated (default is false) |
| `files?` | `string`[] | defines the explicit list of files (undefined by default) |
| `prefiltered?` | `boolean` |  |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:689

## Properties

### extensions

• `Optional` **extensions**: `string`[]

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:701

___

### files

• `Optional` **files**: `string`[]

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:709

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:693

___

### noMipmap

• `Optional` **noMipmap**: `boolean`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:705

___

### onError

• **onError**: (`task`: [`CubeTextureAssetTask`](CubeTextureAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`CubeTextureAssetTask`](CubeTextureAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:678

___

### onSuccess

• **onSuccess**: (`task`: [`CubeTextureAssetTask`](CubeTextureAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`CubeTextureAssetTask`](CubeTextureAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:674

___

### prefiltered

• `Optional` **prefiltered**: `boolean`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:713

___

### texture

• **texture**: [`CubeTexture`](CubeTexture.md)

Gets the loaded texture

#### Implementation of

[ITextureAssetTask](../interfaces/ITextureAssetTask.md).[texture](../interfaces/ITextureAssetTask.md#texture)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:669

___

### url

• **url**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:697

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

packages/dev/core/src/Misc/assetsManager.ts:724

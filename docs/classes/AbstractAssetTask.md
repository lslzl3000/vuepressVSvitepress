[@dev/core](../README.md) / [Exports](../modules.md) / AbstractAssetTask

# Class: AbstractAssetTask

Define an abstract asset task used with a AssetsManager class to load assets into a scene

## Hierarchy

- **`AbstractAssetTask`**

  ↳ [`ContainerAssetTask`](ContainerAssetTask.md)

  ↳ [`MeshAssetTask`](MeshAssetTask.md)

  ↳ [`TextFileAssetTask`](TextFileAssetTask.md)

  ↳ [`BinaryFileAssetTask`](BinaryFileAssetTask.md)

  ↳ [`ImageAssetTask`](ImageAssetTask.md)

  ↳ [`TextureAssetTask`](TextureAssetTask.md)

  ↳ [`CubeTextureAssetTask`](CubeTextureAssetTask.md)

  ↳ [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md)

  ↳ [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md)

## Table of contents

### Constructors

- [constructor](AbstractAssetTask.md#constructor)

### Properties

- [\_errorObject](AbstractAssetTask.md#_errorobject)
- [\_isCompleted](AbstractAssetTask.md#_iscompleted)
- [\_taskState](AbstractAssetTask.md#_taskstate)
- [name](AbstractAssetTask.md#name)
- [onError](AbstractAssetTask.md#onerror)
- [onSuccess](AbstractAssetTask.md#onsuccess)

### Accessors

- [errorObject](AbstractAssetTask.md#errorobject)
- [isCompleted](AbstractAssetTask.md#iscompleted)
- [taskState](AbstractAssetTask.md#taskstate)

### Methods

- [\_onDoneCallback](AbstractAssetTask.md#_ondonecallback)
- [\_onErrorCallback](AbstractAssetTask.md#_onerrorcallback)
- [reset](AbstractAssetTask.md#reset)
- [run](AbstractAssetTask.md#run)
- [runTask](AbstractAssetTask.md#runtask)

## Constructors

### constructor

• **new AbstractAssetTask**(`name`)

Creates a new AssetsManager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the task |

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:58

## Properties

### \_errorObject

• `Private` **\_errorObject**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `exception?` | `any` |
| `message?` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:66

___

### \_isCompleted

• `Private` **\_isCompleted**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:64

___

### \_taskState

• `Private` **\_taskState**: [`AssetTaskState`](../enums/AssetTaskState.md) = `AssetTaskState.INIT`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:65

___

### name

• **name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:61

___

### onError

• **onError**: (`task`: `any`, `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is not successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | `any` |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:52

___

### onSuccess

• **onSuccess**: (`task`: `any`) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | `any` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:47

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

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:85

___

### isCompleted

• `get` **isCompleted**(): `boolean`

Get if the task is completed

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:71

___

### taskState

• `get` **taskState**(): [`AssetTaskState`](../enums/AssetTaskState.md)

Gets the current state of the task

#### Returns

[`AssetTaskState`](../enums/AssetTaskState.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:78

## Methods

### \_onDoneCallback

▸ `Private` **_onDoneCallback**(`onSuccess`, `onError`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `onSuccess` | () => `void` |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:159

___

### \_onErrorCallback

▸ `Private` **_onErrorCallback**(`onError`, `message?`, `exception?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` |
| `message?` | `string` |
| `exception?` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:144

___

### reset

▸ **reset**(): `void`

Reset will set the task state back to INIT, so the next load call of the assets manager will execute this task again.
This can be used with failed tasks that have the reason for failure fixed.

#### Returns

`void`

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

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:132

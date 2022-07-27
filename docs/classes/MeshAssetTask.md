[@dev/core](../README.md) / [Exports](../modules.md) / MeshAssetTask

# Class: MeshAssetTask

Define a task used by AssetsManager to load meshes

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`MeshAssetTask`**

## Table of contents

### Constructors

- [constructor](MeshAssetTask.md#constructor)

### Properties

- [loadedAnimationGroups](MeshAssetTask.md#loadedanimationgroups)
- [loadedMeshes](MeshAssetTask.md#loadedmeshes)
- [loadedParticleSystems](MeshAssetTask.md#loadedparticlesystems)
- [loadedSkeletons](MeshAssetTask.md#loadedskeletons)
- [meshesNames](MeshAssetTask.md#meshesnames)
- [name](MeshAssetTask.md#name)
- [onError](MeshAssetTask.md#onerror)
- [onSuccess](MeshAssetTask.md#onsuccess)
- [rootUrl](MeshAssetTask.md#rooturl)
- [sceneFilename](MeshAssetTask.md#scenefilename)

### Accessors

- [errorObject](MeshAssetTask.md#errorobject)
- [isCompleted](MeshAssetTask.md#iscompleted)
- [taskState](MeshAssetTask.md#taskstate)

### Methods

- [reset](MeshAssetTask.md#reset)
- [run](MeshAssetTask.md#run)
- [runTask](MeshAssetTask.md#runtask)

## Constructors

### constructor

• **new MeshAssetTask**(`name`, `meshesNames`, `rootUrl`, `sceneFilename`)

Creates a new MeshAssetTask

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the task |
| `meshesNames` | `any` | defines the list of mesh's names you want to load |
| `rootUrl` | `string` | defines the root url to use as a base to load your meshes and associated resources |
| `sceneFilename` | `string` \| `File` | defines the filename or File of the scene to load from |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:351

## Properties

### loadedAnimationGroups

• **loadedAnimationGroups**: [`AnimationGroup`](AnimationGroup.md)[]

Gets the list of loaded animation groups

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:332

___

### loadedMeshes

• **loadedMeshes**: [`AbstractMesh`](AbstractMesh.md)[]

Gets the list of loaded meshes

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:320

___

### loadedParticleSystems

• **loadedParticleSystems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

Gets the list of loaded particle systems

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:324

___

### loadedSkeletons

• **loadedSkeletons**: [`Skeleton`](Skeleton.md)[]

Gets the list of loaded skeletons

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:328

___

### meshesNames

• **meshesNames**: `any`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:359

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:355

___

### onError

• **onError**: (`task`: [`MeshAssetTask`](MeshAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`MeshAssetTask`](MeshAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:342

___

### onSuccess

• **onSuccess**: (`task`: [`MeshAssetTask`](MeshAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`MeshAssetTask`](MeshAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:337

___

### rootUrl

• **rootUrl**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:363

___

### sceneFilename

• **sceneFilename**: `string` \| `File`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:367

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

packages/dev/core/src/Misc/assetsManager.ts:378

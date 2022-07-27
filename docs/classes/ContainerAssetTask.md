[@dev/core](../README.md) / [Exports](../modules.md) / ContainerAssetTask

# Class: ContainerAssetTask

Define a task used by AssetsManager to load assets into a container

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`ContainerAssetTask`**

## Table of contents

### Constructors

- [constructor](ContainerAssetTask.md#constructor)

### Properties

- [loadedAnimationGroups](ContainerAssetTask.md#loadedanimationgroups)
- [loadedContainer](ContainerAssetTask.md#loadedcontainer)
- [loadedMeshes](ContainerAssetTask.md#loadedmeshes)
- [loadedParticleSystems](ContainerAssetTask.md#loadedparticlesystems)
- [loadedSkeletons](ContainerAssetTask.md#loadedskeletons)
- [meshesNames](ContainerAssetTask.md#meshesnames)
- [name](ContainerAssetTask.md#name)
- [onError](ContainerAssetTask.md#onerror)
- [onSuccess](ContainerAssetTask.md#onsuccess)
- [rootUrl](ContainerAssetTask.md#rooturl)
- [sceneFilename](ContainerAssetTask.md#scenefilename)

### Accessors

- [errorObject](ContainerAssetTask.md#errorobject)
- [isCompleted](ContainerAssetTask.md#iscompleted)
- [taskState](ContainerAssetTask.md#taskstate)

### Methods

- [reset](ContainerAssetTask.md#reset)
- [run](ContainerAssetTask.md#run)
- [runTask](ContainerAssetTask.md#runtask)

## Constructors

### constructor

• **new ContainerAssetTask**(`name`, `meshesNames`, `rootUrl`, `sceneFilename`)

Creates a new ContainerAssetTask

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

packages/dev/core/src/Misc/assetsManager.ts:265

## Properties

### loadedAnimationGroups

• **loadedAnimationGroups**: [`AnimationGroup`](AnimationGroup.md)[]

Gets the list of loaded animation groups

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:246

___

### loadedContainer

• **loadedContainer**: [`AssetContainer`](AssetContainer.md)

Get the loaded asset container

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:230

___

### loadedMeshes

• **loadedMeshes**: [`AbstractMesh`](AbstractMesh.md)[]

Gets the list of loaded meshes

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:234

___

### loadedParticleSystems

• **loadedParticleSystems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

Gets the list of loaded particle systems

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:238

___

### loadedSkeletons

• **loadedSkeletons**: [`Skeleton`](Skeleton.md)[]

Gets the list of loaded skeletons

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:242

___

### meshesNames

• **meshesNames**: `any`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:273

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:269

___

### onError

• **onError**: (`task`: [`ContainerAssetTask`](ContainerAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`ContainerAssetTask`](ContainerAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:256

___

### onSuccess

• **onSuccess**: (`task`: [`ContainerAssetTask`](ContainerAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`ContainerAssetTask`](ContainerAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:251

___

### rootUrl

• **rootUrl**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:277

___

### sceneFilename

• **sceneFilename**: `string` \| `File`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:281

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

packages/dev/core/src/Misc/assetsManager.ts:292

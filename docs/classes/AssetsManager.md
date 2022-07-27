[@dev/core](../README.md) / [Exports](../modules.md) / AssetsManager

# Class: AssetsManager

This class can be used to easily import assets into a scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_assetsmanager

## Table of contents

### Constructors

- [constructor](AssetsManager.md#constructor)

### Properties

- [\_isLoading](AssetsManager.md#_isloading)
- [\_scene](AssetsManager.md#_scene)
- [\_tasks](AssetsManager.md#_tasks)
- [\_totalTasksCount](AssetsManager.md#_totaltaskscount)
- [\_waitingTasksCount](AssetsManager.md#_waitingtaskscount)
- [autoHideLoadingUI](AssetsManager.md#autohideloadingui)
- [onFinish](AssetsManager.md#onfinish)
- [onProgress](AssetsManager.md#onprogress)
- [onProgressObservable](AssetsManager.md#onprogressobservable)
- [onTaskError](AssetsManager.md#ontaskerror)
- [onTaskErrorObservable](AssetsManager.md#ontaskerrorobservable)
- [onTaskSuccess](AssetsManager.md#ontasksuccess)
- [onTaskSuccessObservable](AssetsManager.md#ontasksuccessobservable)
- [onTasksDoneObservable](AssetsManager.md#ontasksdoneobservable)
- [useDefaultLoadingScreen](AssetsManager.md#usedefaultloadingscreen)

### Methods

- [\_decreaseWaitingTasksCount](AssetsManager.md#_decreasewaitingtaskscount)
- [\_formatTaskErrorMessage](AssetsManager.md#_formattaskerrormessage)
- [\_runTask](AssetsManager.md#_runtask)
- [addBinaryFileTask](AssetsManager.md#addbinaryfiletask)
- [addContainerTask](AssetsManager.md#addcontainertask)
- [addCubeTextureTask](AssetsManager.md#addcubetexturetask)
- [addEquiRectangularCubeTextureAssetTask](AssetsManager.md#addequirectangularcubetextureassettask)
- [addHDRCubeTextureTask](AssetsManager.md#addhdrcubetexturetask)
- [addImageTask](AssetsManager.md#addimagetask)
- [addMeshTask](AssetsManager.md#addmeshtask)
- [addTextFileTask](AssetsManager.md#addtextfiletask)
- [addTextureTask](AssetsManager.md#addtexturetask)
- [load](AssetsManager.md#load)
- [loadAsync](AssetsManager.md#loadasync)
- [removeTask](AssetsManager.md#removetask)
- [reset](AssetsManager.md#reset)

## Constructors

### constructor

• **new AssetsManager**(`scene?`)

Creates a new AssetsManager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | defines the scene to work on |

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:960

## Properties

### \_isLoading

• `Private` **\_isLoading**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:897

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:896

___

### \_tasks

• `Protected` **\_tasks**: [`AbstractAssetTask`](AbstractAssetTask.md)[]

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:899

___

### \_totalTasksCount

• `Protected` **\_totalTasksCount**: `number` = `0`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:901

___

### \_waitingTasksCount

• `Protected` **\_waitingTasksCount**: `number` = `0`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:900

___

### autoHideLoadingUI

• **autoHideLoadingUI**: `boolean` = `true`

Gets or sets a boolean defining if the AssetsManager should automatically hide the loading screen
when all assets have been downloaded.
If set to false, you need to manually call in hideLoadingUI() once your scene is ready.

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:954

___

### onFinish

• **onFinish**: (`tasks`: [`AbstractAssetTask`](AbstractAssetTask.md)[]) => `void`

#### Type declaration

▸ (`tasks`): `void`

Callback called when all tasks are processed

##### Parameters

| Name | Type |
| :------ | :------ |
| `tasks` | [`AbstractAssetTask`](AbstractAssetTask.md)[] |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:906

___

### onProgress

• **onProgress**: (`remainingCount`: `number`, `totalCount`: `number`, `task`: [`AbstractAssetTask`](AbstractAssetTask.md)) => `void`

#### Type declaration

▸ (`remainingCount`, `totalCount`, `task`): `void`

Callback called when a task is done (whatever the result is)

##### Parameters

| Name | Type |
| :------ | :------ |
| `remainingCount` | `number` |
| `totalCount` | `number` |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:921

___

### onProgressObservable

• **onProgressObservable**: [`Observable`](Observable.md)[`IAssetsProgressEvent`](../interfaces/IAssetsProgressEvent.md)

Observable called when a task is done (whatever the result is)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:941

___

### onTaskError

• **onTaskError**: (`task`: [`AbstractAssetTask`](AbstractAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when a task had an error

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:916

___

### onTaskErrorObservable

• **onTaskErrorObservable**: [`Observable`](Observable.md)[`AbstractAssetTask`](AbstractAssetTask.md)

Observable called when a task had an error

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:931

___

### onTaskSuccess

• **onTaskSuccess**: (`task`: [`AbstractAssetTask`](AbstractAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when a task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:911

___

### onTaskSuccessObservable

• **onTaskSuccessObservable**: [`Observable`](Observable.md)[`AbstractAssetTask`](AbstractAssetTask.md)

Observable called when all tasks are processed

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:926

___

### onTasksDoneObservable

• **onTasksDoneObservable**: [`Observable`](Observable.md)[`AbstractAssetTask`](AbstractAssetTask.md)[]

Observable called when all tasks were executed

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:936

___

### useDefaultLoadingScreen

• **useDefaultLoadingScreen**: `boolean` = `true`

Gets or sets a boolean defining if the AssetsManager should use the default loading screen

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:947

## Methods

### \_decreaseWaitingTasksCount

▸ `Private` **_decreaseWaitingTasksCount**(`task`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1123

___

### \_formatTaskErrorMessage

▸ `Private` **_formatTaskErrorMessage**(`task`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

#### Returns

`string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1197

___

### \_runTask

▸ `Private` **_runTask**(`task`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1169

___

### addBinaryFileTask

▸ **addBinaryFileTask**(`taskName`, `url`): [`BinaryFileAssetTask`](BinaryFileAssetTask.md)

Add a BinaryFileAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `url` | `string` | defines the url of the file to load |

#### Returns

[`BinaryFileAssetTask`](BinaryFileAssetTask.md)

a new BinaryFileAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1013

___

### addContainerTask

▸ **addContainerTask**(`taskName`, `meshesNames`, `rootUrl`, `sceneFilename`): [`ContainerAssetTask`](ContainerAssetTask.md)

Add a ContainerAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `meshesNames` | `any` | defines the name of meshes to load |
| `rootUrl` | `string` | defines the root url to use to locate files |
| `sceneFilename` | `string` \| `File` | defines the filename of the scene file or the File itself |

#### Returns

[`ContainerAssetTask`](ContainerAssetTask.md)

a new ContainerAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:972

___

### addCubeTextureTask

▸ **addCubeTextureTask**(`taskName`, `url`, `extensions?`, `noMipmap?`, `files?`, `prefiltered?`): [`CubeTextureAssetTask`](CubeTextureAssetTask.md)

Add a CubeTextureAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `url` | `string` | defines the url of the file to load |
| `extensions?` | `string`[] | defines the extension to use to load the cube map (can be null) |
| `noMipmap?` | `boolean` | defines if the texture must not receive mipmaps (false by default) |
| `files?` | `string`[] | defines the list of files to load (can be null) |
| `prefiltered?` | `boolean` | defines the prefiltered texture option (default is false) |

#### Returns

[`CubeTextureAssetTask`](CubeTextureAssetTask.md)

a new CubeTextureAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1059

___

### addEquiRectangularCubeTextureAssetTask

▸ **addEquiRectangularCubeTextureAssetTask**(`taskName`, `url`, `size`, `noMipmap?`, `gammaSpace?`): [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md)

Add a EquiRectangularCubeTextureAssetTask to the list of active tasks

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `taskName` | `string` | `undefined` | defines the name of the new task |
| `url` | `string` | `undefined` | defines the url of the file to load |
| `size` | `number` | `undefined` | defines the size you want for the cubemap (can be null) |
| `noMipmap` | `boolean` | `false` | defines if the texture must not receive mipmaps (false by default) |
| `gammaSpace` | `boolean` | `true` | Specifies if the texture will be used in gamma or linear space  (the PBR material requires those textures in linear space, but the standard material would require them in Gamma space) |

#### Returns

[`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md)

a new EquiRectangularCubeTextureAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1104

___

### addHDRCubeTextureTask

▸ **addHDRCubeTextureTask**(`taskName`, `url`, `size`, `noMipmap?`, `generateHarmonics?`, `gammaSpace?`, `reserved?`): [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md)

Add a HDRCubeTextureAssetTask to the list of active tasks

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `taskName` | `string` | `undefined` | defines the name of the new task |
| `url` | `string` | `undefined` | defines the url of the file to load |
| `size` | `number` | `undefined` | defines the size you want for the cubemap (can be null) |
| `noMipmap` | `boolean` | `false` | defines if the texture must not receive mipmaps (false by default) |
| `generateHarmonics` | `boolean` | `true` | defines if you want to automatically generate (true by default) |
| `gammaSpace` | `boolean` | `false` | specifies if the texture will be use in gamma or linear space (the PBR material requires those texture in linear space, but the standard material would require them in Gamma space) (default is false) |
| `reserved` | `boolean` | `false` | Internal use only |

#### Returns

[`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md)

a new HDRCubeTextureAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1078

___

### addImageTask

▸ **addImageTask**(`taskName`, `url`): [`ImageAssetTask`](ImageAssetTask.md)

Add a ImageAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `url` | `string` | defines the url of the file to load |

#### Returns

[`ImageAssetTask`](ImageAssetTask.md)

a new ImageAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1026

___

### addMeshTask

▸ **addMeshTask**(`taskName`, `meshesNames`, `rootUrl`, `sceneFilename`): [`MeshAssetTask`](MeshAssetTask.md)

Add a MeshAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `meshesNames` | `any` | defines the name of meshes to load |
| `rootUrl` | `string` | defines the root url to use to locate files |
| `sceneFilename` | `string` \| `File` | defines the filename of the scene file or the File itself |

#### Returns

[`MeshAssetTask`](MeshAssetTask.md)

a new MeshAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:987

___

### addTextFileTask

▸ **addTextFileTask**(`taskName`, `url`): [`TextFileAssetTask`](TextFileAssetTask.md)

Add a TextFileAssetTask to the list of active tasks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskName` | `string` | defines the name of the new task |
| `url` | `string` | defines the url of the file to load |

#### Returns

[`TextFileAssetTask`](TextFileAssetTask.md)

a new TextFileAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1000

___

### addTextureTask

▸ **addTextureTask**(`taskName`, `url`, `noMipmap?`, `invertY?`, `samplingMode?`): [`TextureAssetTask`](TextureAssetTask.md)

Add a TextureAssetTask to the list of active tasks

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `taskName` | `string` | `undefined` | defines the name of the new task |
| `url` | `string` | `undefined` | defines the url of the file to load |
| `noMipmap?` | `boolean` | `undefined` | defines if the texture must not receive mipmaps (false by default) |
| `invertY?` | `boolean` | `undefined` | defines if you want to invert Y axis of the loaded texture (false by default) |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | defines the sampling mode to use (Texture.TRILINEAR_SAMPLINGMODE by default) |

#### Returns

[`TextureAssetTask`](TextureAssetTask.md)

a new TextureAssetTask object

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1042

___

### load

▸ **load**(): [`AssetsManager`](AssetsManager.md)

Start the loading process

#### Returns

[`AssetsManager`](AssetsManager.md)

the current instance of the AssetsManager

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1224

___

### loadAsync

▸ **loadAsync**(): `Promise``void`

Start the loading process as an async operation

#### Returns

`Promise``void`

a promise returning the list of failed tasks

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1259

___

### removeTask

▸ **removeTask**(`task`): `void`

Remove a task from the assets manager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) | the task to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1115

___

### reset

▸ **reset**(): [`AssetsManager`](AssetsManager.md)

Reset the AssetsManager and remove all tasks

#### Returns

[`AssetsManager`](AssetsManager.md)

the current instance of the AssetsManager

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:1214

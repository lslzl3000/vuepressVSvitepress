[@dev/core](../README.md) / [Exports](../modules.md) / ISceneLoaderPluginAsync

# Interface: ISceneLoaderPluginAsync

Interface used to define an async SceneLoader plugin

## Hierarchy

- [`ISceneLoaderPluginBase`](ISceneLoaderPluginBase.md)

  ↳ **`ISceneLoaderPluginAsync`**

## Table of contents

### Properties

- [extensions](ISceneLoaderPluginAsync.md#extensions)
- [name](ISceneLoaderPluginAsync.md#name)

### Methods

- [canDirectLoad](ISceneLoaderPluginAsync.md#candirectload)
- [directLoad](ISceneLoaderPluginAsync.md#directload)
- [importMeshAsync](ISceneLoaderPluginAsync.md#importmeshasync)
- [loadAssetContainerAsync](ISceneLoaderPluginAsync.md#loadassetcontainerasync)
- [loadAsync](ISceneLoaderPluginAsync.md#loadasync)
- [loadFile](ISceneLoaderPluginAsync.md#loadfile)
- [rewriteRootURL](ISceneLoaderPluginAsync.md#rewriterooturl)

## Properties

### extensions

• **extensions**: `string` \| [`ISceneLoaderPluginExtensions`](ISceneLoaderPluginExtensions.md)

The file extensions supported by this plugin.

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[extensions](ISceneLoaderPluginBase.md#extensions)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:144

___

### name

• **name**: `string`

The friendly name of this plugin.

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[name](ISceneLoaderPluginBase.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:139

## Methods

### canDirectLoad

▸ `Optional` **canDirectLoad**(`data`): `boolean`

The callback that returns true if the data can be directly loaded.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | string containing the file data |

#### Returns

`boolean`

if the data can be loaded directly

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[canDirectLoad](ISceneLoaderPluginBase.md#candirectload)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:170

___

### directLoad

▸ `Optional` **directLoad**(`scene`, `data`): `any`

The callback that returns the data to pass to the plugin if the data can be directly loaded.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](../classes/Scene.md) | scene loading this data |
| `data` | `string` | string containing the data |

#### Returns

`any`

data to pass to the plugin

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[directLoad](ISceneLoaderPluginBase.md#directload)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:178

___

### importMeshAsync

▸ **importMeshAsync**(`meshesNames`, `scene`, `data`, `rootUrl`, `onProgress?`, `fileName?`): `Promise`[`ISceneLoaderAsyncResult`](ISceneLoaderAsyncResult.md)

Import meshes into a scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshesNames` | `any` | An array of mesh names, a single mesh name, or empty string for all meshes that filter what meshes are imported |
| `scene` | [`Scene`](../classes/Scene.md) | The scene to import into |
| `data` | `any` | The data to import |
| `rootUrl` | `string` | The root url for scene and resources |
| `onProgress?` | (`event`: [`ISceneLoaderProgressEvent`](ISceneLoaderProgressEvent.md)) => `void` | The callback when the load progresses |
| `fileName?` | `string` | Defines the name of the file to load |

#### Returns

`Promise`[`ISceneLoaderAsyncResult`](ISceneLoaderAsyncResult.md)

The loaded objects (e.g. meshes, particle systems, skeletons, animation groups, etc.)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:251

___

### loadAssetContainerAsync

▸ **loadAssetContainerAsync**(`scene`, `data`, `rootUrl`, `onProgress?`, `fileName?`): `Promise`[`AssetContainer`](../classes/AssetContainer.md)

Load into an asset container.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](../classes/Scene.md) | The scene to load into |
| `data` | `any` | The data to import |
| `rootUrl` | `string` | The root url for scene and resources |
| `onProgress?` | (`event`: [`ISceneLoaderProgressEvent`](ISceneLoaderProgressEvent.md)) => `void` | The callback when the load progresses |
| `fileName?` | `string` | Defines the name of the file to load |

#### Returns

`Promise`[`AssetContainer`](../classes/AssetContainer.md)

The loaded asset container

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:280

___

### loadAsync

▸ **loadAsync**(`scene`, `data`, `rootUrl`, `onProgress?`, `fileName?`): `Promise``void`

Load into a scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](../classes/Scene.md) | The scene to load into |
| `data` | `any` | The data to import |
| `rootUrl` | `string` | The root url for scene and resources |
| `onProgress?` | (`event`: [`ISceneLoaderProgressEvent`](ISceneLoaderProgressEvent.md)) => `void` | The callback when the load progresses |
| `fileName?` | `string` | Defines the name of the file to load |

#### Returns

`Promise``void`

Nothing

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:269

___

### loadFile

▸ `Optional` **loadFile**(`scene`, `fileOrUrl`, `onSuccess`, `onProgress?`, `useArrayBuffer?`, `onError?`): [`IFileRequest`](IFileRequest.md)

The callback called when loading from a url.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](../classes/Scene.md) | scene loading this url |
| `fileOrUrl` | `string` \| `File` | file or url to load |
| `onSuccess` | (`data`: `any`, `responseURL?`: `string`) => `void` | callback called when the file successfully loads |
| `onProgress?` | (`ev`: [`ISceneLoaderProgressEvent`](ISceneLoaderProgressEvent.md)) => `void` | callback called while file is loading (if the server supports this mode) |
| `useArrayBuffer?` | `boolean` | defines a boolean indicating that date must be returned as ArrayBuffer |
| `onError?` | (`request?`: [`WebRequest`](../classes/WebRequest.md), `exception?`: `LoadFileError`) => `void` | callback called when the file fails to load |

#### Returns

[`IFileRequest`](IFileRequest.md)

a file request object

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[loadFile](ISceneLoaderPluginBase.md#loadfile)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:156

___

### rewriteRootURL

▸ `Optional` **rewriteRootURL**(`rootUrl`, `responseURL?`): `string`

The callback that allows custom handling of the root url based on the response url.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rootUrl` | `string` | the original root url |
| `responseURL?` | `string` | the response url if available |

#### Returns

`string`

the new root url

#### Inherited from

[ISceneLoaderPluginBase](ISceneLoaderPluginBase.md).[rewriteRootURL](ISceneLoaderPluginBase.md#rewriterooturl)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:186

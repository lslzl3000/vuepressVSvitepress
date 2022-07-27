[@dev/core](../README.md) / [Exports](../modules.md) / ISceneLoaderPluginBase

# Interface: ISceneLoaderPluginBase

Interface used to define the base of ISceneLoaderPlugin and ISceneLoaderPluginAsync

## Hierarchy

- **`ISceneLoaderPluginBase`**

  ↳ [`ISceneLoaderPlugin`](ISceneLoaderPlugin.md)

  ↳ [`ISceneLoaderPluginAsync`](ISceneLoaderPluginAsync.md)

## Table of contents

### Properties

- [extensions](ISceneLoaderPluginBase.md#extensions)
- [name](ISceneLoaderPluginBase.md#name)

### Methods

- [canDirectLoad](ISceneLoaderPluginBase.md#candirectload)
- [directLoad](ISceneLoaderPluginBase.md#directload)
- [loadFile](ISceneLoaderPluginBase.md#loadfile)
- [rewriteRootURL](ISceneLoaderPluginBase.md#rewriterooturl)

## Properties

### extensions

• **extensions**: `string` \| [`ISceneLoaderPluginExtensions`](ISceneLoaderPluginExtensions.md)

The file extensions supported by this plugin.

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:144

___

### name

• **name**: `string`

The friendly name of this plugin.

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

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:178

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

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:186

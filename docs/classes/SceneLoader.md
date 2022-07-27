[@dev/core](../README.md) / [Exports](../modules.md) / SceneLoader

# Class: SceneLoader

Class used to load scene from various file formats using registered plugins

**`See`**

https://doc.babylonjs.com/how_to/load_from_any_file_type

## Table of contents

### Constructors

- [constructor](SceneLoader.md#constructor)

### Properties

- [DETAILED\_LOGGING](SceneLoader.md#detailed_logging)
- [MINIMAL\_LOGGING](SceneLoader.md#minimal_logging)
- [NO\_LOGGING](SceneLoader.md#no_logging)
- [OnPluginActivatedObservable](SceneLoader.md#onpluginactivatedobservable)
- [SUMMARY\_LOGGING](SceneLoader.md#summary_logging)
- [\_RegisteredPlugins](SceneLoader.md#_registeredplugins)
- [\_ShowingLoadingScreen](SceneLoader.md#_showingloadingscreen)

### Accessors

- [CleanBoneMatrixWeights](SceneLoader.md#cleanbonematrixweights)
- [ForceFullSceneLoadingForIncremental](SceneLoader.md#forcefullsceneloadingforincremental)
- [ShowLoadingScreen](SceneLoader.md#showloadingscreen)
- [loggingLevel](SceneLoader.md#logginglevel)

### Methods

- [Append](SceneLoader.md#append)
- [AppendAsync](SceneLoader.md#appendasync)
- [GetDefaultPlugin](SceneLoader.md#getdefaultplugin)
- [GetPluginForExtension](SceneLoader.md#getpluginforextension)
- [ImportAnimations](SceneLoader.md#importanimations)
- [ImportAnimationsAsync](SceneLoader.md#importanimationsasync)
- [ImportMesh](SceneLoader.md#importmesh)
- [ImportMeshAsync](SceneLoader.md#importmeshasync)
- [IsPluginForExtensionAvailable](SceneLoader.md#ispluginforextensionavailable)
- [Load](SceneLoader.md#load)
- [LoadAssetContainer](SceneLoader.md#loadassetcontainer)
- [LoadAssetContainerAsync](SceneLoader.md#loadassetcontainerasync)
- [LoadAsync](SceneLoader.md#loadasync)
- [RegisterPlugin](SceneLoader.md#registerplugin)
- [\_FormatErrorMessage](SceneLoader.md#_formaterrormessage)
- [\_GetDirectLoad](SceneLoader.md#_getdirectload)
- [\_GetFileInfo](SceneLoader.md#_getfileinfo)
- [\_GetPluginForDirectLoad](SceneLoader.md#_getpluginfordirectload)
- [\_GetPluginForExtension](SceneLoader.md#_getpluginforextension)
- [\_GetPluginForFilename](SceneLoader.md#_getpluginforfilename)
- [\_LoadData](SceneLoader.md#_loaddata)

## Constructors

### constructor

• **new SceneLoader**()

## Properties

### DETAILED\_LOGGING

▪ `Static` `Readonly` **DETAILED\_LOGGING**: ``3``

Detailed logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:367

___

### MINIMAL\_LOGGING

▪ `Static` `Readonly` **MINIMAL\_LOGGING**: ``1``

Minimal logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:357

___

### NO\_LOGGING

▪ `Static` `Readonly` **NO\_LOGGING**: ``0``

No logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:352

___

### OnPluginActivatedObservable

▪ `Static` **OnPluginActivatedObservable**: [`Observable`](Observable.md)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

Event raised when a plugin is used to load a scene

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:421

___

### SUMMARY\_LOGGING

▪ `Static` `Readonly` **SUMMARY\_LOGGING**: ``2``

Summary logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:362

___

### \_RegisteredPlugins

▪ `Static` `Private` **\_RegisteredPlugins**: `Object` = `{}`

#### Index signature

▪ [extension: `string`]: `IRegisteredPlugin`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:423

___

### \_ShowingLoadingScreen

▪ `Static` `Private` **\_ShowingLoadingScreen**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:425

## Accessors

### CleanBoneMatrixWeights

• `Static` `get` **CleanBoneMatrixWeights**(): `boolean`

Gets or set a boolean indicating if matrix weights must be cleaned upon loading

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:408

• `Static` `set` **CleanBoneMatrixWeights**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:412

___

### ForceFullSceneLoadingForIncremental

• `Static` `get` **ForceFullSceneLoadingForIncremental**(): `boolean`

Gets or sets a boolean indicating if entire scene must be loaded even if scene contains incremental data

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:372

• `Static` `set` **ForceFullSceneLoadingForIncremental**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:376

___

### ShowLoadingScreen

• `Static` `get` **ShowLoadingScreen**(): `boolean`

Gets or sets a boolean indicating if loading screen must be displayed while loading a scene

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:383

• `Static` `set` **ShowLoadingScreen**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:387

___

### loggingLevel

• `Static` `get` **loggingLevel**(): `number`

Defines the current logging level (while loading the scene)

**`Ignorenaming`**

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:396

• `Static` `set` **loggingLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:401

## Methods

### Append

▸ `Static` **Append**(`rootUrl`, `sceneFilename?`, `scene?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): [`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

Append a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to |
| `onSuccess` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md)) => `void` | `null` | a callback with the scene when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

[`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

The loaded plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:929

___

### AppendAsync

▸ `Static` **AppendAsync**(`rootUrl`, `sceneFilename?`, `scene?`, `onProgress?`, `pluginExtension?`): `Promise`[`Scene`](Scene.md)

Append a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`Promise`[`Scene`](Scene.md)

The given scene

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:1040

___

### GetDefaultPlugin

▸ `Static` **GetDefaultPlugin**(): `IRegisteredPlugin`

Gets the default plugin (used to load Babylon files)

#### Returns

`IRegisteredPlugin`

the .babylon plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:431

___

### GetPluginForExtension

▸ `Static` **GetPluginForExtension**(`extension`): [`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md) \| [`ISceneLoaderPluginFactory`](../interfaces/ISceneLoaderPluginFactory.md)

Gets a plugin that can load the given extension

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extension` | `string` | defines the extension to load |

#### Returns

[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md) \| [`ISceneLoaderPluginFactory`](../interfaces/ISceneLoaderPluginFactory.md)

a plugin or null if none works

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:654

___

### ImportAnimations

▸ `Static` **ImportAnimations**(`rootUrl`, `sceneFilename?`, `scene?`, `overwriteAnimations?`, `animationGroupLoadingMode?`, `targetConverter?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): `void`

Import animations from a file into a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to (default: last created scene) |
| `overwriteAnimations` | `boolean` | `true` | when true, animations are cleaned before importing new ones. Animations are appended otherwise |
| `animationGroupLoadingMode` | [`SceneLoaderAnimationGroupLoadingMode`](../enums/SceneLoaderAnimationGroupLoadingMode.md) | `SceneLoaderAnimationGroupLoadingMode.Clean` | defines how to handle old animations groups before importing new ones |
| `targetConverter` | [`Nullable`](../modules.md#nullable)(`target`: `any`) => `any` | `null` | defines a function used to convert animation targets from loaded scene to current scene (default: search node by name) |
| `onSuccess` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md)) => `void` | `null` | a callback with the scene when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:1217

___

### ImportAnimationsAsync

▸ `Static` **ImportAnimationsAsync**(`rootUrl`, `sceneFilename?`, `scene?`, `overwriteAnimations?`, `animationGroupLoadingMode?`, `targetConverter?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): `Promise`[`Scene`](Scene.md)

Import animations from a file into a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to (default: last created scene) |
| `overwriteAnimations` | `boolean` | `true` | when true, animations are cleaned before importing new ones. Animations are appended otherwise |
| `animationGroupLoadingMode` | [`SceneLoaderAnimationGroupLoadingMode`](../enums/SceneLoaderAnimationGroupLoadingMode.md) | `SceneLoaderAnimationGroupLoadingMode.Clean` | defines how to handle old animations groups before importing new ones |
| `targetConverter` | [`Nullable`](../modules.md#nullable)(`target`: `any`) => `any` | `null` | defines a function used to convert animation targets from loaded scene to current scene (default: search node by name) |
| `onSuccess` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md)) => `void` | `null` | a callback with the scene when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`Promise`[`Scene`](Scene.md)

the updated scene with imported animations

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:1307

___

### ImportMesh

▸ `Static` **ImportMesh**(`meshNames`, `rootUrl`, `sceneFilename?`, `scene?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): [`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

Import meshes into a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshNames` | `any` | `undefined` | an array of mesh names, a single mesh name, or empty string for all meshes that filter what meshes are imported |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | the instance of BABYLON.Scene to append to |
| `onSuccess` | [`Nullable`](../modules.md#nullable)[`SceneLoaderSuccessCallback`](../modules.md#sceneloadersuccesscallback) | `null` | a callback with a list of imported meshes, particleSystems, skeletons, and animationGroups when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

[`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

The loaded plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:701

___

### ImportMeshAsync

▸ `Static` **ImportMeshAsync**(`meshNames`, `rootUrl`, `sceneFilename?`, `scene?`, `onProgress?`, `pluginExtension?`): `Promise`[`ISceneLoaderAsyncResult`](../interfaces/ISceneLoaderAsyncResult.md)

Import meshes into a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshNames` | `any` | `undefined` | an array of mesh names, a single mesh name, or empty string for all meshes that filter what meshes are imported |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | the instance of BABYLON.Scene to append to |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`Promise`[`ISceneLoaderAsyncResult`](../interfaces/ISceneLoaderAsyncResult.md)

The loaded list of imported meshes, particle systems, skeletons, and animation groups

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:823

___

### IsPluginForExtensionAvailable

▸ `Static` **IsPluginForExtensionAvailable**(`extension`): `boolean`

Gets a boolean indicating that the given extension can be loaded

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extension` | `string` | defines the extension to load |

#### Returns

`boolean`

true if the extension is supported

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:663

___

### Load

▸ `Static` **Load**(`rootUrl`, `sceneFilename?`, `engine?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): [`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

Load a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `engine` | [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md) | `EngineStore.LastCreatedEngine` | is the instance of BABYLON.Engine to use to create the scene |
| `onSuccess` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md)) => `void` | `null` | a callback with the scene when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

[`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

The loaded plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:868

___

### LoadAssetContainer

▸ `Static` **LoadAssetContainer**(`rootUrl`, `sceneFilename?`, `scene?`, `onSuccess?`, `onProgress?`, `onError?`, `pluginExtension?`): [`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

Load a scene into an asset container

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to (default: last created scene) |
| `onSuccess` | [`Nullable`](../modules.md#nullable)(`assets`: [`AssetContainer`](AssetContainer.md)) => `void` | `null` | a callback with the scene when import succeeds |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`scene`: [`Scene`](Scene.md), `message`: `string`, `exception?`: `any`) => `void` | `null` | a callback with the scene, a message, and possibly an exception when import fails |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

[`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

The loaded plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:1075

___

### LoadAssetContainerAsync

▸ `Static` **LoadAssetContainerAsync**(`rootUrl`, `sceneFilename?`, `scene?`, `onProgress?`, `pluginExtension?`): `Promise`[`AssetContainer`](AssetContainer.md)

Load a scene into an asset container

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene (default: empty string) |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of Scene to append to |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`Promise`[`AssetContainer`](AssetContainer.md)

The loaded asset container

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:1180

___

### LoadAsync

▸ `Static` **LoadAsync**(`rootUrl`, `sceneFilename?`, `engine?`, `onProgress?`, `pluginExtension?`): `Promise`[`Scene`](Scene.md)

Load a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | a string that defines the root url for the scene and resources or the concatenation of rootURL and filename (e.g. http://example.com/test.glb) |
| `sceneFilename` | `string` \| `File` | `""` | a string that defines the name of the scene file or starts with "data:" following by the stringified version of the scene or a File object (default: empty string) |
| `engine` | [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md) | `EngineStore.LastCreatedEngine` | is the instance of BABYLON.Engine to use to create the scene |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | `null` | a callback with a progress event for each file being loaded |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | the extension used to determine the plugin |

#### Returns

`Promise`[`Scene`](Scene.md)

The loaded scene

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:894

___

### RegisterPlugin

▸ `Static` **RegisterPlugin**(`plugin`): `void`

Adds a new plugin to the list of registered plugins

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plugin` | [`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md) | defines the plugin to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:671

___

### \_FormatErrorMessage

▸ `Static` `Private` **_FormatErrorMessage**(`fileInfo`, `message?`, `exception?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `fileInfo` | `IFileInfo` |
| `message?` | `string` |
| `exception?` | `any` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:481

___

### \_GetDirectLoad

▸ `Static` `Private` **_GetDirectLoad**(`sceneFilename`): [`Nullable`](../modules.md#nullable)`string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneFilename` | `string` |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:473

___

### \_GetFileInfo

▸ `Static` `Private` **_GetFileInfo**(`rootUrl`, `sceneFilename`): [`Nullable`](../modules.md#nullable)`IFileInfo`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rootUrl` | `string` |
| `sceneFilename` | `string` \| `File` |

#### Returns

[`Nullable`](../modules.md#nullable)`IFileInfo`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:611

___

### \_GetPluginForDirectLoad

▸ `Static` `Private` **_GetPluginForDirectLoad**(`data`): `IRegisteredPlugin`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `string` |

#### Returns

`IRegisteredPlugin`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:448

___

### \_GetPluginForExtension

▸ `Static` `Private` **_GetPluginForExtension**(`extension`): `IRegisteredPlugin`

#### Parameters

| Name | Type |
| :------ | :------ |
| `extension` | `string` |

#### Returns

`IRegisteredPlugin`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:435

___

### \_GetPluginForFilename

▸ `Static` `Private` **_GetPluginForFilename**(`sceneFilename`): `IRegisteredPlugin`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneFilename` | `string` |

#### Returns

`IRegisteredPlugin`

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:460

___

### \_LoadData

▸ `Static` `Private` **_LoadData**(`fileInfo`, `scene`, `onSuccess`, `onProgress`, `onError`, `onDispose`, `pluginExtension`): [`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `fileInfo` | `IFileInfo` |
| `scene` | [`Scene`](Scene.md) |
| `onSuccess` | (`plugin`: [`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md), `data`: `any`, `responseURL?`: `string`) => `void` |
| `onProgress` | `undefined` \| (`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` |
| `onDispose` | () => `void` |
| `pluginExtension` | [`Nullable`](../modules.md#nullable)`string` |

#### Returns

[`Nullable`](../modules.md#nullable)[`ISceneLoaderPlugin`](../interfaces/ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](../interfaces/ISceneLoaderPluginAsync.md)

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:493

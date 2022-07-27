[@dev/core](../README.md) / [Exports](../modules.md) / FilesInput

# Class: FilesInput

Class used to help managing file picking and drag-n-drop

## Table of contents

### Constructors

- [constructor](FilesInput.md#constructor)

### Properties

- [\_additionalRenderLoopLogicCallback](FilesInput.md#_additionalrenderlooplogiccallback)
- [\_currentScene](FilesInput.md#_currentscene)
- [\_dragEnterHandler](FilesInput.md#_dragenterhandler)
- [\_dragOverHandler](FilesInput.md#_dragoverhandler)
- [\_dropHandler](FilesInput.md#_drophandler)
- [\_elementToMonitor](FilesInput.md#_elementtomonitor)
- [\_engine](FilesInput.md#_engine)
- [\_errorCallback](FilesInput.md#_errorcallback)
- [\_filesToLoad](FilesInput.md#_filestoload)
- [\_onReloadCallback](FilesInput.md#_onreloadcallback)
- [\_progressCallback](FilesInput.md#_progresscallback)
- [\_sceneFileToLoad](FilesInput.md#_scenefiletoload)
- [\_sceneLoadedCallback](FilesInput.md#_sceneloadedcallback)
- [\_startingProcessingFilesCallback](FilesInput.md#_startingprocessingfilescallback)
- [\_textureLoadingCallback](FilesInput.md#_textureloadingcallback)
- [loadAsync](FilesInput.md#loadasync)
- [onProcessFileCallback](FilesInput.md#onprocessfilecallback)

### Accessors

- [filesToLoad](FilesInput.md#filestoload)
- [FilesToLoad](FilesInput.md#filestoload-1)

### Methods

- [\_drag](FilesInput.md#_drag)
- [\_drop](FilesInput.md#_drop)
- [\_processFiles](FilesInput.md#_processfiles)
- [\_processReload](FilesInput.md#_processreload)
- [\_renderFunction](FilesInput.md#_renderfunction)
- [\_traverseFolder](FilesInput.md#_traversefolder)
- [dispose](FilesInput.md#dispose)
- [loadFiles](FilesInput.md#loadfiles)
- [monitorElementForDragNDrop](FilesInput.md#monitorelementfordragndrop)
- [reload](FilesInput.md#reload)

## Constructors

### constructor

• **new FilesInput**(`engine`, `scene`, `sceneLoadedCallback`, `progressCallback`, `additionalRenderLoopLogicCallback`, `textureLoadingCallback`, `startingProcessingFilesCallback`, `onReloadCallback`, `errorCallback`)

Creates a new FilesInput

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | defines the rendering engine |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the hosting scene |
| `sceneLoadedCallback` | [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`, `scene`: [`Scene`](Scene.md)) => `void` | callback called when scene is loaded |
| `progressCallback` | [`Nullable`](../modules.md#nullable)(`progress`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` | callback called to track progress |
| `additionalRenderLoopLogicCallback` | [`Nullable`](../modules.md#nullable)() => `void` | callback called to add user logic to the rendering loop |
| `textureLoadingCallback` | [`Nullable`](../modules.md#nullable)(`remaining`: `number`) => `void` | callback called when a texture is loading |
| `startingProcessingFilesCallback` | [`Nullable`](../modules.md#nullable)(`files?`: `File`[]) => `void` | callback called when the system is about to process all files |
| `onReloadCallback` | [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`) => `void` | callback called when a reload is requested |
| `errorCallback` | [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`, `scene`: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md), `message`: `string`) => `void` | callback call if an error occurs |

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:61

## Properties

### \_additionalRenderLoopLogicCallback

• `Private` **\_additionalRenderLoopLogicCallback**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:39

___

### \_currentScene

• `Private` **\_currentScene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:36

___

### \_dragEnterHandler

• `Private` **\_dragEnterHandler**: (`e`: `any`) => `void`

#### Type declaration

▸ (`e`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:84

___

### \_dragOverHandler

• `Private` **\_dragOverHandler**: (`e`: `any`) => `void`

#### Type declaration

▸ (`e`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:85

___

### \_dropHandler

• `Private` **\_dropHandler**: (`e`: `any`) => `void`

#### Type declaration

▸ (`e`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:86

___

### \_elementToMonitor

• `Private` **\_elementToMonitor**: `HTMLElement`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:44

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:35

___

### \_errorCallback

• `Private` **\_errorCallback**: [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`, `scene`: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md), `message`: `string`) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:43

___

### \_filesToLoad

• `Private` **\_filesToLoad**: `File`[]

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:47

___

### \_onReloadCallback

• `Private` **\_onReloadCallback**: [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:42

___

### \_progressCallback

• `Private` **\_progressCallback**: [`Nullable`](../modules.md#nullable)(`progress`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:38

___

### \_sceneFileToLoad

• `Private` **\_sceneFileToLoad**: `File`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:46

___

### \_sceneLoadedCallback

• `Private` **\_sceneLoadedCallback**: [`Nullable`](../modules.md#nullable)(`sceneFile`: `File`, `scene`: [`Scene`](Scene.md)) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:37

___

### \_startingProcessingFilesCallback

• `Private` **\_startingProcessingFilesCallback**: [`Nullable`](../modules.md#nullable)(`files?`: `File`[]) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:41

___

### \_textureLoadingCallback

• `Private` **\_textureLoadingCallback**: [`Nullable`](../modules.md#nullable)(`remaining`: `number`) => `void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:40

___

### loadAsync

• **loadAsync**: (`sceneFile`: `File`, `onProgress`: [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void`) => `Promise`[`Scene`](Scene.md)

#### Type declaration

▸ (`sceneFile`, `onProgress`): `Promise`[`Scene`](Scene.md)

Function used when loading the scene file

##### Parameters

| Name | Type |
| :------ | :------ |
| `sceneFile` | `File` |
| `onProgress` | [`Nullable`](../modules.md#nullable)(`event`: [`ISceneLoaderProgressEvent`](../interfaces/ISceneLoaderProgressEvent.md)) => `void` |

##### Returns

`Promise`[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:32

___

### onProcessFileCallback

• **onProcessFileCallback**: (`file`: `File`, `name`: `string`, `extension`: `string`, `setSceneFileToLoad`: (`sceneFile`: `File`) => `void`) => `boolean`

#### Type declaration

▸ (`file`, `name`, `extension`, `setSceneFileToLoad`): `boolean`

Callback called when a file is processed

##### Parameters

| Name | Type |
| :------ | :------ |
| `file` | `File` |
| `name` | `string` |
| `extension` | `string` |
| `setSceneFileToLoad` | (`sceneFile`: `File`) => `void` |

##### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:23

## Accessors

### filesToLoad

• `get` **filesToLoad**(): `File`[]

Gets the current list of files to load

#### Returns

`File`[]

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:113

___

### FilesToLoad

• `Static` `get` **FilesToLoad**(): `Object`

List of files ready to be loaded

#### Returns

`Object`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:16

## Methods

### \_drag

▸ `Private` **_drag**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `DragEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:147

___

### \_drop

▸ `Private` **_drop**(`eventDrop`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventDrop` | `DragEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:152

___

### \_processFiles

▸ `Private` **_processFiles**(`files`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `files` | `any`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:185

___

### \_processReload

▸ `Private` **_processReload**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:275

___

### \_renderFunction

▸ `Private` **_renderFunction**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:130

___

### \_traverseFolder

▸ `Private` **_traverseFolder**(`folder`, `files`, `remaining`, `callback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `folder` | `any` |
| `files` | `any`[] |
| `remaining` | `Object` |
| `remaining.count` | `number` |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:159

___

### dispose

▸ **dispose**(): `void`

Release all associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:120

___

### loadFiles

▸ **loadFiles**(`event`): `void`

Load files from a drop event

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `any` | defines the drop event to use as source |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:206

___

### monitorElementForDragNDrop

▸ **monitorElementForDragNDrop**(`elementToMonitor`): `void`

Calls this function to listen to drag'n'drop events on a specific DOM element

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `elementToMonitor` | `HTMLElement` | defines the DOM element to track |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:92

___

### reload

▸ **reload**(): `void`

Reload the current scene from the loaded files

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/filesInput.ts:286

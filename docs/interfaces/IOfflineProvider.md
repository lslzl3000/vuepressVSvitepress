[@dev/core](../README.md) / [Exports](../modules.md) / IOfflineProvider

# Interface: IOfflineProvider

Class used to enable access to offline support

**`See`**

https://doc.babylonjs.com/how_to/caching_resources_in_indexeddb

## Implemented by

- [`Database`](../classes/Database.md)

## Table of contents

### Properties

- [enableSceneOffline](IOfflineProvider.md#enablesceneoffline)
- [enableTexturesOffline](IOfflineProvider.md#enabletexturesoffline)

### Methods

- [loadFile](IOfflineProvider.md#loadfile)
- [loadImage](IOfflineProvider.md#loadimage)
- [open](IOfflineProvider.md#open)

## Properties

### enableSceneOffline

• **enableSceneOffline**: `boolean`

Gets a boolean indicating if scene must be saved in the database

#### Defined in

https://github.com/babylon.js/core/src/Offline/IOfflineProvider.ts:9

___

### enableTexturesOffline

• **enableTexturesOffline**: `boolean`

Gets a boolean indicating if textures must be saved in the database

#### Defined in

https://github.com/babylon.js/core/src/Offline/IOfflineProvider.ts:14

## Methods

### loadFile

▸ **loadFile**(`url`, `sceneLoaded`, `progressCallBack?`, `errorCallback?`, `useArrayBuffer?`): `void`

Loads a file from offline support

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the URL to load from |
| `sceneLoaded` | (`data`: `any`) => `void` | defines a callback to call on success |
| `progressCallBack?` | (`data`: `any`) => `void` | defines a callback to call when progress changed |
| `errorCallback?` | () => `void` | defines a callback to call on error |
| `useArrayBuffer?` | `boolean` | defines a boolean to use array buffer instead of text string |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/IOfflineProvider.ts:38

___

### loadImage

▸ **loadImage**(`url`, `image`): `void`

Loads an image from the offline support

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the url to load from |
| `image` | `HTMLImageElement` | defines the target DOM image |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/IOfflineProvider.ts:28

___

### open

▸ **open**(`successCallback`, `errorCallback`): `void`

Open the offline support and make it available

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallback` | () => `void` | defines the callback to call on success |
| `errorCallback` | () => `void` | defines the callback to call on error |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/IOfflineProvider.ts:21

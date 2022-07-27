[@dev/core](../README.md) / [Exports](../modules.md) / Database

# Class: Database

Class used to enable access to IndexedDB

**`See`**

https://doc.babylonjs.com/how_to/caching_resources_in_indexeddb

## Implements

- [`IOfflineProvider`](../interfaces/IOfflineProvider.md)

## Table of contents

### Constructors

- [constructor](Database.md#constructor)

### Properties

- [\_currentSceneUrl](Database.md#_currentsceneurl)
- [\_db](Database.md#_db)
- [\_enableSceneOffline](Database.md#_enablesceneoffline)
- [\_enableTexturesOffline](Database.md#_enabletexturesoffline)
- [\_hasReachedQuota](Database.md#_hasreachedquota)
- [\_idbFactory](Database.md#_idbfactory)
- [\_isSupported](Database.md#_issupported)
- [\_manifestVersionFound](Database.md#_manifestversionfound)
- [\_mustUpdateRessources](Database.md#_mustupdateressources)
- [IDBStorageEnabled](Database.md#idbstorageenabled)
- [\_IsUASupportingBlobStorage](Database.md#_isuasupportingblobstorage)

### Accessors

- [enableSceneOffline](Database.md#enablesceneoffline)
- [enableTexturesOffline](Database.md#enabletexturesoffline)

### Methods

- [\_checkManifestFile](Database.md#_checkmanifestfile)
- [\_checkVersionFromDB](Database.md#_checkversionfromdb)
- [\_loadFileAsync](Database.md#_loadfileasync)
- [\_loadImageFromDBAsync](Database.md#_loadimagefromdbasync)
- [\_loadVersionFromDBAsync](Database.md#_loadversionfromdbasync)
- [\_saveFileAsync](Database.md#_savefileasync)
- [\_saveImageIntoDBAsync](Database.md#_saveimageintodbasync)
- [\_saveVersionIntoDBAsync](Database.md#_saveversionintodbasync)
- [loadFile](Database.md#loadfile)
- [loadImage](Database.md#loadimage)
- [open](Database.md#open)
- [\_ParseURL](Database.md#_parseurl)
- [\_ReturnFullUrlLocation](Database.md#_returnfullurllocation)
- [\_ValidateXHRData](Database.md#_validatexhrdata)

## Constructors

### constructor

• **new Database**(`urlToScene`, `callbackManifestChecked`, `disableManifestCheck?`)

Creates a new Database

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `urlToScene` | `string` | `undefined` | defines the url to load the scene |
| `callbackManifestChecked` | (`checked`: `boolean`) => `any` | `undefined` | defines the callback to use when manifest is checked |
| `disableManifestCheck` | `boolean` | `false` | defines a boolean indicating that we want to skip the manifest validation (it will be considered validated and up to date) |

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:59

## Properties

### \_currentSceneUrl

• `Private` **\_currentSceneUrl**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:19

___

### \_db

• `Private` **\_db**: [`Nullable`](../modules.md#nullable)`IDBDatabase`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:20

___

### \_enableSceneOffline

• `Private` **\_enableSceneOffline**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:21

___

### \_enableTexturesOffline

• `Private` **\_enableTexturesOffline**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:22

___

### \_hasReachedQuota

• `Private` **\_hasReachedQuota**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:25

___

### \_idbFactory

• `Private` **\_idbFactory**: `IDBFactory`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:29

___

### \_isSupported

• `Private` **\_isSupported**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:26

___

### \_manifestVersionFound

• `Private` **\_manifestVersionFound**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:23

___

### \_mustUpdateRessources

• `Private` **\_mustUpdateRessources**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:24

___

### IDBStorageEnabled

▪ `Static` **IDBStorageEnabled**: `boolean` = `false`

Gets a boolean indicating if Database storage is enabled (off by default)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:37

___

### \_IsUASupportingBlobStorage

▪ `Static` `Private` **\_IsUASupportingBlobStorage**: `boolean` = `true`

Gets a boolean indicating if the user agent supports blob storage (this value will be updated after creating the first Database object)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:32

## Accessors

### enableSceneOffline

• `get` **enableSceneOffline**(): `boolean`

Gets a boolean indicating if scene must be saved in the database

#### Returns

`boolean`

#### Implementation of

[IOfflineProvider](../interfaces/IOfflineProvider.md).[enableSceneOffline](../interfaces/IOfflineProvider.md#enablesceneoffline)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:42

___

### enableTexturesOffline

• `get` **enableTexturesOffline**(): `boolean`

Gets a boolean indicating if textures must be saved in the database

#### Returns

`boolean`

#### Implementation of

[IOfflineProvider](../interfaces/IOfflineProvider.md).[enableTexturesOffline](../interfaces/IOfflineProvider.md#enabletexturesoffline)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:49

## Methods

### \_checkManifestFile

▸ `Private` **_checkManifestFile**(`callbackManifestChecked`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `callbackManifestChecked` | (`checked`: `boolean`) => `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:101

___

### \_checkVersionFromDB

▸ `Private` **_checkVersionFromDB**(`url`, `versionLoaded`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `versionLoaded` | (`version`: `number`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:418

___

### \_loadFileAsync

▸ `Private` **_loadFileAsync**(`url`, `callback`, `notInDBCallback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `callback` | (`data?`: `any`) => `void` |
| `notInDBCallback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:542

___

### \_loadImageFromDBAsync

▸ `Private` **_loadImageFromDBAsync**(`url`, `image`, `notInDBCallback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `image` | `HTMLImageElement` |
| `notInDBCallback` | () => `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:280

___

### \_loadVersionFromDBAsync

▸ `Private` **_loadVersionFromDBAsync**(`url`, `callback`, `updateInDBCallback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `callback` | (`version`: `number`) => `void` |
| `updateInDBCallback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:426

___

### \_saveFileAsync

▸ `Private` **_saveFileAsync**(`url`, `callback`, `progressCallback?`, `useArrayBuffer?`, `errorCallback?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `callback` | (`data?`: `any`) => `void` |
| `progressCallback?` | (`this`: `XMLHttpRequestEventTarget`, `ev`: `ProgressEvent``EventTarget`) => `any` |
| `useArrayBuffer?` | `boolean` |
| `errorCallback?` | (`data?`: `any`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:583

___

### \_saveImageIntoDBAsync

▸ `Private` **_saveImageIntoDBAsync**(`url`, `image`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `image` | `HTMLImageElement` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:319

___

### \_saveVersionIntoDBAsync

▸ `Private` **_saveVersionIntoDBAsync**(`url`, `callback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `callback` | (`version`: `number`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:472

___

### loadFile

▸ **loadFile**(`url`, `sceneLoaded`, `progressCallBack?`, `errorCallback?`, `useArrayBuffer?`): `void`

Loads a file from database

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

#### Implementation of

[IOfflineProvider](../interfaces/IOfflineProvider.md).[loadFile](../interfaces/IOfflineProvider.md#loadfile)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:519

___

### loadImage

▸ **loadImage**(`url`, `image`): `void`

Loads an image from the database

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the url to load from |
| `image` | `HTMLImageElement` | defines the target DOM image |

#### Returns

`void`

#### Implementation of

[IOfflineProvider](../interfaces/IOfflineProvider.md).[loadImage](../interfaces/IOfflineProvider.md#loadimage)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:256

___

### open

▸ **open**(`successCallback`, `errorCallback`): `void`

Open the database and make it available

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallback` | () => `void` | defines the callback to call on success |
| `errorCallback` | () => `void` | defines the callback to call on error |

#### Returns

`void`

#### Implementation of

[IOfflineProvider](../interfaces/IOfflineProvider.md).[open](../interfaces/IOfflineProvider.md#open)

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:188

___

### \_ParseURL

▸ `Static` `Private` **_ParseURL**(`url`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:84

___

### \_ReturnFullUrlLocation

▸ `Static` `Private` **_ReturnFullUrlLocation**(`url`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:93

___

### \_ValidateXHRData

▸ `Static` `Private` **_ValidateXHRData**(`xhr`, `dataType?`): `boolean`

Validates if xhr data is correct

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `xhr` | [`WebRequest`](WebRequest.md) | `undefined` | defines the request to validate |
| `dataType` | `number` | `7` | defines the expected data type |

#### Returns

`boolean`

true if data is correct

#### Defined in

https://github.com/babylon.js/core/src/Offline/database.ts:691

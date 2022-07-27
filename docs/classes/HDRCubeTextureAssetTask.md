[@dev/core](../README.md) / [Exports](../modules.md) / HDRCubeTextureAssetTask

# Class: HDRCubeTextureAssetTask

Define a task used by AssetsManager to load HDR cube textures

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`HDRCubeTextureAssetTask`**

## Implements

- [`ITextureAssetTask`](../interfaces/ITextureAssetTask.md)[`HDRCubeTexture`](HDRCubeTexture.md)

## Table of contents

### Constructors

- [constructor](HDRCubeTextureAssetTask.md#constructor)

### Properties

- [gammaSpace](HDRCubeTextureAssetTask.md#gammaspace)
- [generateHarmonics](HDRCubeTextureAssetTask.md#generateharmonics)
- [name](HDRCubeTextureAssetTask.md#name)
- [noMipmap](HDRCubeTextureAssetTask.md#nomipmap)
- [onError](HDRCubeTextureAssetTask.md#onerror)
- [onSuccess](HDRCubeTextureAssetTask.md#onsuccess)
- [reserved](HDRCubeTextureAssetTask.md#reserved)
- [size](HDRCubeTextureAssetTask.md#size)
- [texture](HDRCubeTextureAssetTask.md#texture)
- [url](HDRCubeTextureAssetTask.md#url)

### Accessors

- [errorObject](HDRCubeTextureAssetTask.md#errorobject)
- [isCompleted](HDRCubeTextureAssetTask.md#iscompleted)
- [taskState](HDRCubeTextureAssetTask.md#taskstate)

### Methods

- [reset](HDRCubeTextureAssetTask.md#reset)
- [run](HDRCubeTextureAssetTask.md#run)
- [runTask](HDRCubeTextureAssetTask.md#runtask)

## Constructors

### constructor

• **new HDRCubeTextureAssetTask**(`name`, `url`, `size`, `noMipmap?`, `generateHarmonics?`, `gammaSpace?`, `reserved?`)

Creates a new HDRCubeTextureAssetTask object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the task |
| `url` | `string` | `undefined` | defines the location of the file to load |
| `size` | `number` | `undefined` | defines the desired size (the more it increases the longer the generation will be) If the size is omitted this implies you are using a preprocessed cubemap. |
| `noMipmap` | `boolean` | `false` | defines if mipmaps should not be generated (default is false) |
| `generateHarmonics` | `boolean` | `true` | specifies whether you want to extract the polynomial harmonics during the generation process (default is true) |
| `gammaSpace` | `boolean` | `false` | specifies if the texture will be use in gamma or linear space (the PBR material requires those texture in linear space, but the standard material would require them in Gamma space) (default is false) |
| `reserved` | `boolean` | `false` | Internal use only |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:765

## Properties

### gammaSpace

• **gammaSpace**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:789

___

### generateHarmonics

• **generateHarmonics**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:785

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:769

___

### noMipmap

• **noMipmap**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:781

___

### onError

• **onError**: (`task`: [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:753

___

### onSuccess

• **onSuccess**: (`task`: [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`HDRCubeTextureAssetTask`](HDRCubeTextureAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:749

___

### reserved

• **reserved**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:793

___

### size

• **size**: `number`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:777

___

### texture

• **texture**: [`HDRCubeTexture`](HDRCubeTexture.md)

Gets the loaded texture

#### Implementation of

[ITextureAssetTask](../interfaces/ITextureAssetTask.md).[texture](../interfaces/ITextureAssetTask.md#texture)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:744

___

### url

• **url**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:773

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

packages/dev/core/src/Misc/assetsManager.ts:804

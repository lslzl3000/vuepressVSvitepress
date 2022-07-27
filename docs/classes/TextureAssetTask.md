[@dev/core](../README.md) / [Exports](../modules.md) / TextureAssetTask

# Class: TextureAssetTask

Define a task used by AssetsManager to load 2D textures

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`TextureAssetTask`**

## Implements

- [`ITextureAssetTask`](../interfaces/ITextureAssetTask.md)[`Texture`](Texture.md)

## Table of contents

### Constructors

- [constructor](TextureAssetTask.md#constructor)

### Properties

- [invertY](TextureAssetTask.md#inverty)
- [name](TextureAssetTask.md#name)
- [noMipmap](TextureAssetTask.md#nomipmap)
- [onError](TextureAssetTask.md#onerror)
- [onSuccess](TextureAssetTask.md#onsuccess)
- [samplingMode](TextureAssetTask.md#samplingmode)
- [texture](TextureAssetTask.md#texture)
- [url](TextureAssetTask.md#url)

### Accessors

- [errorObject](TextureAssetTask.md#errorobject)
- [isCompleted](TextureAssetTask.md#iscompleted)
- [taskState](TextureAssetTask.md#taskstate)

### Methods

- [reset](TextureAssetTask.md#reset)
- [run](TextureAssetTask.md#run)
- [runTask](TextureAssetTask.md#runtask)

## Constructors

### constructor

• **new TextureAssetTask**(`name`, `url`, `noMipmap?`, `invertY?`, `samplingMode?`)

Creates a new TextureAssetTask object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the task |
| `url` | `string` | `undefined` | defines the location of the file to load |
| `noMipmap?` | `boolean` | `undefined` | defines if mipmap should not be generated (default is false) |
| `invertY` | `boolean` | `true` | defines if texture must be inverted on Y axis (default is true) |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | defines the sampling mode to use (default is Texture.TRILINEAR_SAMPLINGMODE) |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:618

## Properties

### invertY

• **invertY**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:634

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:622

___

### noMipmap

• `Optional` **noMipmap**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:630

___

### onError

• **onError**: (`task`: [`TextureAssetTask`](TextureAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`TextureAssetTask`](TextureAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:608

___

### onSuccess

• **onSuccess**: (`task`: [`TextureAssetTask`](TextureAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`TextureAssetTask`](TextureAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:604

___

### samplingMode

• **samplingMode**: `number` = `Texture.TRILINEAR_SAMPLINGMODE`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:638

___

### texture

• **texture**: [`Texture`](Texture.md)

Gets the loaded texture

#### Implementation of

[ITextureAssetTask](../interfaces/ITextureAssetTask.md).[texture](../interfaces/ITextureAssetTask.md#texture)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:599

___

### url

• **url**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:626

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

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:85

___

### isCompleted

• `get` **isCompleted**(): `boolean`

Get if the task is completed

#### Returns

`boolean`

#### Inherited from

AbstractAssetTask.isCompleted

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:71

___

### taskState

• `get` **taskState**(): [`AssetTaskState`](../enums/AssetTaskState.md)

Gets the current state of the task

#### Returns

[`AssetTaskState`](../enums/AssetTaskState.md)

#### Inherited from

AbstractAssetTask.taskState

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:78

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

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:140

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

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:112

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

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:649

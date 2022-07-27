[@dev/core](../README.md) / [Exports](../modules.md) / EquiRectangularCubeTextureAssetTask

# Class: EquiRectangularCubeTextureAssetTask

Define a task used by AssetsManager to load Equirectangular cube textures

## Hierarchy

- [`AbstractAssetTask`](AbstractAssetTask.md)

  ↳ **`EquiRectangularCubeTextureAssetTask`**

## Implements

- [`ITextureAssetTask`](../interfaces/ITextureAssetTask.md)[`EquiRectangularCubeTexture`](EquiRectangularCubeTexture.md)

## Table of contents

### Constructors

- [constructor](EquiRectangularCubeTextureAssetTask.md#constructor)

### Properties

- [gammaSpace](EquiRectangularCubeTextureAssetTask.md#gammaspace)
- [name](EquiRectangularCubeTextureAssetTask.md#name)
- [noMipmap](EquiRectangularCubeTextureAssetTask.md#nomipmap)
- [onError](EquiRectangularCubeTextureAssetTask.md#onerror)
- [onSuccess](EquiRectangularCubeTextureAssetTask.md#onsuccess)
- [size](EquiRectangularCubeTextureAssetTask.md#size)
- [texture](EquiRectangularCubeTextureAssetTask.md#texture)
- [url](EquiRectangularCubeTextureAssetTask.md#url)

### Accessors

- [errorObject](EquiRectangularCubeTextureAssetTask.md#errorobject)
- [isCompleted](EquiRectangularCubeTextureAssetTask.md#iscompleted)
- [taskState](EquiRectangularCubeTextureAssetTask.md#taskstate)

### Methods

- [reset](EquiRectangularCubeTextureAssetTask.md#reset)
- [run](EquiRectangularCubeTextureAssetTask.md#run)
- [runTask](EquiRectangularCubeTextureAssetTask.md#runtask)

## Constructors

### constructor

• **new EquiRectangularCubeTextureAssetTask**(`name`, `url`, `size`, `noMipmap?`, `gammaSpace?`)

Creates a new EquiRectangularCubeTextureAssetTask object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the task |
| `url` | `string` | `undefined` | defines the location of the file to load |
| `size` | `number` | `undefined` | defines the desired size (the more it increases the longer the generation will be)  If the size is omitted this implies you are using a preprocessed cubemap. |
| `noMipmap` | `boolean` | `false` | defines if mipmaps should not be generated (default is false) |
| `gammaSpace` | `boolean` | `true` | specifies if the texture will be used in gamma or linear space  (the PBR material requires those texture in linear space, but the standard material would require them in Gamma space)  (default is true) |

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[constructor](AbstractAssetTask.md#constructor)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:846

## Properties

### gammaSpace

• **gammaSpace**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:867

___

### name

• **name**: `string`

#### Inherited from

[AbstractAssetTask](AbstractAssetTask.md).[name](AbstractAssetTask.md#name)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:850

___

### noMipmap

• **noMipmap**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:862

___

### onError

• **onError**: (`task`: [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md), `message?`: `string`, `exception?`: `any`) => `void`

#### Type declaration

▸ (`task`, `message?`, `exception?`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md) |
| `message?` | `string` |
| `exception?` | `any` |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onError](AbstractAssetTask.md#onerror)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:833

___

### onSuccess

• **onSuccess**: (`task`: [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md)) => `void`

#### Type declaration

▸ (`task`): `void`

Callback called when the task is successful

##### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`EquiRectangularCubeTextureAssetTask`](EquiRectangularCubeTextureAssetTask.md) |

##### Returns

`void`

#### Overrides

[AbstractAssetTask](AbstractAssetTask.md).[onSuccess](AbstractAssetTask.md#onsuccess)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:829

___

### size

• **size**: `number`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:858

___

### texture

• **texture**: [`EquiRectangularCubeTexture`](EquiRectangularCubeTexture.md)

Gets the loaded texture

#### Implementation of

[ITextureAssetTask](../interfaces/ITextureAssetTask.md).[texture](../interfaces/ITextureAssetTask.md#texture)

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:824

___

### url

• **url**: `string`

#### Defined in

packages/dev/core/src/Misc/assetsManager.ts:854

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

packages/dev/core/src/Misc/assetsManager.ts:878

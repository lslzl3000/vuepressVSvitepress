[@dev/core](../README.md) / [Exports](../modules.md) / SceneRecorder

# Class: SceneRecorder

Class used to record delta files between 2 scene states

## Table of contents

### Constructors

- [constructor](SceneRecorder.md#constructor)

### Properties

- [\_savedJSON](SceneRecorder.md#_savedjson)
- [\_trackedScene](SceneRecorder.md#_trackedscene)

### Methods

- [\_compareArray](SceneRecorder.md#_comparearray)
- [\_compareCollections](SceneRecorder.md#_comparecollections)
- [\_compareObjects](SceneRecorder.md#_compareobjects)
- [getDelta](SceneRecorder.md#getdelta)
- [track](SceneRecorder.md#track)
- [ApplyDelta](SceneRecorder.md#applydelta)
- [GetShadowGeneratorById](SceneRecorder.md#getshadowgeneratorbyid)
- [\_ApplyDeltaForEntity](SceneRecorder.md#_applydeltaforentity)
- [\_ApplyPropertiesToEntity](SceneRecorder.md#_applypropertiestoentity)

## Constructors

### constructor

• **new SceneRecorder**()

## Properties

### \_savedJSON

• `Private` **\_savedJSON**: `any`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:24

___

### \_trackedScene

• `Private` **\_trackedScene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:23

## Methods

### \_compareArray

▸ `Private` **_compareArray**(`key`, `original`, `current`, `deltaJSON`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `string` |
| `original` | `any`[] |
| `current` | `any`[] |
| `deltaJSON` | `any` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:64

___

### \_compareCollections

▸ `Private` **_compareCollections**(`key`, `original`, `current`, `deltaJSON`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `string` |
| `original` | `any`[] |
| `current` | `any`[] |
| `deltaJSON` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:171

___

### \_compareObjects

▸ `Private` **_compareObjects**(`originalObjet`, `currentObject`, `deltaJSON`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `originalObjet` | `any` |
| `currentObject` | `any` |
| `deltaJSON` | `any` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:139

___

### getDelta

▸ **getDelta**(): `any`

Get the delta between current state and original state

#### Returns

`any`

a any containing the delta

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:42

___

### track

▸ **track**(`scene`): `void`

Track a given scene. This means the current scene state will be considered the original state

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene to track |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:30

___

### ApplyDelta

▸ `Static` **ApplyDelta**(`deltaJSON`, `scene`): `void`

Apply a given delta to a given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `deltaJSON` | `any` | defines the JSON containing the delta |
| `scene` | [`Scene`](Scene.md) | defines the scene to apply the delta to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:211

___

### GetShadowGeneratorById

▸ `Static` `Private` **GetShadowGeneratorById**(`scene`, `id`): ``null`` \| [`IShadowGenerator`](../interfaces/IShadowGenerator.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `id` | `string` |

#### Returns

``null`` \| [`IShadowGenerator`](../interfaces/IShadowGenerator.md)

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:194

___

### \_ApplyDeltaForEntity

▸ `Static` `Private` **_ApplyDeltaForEntity**(`sources`, `scene`, `finder`, `addNew`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sources` | `any`[] |
| `scene` | [`Scene`](Scene.md) |
| `finder` | (`id`: `string`) => `any` |
| `addNew` | (`data`: `any`) => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:291

___

### \_ApplyPropertiesToEntity

▸ `Static` `Private` **_ApplyPropertiesToEntity**(`deltaJSON`, `entity`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `deltaJSON` | `any` |
| `entity` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneRecorder.ts:272

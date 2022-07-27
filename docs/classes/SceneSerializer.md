[@dev/core](../README.md) / [Exports](../modules.md) / SceneSerializer

# Class: SceneSerializer

Class used to serialize a scene into a string

## Table of contents

### Constructors

- [constructor](SceneSerializer.md#constructor)

### Methods

- [ClearCache](SceneSerializer.md#clearcache)
- [Serialize](SceneSerializer.md#serialize)
- [SerializeAsync](SceneSerializer.md#serializeasync)
- [SerializeMesh](SceneSerializer.md#serializemesh)
- [\_CollectPromises](SceneSerializer.md#_collectpromises)
- [\_Serialize](SceneSerializer.md#_serialize)

## Constructors

### constructor

• **new SceneSerializer**()

## Methods

### ClearCache

▸ `Static` **ClearCache**(): `void`

Clear cache used by a previous serialization

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:109

___

### Serialize

▸ `Static` **Serialize**(`scene`): `any`

Serialize a scene into a JSON compatible object
Note that if the current engine does not support synchronous texture reading (like WebGPU), you should use SerializeAsync instead
as else you may not retrieve the proper base64 encoded texture data (when using the Texture.ForceSerializeBuffers flag)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene to serialize |

#### Returns

`any`

a JSON compatible object

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:120

___

### SerializeAsync

▸ `Static` **SerializeAsync**(`scene`): `Promise``any`

Serialize a scene into a JSON compatible object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene to serialize |

#### Returns

`Promise``any`

a JSON promise compatible object

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:341

___

### SerializeMesh

▸ `Static` **SerializeMesh**(`toSerialize`, `withParents?`, `withChildren?`): `any`

Serialize a mesh into a JSON compatible object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `toSerialize` | `any` | `undefined` | defines the mesh to serialize |
| `withParents` | `boolean` | `false` | defines if parents must be serialized as well |
| `withChildren` | `boolean` | `false` | defines if children must be serialized as well |

#### Returns

`any`

a JSON compatible object

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:382

___

### \_CollectPromises

▸ `Static` `Private` **_CollectPromises**(`obj`, `promises`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `obj` | `any` |
| `promises` | `Promise``any`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:351

___

### \_Serialize

▸ `Static` `Private` **_Serialize**(`scene`, `checkSyncReadSupported?`): `any`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` |
| `checkSyncReadSupported` | `boolean` | `true` |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/sceneSerializer.ts:124

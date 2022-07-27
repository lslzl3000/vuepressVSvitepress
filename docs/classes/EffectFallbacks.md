[@dev/core](../README.md) / [Exports](../modules.md) / EffectFallbacks

# Class: EffectFallbacks

EffectFallbacks can be used to add fallbacks (properties to disable) to certain properties when desired to improve performance.
(Eg. Start at high quality with reflection and fog, if fps is low, remove reflection, if still low remove fog)

## Implements

- [`IEffectFallbacks`](../interfaces/IEffectFallbacks.md)

## Table of contents

### Constructors

- [constructor](EffectFallbacks.md#constructor)

### Properties

- [\_currentRank](EffectFallbacks.md#_currentrank)
- [\_defines](EffectFallbacks.md#_defines)
- [\_maxRank](EffectFallbacks.md#_maxrank)
- [\_mesh](EffectFallbacks.md#_mesh)

### Accessors

- [hasMoreFallbacks](EffectFallbacks.md#hasmorefallbacks)

### Methods

- [addCPUSkinningFallback](EffectFallbacks.md#addcpuskinningfallback)
- [addFallback](EffectFallbacks.md#addfallback)
- [reduce](EffectFallbacks.md#reduce)
- [unBindMesh](EffectFallbacks.md#unbindmesh)

## Constructors

### constructor

• **new EffectFallbacks**()

## Properties

### \_currentRank

• `Private` **\_currentRank**: `number` = `32`

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:14

___

### \_defines

• `Private` **\_defines**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `String`[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:12

___

### \_maxRank

• `Private` **\_maxRank**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:15

___

### \_mesh

• `Private` **\_mesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:17

## Accessors

### hasMoreFallbacks

• `get` **hasMoreFallbacks**(): `boolean`

Checks to see if more fallbacks are still available.

#### Returns

`boolean`

#### Implementation of

[IEffectFallbacks](../interfaces/IEffectFallbacks.md).[hasMoreFallbacks](../interfaces/IEffectFallbacks.md#hasmorefallbacks)

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:66

## Methods

### addCPUSkinningFallback

▸ **addCPUSkinningFallback**(`rank`, `mesh`): `void`

Sets the mesh to use CPU skinning when needing to fallback.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rank` | `number` | The rank of the fallback (Lower ranks will be fallbacked to first) |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to use the fallbacks. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:52

___

### addFallback

▸ **addFallback**(`rank`, `define`): `void`

Adds a fallback on the specified property.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rank` | `number` | The rank of the fallback (Lower ranks will be fallbacked to first) |
| `define` | `string` | The name of the define in the shader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:31

___

### reduce

▸ **reduce**(`currentDefines`, `effect`): `string`

Removes the defines that should be removed when falling back.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentDefines` | `string` | defines the current define statements for the shader. |
| `effect` | [`Effect`](Effect.md) | defines the current effect we try to compile |

#### Returns

`string`

The resulting defines with defines of the current rank removed.

#### Implementation of

[IEffectFallbacks](../interfaces/IEffectFallbacks.md).[reduce](../interfaces/IEffectFallbacks.md#reduce)

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:76

___

### unBindMesh

▸ **unBindMesh**(): `void`

Removes the fallback from the bound mesh.

#### Returns

`void`

#### Implementation of

[IEffectFallbacks](../interfaces/IEffectFallbacks.md).[unBindMesh](../interfaces/IEffectFallbacks.md#unbindmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/effectFallbacks.ts:22

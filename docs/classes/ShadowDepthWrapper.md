[@dev/core](../README.md) / [Exports](../modules.md) / ShadowDepthWrapper

# Class: ShadowDepthWrapper

Class that can be used to wrap a base material to generate accurate shadows when using custom vertex/fragment code in the base material

## Table of contents

### Constructors

- [constructor](ShadowDepthWrapper.md#constructor)

### Properties

- [\_baseMaterial](ShadowDepthWrapper.md#_basematerial)
- [\_meshes](ShadowDepthWrapper.md#_meshes)
- [\_onEffectCreatedObserver](ShadowDepthWrapper.md#_oneffectcreatedobserver)
- [\_options](ShadowDepthWrapper.md#_options)
- [\_scene](ShadowDepthWrapper.md#_scene)
- [\_subMeshToDepthWrapper](ShadowDepthWrapper.md#_submeshtodepthwrapper)
- [\_subMeshToEffect](ShadowDepthWrapper.md#_submeshtoeffect)

### Accessors

- [baseMaterial](ShadowDepthWrapper.md#basematerial)
- [standalone](ShadowDepthWrapper.md#standalone)

### Methods

- [\_makeEffect](ShadowDepthWrapper.md#_makeeffect)
- [dispose](ShadowDepthWrapper.md#dispose)
- [getEffect](ShadowDepthWrapper.md#geteffect)
- [isReadyForSubMesh](ShadowDepthWrapper.md#isreadyforsubmesh)

## Constructors

### constructor

• **new ShadowDepthWrapper**(`baseMaterial`, `scene?`, `options?`)

Instantiate a new shadow depth wrapper.
It works by injecting some specific code in the vertex/fragment shaders of the base material and is used by a shadow generator to
generate the shadow depth map. For more information, please refer to the documentation:
https://doc.babylonjs.com/babylon101/shadows

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseMaterial` | [`Material`](Material.md) | Material to wrap |
| `scene?` | [`Scene`](Scene.md) | Define the scene the material belongs to |
| `options?` | [`IIOptionShadowDepthMaterial`](../interfaces/IIOptionShadowDepthMaterial.md) | Options used to create the wrapper |

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:87

## Properties

### \_baseMaterial

• `Private` **\_baseMaterial**: [`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:58

___

### \_meshes

• `Private` **\_meshes**: `Map`[`AbstractMesh`](AbstractMesh.md), [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Node`](Node.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:66

___

### \_onEffectCreatedObserver

• `Private` **\_onEffectCreatedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:59

___

### \_options

• `Private` `Optional` **\_options**: [`IIOptionShadowDepthMaterial`](../interfaces/IIOptionShadowDepthMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:57

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:56

___

### \_subMeshToDepthWrapper

• `Private` **\_subMeshToDepthWrapper**: `MapMap`[`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md), [`ShadowGenerator`](ShadowGenerator.md), { `depthDefines`: `string` ; `drawWrapper`: [`Nullable`](../modules.md#nullable)`DrawWrapper`[] ; `mainDrawWrapper`: `DrawWrapper` ; `token`: `string`  }

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:61

___

### \_subMeshToEffect

• `Private` **\_subMeshToEffect**: `Map`[`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md), [[`Effect`](Effect.md), `number`]

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:60

## Accessors

### baseMaterial

• `get` **baseMaterial**(): [`Material`](Material.md)

Gets the base material the wrapper is built upon

#### Returns

[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:74

___

### standalone

• `get` **standalone**(): `boolean`

Gets the standalone status of the wrapper

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:69

## Methods

### \_makeEffect

▸ `Private` **_makeEffect**(`subMesh`, `defines`, `shadowGenerator`, `passIdForDrawWrapper`): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `defines` | `string`[] |
| `shadowGenerator` | [`ShadowGenerator`](ShadowGenerator.md) |
| `passIdForDrawWrapper` | `number` |

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:179

___

### dispose

▸ **dispose**(): `void`

Disposes the resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:167

___

### getEffect

▸ **getEffect**(`subMesh`, `shadowGenerator`, `passIdForDrawWrapper`): [`Nullable`](../modules.md#nullable)`DrawWrapper`

Gets the effect to use to generate the depth map

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md) | subMesh to get the effect for |
| `shadowGenerator` | [`ShadowGenerator`](ShadowGenerator.md) | shadow generator to get the effect for |
| `passIdForDrawWrapper` | `number` | Id of the pass for which the effect from the draw wrapper must be retrieved from |

#### Returns

[`Nullable`](../modules.md#nullable)`DrawWrapper`

the effect to use to generate the depth map for the subMesh + shadow generator specified

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:130

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`subMesh`, `defines`, `shadowGenerator`, `useInstances`, `passIdForDrawWrapper`): `boolean`

Specifies that the submesh is ready to be used for depth rendering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | submesh to check |
| `defines` | `string`[] | the list of defines to take into account when checking the effect |
| `shadowGenerator` | [`ShadowGenerator`](ShadowGenerator.md) | combined with subMesh, it defines the effect to check |
| `useInstances` | `boolean` | specifies that instances should be used |
| `passIdForDrawWrapper` | `number` | Id of the pass for which the draw wrapper should be created |

#### Returns

`boolean`

a boolean indicating that the submesh is ready or not

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:153

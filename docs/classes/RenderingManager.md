[@dev/core](../README.md) / [Exports](../modules.md) / RenderingManager

# Class: RenderingManager

This is the manager responsible of all the rendering for meshes sprites and particles.
It is enable to manage the different groups as well as the different necessary sort functions.
This should not be used directly aside of the few static configurations

## Table of contents

### Constructors

- [constructor](RenderingManager.md#constructor)

### Properties

- [\_autoClearDepthStencil](RenderingManager.md#_autocleardepthstencil)
- [\_customAlphaTestSortCompareFn](RenderingManager.md#_customalphatestsortcomparefn)
- [\_customOpaqueSortCompareFn](RenderingManager.md#_customopaquesortcomparefn)
- [\_customTransparentSortCompareFn](RenderingManager.md#_customtransparentsortcomparefn)
- [\_depthStencilBufferAlreadyCleaned](RenderingManager.md#_depthstencilbufferalreadycleaned)
- [\_renderingGroupInfo](RenderingManager.md#_renderinggroupinfo)
- [\_renderingGroups](RenderingManager.md#_renderinggroups)
- [\_scene](RenderingManager.md#_scene)
- [AUTOCLEAR](RenderingManager.md#autoclear)
- [MAX\_RENDERINGGROUPS](RenderingManager.md#max_renderinggroups)
- [MIN\_RENDERINGGROUPS](RenderingManager.md#min_renderinggroups)

### Methods

- [\_clearDepthStencilBuffer](RenderingManager.md#_cleardepthstencilbuffer)
- [\_prepareRenderingGroup](RenderingManager.md#_preparerenderinggroup)
- [dispatch](RenderingManager.md#dispatch)
- [dispatchParticles](RenderingManager.md#dispatchparticles)
- [dispatchSprites](RenderingManager.md#dispatchsprites)
- [freeRenderingGroups](RenderingManager.md#freerenderinggroups)
- [getAutoClearDepthStencilSetup](RenderingManager.md#getautocleardepthstencilsetup)
- [setRenderingAutoClearDepthStencil](RenderingManager.md#setrenderingautocleardepthstencil)
- [setRenderingOrder](RenderingManager.md#setrenderingorder)

## Constructors

### constructor

• **new RenderingManager**(`scene`)

Instantiates a new rendering group for a particular scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene the groups belongs to |

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:92

## Properties

### \_autoClearDepthStencil

• `Private` **\_autoClearDepthStencil**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: [`IRenderingManagerAutoClearSetup`](../interfaces/IRenderingManagerAutoClearSetup.md)

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:82

___

### \_customAlphaTestSortCompareFn

• `Private` **\_customAlphaTestSortCompareFn**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: [`Nullable`](../modules.md#nullable)(`a`: `SubMesh`, `b`: `SubMesh`) => `number`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:84

___

### \_customOpaqueSortCompareFn

• `Private` **\_customOpaqueSortCompareFn**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: [`Nullable`](../modules.md#nullable)(`a`: `SubMesh`, `b`: `SubMesh`) => `number`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:83

___

### \_customTransparentSortCompareFn

• `Private` **\_customTransparentSortCompareFn**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: [`Nullable`](../modules.md#nullable)(`a`: `SubMesh`, `b`: `SubMesh`) => `number`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:85

___

### \_depthStencilBufferAlreadyCleaned

• `Private` **\_depthStencilBufferAlreadyCleaned**: `boolean`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:80

___

### \_renderingGroupInfo

• `Private` **\_renderingGroupInfo**: [`Nullable`](../modules.md#nullable)[`RenderingGroupInfo`](RenderingGroupInfo.md)

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:86

___

### \_renderingGroups

• `Private` **\_renderingGroups**: `RenderingGroup`[]

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:79

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:78

___

### AUTOCLEAR

▪ `Static` **AUTOCLEAR**: `boolean` = `true`

Used to globally prevent autoclearing scenes.

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:71

___

### MAX\_RENDERINGGROUPS

▪ `Static` **MAX\_RENDERINGGROUPS**: `number` = `4`

The max id used for rendering groups (not included)

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:61

___

### MIN\_RENDERINGGROUPS

▪ `Static` **MIN\_RENDERINGGROUPS**: `number` = `0`

The min id used for rendering groups (included)

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:66

## Methods

### \_clearDepthStencilBuffer

▸ `Private` **_clearDepthStencilBuffer**(`depth?`, `stencil?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `depth` | `boolean` | `true` |
| `stencil` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:100

___

### \_prepareRenderingGroup

▸ `Private` **_prepareRenderingGroup**(`renderingGroupId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderingGroupId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:215

___

### dispatch

▸ **dispatch**(`subMesh`, `mesh?`, `material?`): `void`

Add a submesh to the manager in order to render it this frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | The submesh to dispatch |
| `mesh?` | [`AbstractMesh`](AbstractMesh.md) | Optional reference to the submeshes's mesh. Provide if you have an exiting reference to improve performance. |
| `material?` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md) | Optional reference to the submeshes's material. Provide if you have an exiting reference to improve performance. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:257

___

### dispatchParticles

▸ **dispatchParticles**(`particleSystem`): `void`

Add a particle system to the rendering manager in order to render it this frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particleSystem` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | Define the particle system to render |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:243

___

### dispatchSprites

▸ **dispatchSprites**(`spriteManager`): `void`

Add a sprite manager to the rendering manager in order to render it this frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `spriteManager` | [`ISpriteManager`](../interfaces/ISpriteManager.md) | Define the sprite manager to render |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:231

___

### freeRenderingGroups

▸ **freeRenderingGroups**(): `void`

Clear the info related to rendering groups preventing retention points during dispose.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:206

___

### getAutoClearDepthStencilSetup

▸ **getAutoClearDepthStencilSetup**(`index`): [`IRenderingManagerAutoClearSetup`](../interfaces/IRenderingManagerAutoClearSetup.md)

Gets the current auto clear configuration for one rendering group of the rendering
manager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | the rendering group index to get the information for |

#### Returns

[`IRenderingManagerAutoClearSetup`](../interfaces/IRenderingManagerAutoClearSetup.md)

The auto clear setup for the requested rendering group

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:317

___

### setRenderingAutoClearDepthStencil

▸ **setRenderingAutoClearDepthStencil**(`renderingGroupId`, `autoClearDepthStencil`, `depth?`, `stencil?`): `void`

Specifies whether or not the stencil and depth buffer are cleared between two rendering groups.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderingGroupId` | `number` | `undefined` | The rendering group id corresponding to its index |
| `autoClearDepthStencil` | `boolean` | `undefined` | Automatically clears depth and stencil between groups if true. |
| `depth` | `boolean` | `true` | Automatically clears depth between groups if true and autoClear is true. |
| `stencil` | `boolean` | `true` | Automatically clears stencil between groups if true and autoClear is true. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:303

___

### setRenderingOrder

▸ **setRenderingOrder**(`renderingGroupId`, `opaqueSortCompareFn?`, `alphaTestSortCompareFn?`, `transparentSortCompareFn?`): `void`

Overrides the default sort function applied in the rendering group to prepare the meshes.
This allowed control for front to back rendering or reversely depending of the special needs.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderingGroupId` | `number` | `undefined` | The rendering group id corresponding to its index |
| `opaqueSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The opaque queue comparison function use to sort. |
| `alphaTestSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The alpha test queue comparison function use to sort. |
| `transparentSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The transparent queue comparison function use to sort. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/renderingManager.ts:277

[@dev/core](../README.md) / [Exports](../modules.md) / GeometryBufferRenderer

# Class: GeometryBufferRenderer

This renderer is helpful to fill one of the render target with a geometry buffer.

## Table of contents

### Constructors

- [constructor](GeometryBufferRenderer.md#constructor)

### Properties

- [\_attachments](GeometryBufferRenderer.md#_attachments)
- [\_cachedDefines](GeometryBufferRenderer.md#_cacheddefines)
- [\_depthIndex](GeometryBufferRenderer.md#_depthindex)
- [\_enablePosition](GeometryBufferRenderer.md#_enableposition)
- [\_enableReflectivity](GeometryBufferRenderer.md#_enablereflectivity)
- [\_enableVelocity](GeometryBufferRenderer.md#_enablevelocity)
- [\_linkedWithPrePass](GeometryBufferRenderer.md#_linkedwithprepass)
- [\_multiRenderTarget](GeometryBufferRenderer.md#_multirendertarget)
- [\_normalIndex](GeometryBufferRenderer.md#_normalindex)
- [\_positionIndex](GeometryBufferRenderer.md#_positionindex)
- [\_prePassRenderer](GeometryBufferRenderer.md#_prepassrenderer)
- [\_ratio](GeometryBufferRenderer.md#_ratio)
- [\_reflectivityIndex](GeometryBufferRenderer.md#_reflectivityindex)
- [\_resizeObserver](GeometryBufferRenderer.md#_resizeobserver)
- [\_scene](GeometryBufferRenderer.md#_scene)
- [\_useUbo](GeometryBufferRenderer.md#_useubo)
- [\_velocityIndex](GeometryBufferRenderer.md#_velocityindex)
- [excludedSkinnedMeshesFromVelocity](GeometryBufferRenderer.md#excludedskinnedmeshesfromvelocity)
- [renderTransparentMeshes](GeometryBufferRenderer.md#rendertransparentmeshes)
- [DEPTH\_TEXTURE\_TYPE](GeometryBufferRenderer.md#depth_texture_type)
- [NORMAL\_TEXTURE\_TYPE](GeometryBufferRenderer.md#normal_texture_type)
- [POSITION\_TEXTURE\_TYPE](GeometryBufferRenderer.md#position_texture_type)
- [REFLECTIVITY\_TEXTURE\_TYPE](GeometryBufferRenderer.md#reflectivity_texture_type)
- [VELOCITY\_TEXTURE\_TYPE](GeometryBufferRenderer.md#velocity_texture_type)

### Accessors

- [enablePosition](GeometryBufferRenderer.md#enableposition)
- [enableReflectivity](GeometryBufferRenderer.md#enablereflectivity)
- [enableVelocity](GeometryBufferRenderer.md#enablevelocity)
- [isSupported](GeometryBufferRenderer.md#issupported)
- [ratio](GeometryBufferRenderer.md#ratio)
- [renderList](GeometryBufferRenderer.md#renderlist)
- [samples](GeometryBufferRenderer.md#samples)
- [scene](GeometryBufferRenderer.md#scene)

### Methods

- [\_assignRenderTargetIndices](GeometryBufferRenderer.md#_assignrendertargetindices)
- [\_copyBonesTransformationMatrices](GeometryBufferRenderer.md#_copybonestransformationmatrices)
- [\_createRenderTargets](GeometryBufferRenderer.md#_createrendertargets)
- [dispose](GeometryBufferRenderer.md#dispose)
- [getGBuffer](GeometryBufferRenderer.md#getgbuffer)
- [getTextureIndex](GeometryBufferRenderer.md#gettextureindex)
- [isReady](GeometryBufferRenderer.md#isready)

## Constructors

### constructor

• **new GeometryBufferRenderer**(`scene`, `ratio?`)

Creates a new G Buffer for the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the buffer belongs to |
| `ratio` | `number` | `1` | How big is the buffer related to the main canvas. |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:323

## Properties

### \_attachments

• `Private` **\_attachments**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:98

___

### \_cachedDefines

• `Protected` **\_cachedDefines**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:101

___

### \_depthIndex

• `Private` **\_depthIndex**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:93

___

### \_enablePosition

• `Private` **\_enablePosition**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:86

___

### \_enableReflectivity

• `Private` **\_enableReflectivity**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:88

___

### \_enableVelocity

• `Private` **\_enableVelocity**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:87

___

### \_linkedWithPrePass

• `Private` **\_linkedWithPrePass**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:96

___

### \_multiRenderTarget

• `Private` **\_multiRenderTarget**: [`MultiRenderTarget`](MultiRenderTarget.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:84

___

### \_normalIndex

• `Private` **\_normalIndex**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:94

___

### \_positionIndex

• `Private` **\_positionIndex**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:90

___

### \_prePassRenderer

• `Private` **\_prePassRenderer**: [`PrePassRenderer`](PrePassRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:97

___

### \_ratio

• `Private` **\_ratio**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:85

___

### \_reflectivityIndex

• `Private` **\_reflectivityIndex**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:92

___

### \_resizeObserver

• `Private` **\_resizeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:83

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:82

___

### \_useUbo

• `Private` **\_useUbo**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:99

___

### \_velocityIndex

• `Private` **\_velocityIndex**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:91

___

### excludedSkinnedMeshesFromVelocity

• **excludedSkinnedMeshesFromVelocity**: [`AbstractMesh`](AbstractMesh.md)[] = `[]`

Array used to store the ignored skinned meshes while computing velocity map (typically used by the motion blur post-process).
Avoids computing bones velocities and computes only mesh's velocity itself (position, rotation, scaling).

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:77

___

### renderTransparentMeshes

• **renderTransparentMeshes**: `boolean` = `true`

Gets or sets a boolean indicating if transparent meshes should be rendered

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:80

___

### DEPTH\_TEXTURE\_TYPE

▪ `Static` `Readonly` **DEPTH\_TEXTURE\_TYPE**: ``0``

Constant used to retrieve the depth texture index in the G-Buffer textures array
using getIndex(GeometryBufferRenderer.DEPTH_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:39

___

### NORMAL\_TEXTURE\_TYPE

▪ `Static` `Readonly` **NORMAL\_TEXTURE\_TYPE**: ``1``

Constant used to retrieve the normal texture index in the G-Buffer textures array
using getIndex(GeometryBufferRenderer.NORMAL_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:44

___

### POSITION\_TEXTURE\_TYPE

▪ `Static` `Readonly` **POSITION\_TEXTURE\_TYPE**: ``2``

Constant used to retrieve the position texture index in the G-Buffer textures array
using getIndex(GeometryBufferRenderer.POSITION_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:49

___

### REFLECTIVITY\_TEXTURE\_TYPE

▪ `Static` `Readonly` **REFLECTIVITY\_TEXTURE\_TYPE**: ``4``

Constant used to retrieve the reflectivity texture index in the G-Buffer textures array
using the getIndex(GeometryBufferRenderer.REFLECTIVITY_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:59

___

### VELOCITY\_TEXTURE\_TYPE

▪ `Static` `Readonly` **VELOCITY\_TEXTURE\_TYPE**: ``3``

Constant used to retrieve the velocity texture index in the G-Buffer textures array
using getIndex(GeometryBufferRenderer.VELOCITY_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:54

## Accessors

### enablePosition

• `get` **enablePosition**(): `boolean`

Gets a boolean indicating if objects positions are enabled for the G buffer.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:230

• `set` **enablePosition**(`enable`): `void`

Sets whether or not objects positions are enabled for the G buffer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enable` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:237

___

### enableReflectivity

• `get` **enableReflectivity**(): `boolean`

Gets a boolean indicating if objects reflectivity are enabled in the G buffer.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:275

• `set` **enableReflectivity**(`enable`): `void`

Sets whether or not objects reflectivity are enabled for the G buffer.
For Metallic-Roughness workflow with ORM texture, we assume that ORM texture is defined according to the default layout:
pbr.useRoughnessFromMetallicTextureAlpha = false;
pbr.useRoughnessFromMetallicTextureGreen = true;
pbr.useMetallnessFromMetallicTextureBlue = true;

#### Parameters

| Name | Type |
| :------ | :------ |
| `enable` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:286

___

### enableVelocity

• `get` **enableVelocity**(): `boolean`

Gets a boolean indicating if objects velocities are enabled for the G buffer.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:250

• `set` **enableVelocity**(`enable`): `void`

Sets whether or not objects velocities are enabled for the G buffer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enable` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:257

___

### isSupported

• `get` **isSupported**(): `boolean`

Gets whether or not G buffer are supported by the running hardware.
This requires draw buffer supports

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:205

___

### ratio

• `get` **ratio**(): `number`

Gets the ratio used by the buffer during its creation.
How big is the buffer related to the main canvas.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:306

___

### renderList

• `get` **renderList**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Gets the render list (meshes to be rendered) used in the G buffer.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:190

• `set` **renderList**(`meshes`): `void`

Set the render list (meshes to be rendered) used in the G buffer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshes` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:197

___

### samples

• `get` **samples**(): `number`

Gets the number of samples used to render the buffer (anti aliasing).

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:635

• `set` **samples**(`value`): `void`

Sets the number of samples used to render the buffer (anti aliasing).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:642

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets the scene associated with the buffer.

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:298

## Methods

### \_assignRenderTargetIndices

▸ `Private` **_assignRenderTargetIndices**(): [`number`, `string`[]]

#### Returns

[`number`, `string`[]]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:658

___

### \_copyBonesTransformationMatrices

▸ `Private` **_copyBonesTransformationMatrices**(`source`, `target`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `Float32Array` |
| `target` | `Float32Array` |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:1019

___

### \_createRenderTargets

▸ `Protected` **_createRenderTargets**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:685

___

### dispose

▸ **dispose**(): `void`

Disposes the renderer and frees up associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:649

___

### getGBuffer

▸ **getGBuffer**(): [`MultiRenderTarget`](MultiRenderTarget.md)

Gets the current underlying G Buffer.

#### Returns

[`MultiRenderTarget`](MultiRenderTarget.md)

the buffer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:628

___

### getTextureIndex

▸ **getTextureIndex**(`textureType`): `number`

Returns the index of the given texture type in the G-Buffer textures array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `textureType` | `number` | The texture type constant. For example GeometryBufferRenderer.POSITION_TEXTURE_INDEX |

#### Returns

`number`

the index of the given texture type in the G-Buffer textures array

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:214

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`): `boolean`

Checks whether everything is ready to render a submesh to the G buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | the submesh to check readiness for |
| `useInstances` | `boolean` | is the mesh drawn using instance or not |

#### Returns

`boolean`

true if ready otherwise false

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRenderer.ts:340

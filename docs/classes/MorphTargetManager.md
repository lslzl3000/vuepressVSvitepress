[@dev/core](../README.md) / [Exports](../modules.md) / MorphTargetManager

# Class: MorphTargetManager

This class is used to deform meshes using morphing between different targets

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](MorphTargetManager.md#constructor)

### Properties

- [\_activeTargets](MorphTargetManager.md#_activetargets)
- [\_blockCounter](MorphTargetManager.md#_blockcounter)
- [\_canUseTextureForTargets](MorphTargetManager.md#_canusetexturefortargets)
- [\_influences](MorphTargetManager.md#_influences)
- [\_morphTargetTextureIndices](MorphTargetManager.md#_morphtargettextureindices)
- [\_scene](MorphTargetManager.md#_scene)
- [\_supportsNormals](MorphTargetManager.md#_supportsnormals)
- [\_supportsTangents](MorphTargetManager.md#_supportstangents)
- [\_supportsUVs](MorphTargetManager.md#_supportsuvs)
- [\_targetDataLayoutChangedObservers](MorphTargetManager.md#_targetdatalayoutchangedobservers)
- [\_targetInfluenceChangedObservers](MorphTargetManager.md#_targetinfluencechangedobservers)
- [\_targets](MorphTargetManager.md#_targets)
- [\_tempInfluences](MorphTargetManager.md#_tempinfluences)
- [\_textureHeight](MorphTargetManager.md#_textureheight)
- [\_textureVertexStride](MorphTargetManager.md#_texturevertexstride)
- [\_textureWidth](MorphTargetManager.md#_texturewidth)
- [\_uniqueId](MorphTargetManager.md#_uniqueid)
- [\_useTextureToStoreTargets](MorphTargetManager.md#_usetexturetostoretargets)
- [\_vertexCount](MorphTargetManager.md#_vertexcount)
- [enableNormalMorphing](MorphTargetManager.md#enablenormalmorphing)
- [enableTangentMorphing](MorphTargetManager.md#enabletangentmorphing)
- [enableUVMorphing](MorphTargetManager.md#enableuvmorphing)
- [optimizeInfluencers](MorphTargetManager.md#optimizeinfluencers)
- [EnableTextureStorage](MorphTargetManager.md#enabletexturestorage)

### Accessors

- [areUpdatesFrozen](MorphTargetManager.md#areupdatesfrozen)
- [influences](MorphTargetManager.md#influences)
- [isUsingTextureForTargets](MorphTargetManager.md#isusingtexturefortargets)
- [numInfluencers](MorphTargetManager.md#numinfluencers)
- [numTargets](MorphTargetManager.md#numtargets)
- [supportsNormals](MorphTargetManager.md#supportsnormals)
- [supportsTangents](MorphTargetManager.md#supportstangents)
- [supportsUVs](MorphTargetManager.md#supportsuvs)
- [uniqueId](MorphTargetManager.md#uniqueid)
- [useTextureToStoreTargets](MorphTargetManager.md#usetexturetostoretargets)
- [vertexCount](MorphTargetManager.md#vertexcount)

### Methods

- [\_syncActiveTargets](MorphTargetManager.md#_syncactivetargets)
- [addTarget](MorphTargetManager.md#addtarget)
- [clone](MorphTargetManager.md#clone)
- [dispose](MorphTargetManager.md#dispose)
- [getActiveTarget](MorphTargetManager.md#getactivetarget)
- [getTarget](MorphTargetManager.md#gettarget)
- [removeTarget](MorphTargetManager.md#removetarget)
- [serialize](MorphTargetManager.md#serialize)
- [synchronize](MorphTargetManager.md#synchronize)
- [Parse](MorphTargetManager.md#parse)

## Constructors

### constructor

• **new MorphTargetManager**(`scene?`)

Creates a new MorphTargetManager

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `null` | defines the current scene |

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:90

## Properties

### \_activeTargets

• `Private` **\_activeTargets**: [`SmartArray`](SmartArray.md)[`MorphTarget`](MorphTarget.md)

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:24

___

### \_blockCounter

• `Private` **\_blockCounter**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:38

___

### \_canUseTextureForTargets

• `Private` **\_canUseTextureForTargets**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:37

___

### \_influences

• `Private` **\_influences**: `Float32Array`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:26

___

### \_morphTargetTextureIndices

• `Private` **\_morphTargetTextureIndices**: `Float32Array`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:27

___

### \_scene

• `Private` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:25

___

### \_supportsNormals

• `Private` **\_supportsNormals**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:28

___

### \_supportsTangents

• `Private` **\_supportsTangents**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:29

___

### \_supportsUVs

• `Private` **\_supportsUVs**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:30

___

### \_targetDataLayoutChangedObservers

• `Private` **\_targetDataLayoutChangedObservers**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`void`[]

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:23

___

### \_targetInfluenceChangedObservers

• `Private` **\_targetInfluenceChangedObservers**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`boolean`[]

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:22

___

### \_targets

• `Private` **\_targets**: [`MorphTarget`](MorphTarget.md)[]

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:21

___

### \_tempInfluences

• `Private` **\_tempInfluences**: `number`[]

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:36

___

### \_textureHeight

• `Private` **\_textureHeight**: `number` = `1`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:34

___

### \_textureVertexStride

• `Private` **\_textureVertexStride**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:32

___

### \_textureWidth

• `Private` **\_textureWidth**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:33

___

### \_uniqueId

• `Private` **\_uniqueId**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:35

___

### \_useTextureToStoreTargets

• `Private` **\_useTextureToStoreTargets**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:164

___

### \_vertexCount

• `Private` **\_vertexCount**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:31

___

### enableNormalMorphing

• **enableNormalMorphing**: `boolean` = `true`

Gets or sets a boolean indicating if normals must be morphed

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:54

___

### enableTangentMorphing

• **enableTangentMorphing**: `boolean` = `true`

Gets or sets a boolean indicating if tangents must be morphed

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:59

___

### enableUVMorphing

• **enableUVMorphing**: `boolean` = `true`

Gets or sets a boolean indicating if UV must be morphed

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:64

___

### optimizeInfluencers

• **optimizeInfluencers**: `boolean` = `true`

Gets or sets a boolean indicating if influencers must be optimized (eg. recompiling the shader if less influencers are used)

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:49

___

### EnableTextureStorage

▪ `Static` **EnableTextureStorage**: `boolean` = `true`

Enable storing morph target data into textures when set to true (true by default)

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:19

## Accessors

### areUpdatesFrozen

• `get` **areUpdatesFrozen**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:82

• `set` **areUpdatesFrozen**(`block`): `void`

Sets a boolean indicating that adding new target or updating an existing target will not update the underlying data buffers

#### Parameters

| Name | Type |
| :------ | :------ |
| `block` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:69

___

### influences

• `get` **influences**(): `Float32Array`

Gets the list of influences (one per target)

#### Returns

`Float32Array`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:160

___

### isUsingTextureForTargets

• `get` **isUsingTextureForTargets**(): `boolean`

Gets a boolean indicating that the targets are stored into a texture (instead of as attributes)

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:180

___

### numInfluencers

• `get` **numInfluencers**(): `number`

Gets the number of influencers (ie. the number of targets with influences > 0)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:153

___

### numTargets

• `get` **numTargets**(): `number`

Gets the number of targets stored in this manager

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:146

___

### supportsNormals

• `get` **supportsNormals**(): `boolean`

Gets a boolean indicating if this manager supports morphing of normals

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:125

___

### supportsTangents

• `get` **supportsTangents**(): `boolean`

Gets a boolean indicating if this manager supports morphing of tangents

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:132

___

### supportsUVs

• `get` **supportsUVs**(): `boolean`

Gets a boolean indicating if this manager supports morphing of texture coordinates

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:139

___

### uniqueId

• `get` **uniqueId**(): `number`

Gets the unique ID of this manager

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:111

___

### useTextureToStoreTargets

• `get` **useTextureToStoreTargets**(): `boolean`

Gets or sets a boolean indicating that targets should be stored as a texture instead of using vertex attributes (default is true).
Please note that this option is not available if the hardware does not support it

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:169

• `set` **useTextureToStoreTargets**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:173

___

### vertexCount

• `get` **vertexCount**(): `number`

Gets the number of vertices handled by this manager

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:118

## Methods

### \_syncActiveTargets

▸ `Private` **_syncActiveTargets**(`needUpdate`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `needUpdate` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:281

___

### addTarget

▸ **addTarget**(`target`): `void`

Add a new target to this manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`MorphTarget`](MorphTarget.md) | defines the target to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:206

___

### clone

▸ **clone**(): [`MorphTargetManager`](MorphTargetManager.md)

Clone the current manager

#### Returns

[`MorphTargetManager`](MorphTargetManager.md)

a new MorphTargetManager

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:250

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:456

___

### getActiveTarget

▸ **getActiveTarget**(`index`): [`MorphTarget`](MorphTarget.md)

Gets the active target at specified index. An active target is a target with an influence > 0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | defines the index to check |

#### Returns

[`MorphTarget`](MorphTarget.md)

the requested target

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:189

___

### getTarget

▸ **getTarget**(`index`): [`MorphTarget`](MorphTarget.md)

Gets the target at specified index

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | defines the index to check |

#### Returns

[`MorphTarget`](MorphTarget.md)

the requested target

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:198

___

### removeTarget

▸ **removeTarget**(`target`): `void`

Removes a target from the manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`MorphTarget`](MorphTarget.md) | defines the target to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:225

___

### serialize

▸ **serialize**(): `any`

Serializes the current manager into a Serialization object

#### Returns

`any`

the serialized object

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:268

___

### synchronize

▸ **synchronize**(): `void`

Synchronize the targets with all the meshes using this morph target manager

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:340

___

### Parse

▸ `Static` **Parse**(`serializationObject`, `scene`): [`MorphTargetManager`](MorphTargetManager.md)

Creates a new MorphTargetManager from serialized data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the serialized data |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`MorphTargetManager`](MorphTargetManager.md)

the new MorphTargetManager

#### Defined in

packages/dev/core/src/Morph/morphTargetManager.ts:485

[@dev/core](../README.md) / [Exports](../modules.md) / SolidParticle

# Class: SolidParticle

Represents one particle of a solid particle system.

## Table of contents

### Constructors

- [constructor](SolidParticle.md#constructor)

### Properties

- [\_boundingInfo](SolidParticle.md#_boundinginfo)
- [alive](SolidParticle.md#alive)
- [color](SolidParticle.md#color)
- [cullingStrategy](SolidParticle.md#cullingstrategy)
- [id](SolidParticle.md#id)
- [idx](SolidParticle.md#idx)
- [idxInShape](SolidParticle.md#idxinshape)
- [isVisible](SolidParticle.md#isvisible)
- [materialIndex](SolidParticle.md#materialindex)
- [parentId](SolidParticle.md#parentid)
- [pivot](SolidParticle.md#pivot)
- [position](SolidParticle.md#position)
- [props](SolidParticle.md#props)
- [rotation](SolidParticle.md#rotation)
- [rotationQuaternion](SolidParticle.md#rotationquaternion)
- [scaling](SolidParticle.md#scaling)
- [shapeId](SolidParticle.md#shapeid)
- [translateFromPivot](SolidParticle.md#translatefrompivot)
- [uvs](SolidParticle.md#uvs)
- [velocity](SolidParticle.md#velocity)

### Accessors

- [hasBoundingInfo](SolidParticle.md#hasboundinginfo)
- [quaternion](SolidParticle.md#quaternion)
- [scale](SolidParticle.md#scale)

### Methods

- [copyToRef](SolidParticle.md#copytoref)
- [getBoundingInfo](SolidParticle.md#getboundinginfo)
- [intersectsMesh](SolidParticle.md#intersectsmesh)
- [isInFrustum](SolidParticle.md#isinfrustum)

## Constructors

### constructor

• **new SolidParticle**(`particleIndex`, `particleId`, `positionIndex`, `indiceIndex`, `model`, `shapeId`, `idxInShape`, `sps`, `modelBoundingInfo?`, `materialIndex?`)

Creates a Solid Particle object.
Don't create particles manually, use instead the Solid Particle System internal tools like _addParticle()

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `particleIndex` | `number` | `undefined` | (integer) is the particle index in the Solid Particle System pool. |
| `particleId` | `number` | `undefined` | (integer) is the particle identifier. Unless some particles are removed from the SPS, it's the same value than the particle idx. |
| `positionIndex` | `number` | `undefined` | (integer) is the starting index of the particle vertices in the SPS "positions" array. |
| `indiceIndex` | `number` | `undefined` | (integer) is the starting index of the particle indices in the SPS "indices" array. |
| `model` | [`Nullable`](../modules.md#nullable)[`ModelShape`](ModelShape.md) | `undefined` | (ModelShape) is a reference to the model shape on what the particle is designed. |
| `shapeId` | `number` | `undefined` | (integer) is the model shape identifier in the SPS. |
| `idxInShape` | `number` | `undefined` | (integer) is the index of the particle in the current model (ex: the 10th box of addShape(box, 30)) |
| `sps` | [`SolidParticleSystem`](SolidParticleSystem.md) | `undefined` | defines the sps it is associated to |
| `modelBoundingInfo` | [`Nullable`](../modules.md#nullable)[`BoundingInfo`](BoundingInfo.md) | `null` | is the reference to the model BoundingInfo used for intersection computations. |
| `materialIndex` | [`Nullable`](../modules.md#nullable)`number` | `null` | is the particle material identifier (integer) when the MultiMaterials are enabled in the SPS. |

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:167

## Properties

### \_boundingInfo

• `Private` **\_boundingInfo**: [`BoundingInfo`](BoundingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:95

___

### alive

• **alive**: `boolean` = `true`

Is the particle active or not ?

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:65

___

### color

• **color**: [`Nullable`](../modules.md#nullable)[`Color4`](Color4.md)

The color of the particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:27

___

### cullingStrategy

• **cullingStrategy**: `number` = `AbstractMesh.CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY`

The culling strategy to use to check whether the solid particle must be culled or not when using isInFrustum().
The possible values are :
- AbstractMesh.CULLINGSTRATEGY_STANDARD
- AbstractMesh.CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY
- AbstractMesh.CULLINGSTRATEGY_OPTIMISTIC_INCLUSION
- AbstractMesh.CULLINGSTRATEGY_OPTIMISTIC_INCLUSION_THEN_BSPHERE_ONLY
The default value for solid particles is AbstractMesh.CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY
Please read each static variable documentation in the class AbstractMesh to get details about the culling process.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:131

___

### id

• **id**: `number` = `0`

particle identifier

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:23

___

### idx

• **idx**: `number` = `0`

particle global index

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:19

___

### idxInShape

• **idxInShape**: `number` = `0`

Index of the particle in its shape id

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:90

___

### isVisible

• **isVisible**: `boolean` = `true`

Is the particle visible or not ?

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:69

___

### materialIndex

• **materialIndex**: [`Nullable`](../modules.md#nullable)`number` = `null`

The particle material identifier (integer) when MultiMaterials are enabled in the SPS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:116

___

### parentId

• **parentId**: [`Nullable`](../modules.md#nullable)`number` = `null`

Parent particle Id, if any.
Default null.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:112

___

### pivot

• **pivot**: [`Vector3`](Vector3.md)

The pivot point in the particle local space.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:55

___

### position

• **position**: [`Vector3`](Vector3.md)

The world space position of the particle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:31

___

### props

• **props**: `any` = `null`

Custom object or properties.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:120

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

The world space rotation of the particle. (Not use if rotationQuaternion is set)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:35

___

### rotationQuaternion

• **rotationQuaternion**: [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

The world space rotation quaternion of the particle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:39

___

### scaling

• **scaling**: [`Vector3`](Vector3.md)

The scaling of the particle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:43

___

### shapeId

• **shapeId**: `number` = `0`

ModelShape id of this particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:86

___

### translateFromPivot

• **translateFromPivot**: `boolean` = `false`

Must the particle be translated from its pivot point in its local space ?
In this case, the pivot point is set at the origin of the particle local space and the particle is translated.
Default : false

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:61

___

### uvs

• **uvs**: [`Vector4`](Vector4.md)

The uvs of the particle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:47

___

### velocity

• **velocity**: [`Vector3`](Vector3.md)

The current speed of the particle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:51

## Accessors

### hasBoundingInfo

• `get` **hasBoundingInfo**(): `boolean`

Returns true if there is already a bounding info

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:149

___

### quaternion

• `get` **quaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Legacy support, changed quaternion to rotationQuaternion

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:248

• `set` **quaternion**(`q`): `void`

Legacy support, changed quaternion to rotationQuaternion

#### Parameters

| Name | Type |
| :------ | :------ |
| `q` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:255

___

### scale

• `get` **scale**(): [`Vector3`](Vector3.md)

Legacy support, changed scale to scaling

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:234

• `set` **scale**(`scale`): `void`

Legacy support, changed scale to scaling

#### Parameters

| Name | Type |
| :------ | :------ |
| `scale` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:241

## Methods

### copyToRef

▸ **copyToRef**(`target`): [`SolidParticle`](SolidParticle.md)

Copies the particle property values into the existing target : position, rotation, scaling, uvs, colors, pivot, parent, visibility, alive

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`SolidParticle`](SolidParticle.md) | the particle target |

#### Returns

[`SolidParticle`](SolidParticle.md)

the current particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:200

___

### getBoundingInfo

▸ **getBoundingInfo**(): [`BoundingInfo`](BoundingInfo.md)

Particle BoundingInfo object

#### Returns

[`BoundingInfo`](BoundingInfo.md)

a BoundingInfo

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:142

___

### intersectsMesh

▸ **intersectsMesh**(`target`): `boolean`

Returns a boolean. True if the particle intersects another particle or another mesh, else false.
The intersection is computed on the particle bounding sphere and Axis Aligned Bounding Box (AABB)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Mesh`](Mesh.md) \| [`SolidParticle`](SolidParticle.md) | is the object (solid particle or mesh) what the intersection is computed against. |

#### Returns

`boolean`

true if it intersects

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:265

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

Returns `true` if the solid particle is within the frustum defined by the passed array of planes.
A particle is in the frustum if its bounding box intersects the frustum

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum to test |

#### Returns

`boolean`

true if the particle is in the frustum planes

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticle.ts:281

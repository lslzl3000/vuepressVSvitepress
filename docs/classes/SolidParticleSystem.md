[@dev/core](../README.md) / [Exports](../modules.md) / SolidParticleSystem

# Class: SolidParticleSystem

The SPS is a single updatable mesh. The solid particles are simply separate parts or faces fo this big mesh.
As it is just a mesh, the SPS has all the same properties than any other BJS mesh : not more, not less. It can be scaled, rotated, translated, enlighted, textured, moved, etc.

The SPS is also a particle system. It provides some methods to manage the particles.
However it is behavior agnostic. This means it has no emitter, no particle physics, no particle recycler. You have to implement your own behavior.

Full documentation here : https://doc.babylonjs.com/how_to/Solid_Particle_System

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](SolidParticleSystem.md#constructor)

### Properties

- [\_alwaysVisible](SolidParticleSystem.md#_alwaysvisible)
- [\_autoUpdateSubMeshes](SolidParticleSystem.md#_autoupdatesubmeshes)
- [\_camera](SolidParticleSystem.md#_camera)
- [\_color](SolidParticleSystem.md#_color)
- [\_colors](SolidParticleSystem.md#_colors)
- [\_colors32](SolidParticleSystem.md#_colors32)
- [\_computeBoundingBox](SolidParticleSystem.md#_computeboundingbox)
- [\_computeParticleColor](SolidParticleSystem.md#_computeparticlecolor)
- [\_computeParticleRotation](SolidParticleSystem.md#_computeparticlerotation)
- [\_computeParticleTexture](SolidParticleSystem.md#_computeparticletexture)
- [\_computeParticleVertex](SolidParticleSystem.md#_computeparticlevertex)
- [\_copy](SolidParticleSystem.md#_copy)
- [\_defaultMaterial](SolidParticleSystem.md#_defaultmaterial)
- [\_depthSort](SolidParticleSystem.md#_depthsort)
- [\_depthSortParticles](SolidParticleSystem.md#_depthsortparticles)
- [\_expandable](SolidParticleSystem.md#_expandable)
- [\_fixedNormal32](SolidParticleSystem.md#_fixednormal32)
- [\_idxOfId](SolidParticleSystem.md#_idxofid)
- [\_index](SolidParticleSystem.md#_index)
- [\_indices](SolidParticleSystem.md#_indices)
- [\_indices32](SolidParticleSystem.md#_indices32)
- [\_indicesByMaterial](SolidParticleSystem.md#_indicesbymaterial)
- [\_isNotBuilt](SolidParticleSystem.md#_isnotbuilt)
- [\_isVisibilityBoxLocked](SolidParticleSystem.md#_isvisibilityboxlocked)
- [\_lastParticleId](SolidParticleSystem.md#_lastparticleid)
- [\_materialIndexes](SolidParticleSystem.md#_materialindexes)
- [\_materialIndexesById](SolidParticleSystem.md#_materialindexesbyid)
- [\_materials](SolidParticleSystem.md#_materials)
- [\_multimaterial](SolidParticleSystem.md#_multimaterial)
- [\_multimaterialEnabled](SolidParticleSystem.md#_multimaterialenabled)
- [\_mustUnrotateFixedNormals](SolidParticleSystem.md#_mustunrotatefixednormals)
- [\_needs32Bits](SolidParticleSystem.md#_needs32bits)
- [\_normals](SolidParticleSystem.md#_normals)
- [\_normals32](SolidParticleSystem.md#_normals32)
- [\_particlesIntersect](SolidParticleSystem.md#_particlesintersect)
- [\_pickable](SolidParticleSystem.md#_pickable)
- [\_positions](SolidParticleSystem.md#_positions)
- [\_positions32](SolidParticleSystem.md#_positions32)
- [\_scene](SolidParticleSystem.md#_scene)
- [\_shapeCounter](SolidParticleSystem.md#_shapecounter)
- [\_tmpVertex](SolidParticleSystem.md#_tmpvertex)
- [\_updatable](SolidParticleSystem.md#_updatable)
- [\_useModelMaterial](SolidParticleSystem.md#_usemodelmaterial)
- [\_uvs](SolidParticleSystem.md#_uvs)
- [\_uvs32](SolidParticleSystem.md#_uvs32)
- [billboard](SolidParticleSystem.md#billboard)
- [counter](SolidParticleSystem.md#counter)
- [depthSortedParticles](SolidParticleSystem.md#depthsortedparticles)
- [mesh](SolidParticleSystem.md#mesh)
- [name](SolidParticleSystem.md#name)
- [nbParticles](SolidParticleSystem.md#nbparticles)
- [particles](SolidParticleSystem.md#particles)
- [pickedBySubMesh](SolidParticleSystem.md#pickedbysubmesh)
- [pickedParticles](SolidParticleSystem.md#pickedparticles)
- [recomputeNormals](SolidParticleSystem.md#recomputenormals)
- [vars](SolidParticleSystem.md#vars)

### Accessors

- [autoUpdateSubMeshes](SolidParticleSystem.md#autoupdatesubmeshes)
- [computeBoundingBox](SolidParticleSystem.md#computeboundingbox)
- [computeParticleColor](SolidParticleSystem.md#computeparticlecolor)
- [computeParticleRotation](SolidParticleSystem.md#computeparticlerotation)
- [computeParticleTexture](SolidParticleSystem.md#computeparticletexture)
- [computeParticleVertex](SolidParticleSystem.md#computeparticlevertex)
- [depthSortParticles](SolidParticleSystem.md#depthsortparticles)
- [expandable](SolidParticleSystem.md#expandable)
- [isAlwaysVisible](SolidParticleSystem.md#isalwaysvisible)
- [isVisibilityBoxLocked](SolidParticleSystem.md#isvisibilityboxlocked)
- [materials](SolidParticleSystem.md#materials)
- [multimaterial](SolidParticleSystem.md#multimaterial)
- [multimaterialEnabled](SolidParticleSystem.md#multimaterialenabled)
- [useModelMaterial](SolidParticleSystem.md#usemodelmaterial)

### Methods

- [\_depthSortFunction](SolidParticleSystem.md#_depthsortfunction)
- [\_materialSortFunction](SolidParticleSystem.md#_materialsortfunction)
- [addShape](SolidParticleSystem.md#addshape)
- [afterUpdateParticles](SolidParticleSystem.md#afterupdateparticles)
- [beforeUpdateParticles](SolidParticleSystem.md#beforeupdateparticles)
- [buildMesh](SolidParticleSystem.md#buildmesh)
- [computeSubMeshes](SolidParticleSystem.md#computesubmeshes)
- [digest](SolidParticleSystem.md#digest)
- [dispose](SolidParticleSystem.md#dispose)
- [getParticleById](SolidParticleSystem.md#getparticlebyid)
- [getParticlesByShapeId](SolidParticleSystem.md#getparticlesbyshapeid)
- [getParticlesByShapeIdToRef](SolidParticleSystem.md#getparticlesbyshapeidtoref)
- [initParticles](SolidParticleSystem.md#initparticles)
- [insertParticlesFromArray](SolidParticleSystem.md#insertparticlesfromarray)
- [pickedParticle](SolidParticleSystem.md#pickedparticle)
- [rebuildMesh](SolidParticleSystem.md#rebuildmesh)
- [recycleParticle](SolidParticleSystem.md#recycleparticle)
- [refreshVisibleSize](SolidParticleSystem.md#refreshvisiblesize)
- [removeParticles](SolidParticleSystem.md#removeparticles)
- [setMultiMaterial](SolidParticleSystem.md#setmultimaterial)
- [setParticles](SolidParticleSystem.md#setparticles)
- [setVisibilityBox](SolidParticleSystem.md#setvisibilitybox)
- [updateParticle](SolidParticleSystem.md#updateparticle)
- [updateParticleVertex](SolidParticleSystem.md#updateparticlevertex)

## Constructors

### constructor

• **new SolidParticleSystem**(`name`, `scene`, `options?`)

Creates a SPS (Solid Particle System) object.

**`Example`**

```ts
bSphereRadiusFactor = 1.0 / Math.sqrt(3.0) => the bounding sphere exactly matches a spherical mesh.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | (String) is the SPS name, this will be the underlying mesh name. |
| `scene` | [`Scene`](Scene.md) | (Scene) is the scene in which the SPS is added. |
| `options?` | `Object` | defines the options of the sps e.g.  * updatable (optional boolean, default true) : if the SPS must be updatable or immutable.  * isPickable (optional boolean, default false) : if the solid particles must be pickable.  * enableDepthSort (optional boolean, default false) : if the solid particles must be sorted in the geometry according to their distance to the camera.  * useModelMaterial (optional boolean, default false) : if the model materials must be used to create the SPS multimaterial. This enables the multimaterial supports of the SPS.  * enableMultiMaterial (optional boolean, default false) : if the solid particles can be given different materials.  * expandable (optional boolean, default false) : if particles can still be added after the initial SPS mesh creation.  * particleIntersection (optional boolean, default false) : if the solid particle intersections must be computed.  * boundingSphereOnly (optional boolean, default false) : if the particle intersection must be computed only with the bounding sphere (no bounding box computation, so faster).  * bSphereRadiusFactor (optional float, default 1.0) : a number to multiply the bounding sphere radius by in order to reduce it for instance.  * computeBoundingBox (optional boolean, default false): if the bounding box of the entire SPS will be computed (for occlusion detection, for example). If it is false, the bounding box will be the bounding box of the first particle. |
| `options.bSphereRadiusFactor?` | `number` |  |
| `options.boundingSphereOnly?` | `boolean` |  |
| `options.computeBoundingBox?` | `boolean` |  |
| `options.enableDepthSort?` | `boolean` |  |
| `options.enableMultiMaterial?` | `boolean` |  |
| `options.expandable?` | `boolean` |  |
| `options.isPickable?` | `boolean` |  |
| `options.particleIntersection?` | `boolean` |  |
| `options.updatable?` | `boolean` |  |
| `options.useModelMaterial?` | `boolean` |  |

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:180

## Properties

### \_alwaysVisible

• `Private` **\_alwaysVisible**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:121

___

### \_autoUpdateSubMeshes

• `Private` **\_autoUpdateSubMeshes**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:150

___

### \_camera

• `Private` **\_camera**: [`TargetCamera`](TargetCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:133

___

### \_color

• `Private` **\_color**: [`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:126

___

### \_colors

• `Private` **\_colors**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:109

___

### \_colors32

• `Private` **\_colors32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:115

___

### \_computeBoundingBox

• `Private` **\_computeBoundingBox**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:131

___

### \_computeParticleColor

• `Private` **\_computeParticleColor**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:127

___

### \_computeParticleRotation

• `Private` **\_computeParticleRotation**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:129

___

### \_computeParticleTexture

• `Private` **\_computeParticleTexture**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:128

___

### \_computeParticleVertex

• `Private` **\_computeParticleVertex**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:130

___

### \_copy

• `Private` **\_copy**: [`SolidParticle`](SolidParticle.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:125

___

### \_defaultMaterial

• `Private` **\_defaultMaterial**: [`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:149

___

### \_depthSort

• `Private` **\_depthSort**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:122

___

### \_depthSortParticles

• `Private` **\_depthSortParticles**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:132

___

### \_expandable

• `Private` **\_expandable**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:123

___

### \_fixedNormal32

• `Private` **\_fixedNormal32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:114

___

### \_idxOfId

• `Private` **\_idxOfId**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:139

___

### \_index

• `Private` **\_index**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:117

___

### \_indices

• `Private` **\_indices**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:107

___

### \_indices32

• `Private` **\_indices32**: [`IndicesArray`](../modules.md#indicesarray)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:111

___

### \_indicesByMaterial

• `Private` **\_indicesByMaterial**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:142

___

### \_isNotBuilt

• `Private` **\_isNotBuilt**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:137

___

### \_isVisibilityBoxLocked

• `Private` **\_isVisibilityBoxLocked**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:120

___

### \_lastParticleId

• `Private` **\_lastParticleId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:138

___

### \_materialIndexes

• `Private` **\_materialIndexes**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:143

___

### \_materialIndexesById

• `Private` **\_materialIndexesById**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:148

___

### \_materials

• `Private` **\_materials**: [`Material`](Material.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:146

___

### \_multimaterial

• `Private` **\_multimaterial**: [`MultiMaterial`](MultiMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:147

___

### \_multimaterialEnabled

• `Private` **\_multimaterialEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:140

___

### \_mustUnrotateFixedNormals

• `Private` **\_mustUnrotateFixedNormals**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:134

___

### \_needs32Bits

• `Private` **\_needs32Bits**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:136

___

### \_normals

• `Private` **\_normals**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:108

___

### \_normals32

• `Private` **\_normals32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:113

___

### \_particlesIntersect

• `Private` **\_particlesIntersect**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:135

___

### \_pickable

• `Private` **\_pickable**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:119

___

### \_positions

• `Private` **\_positions**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:106

___

### \_positions32

• `Private` **\_positions32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:112

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:105

___

### \_shapeCounter

• `Private` **\_shapeCounter**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:124

___

### \_tmpVertex

• `Private` **\_tmpVertex**: [`SolidParticleVertex`](SolidParticleVertex.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:151

___

### \_updatable

• `Private` **\_updatable**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:118

___

### \_useModelMaterial

• `Private` **\_useModelMaterial**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:141

___

### \_uvs

• `Private` **\_uvs**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:110

___

### \_uvs32

• `Private` **\_uvs32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:116

___

### billboard

• **billboard**: `boolean` = `false`

If the particles must ever face the camera (default false). Useful for planar particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:42

___

### counter

• **counter**: `number` = `0`

This a counter ofr your own usage. It's not set by any SPS functions.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:50

___

### depthSortedParticles

• **depthSortedParticles**: `DepthSortedParticle`[]

This array is populated when `enableDepthSort` is set to true.
Each element of this array is an instance of the class DepthSortedParticle.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:92

___

### mesh

• **mesh**: [`Mesh`](Mesh.md)

The SPS mesh. It's a standard BJS Mesh, so all the methods from the Mesh class are available.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:58

___

### name

• **name**: `string`

The SPS name. This name is also given to the underlying mesh.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:54

___

### nbParticles

• **nbParticles**: `number` = `0`

The SPS total number of particles. Read only. Use SPS.counter instead if you need to set your own value.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:38

___

### particles

• **particles**: [`SolidParticle`](SolidParticle.md)[]

The SPS array of Solid Particle objects. Just access each particle as with any classic array.
 Example : var p = SPS.particles[i];

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:34

___

### pickedBySubMesh

• **pickedBySubMesh**: { `faceId`: `number` ; `idx`: `number`  }[][]

This array is populated when the SPS is set as 'pickable'
Each key of this array is a submesh index.
Each element of this array is a second array defined like this :
Each key of this second array is a `faceId` value that you can get from a pickResult object.
Each element of this second array is an object `{idx: int, faceId: int}`.
`idx` is the picked particle index in the `SPS.particles` array
`faceId` is the picked face index counted within this particle.
It's better to use the method SPS.pickedParticle(pickingInfo) rather than using directly this array.
Please read : https://doc.babylonjs.com/how_to/Solid_Particle_System#pickable-particles

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:87

___

### pickedParticles

• **pickedParticles**: { `faceId`: `number` ; `idx`: `number`  }[]

This array is populated when the SPS is set as 'pickable'.
Each key of this array is a `faceId` value that you can get from a pickResult object.
Each element of this array is an object `{idx: int, faceId: int}`.
`idx` is the picked particle index in the `SPS.particles` array
`faceId` is the picked face index counted within this particle.
This array is the first element of the pickedBySubMesh array : sps.pickBySubMesh[0].
It's not pertinent to use it when using a SPS with the support for MultiMaterial enabled.
Use the method SPS.pickedParticle(pickingInfo) instead.
Please read : https://doc.babylonjs.com/how_to/Solid_Particle_System#pickable-particles

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:75

___

### recomputeNormals

• **recomputeNormals**: `boolean` = `false`

Recompute normals when adding a shape

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:46

___

### vars

• **vars**: `any` = `{}`

This empty object is intended to store some SPS specific or temporary values in order to lower the Garbage Collector activity.
Please read : https://doc.babylonjs.com/how_to/Solid_Particle_System#garbage-collector-concerns

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:63

## Accessors

### autoUpdateSubMeshes

• `get` **autoUpdateSubMeshes**(): `boolean`

If the subMeshes must be updated on the next call to setParticles()

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1941

• `set` **autoUpdateSubMeshes**(`val`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1944

___

### computeBoundingBox

• `get` **computeBoundingBox**(): `boolean`

Gets if `setParticles()` computes or not the mesh bounding box when computing the particle positions.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1873

• `set` **computeBoundingBox**(`val`): `void`

Tells to `setParticles()` to compute or not the mesh bounding box when computing the particle positions.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1822

___

### computeParticleColor

• `get` **computeParticleColor**(): `boolean`

Gets if `setParticles()` computes the particle colors or not.
Default value : true. The SPS is faster when it's set to false.
Note : the particle colors are stored values, so setting `computeParticleColor` to false will keep yet the last colors set.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1848

• `set` **computeParticleColor**(`val`): `void`

Tells to `setParticles()` to compute the particle colors or not.
Default value : true. The SPS is faster when it's set to false.
Note : the particle colors are stored values, so setting `computeParticleColor` to false will keep yet the last colors set.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1804

___

### computeParticleRotation

• `get` **computeParticleRotation**(): `boolean`

Gets if `setParticles()` computes the particle rotations or not.
Default value : true. The SPS is faster when it's set to false.
Note : the particle rotations aren't stored values, so setting `computeParticleRotation` to false will prevents the particle to rotate.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1839

• `set` **computeParticleRotation**(`val`): `void`

Tells to `setParticles()` to compute the particle rotations or not.
Default value : true. The SPS is faster when it's set to false.
Note : the particle rotations aren't stored values, so setting `computeParticleRotation` to false will prevents the particle to rotate.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1795

___

### computeParticleTexture

• `get` **computeParticleTexture**(): `boolean`

Gets if `setParticles()` computes the particle textures or not.
Default value : true. The SPS is faster when it's set to false.
Note : the particle textures are stored values, so setting `computeParticleTexture` to false will keep yet the last colors set.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1857

• `set` **computeParticleTexture**(`val`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1808

___

### computeParticleVertex

• `get` **computeParticleVertex**(): `boolean`

Gets if `setParticles()` calls the vertex function for each vertex of each particle, or not.
Default value : false. The SPS is faster when it's set to false.
Note : the particle custom vertex positions aren't stored values.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1866

• `set` **computeParticleVertex**(`val`): `void`

Tells to `setParticles()` to call the vertex function for each vertex of each particle, or not.
Default value : false. The SPS is faster when it's set to false.
Note : the particle custom vertex positions aren't stored values.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1816

___

### depthSortParticles

• `get` **depthSortParticles**(): `boolean`

Gets if `setParticles()` sorts or not the distance between each particle and the camera.
Skipped when `enableDepthSort` is set to `false` (default) at construction time.
Default : `true`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1882

• `set` **depthSortParticles**(`val`): `void`

Tells to `setParticles()` to sort or not the distance between each particle and the camera.
Skipped when `enableDepthSort` is set to `false` (default) at construction time.
Default : `true`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1830

___

### expandable

• `get` **expandable**(): `boolean`

Gets if the SPS is created as expandable at construction time.
Default : `false`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1890

___

### isAlwaysVisible

• `get` **isAlwaysVisible**(): `boolean`

Gets whether the SPS as always visible or not
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1757

• `set` **isAlwaysVisible**(`val`): `void`

Sets the SPS as always visible or not
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1765

___

### isVisibilityBoxLocked

• `get` **isVisibilityBoxLocked**(): `boolean`

Gets if the SPS visibility box as locked or not. This enables/disables the underlying mesh bounding box updates.
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1786

• `set` **isVisibilityBoxLocked**(`val`): `void`

Sets the SPS visibility box as locked or not. This enables/disables the underlying mesh bounding box updates.
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1774

___

### materials

• `get` **materials**(): [`Material`](Material.md)[]

The SPS used material array.

#### Returns

[`Material`](Material.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1908

___

### multimaterial

• `get` **multimaterial**(): [`MultiMaterial`](MultiMaterial.md)

The SPS computed multimaterial object

#### Returns

[`MultiMaterial`](MultiMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1932

• `set` **multimaterial**(`mm`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mm` | [`MultiMaterial`](MultiMaterial.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1935

___

### multimaterialEnabled

• `get` **multimaterialEnabled**(): `boolean`

Gets if the SPS supports the Multi Materials

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1896

___

### useModelMaterial

• `get` **useModelMaterial**(): `boolean`

Gets if the SPS uses the model materials for its own multimaterial.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1902

## Methods

### \_depthSortFunction

▸ `Private` **_depthSortFunction**(`p1`, `p2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `p1` | `DepthSortedParticle` |
| `p2` | `DepthSortedParticle` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:144

___

### \_materialSortFunction

▸ `Private` **_materialSortFunction**(`p1`, `p2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `p1` | `DepthSortedParticle` |
| `p2` | `DepthSortedParticle` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:145

___

### addShape

▸ **addShape**(`mesh`, `nb`, `options?`): `number`

Adds some particles to the SPS from the model shape. Returns the shape id.
Please read the doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#create-an-immutable-sps

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | is any Mesh object that will be used as a model for the solid particles. |
| `nb` | `number` | (positive integer) the number of particles to be created from this model |
| `options?` | `Object` | {positionFunction} is an optional javascript function to called for each particle on SPS creation.  {vertexFunction} is an optional javascript function to called for each vertex of each particle on SPS creation  {storage} (optional existing array) is an array where the particles will be stored for a further use instead of being inserted in the SPS. |
| `options.positionFunction?` | `any` |  |
| `options.storage?` | [] |  |
| `options.vertexFunction?` | `any` |  |

#### Returns

`number`

the number of shapes in the system

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:750

___

### afterUpdateParticles

▸ **afterUpdateParticles**(`start?`, `stop?`, `update?`): `void`

This will be called  by `setParticles()` after all the other treatments and just before the actual mesh update.
This will be passed three parameters.
This does nothing and may be overwritten by the user.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `stop?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `update?` | `boolean` | the boolean update value actually passed to setParticles() |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:2014

___

### beforeUpdateParticles

▸ **beforeUpdateParticles**(`start?`, `stop?`, `update?`): `void`

This will be called before any other treatment by `setParticles()` and will be passed three parameters.
This does nothing and may be overwritten by the user.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `stop?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `update?` | `boolean` | the boolean update value actually passed to setParticles() |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:2004

___

### buildMesh

▸ **buildMesh**(): [`Mesh`](Mesh.md)

Builds the SPS underlying mesh. Returns a standard Mesh.
If no model shape was added to the SPS, the returned mesh is just a single triangular plane.

#### Returns

[`Mesh`](Mesh.md)

the created mesh

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:234

___

### computeSubMeshes

▸ **computeSubMeshes**(): [`SolidParticleSystem`](SolidParticleSystem.md)

Computes the required SubMeshes according the materials assigned to the particles.

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the solid particle system.
Does nothing if called before the SPS mesh is built.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1597

___

### digest

▸ **digest**(`mesh`, `options?`): [`SolidParticleSystem`](SolidParticleSystem.md)

Digests the mesh and generates as many solid particles in the system as wanted. Returns the SPS.
These particles will have the same geometry than the mesh parts and will be positioned at the same localisation than the mesh original places.
Thus the particles generated from `digest()` have their property `position` set yet.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | ( Mesh ) is the mesh to be digested |
| `options?` | `Object` | {facetNb} (optional integer, default 1) is the number of mesh facets per particle, this parameter is overridden by the parameter `number` if any  {delta} (optional integer, default 0) is the random extra number of facets per particle , each particle will have between `facetNb` and `facetNb + delta` facets  {number} (optional positive integer) is the wanted number of particles : each particle is built with `mesh_total_facets / number` facets  {storage} (optional existing array) is an array where the particles will be stored for a further use instead of being inserted in the SPS. |
| `options.delta?` | `number` |  |
| `options.facetNb?` | `number` |  |
| `options.number?` | `number` |  |
| `options.storage?` | [] |  |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the current SPS

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:335

___

### dispose

▸ **dispose**(): `void`

Disposes the SPS.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1497

___

### getParticleById

▸ **getParticleById**(`id`): [`Nullable`](../modules.md#nullable)[`SolidParticle`](SolidParticle.md)

Returns a SolidParticle object from its identifier : particle.id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | (integer) the particle Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`SolidParticle`](SolidParticle.md)

the searched particle or null if not found in the SPS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1543

___

### getParticlesByShapeId

▸ **getParticlesByShapeId**(`shapeId`): [`SolidParticle`](SolidParticle.md)[]

Returns a new array populated with the particles having the passed shapeId.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapeId` | `number` | (integer) the shape identifier |

#### Returns

[`SolidParticle`](SolidParticle.md)[]

a new solid particle array

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1570

___

### getParticlesByShapeIdToRef

▸ **getParticlesByShapeIdToRef**(`shapeId`, `ref`): [`SolidParticleSystem`](SolidParticleSystem.md)

Populates the passed array "ref" with the particles having the passed shapeId.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapeId` | `number` | the shape identifier |
| `ref` | [`SolidParticle`](SolidParticle.md)[] |  |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the SPS

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1582

___

### initParticles

▸ **initParticles**(): `void`

This function does nothing. It may be overwritten to set all the particle first values.
The SPS doesn't call this function, you may have to call it by your own.
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#particle-management

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1956

___

### insertParticlesFromArray

▸ **insertParticlesFromArray**(`solidParticleArray`): [`SolidParticleSystem`](SolidParticleSystem.md)

Inserts some pre-created particles in the solid particle system so that they can be managed by setParticles().

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `solidParticleArray` | [`SolidParticle`](SolidParticle.md)[] | an array populated with Solid Particles objects |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the SPS

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:937

___

### pickedParticle

▸ **pickedParticle**(`pickingInfo`): [`Nullable`](../modules.md#nullable){ `faceId`: `number` ; `idx`: `number`  }

Returns an object {idx: number faceId: number} for the picked particle from the passed pickingInfo object.
idx is the particle index in the SPS
faceId is the picked face index counted within this particle.
Returns null if the pickInfo can't identify a picked particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pickingInfo` | [`PickingInfo`](PickingInfo.md) | (PickingInfo object) |

#### Returns

[`Nullable`](../modules.md#nullable){ `faceId`: `number` ; `idx`: `number`  }

or null

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1526

___

### rebuildMesh

▸ **rebuildMesh**(`reset?`): [`SolidParticleSystem`](SolidParticleSystem.md)

Rebuilds the whole mesh and updates the VBO : custom positions and vertices are recomputed if needed.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `reset` | `boolean` | `false` | boolean, default false : if the particles must be reset at position and rotation zero, scaling 1, color white, initial UVs and not parented. |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the SPS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:848

___

### recycleParticle

▸ **recycleParticle**(`particle`): [`SolidParticle`](SolidParticle.md)

This function does nothing. It may be overwritten to recycle a particle.
The SPS doesn't call this function, you may have to call it by your own.
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#particle-management

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particle` | [`SolidParticle`](SolidParticle.md) | The particle to recycle |

#### Returns

[`SolidParticle`](SolidParticle.md)

the recycled particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1965

___

### refreshVisibleSize

▸ **refreshVisibleSize**(): [`SolidParticleSystem`](SolidParticleSystem.md)

Visibility helper : Recomputes the visible size according to the mesh bounding box
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the SPS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1735

___

### removeParticles

▸ **removeParticles**(`start`, `end`): [`SolidParticle`](SolidParticle.md)[]

Removes the particles from the start-th to the end-th included from an expandable SPS (required).
 Returns an array with the removed particles.
 If the number of particles to remove is lower than zero or greater than the global remaining particle number, then an empty array is returned.
 The SPS can't be empty so at least one particle needs to remain in place.
 Under the hood, the VertexData array, so the VBO buffer, is recreated each call.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | index of the first particle to remove |
| `end` | `number` | index of the last particle to remove (included) |

#### Returns

[`SolidParticle`](SolidParticle.md)[]

an array populated with the removed particles

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:865

___

### setMultiMaterial

▸ **setMultiMaterial**(`materials`): `void`

Sets the SPS MultiMaterial from the passed materials.
Note : the passed array is internally copied and not used then by reference.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `materials` | [`Material`](Material.md)[] | an array of material objects. This array indexes are the materialIndex values of the particles. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1916

___

### setParticles

▸ **setParticles**(`start?`, `end?`, `update?`): [`SolidParticleSystem`](SolidParticleSystem.md)

Sets all the particles : this method actually really updates the mesh according to the particle positions, rotations, colors, textures, etc.
 This method calls `updateParticle()` for each particle of the SPS.
 For an animated SPS, it is usually called within the render loop.
This methods does nothing if called on a non updatable or not yet built SPS. Example : buildMesh() not called after having added or removed particles from an expandable SPS.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `start` | `number` | `0` | The particle index in the particle array where to start to compute the particle property values _(default 0)_ |
| `end` | `number` | `undefined` | The particle index in the particle array where to stop to compute the particle property values _(default nbParticle - 1)_ |
| `update` | `boolean` | `true` | If the mesh must be finally updated on this call after all the particle computations _(default true)_ |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the SPS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1065

___

### setVisibilityBox

▸ **setVisibilityBox**(`size`): `void`

Visibility helper : Sets the size of a visibility box, this sets the underlying mesh bounding box.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | the size (float) of the visibility box  note : this doesn't lock the SPS mesh bounding box.  doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#sps-visibility |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1748

___

### updateParticle

▸ **updateParticle**(`particle`): [`SolidParticle`](SolidParticle.md)

Updates a particle : this function should  be overwritten by the user.
It is called on each particle by `setParticles()`. This is the place to code each particle behavior.
doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#particle-management

**`Example`**

```ts
: just set a particle position or velocity and recycle conditions
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particle` | [`SolidParticle`](SolidParticle.md) | The particle to update |

#### Returns

[`SolidParticle`](SolidParticle.md)

the updated particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1977

___

### updateParticleVertex

▸ **updateParticleVertex**(`particle`, `vertex`, `pt`): [`SolidParticleSystem`](SolidParticleSystem.md)

Updates a vertex of a particle : it can be overwritten by the user.
This will be called on each vertex particle by `setParticles()` if `computeParticleVertex` is set to true only.

**`Example`**

```ts
: just set a vertex particle position or color
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particle` | [`SolidParticle`](SolidParticle.md) | the current particle |
| `vertex` | [`SolidParticleVertex`](SolidParticleVertex.md) | the current vertex of the current particle : a SolidParticleVertex object |
| `pt` | `number` | the index of the current vertex in the particle shape  doc : https://doc.babylonjs.com/how_to/Solid_Particle_System#update-each-particle-shape |

#### Returns

[`SolidParticleSystem`](SolidParticleSystem.md)

the sps

#### Defined in

https://github.com/babylon.js/core/src/Particles/solidParticleSystem.ts:1992

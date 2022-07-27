[@dev/core](../README.md) / [Exports](../modules.md) / PointsCloudSystem

# Class: PointsCloudSystem

The PointCloudSystem (PCS) is a single updatable mesh. The points corresponding to the vertices of this big mesh.
As it is just a mesh, the PointCloudSystem has all the same properties as any other BJS mesh : not more, not less. It can be scaled, rotated, translated, enlighted, textured, moved, etc.

The PointCloudSystem is also a particle system, with each point being a particle. It provides some methods to manage the particles.
However it is behavior agnostic. This means it has no emitter, no particle physics, no particle recycler. You have to implement your own behavior.

Full documentation here : TO BE ENTERED

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](PointsCloudSystem.md#constructor)

### Properties

- [\_alwaysVisible](PointsCloudSystem.md#_alwaysvisible)
- [\_colors](PointsCloudSystem.md#_colors)
- [\_colors32](PointsCloudSystem.md#_colors32)
- [\_computeBoundingBox](PointsCloudSystem.md#_computeboundingbox)
- [\_computeParticleColor](PointsCloudSystem.md#_computeparticlecolor)
- [\_computeParticleRotation](PointsCloudSystem.md#_computeparticlerotation)
- [\_computeParticleTexture](PointsCloudSystem.md#_computeparticletexture)
- [\_groupCounter](PointsCloudSystem.md#_groupcounter)
- [\_groups](PointsCloudSystem.md#_groups)
- [\_indices](PointsCloudSystem.md#_indices)
- [\_indices32](PointsCloudSystem.md#_indices32)
- [\_isReady](PointsCloudSystem.md#_isready)
- [\_isVisibilityBoxLocked](PointsCloudSystem.md#_isvisibilityboxlocked)
- [\_normals](PointsCloudSystem.md#_normals)
- [\_positions](PointsCloudSystem.md#_positions)
- [\_positions32](PointsCloudSystem.md#_positions32)
- [\_promises](PointsCloudSystem.md#_promises)
- [\_scene](PointsCloudSystem.md#_scene)
- [\_updatable](PointsCloudSystem.md#_updatable)
- [\_uvs](PointsCloudSystem.md#_uvs)
- [\_uvs32](PointsCloudSystem.md#_uvs32)
- [counter](PointsCloudSystem.md#counter)
- [mesh](PointsCloudSystem.md#mesh)
- [name](PointsCloudSystem.md#name)
- [nbParticles](PointsCloudSystem.md#nbparticles)
- [particles](PointsCloudSystem.md#particles)
- [vars](PointsCloudSystem.md#vars)

### Accessors

- [colors](PointsCloudSystem.md#colors)
- [computeBoundingBox](PointsCloudSystem.md#computeboundingbox)
- [computeParticleColor](PointsCloudSystem.md#computeparticlecolor)
- [computeParticleRotation](PointsCloudSystem.md#computeparticlerotation)
- [computeParticleTexture](PointsCloudSystem.md#computeparticletexture)
- [isAlwaysVisible](PointsCloudSystem.md#isalwaysvisible)
- [positions](PointsCloudSystem.md#positions)
- [uvs](PointsCloudSystem.md#uvs)

### Methods

- [\_addParticle](PointsCloudSystem.md#_addparticle)
- [\_calculateDensity](PointsCloudSystem.md#_calculatedensity)
- [\_colorFromTexture](PointsCloudSystem.md#_colorfromtexture)
- [\_getColorIndicesForCoord](PointsCloudSystem.md#_getcolorindicesforcoord)
- [\_randomUnitVector](PointsCloudSystem.md#_randomunitvector)
- [\_setPointsColorOrUV](PointsCloudSystem.md#_setpointscolororuv)
- [addPoints](PointsCloudSystem.md#addpoints)
- [addSurfacePoints](PointsCloudSystem.md#addsurfacepoints)
- [addVolumePoints](PointsCloudSystem.md#addvolumepoints)
- [afterUpdateParticles](PointsCloudSystem.md#afterupdateparticles)
- [beforeUpdateParticles](PointsCloudSystem.md#beforeupdateparticles)
- [buildMeshAsync](PointsCloudSystem.md#buildmeshasync)
- [dispose](PointsCloudSystem.md#dispose)
- [initParticles](PointsCloudSystem.md#initparticles)
- [recycleParticle](PointsCloudSystem.md#recycleparticle)
- [refreshVisibleSize](PointsCloudSystem.md#refreshvisiblesize)
- [setParticles](PointsCloudSystem.md#setparticles)
- [setVisibilityBox](PointsCloudSystem.md#setvisibilitybox)
- [updateParticle](PointsCloudSystem.md#updateparticle)

## Constructors

### constructor

• **new PointsCloudSystem**(`name`, `pointSize`, `scene`, `options?`)

Creates a PCS (Points Cloud System) object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | (String) is the PCS name, this will be the underlying mesh name |
| `pointSize` | `number` | (number) is the size for each point. Has no effect on a WebGPU engine. |
| `scene` | [`Scene`](Scene.md) | (Scene) is the scene in which the PCS is added |
| `options?` | `Object` | defines the options of the PCS e.g.  * updatable (optional boolean, default true) : if the PCS must be updatable or immutable |
| `options.updatable?` | `boolean` |  |

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:123

## Properties

### \_alwaysVisible

• `Private` **\_alwaysVisible**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:84

___

### \_colors

• `Private` **\_colors**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:76

___

### \_colors32

• `Private` **\_colors32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:80

___

### \_computeBoundingBox

• `Private` **\_computeBoundingBox**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:90

___

### \_computeParticleColor

• `Private` **\_computeParticleColor**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:87

___

### \_computeParticleRotation

• `Private` **\_computeParticleRotation**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:89

___

### \_computeParticleTexture

• `Private` **\_computeParticleTexture**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:88

___

### \_groupCounter

• `Private` **\_groupCounter**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:86

___

### \_groups

• `Private` **\_groups**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:85

___

### \_indices

• `Private` **\_indices**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:74

___

### \_indices32

• `Private` **\_indices32**: [`IndicesArray`](../modules.md#indicesarray)

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:78

___

### \_isReady

• `Private` **\_isReady**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:91

___

### \_isVisibilityBoxLocked

• `Private` **\_isVisibilityBoxLocked**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:83

___

### \_normals

• `Private` **\_normals**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:75

___

### \_positions

• `Private` **\_positions**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:73

___

### \_positions32

• `Private` **\_positions32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:79

___

### \_promises

• `Private` **\_promises**: `Promise``any`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:72

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:71

___

### \_updatable

• `Private` **\_updatable**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:82

___

### \_uvs

• `Private` **\_uvs**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:77

___

### \_uvs32

• `Private` **\_uvs32**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:81

___

### counter

• **counter**: `number` = `0`

This a counter for your own usage. It's not set by any SPS functions.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:52

___

### mesh

• **mesh**: [`Mesh`](Mesh.md)

The PCS mesh. It's a standard BJS Mesh, so all the methods from the Mesh class are available.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:60

___

### name

• **name**: `string`

The PCS name. This name is also given to the underlying mesh.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:56

___

### nbParticles

• **nbParticles**: `number` = `0`

The PCS total number of particles. Read only. Use PCS.counter instead if you need to set your own value.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:48

___

### particles

• **particles**: [`CloudPoint`](CloudPoint.md)[]

The PCS array of cloud point objects. Just access each particle as with any classic array.
 Example : var p = SPS.particles[i];

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:44

___

### vars

• **vars**: `any` = `{}`

This empty object is intended to store some PCS specific or temporary values in order to lower the Garbage Collector activity.
Please read :

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:65

## Accessors

### colors

• `get` **colors**(): `Float32Array`

Gets the particle colors computed by the Point Cloud System

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:103

___

### computeBoundingBox

• `get` **computeBoundingBox**(): `boolean`

Gets if `setParticles()` computes or not the mesh bounding box when computing the particle positions.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1036

• `set` **computeBoundingBox**(`val`): `void`

Tells to `setParticles()` to compute or not the mesh bounding box when computing the particle positions.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1030

___

### computeParticleColor

• `get` **computeParticleColor**(): `boolean`

Gets if `setParticles()` computes the particle colors or not.
Default value : false. The PCS is faster when it's set to false.
Note : the particle colors are stored values, so setting `computeParticleColor` to false will keep yet the last colors set.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1016

• `set` **computeParticleColor**(`val`): `void`

Tells to `setParticles()` to compute the particle colors or not.
Default value : true. The PCS is faster when it's set to false.
Note : the particle colors are stored values, so setting `computeParticleColor` to false will keep yet the last colors set.

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1004

___

### computeParticleRotation

• `set` **computeParticleRotation**(`val`): `void`

Tells to `setParticles()` to compute the particle rotations or not
Default value : false. The PCS is faster when it's set to false
Note : particle rotations are only applied to parent particles
Note : the particle rotations aren't stored values, so setting `computeParticleRotation` to false will prevents the particle to rotate

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:995

___

### computeParticleTexture

• `get` **computeParticleTexture**(): `boolean`

Gets if `setParticles()` computes the particle textures or not.
Default value : false. The PCS is faster when it's set to false.
Note : the particle textures are stored values, so setting `computeParticleTexture` to false will keep yet the last colors set.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1024

• `set` **computeParticleTexture**(`val`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1008

___

### isAlwaysVisible

• `get` **isAlwaysVisible**(): `boolean`

Gets whether the PCS is always visible or not
doc :

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:976

• `set` **isAlwaysVisible**(`val`): `void`

Sets the PCS as always visible or not
doc :

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:984

___

### positions

• `get` **positions**(): `Float32Array`

Gets the particle positions computed by the Point Cloud System

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:96

___

### uvs

• `get` **uvs**(): `Float32Array`

Gets the particle uvs computed by the Point Cloud System

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:110

## Methods

### \_addParticle

▸ `Private` **_addParticle**(`idx`, `group`, `groupId`, `idxInGroup`): [`CloudPoint`](CloudPoint.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `idx` | `number` |
| `group` | [`PointsGroup`](PointsGroup.md) |
| `groupId` | `number` |
| `idxInGroup` | `number` |

#### Returns

[`CloudPoint`](CloudPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:199

___

### \_calculateDensity

▸ `Private` **_calculateDensity**(`nbPoints`, `positions`, `indices`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `nbPoints` | `number` |
| `positions` | [`FloatArray`](../modules.md#floatarray) |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) |

#### Returns

`number`[]

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:532

___

### \_colorFromTexture

▸ `Private` **_colorFromTexture**(`mesh`, `pointsGroup`, `isVolume`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `pointsGroup` | [`PointsGroup`](PointsGroup.md) |
| `isVolume` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:480

___

### \_getColorIndicesForCoord

▸ `Private` **_getColorIndicesForCoord**(`pointsGroup`, `x`, `y`, `width`): [`Color4`](Color4.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointsGroup` | [`PointsGroup`](PointsGroup.md) |
| `x` | `number` |
| `y` | `number` |
| `width` | `number` |

#### Returns

[`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:210

___

### \_randomUnitVector

▸ `Private` **_randomUnitVector**(`particle`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `particle` | [`CloudPoint`](CloudPoint.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:205

___

### \_setPointsColorOrUV

▸ `Private` **_setPointsColorOrUV**(`mesh`, `pointsGroup`, `isVolume`, `colorFromTexture?`, `hasTexture?`, `color?`, `range?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `pointsGroup` | [`PointsGroup`](PointsGroup.md) |
| `isVolume` | `boolean` |
| `colorFromTexture?` | `boolean` |
| `hasTexture?` | `boolean` |
| `color?` | [`Color4`](Color4.md) |
| `range?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:225

___

### addPoints

▸ **addPoints**(`nb`, `pointFunction?`): `number`

Adds points to the PCS in random positions within a unit sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nb` | `number` | (positive integer) the number of particles to be created from this model |
| `pointFunction` | `any` | is an optional javascript function to be called for each particle on PCS creation |

#### Returns

`number`

the number of groups in the system

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:618

___

### addSurfacePoints

▸ **addSurfacePoints**(`mesh`, `nb`, `colorWith?`, `color?`, `range?`): `number`

Adds points to the PCS from the surface of the model shape

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | is any Mesh object that will be used as a surface model for the points |
| `nb` | `number` | (positive integer) the number of particles to be created from this model |
| `colorWith?` | `number` | determines whether a point is colored using color (default), uv, random, stated or none (invisible) |
| `color?` | `number` \| [`Color4`](Color4.md) | (color4) to be used when colorWith is stated or color (number) when used to specify texture position |
| `range?` | `number` | (number from 0 to 1) to determine the variation in shape and tone for a stated color |

#### Returns

`number`

the number of groups in the system

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:652

___

### addVolumePoints

▸ **addVolumePoints**(`mesh`, `nb`, `colorWith?`, `color?`, `range?`): `number`

Adds points to the PCS inside the model shape

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | is any Mesh object that will be used as a surface model for the points |
| `nb` | `number` | (positive integer) the number of particles to be created from this model |
| `colorWith?` | `number` | determines whether a point is colored using color (default), uv, random, stated or none (invisible) |
| `color?` | `number` \| [`Color4`](Color4.md) | (color4) to be used when colorWith is stated or color (number) when used to specify texture position |
| `range?` | `number` | (number from 0 to 1) to determine the variation in shape and tone for a stated color |

#### Returns

`number`

the number of groups in the system

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:698

___

### afterUpdateParticles

▸ **afterUpdateParticles**(`start?`, `stop?`, `update?`): `void`

This will be called  by `setParticles()` after all the other treatments and just before the actual mesh update.
This will be passed three parameters.
This does nothing and may be overwritten by the user.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | `number` | the particle index in the particle array where to start to iterate, same than the value passed to setParticle() |
| `stop?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `update?` | `boolean` | the boolean update value actually passed to setParticles() |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1092

___

### beforeUpdateParticles

▸ **beforeUpdateParticles**(`start?`, `stop?`, `update?`): `void`

This will be called before any other treatment by `setParticles()` and will be passed three parameters.
This does nothing and may be overwritten by the user.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | `number` | the particle index in the particle array where to start to iterate, same than the value passed to setParticle() |
| `stop?` | `number` | the particle index in the particle array where to stop to iterate, same than the value passed to setParticle() |
| `update?` | `boolean` | the boolean update value actually passed to setParticles() |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1082

___

### buildMeshAsync

▸ **buildMeshAsync**(`material?`): `Promise`[`Mesh`](Mesh.md)

Builds the PCS underlying mesh. Returns a standard Mesh.
If no points were added to the PCS, the returned mesh is just a single point.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `material?` | [`Material`](Material.md) | The material to use to render the mesh. If not provided, will create a default one |

#### Returns

`Promise`[`Mesh`](Mesh.md)

a promise for the created mesh

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:140

___

### dispose

▸ **dispose**(): `void`

Disposes the PCS.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:934

___

### initParticles

▸ **initParticles**(): `void`

This function does nothing. It may be overwritten to set all the particle first values.
The PCS doesn't call this function, you may have to call it by your own.
doc :

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1049

___

### recycleParticle

▸ **recycleParticle**(`particle`): [`CloudPoint`](CloudPoint.md)

This function does nothing. It may be overwritten to recycle a particle
The PCS doesn't call this function, you can to call it
doc :

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particle` | [`CloudPoint`](CloudPoint.md) | The particle to recycle |

#### Returns

[`CloudPoint`](CloudPoint.md)

the recycled particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1058

___

### refreshVisibleSize

▸ **refreshVisibleSize**(): [`PointsCloudSystem`](PointsCloudSystem.md)

Visibility helper : Recomputes the visible size according to the mesh bounding box
doc :

#### Returns

[`PointsCloudSystem`](PointsCloudSystem.md)

the PCS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:954

___

### setParticles

▸ **setParticles**(`start?`, `end?`, `update?`): [`PointsCloudSystem`](PointsCloudSystem.md)

Sets all the particles : this method actually really updates the mesh according to the particle positions, rotations, colors, textures, etc.
 This method calls `updateParticle()` for each particle of the SPS.
 For an animated SPS, it is usually called within the render loop.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `start` | `number` | `0` | The particle index in the particle array where to start to compute the particle property values _(default 0)_ |
| `end` | `number` | `undefined` | The particle index in the particle array where to stop to compute the particle property values _(default nbParticle - 1)_ |
| `update` | `boolean` | `true` | If the mesh must be finally updated on this call after all the particle computations _(default true)_ |

#### Returns

[`PointsCloudSystem`](PointsCloudSystem.md)

the PCS.

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:744

___

### setVisibilityBox

▸ **setVisibilityBox**(`size`): `void`

Visibility helper : Sets the size of a visibility box, this sets the underlying mesh bounding box.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | the size (float) of the visibility box  note : this doesn't lock the PCS mesh bounding box.  doc : |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:967

___

### updateParticle

▸ **updateParticle**(`particle`): [`CloudPoint`](CloudPoint.md)

Updates a particle : this function should  be overwritten by the user.
It is called on each particle by `setParticles()`. This is the place to code each particle behavior.
doc :

**`Example`**

```ts
: just set a particle position or velocity and recycle conditions
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particle` | [`CloudPoint`](CloudPoint.md) | The particle to update |

#### Returns

[`CloudPoint`](CloudPoint.md)

the updated particle

#### Defined in

https://github.com/babylon.js/core/src/Particles/pointsCloudSystem.ts:1070

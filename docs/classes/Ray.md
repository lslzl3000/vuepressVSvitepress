[@dev/core](../README.md) / [Exports](../modules.md) / Ray

# Class: Ray

Class representing a ray with position and direction

## Table of contents

### Constructors

- [constructor](Ray.md#constructor)

### Properties

- [\_tmpRay](Ray.md#_tmpray)
- [direction](Ray.md#direction)
- [length](Ray.md#length)
- [origin](Ray.md#origin)
- [\_RayDistant](Ray.md#_raydistant)
- [\_Rayl](Ray.md#_rayl)
- [\_Smallnum](Ray.md#_smallnum)
- [\_TmpVector3](Ray.md#_tmpvector3)

### Methods

- [\_comparePickingInfo](Ray.md#_comparepickinginfo)
- [clone](Ray.md#clone)
- [intersectionSegment](Ray.md#intersectionsegment)
- [intersectsAxis](Ray.md#intersectsaxis)
- [intersectsBox](Ray.md#intersectsbox)
- [intersectsBoxMinMax](Ray.md#intersectsboxminmax)
- [intersectsMesh](Ray.md#intersectsmesh)
- [intersectsMeshes](Ray.md#intersectsmeshes)
- [intersectsPlane](Ray.md#intersectsplane)
- [intersectsSphere](Ray.md#intersectssphere)
- [intersectsTriangle](Ray.md#intersectstriangle)
- [unprojectRayToRef](Ray.md#unprojectraytoref)
- [update](Ray.md#update)
- [CreateNew](Ray.md#createnew)
- [CreateNewFromTo](Ray.md#createnewfromto)
- [Transform](Ray.md#transform)
- [TransformToRef](Ray.md#transformtoref)
- [Zero](Ray.md#zero)

## Constructors

### constructor

• **new Ray**(`origin`, `direction`, `length?`)

Creates a new ray

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | `undefined` | origin point |
| `direction` | [`Vector3`](Vector3.md) | `undefined` | direction |
| `length` | `number` | `Number.MAX_VALUE` | length of the ray |

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:30

## Properties

### \_tmpRay

• `Private` **\_tmpRay**: [`Ray`](Ray.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:22

___

### direction

• **direction**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:34

___

### length

• **length**: `number` = `Number.MAX_VALUE`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:36

___

### origin

• **origin**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:32

___

### \_RayDistant

▪ `Static` `Private` **\_RayDistant**: [`Ray`](Ray.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:21

___

### \_Rayl

▪ `Static` `Private` **\_Rayl**: `number` = `10e8`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:353

___

### \_Smallnum

▪ `Static` `Private` **\_Smallnum**: `number` = `0.00000001`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:352

___

### \_TmpVector3

▪ `Static` `Private` `Readonly` **\_TmpVector3**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:20

## Methods

### \_comparePickingInfo

▸ `Private` **_comparePickingInfo**(`pickingInfoA`, `pickingInfoB`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pickingInfoA` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`PickingInfo`](PickingInfo.md) |
| `pickingInfoB` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`PickingInfo`](PickingInfo.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:342

___

### clone

▸ **clone**(): [`Ray`](Ray.md)

Clone the current ray

#### Returns

[`Ray`](Ray.md)

a new ray

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:45

___

### intersectionSegment

▸ **intersectionSegment**(`sega`, `segb`, `threshold`): `number`

Intersection test between the ray and a given segment within a given tolerance (threshold)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sega` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the first point of the segment to test the intersection against |
| `segb` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the second point of the segment to test the intersection against |
| `threshold` | `number` | the tolerance margin, if the ray doesn't intersect the segment but is close to the given threshold, the intersection is successful |

#### Returns

`number`

the distance from the ray origin to the intersection point if there's intersection, or -1 if there's no intersection

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:362

___

### intersectsAxis

▸ **intersectsAxis**(`axis`, `offset?`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Calculate the intercept of a ray on a given axis

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `axis` | `string` | `undefined` | to check 'x' \| 'y' \| 'z' |
| `offset` | `number` | `0` | from axis interception (i.e. an offset of 1y is intercepted above ground) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

a vector containing the coordinates where 'axis' is equal to zero (else offset), or null if there is no intercept.

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:267

___

### intersectsBox

▸ **intersectsBox**(`box`, `intersectionTreshold?`): `boolean`

Checks if the ray intersects a box
This does not account for the ray lenght by design to improve perfs.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `box` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingBox`](BoundingBox.md) | `undefined` | the bounding box to check |
| `intersectionTreshold` | `number` | `0` | extra extend to be added to the BoundingBox in all direction |

#### Returns

`boolean`

if the box was hit

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:155

___

### intersectsBoxMinMax

▸ **intersectsBoxMinMax**(`minimum`, `maximum`, `intersectionTreshold?`): `boolean`

Checks if the ray intersects a box
This does not account for the ray length by design to improve perfs.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `minimum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | `undefined` | bound of the box |
| `maximum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | `undefined` | bound of the box |
| `intersectionTreshold` | `number` | `0` | extra extend to be added to the box in all direction |

#### Returns

`boolean`

if the box was hit

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:57

___

### intersectsMesh

▸ **intersectsMesh**(`mesh`, `fastCheck?`): [`PickingInfo`](PickingInfo.md)

Checks if ray intersects a mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`AbstractMesh`](AbstractMesh.md) | the mesh to check |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |

#### Returns

[`PickingInfo`](PickingInfo.md)

picking info of the intersection

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:301

___

### intersectsMeshes

▸ **intersectsMeshes**(`meshes`, `fastCheck?`, `results?`): [`PickingInfo`](PickingInfo.md)[]

Checks if ray intersects a mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`AbstractMesh`](AbstractMesh.md)[] | the meshes to check |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `results?` | [`PickingInfo`](PickingInfo.md)[] | array to store result in |

#### Returns

[`PickingInfo`](PickingInfo.md)[]

Array of picking infos

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:322

___

### intersectsPlane

▸ **intersectsPlane**(`plane`): [`Nullable`](../modules.md#nullable)`number`

Checks if ray intersects a plane

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plane` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md) | the plane to check |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

the distance away it was hit

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:242

___

### intersectsSphere

▸ **intersectsSphere**(`sphere`, `intersectionTreshold?`): `boolean`

If the ray hits a sphere

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sphere` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingSphere`](BoundingSphere.md) | `undefined` | the bounding sphere to check |
| `intersectionTreshold` | `number` | `0` | extra extend to be added to the BoundingSphere in all direction |

#### Returns

`boolean`

true if it hits the sphere

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:165

___

### intersectsTriangle

▸ **intersectsTriangle**(`vertex0`, `vertex1`, `vertex2`): [`Nullable`](../modules.md#nullable)`IntersectionInfo`

If the ray hits a triange

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertex0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | triangle vertex |
| `vertex1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | triangle vertex |
| `vertex2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | triangle vertex |

#### Returns

[`Nullable`](../modules.md#nullable)`IntersectionInfo`

intersection information if hit

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:194

___

### unprojectRayToRef

▸ **unprojectRayToRef**(`sourceX`, `sourceY`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`): `void`

Unproject a ray from screen space to object space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceX` | `number` | defines the screen space x coordinate to use |
| `sourceY` | `number` | defines the screen space y coordinate to use |
| `viewportWidth` | `number` | defines the current width of the viewport |
| `viewportHeight` | `number` | defines the current height of the viewport |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use (can be set to Identity to go to world space) |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the view matrix to use |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the projection matrix to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:597

___

### update

▸ **update**(`x`, `y`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`, `enableDistantPicking?`): [`Ray`](Ray.md)

Update the ray from viewport position

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | position |
| `y` | `number` | `undefined` | y position |
| `viewportWidth` | `number` | `undefined` | viewport width |
| `viewportHeight` | `number` | `undefined` | viewport height |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` | world matrix |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` | view matrix |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` | projection matrix |
| `enableDistantPicking` | `boolean` | `false` | defines if picking should handle large values for mesh position/scaling (false by default) |

#### Returns

[`Ray`](Ray.md)

this ray updated

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:469

___

### CreateNew

▸ `Static` **CreateNew**(`x`, `y`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`): [`Ray`](Ray.md)

Creates a new ray from screen space and viewport

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | position |
| `y` | `number` | y position |
| `viewportWidth` | `number` | viewport width |
| `viewportHeight` | `number` | viewport height |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | world matrix |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | view matrix |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | projection matrix |

#### Returns

[`Ray`](Ray.md)

new ray

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:521

___

### CreateNewFromTo

▸ `Static` **CreateNewFromTo**(`origin`, `end`, `world?`): [`Ray`](Ray.md)

Function will create a new transformed ray starting from origin and ending at the end point. Ray's length will be set, and ray will be
transformed to the given world matrix.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | `undefined` | The origin point |
| `end` | [`Vector3`](Vector3.md) | `undefined` | The end point |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `Matrix.IdentityReadOnly` | a matrix to transform the ray to. Default is the identity matrix. |

#### Returns

[`Ray`](Ray.md)

the new ray

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:543

___

### Transform

▸ `Static` **Transform**(`ray`, `matrix`): [`Ray`](Ray.md)

Transforms a ray by a matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Ray`](Ray.md) | ray to transform |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | matrix to apply |

#### Returns

[`Ray`](Ray.md)

the resulting new ray

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:557

___

### TransformToRef

▸ `Static` **TransformToRef**(`ray`, `matrix`, `result`): `void`

Transforms a ray by a matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Ray`](Ray.md) | ray to transform |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | matrix to apply |
| `result` | [`Ray`](Ray.md) | ray to store result in |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:570

___

### Zero

▸ `Static` **Zero**(): [`Ray`](Ray.md)

Creates a ray with origin and direction of 0,0,0

#### Returns

[`Ray`](Ray.md)

the new ray

#### Defined in

https://github.com/babylon.js/core/src/Culling/ray.ts:506

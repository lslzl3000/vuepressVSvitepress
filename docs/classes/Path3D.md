[@dev/core](../README.md) / [Exports](../modules.md) / Path3D

# Class: Path3D

Represents a 3D path made up of multiple 3D points

**`See`**

https://doc.babylonjs.com/divingDeeper/mesh/path3D

## Table of contents

### Constructors

- [constructor](Path3D.md#constructor)

### Properties

- [\_alignTangentsWithPath](Path3D.md#_aligntangentswithpath)
- [\_binormals](Path3D.md#_binormals)
- [\_curve](Path3D.md#_curve)
- [\_distances](Path3D.md#_distances)
- [\_normals](Path3D.md#_normals)
- [\_pointAtData](Path3D.md#_pointatdata)
- [\_raw](Path3D.md#_raw)
- [\_tangents](Path3D.md#_tangents)
- [path](Path3D.md#path)

### Methods

- [\_compute](Path3D.md#_compute)
- [\_getFirstNonNullVector](Path3D.md#_getfirstnonnullvector)
- [\_getLastNonNullVector](Path3D.md#_getlastnonnullvector)
- [\_normalVector](Path3D.md#_normalvector)
- [\_setPointAtData](Path3D.md#_setpointatdata)
- [\_updateInterpolationMatrix](Path3D.md#_updateinterpolationmatrix)
- [\_updatePointAtData](Path3D.md#_updatepointatdata)
- [getBinormalAt](Path3D.md#getbinormalat)
- [getBinormals](Path3D.md#getbinormals)
- [getClosestPositionTo](Path3D.md#getclosestpositionto)
- [getCurve](Path3D.md#getcurve)
- [getDistanceAt](Path3D.md#getdistanceat)
- [getDistances](Path3D.md#getdistances)
- [getNormalAt](Path3D.md#getnormalat)
- [getNormals](Path3D.md#getnormals)
- [getPointAt](Path3D.md#getpointat)
- [getPoints](Path3D.md#getpoints)
- [getPreviousPointIndexAt](Path3D.md#getpreviouspointindexat)
- [getSubPositionAt](Path3D.md#getsubpositionat)
- [getTangentAt](Path3D.md#gettangentat)
- [getTangents](Path3D.md#gettangents)
- [length](Path3D.md#length)
- [slice](Path3D.md#slice)
- [update](Path3D.md#update)

## Constructors

### constructor

• **new Path3D**(`path`, `firstNormal?`, `raw?`, `alignTangentsWithPath?`)

new Path3D(path, normal, raw)
Creates a Path3D. A Path3D is a logical math object, so not a mesh.
please read the description in the tutorial : https://doc.babylonjs.com/how_to/how_to_use_path3d

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `path` | [`Vector3`](Vector3.md)[] | `undefined` | an array of Vector3, the curve axis of the Path3D |
| `firstNormal` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | `null` | (options) Vector3, the first wanted normal to the curve. Ex (0, 1, 0) for a vertical normal. |
| `raw?` | `boolean` | `undefined` | (optional, default false) : boolean, if true the returned Path3D isn't normalized. Useful to depict path acceleration or speed. |
| `alignTangentsWithPath` | `boolean` | `false` | (optional, default false) : boolean, if true the tangents will be aligned with the path. |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:371

## Properties

### \_alignTangentsWithPath

• `Private` **\_alignTangentsWithPath**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:347

___

### \_binormals

• `Private` **\_binormals**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:345

___

### \_curve

• `Private` **\_curve**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:341

___

### \_distances

• `Private` **\_distances**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:342

___

### \_normals

• `Private` **\_normals**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:344

___

### \_pointAtData

• `Private` `Readonly` **\_pointAtData**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `id` | `number` |
| `interpolateReady` | `boolean` |
| `interpolationMatrix` | [`Matrix`](Matrix.md) |
| `point` | [`Vector3`](Vector3.md) |
| `position` | `number` |
| `previousPointArrayIndex` | `number` |
| `subPosition` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:350

___

### \_raw

• `Private` **\_raw**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:346

___

### \_tangents

• `Private` **\_tangents**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:343

___

### path

• **path**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:375

## Methods

### \_compute

▸ `Private` **_compute**(`firstNormal`, `alignTangentsWithPath?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `firstNormal` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | `undefined` |
| `alignTangentsWithPath` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:594

___

### \_getFirstNonNullVector

▸ `Private` **_getFirstNonNullVector**(`index`): [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:665

___

### \_getLastNonNullVector

▸ `Private` **_getLastNonNullVector**(`index`): [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:677

___

### \_normalVector

▸ `Private` **_normalVector**(`vt`, `va`): [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `vt` | [`Vector3`](Vector3.md) |
| `va` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) |

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:690

___

### \_setPointAtData

▸ `Private` **_setPointAtData**(`position`, `subPosition`, `point`, `parentIndex`, `interpolateTNB`): `Object`

Updates the point at data from the specified parameters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | `number` | where along the path the interpolated point is, from 0.0 to 1.0 |
| `subPosition` | `number` |  |
| `point` | [`Vector3`](Vector3.md) | the interpolated point |
| `parentIndex` | `number` | the index of an existing curve point that is on, or else positionally the first behind, the interpolated point |
| `interpolateTNB` | `boolean` |  |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `id` | `number` |
| `interpolateReady` | `boolean` |
| `interpolationMatrix` | [`Matrix`](Matrix.md) |
| `point` | [`Vector3`](Vector3.md) |
| `position` | `number` |
| `previousPointArrayIndex` | `number` |
| `subPosition` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:775

___

### \_updateInterpolationMatrix

▸ `Private` **_updateInterpolationMatrix**(): `void`

Updates the point at interpolation matrix for the tangents, normals and binormals

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:791

___

### \_updatePointAtData

▸ `Private` **_updatePointAtData**(`position`, `interpolateTNB?`): `Object`

Updates the point at data for an interpolated point along this curve

**`Interpolate TNB`**

whether to compute the interpolated tangent, normal and binormal

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | `number` | `undefined` | the position of the point along this curve, from 0.0 to 1.0 |
| `interpolateTNB` | `boolean` | `false` |  |

#### Returns

`Object`

the (updated) point at data

| Name | Type |
| :------ | :------ |
| `id` | `number` |
| `interpolateReady` | `boolean` |
| `interpolationMatrix` | [`Matrix`](Matrix.md) |
| `point` | [`Vector3`](Vector3.md) |
| `position` | `number` |
| `previousPointArrayIndex` | `number` |
| `subPosition` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:725

___

### getBinormalAt

▸ **getBinormalAt**(`position`, `interpolated?`): [`Vector3`](Vector3.md)

Returns the binormal vector of an interpolated Path3D curve point at the specified position along this path.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | `number` | `undefined` | the position of the point along this path, from 0.0 to 1.0 |
| `interpolated` | `boolean` | `false` | (optional, default false) : boolean, if true returns an interpolated binormal instead of the binormal of the previous path point. |

#### Returns

[`Vector3`](Vector3.md)

a binormal vector corresponding to the interpolated Path3D curve point, if not interpolated, the binormal is taken from the precomputed binormals array.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:480

___

### getBinormals

▸ **getBinormals**(): [`Vector3`](Vector3.md)[]

Returns an array populated with binormal vectors on each Path3D curve point.

#### Returns

[`Vector3`](Vector3.md)[]

an array populated with binormal vectors on each Path3D curve point.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:431

___

### getClosestPositionTo

▸ **getClosestPositionTo**(`target`): `number`

Returns the position of the closest virtual point on this path to an arbitrary Vector3, from 0.0 to 1.0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Vector3`](Vector3.md) | the vector of which to get the closest position to |

#### Returns

`number`

the position of the closest virtual point on this path to the target vector

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:519

___

### getCurve

▸ **getCurve**(): [`Vector3`](Vector3.md)[]

Returns the Path3D array of successive Vector3 designing its curve.

#### Returns

[`Vector3`](Vector3.md)[]

the Path3D array of successive Vector3 designing its curve.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:392

___

### getDistanceAt

▸ **getDistanceAt**(`position`): `number`

Returns the distance (float) of an interpolated Path3D curve point at the specified position along this path.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | `number` | the position of the point along this path, from 0.0 to 1.0 |

#### Returns

`number`

the distance of the interpolated Path3D curve point at the specified position along this path.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:490

___

### getDistances

▸ **getDistances**(): `number`[]

Returns an array populated with distances (float) of the i-th point from the first curve point.

#### Returns

`number`[]

an array populated with distances (float) of the i-th point from the first curve point.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:439

___

### getNormalAt

▸ **getNormalAt**(`position`, `interpolated?`): [`Vector3`](Vector3.md)

Returns the tangent vector of an interpolated Path3D curve point at the specified position along this path.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | `number` | `undefined` | the position of the point along this path, from 0.0 to 1.0 |
| `interpolated` | `boolean` | `false` | (optional, default false) : boolean, if true returns an interpolated normal instead of the normal of the previous path point. |

#### Returns

[`Vector3`](Vector3.md)

a normal vector corresponding to the interpolated Path3D curve point, if not interpolated, the normal is taken from the precomputed normals array.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:469

___

### getNormals

▸ **getNormals**(): [`Vector3`](Vector3.md)[]

Returns an array populated with normal vectors on each Path3D curve point.

#### Returns

[`Vector3`](Vector3.md)[]

an array populated with normal vectors on each Path3D curve point.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:423

___

### getPointAt

▸ **getPointAt**(`position`): [`Vector3`](Vector3.md)

Returns an interpolated point along this path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | `number` | the position of the point along this path, from 0.0 to 1.0 |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 as the point

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:448

___

### getPoints

▸ **getPoints**(): [`Vector3`](Vector3.md)[]

Returns the Path3D array of successive Vector3 designing its curve.

#### Returns

[`Vector3`](Vector3.md)[]

the Path3D array of successive Vector3 designing its curve.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:400

___

### getPreviousPointIndexAt

▸ **getPreviousPointIndexAt**(`position`): `number`

Returns the array index of the previous point of an interpolated point along this path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | `number` | the position of the point to interpolate along this path, from 0.0 to 1.0 |

#### Returns

`number`

the array index

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:499

___

### getSubPositionAt

▸ **getSubPositionAt**(`position`): `number`

Returns the position of an interpolated point relative to the two path points it lies between, from 0.0 (point A) to 1.0 (point B)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | `number` | the position of the point to interpolate along this path, from 0.0 to 1.0 |

#### Returns

`number`

the sub position

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:509

___

### getTangentAt

▸ **getTangentAt**(`position`, `interpolated?`): [`Vector3`](Vector3.md)

Returns the tangent vector of an interpolated Path3D curve point at the specified position along this path.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | `number` | `undefined` | the position of the point along this path, from 0.0 to 1.0 |
| `interpolated` | `boolean` | `false` | (optional, default false) : boolean, if true returns an interpolated tangent instead of the tangent of the previous path point. |

#### Returns

[`Vector3`](Vector3.md)

a tangent vector corresponding to the interpolated Path3D curve point, if not interpolated, the tangent is taken from the precomputed tangents array.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:458

___

### getTangents

▸ **getTangents**(): [`Vector3`](Vector3.md)[]

Returns an array populated with tangent vectors on each Path3D curve point.

#### Returns

[`Vector3`](Vector3.md)[]

an array populated with tangent vectors on each Path3D curve point.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:415

___

### length

▸ **length**(): `number`

#### Returns

`number`

the computed length (float) of the path.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:407

___

### slice

▸ **slice**(`start?`, `end?`): [`Path3D`](Path3D.md)

Returns a sub path (slice) of this path

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `start` | `number` | `0.0` | the position of the fist path point, from 0.0 to 1.0, or a negative value, which will get wrapped around from the end of the path to 0.0 to 1.0 values |
| `end` | `number` | `1.0` | the position of the last path point, from 0.0 to 1.0, or a negative value, which will get wrapped around from the end of the path to 0.0 to 1.0 values |

#### Returns

[`Path3D`](Path3D.md)

a sub path (slice) of this path

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:543

___

### update

▸ **update**(`path`, `firstNormal?`, `alignTangentsWithPath?`): [`Path3D`](Path3D.md)

Forces the Path3D tangent, normal, binormal and distance recomputation.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `path` | [`Vector3`](Vector3.md)[] | `undefined` | path which all values are copied into the curves points |
| `firstNormal` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | `null` | which should be projected onto the curve |
| `alignTangentsWithPath` | `boolean` | `false` | (optional, default false) : boolean, if true the tangents will be aligned with the path |

#### Returns

[`Path3D`](Path3D.md)

the same object updated.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:583

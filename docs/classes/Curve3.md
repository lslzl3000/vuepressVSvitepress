[@dev/core](../README.md) / [Exports](../modules.md) / Curve3

# Class: Curve3

A Curve3 object is a logical object, so not a mesh, to handle curves in the 3D geometric space.
A Curve3 is designed from a series of successive Vector3.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_curve3

## Table of contents

### Constructors

- [constructor](Curve3.md#constructor)

### Properties

- [\_length](Curve3.md#_length)
- [\_points](Curve3.md#_points)

### Methods

- [\_computeLength](Curve3.md#_computelength)
- [continue](Curve3.md#continue)
- [getPoints](Curve3.md#getpoints)
- [length](Curve3.md#length)
- [ArcThru3Points](Curve3.md#arcthru3points)
- [CreateCatmullRomSpline](Curve3.md#createcatmullromspline)
- [CreateCubicBezier](Curve3.md#createcubicbezier)
- [CreateHermiteSpline](Curve3.md#createhermitespline)
- [CreateQuadraticBezier](Curve3.md#createquadraticbezier)

## Constructors

### constructor

• **new Curve3**(`points`)

A Curve3 object is a logical object, so not a mesh, to handle curves in the 3D geometric space.
A Curve3 is designed from a series of successive Vector3.
Tuto : https://doc.babylonjs.com/how_to/how_to_use_curve3#curve3-object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `points` | [`Vector3`](Vector3.md)[] | points which make up the curve |

#### Defined in

packages/dev/core/src/Maths/math.path.ts:995

## Properties

### \_length

• `Private` **\_length**: `number` = `0.0`

#### Defined in

packages/dev/core/src/Maths/math.path.ts:822

___

### \_points

• `Private` **\_points**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Maths/math.path.ts:821

## Methods

### \_computeLength

▸ `Private` **_computeLength**(`path`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `DeepImmutableArray`[`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Maths/math.path.ts:1032

___

### continue

▸ **continue**(`curve`): [`Curve3`](Curve3.md)

Returns a new instance of Curve3 object : var curve = curveA.continue(curveB);
This new Curve3 is built by translating and sticking the curveB at the end of the curveA.
curveA and curveB keep unchanged.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `curve` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Curve3`](Curve3.md) | the curve to continue from this curve |

#### Returns

[`Curve3`](Curve3.md)

the newly constructed curve

#### Defined in

packages/dev/core/src/Maths/math.path.ts:1021

___

### getPoints

▸ **getPoints**(): [`Vector3`](Vector3.md)[]

#### Returns

[`Vector3`](Vector3.md)[]

the Curve3 stored array of successive Vector3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:1003

___

### length

▸ **length**(): `number`

#### Returns

`number`

the computed length (float) of the curve.

#### Defined in

packages/dev/core/src/Maths/math.path.ts:1010

___

### ArcThru3Points

▸ `Static` **ArcThru3Points**(`first`, `second`, `third`, `steps?`, `closed?`, `fullCircle?`): [`Curve3`](Curve3.md)

Returns a Curve3 object along an arc through three vector3 points:
The three points should not be colinear. When they are the Curve3 is empty.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `first` | [`Vector3`](Vector3.md) | `undefined` | (Vector3) the first point the arc must pass through. |
| `second` | [`Vector3`](Vector3.md) | `undefined` | (Vector3) the second point the arc must pass through. |
| `third` | [`Vector3`](Vector3.md) | `undefined` | (Vector3) the third point the arc must pass through. |
| `steps` | `number` | `32` | (number) the larger the number of steps the more detailed the arc. |
| `closed` | `boolean` | `false` | (boolean) optional with default false, when true forms the chord from the first and third point |
| `fullCircle` | `boolean` | `false` | Circle (boolean) optional with default false, when true forms the complete circle through the three points |

#### Returns

[`Curve3`](Curve3.md)

the created Curve3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:938

___

### CreateCatmullRomSpline

▸ `Static` **CreateCatmullRomSpline**(`points`, `nbPoints`, `closed?`): [`Curve3`](Curve3.md)

Returns a Curve3 object along a CatmullRom Spline curve :

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `points` | `DeepImmutableArray`[`Vector3`](Vector3.md) | (array of Vector3) the points the spline must pass through. At least, four points required |
| `nbPoints` | `number` | (integer) the wanted number of points between each curve control points |
| `closed?` | `boolean` | (boolean) optional with default false, when true forms a closed loop from the points |

#### Returns

[`Curve3`](Curve3.md)

the created Curve3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:892

___

### CreateCubicBezier

▸ `Static` **CreateCubicBezier**(`v0`, `v1`, `v2`, `v3`, `nbPoints`): [`Curve3`](Curve3.md)

Returns a Curve3 object along a Cubic Bezier curve : https://doc.babylonjs.com/how_to/how_to_use_curve3#cubic-bezier-curve

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the origin point of the Cubic Bezier |
| `v1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the first control point |
| `v2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the second control point |
| `v3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the end point of the Cubic Bezier |
| `nbPoints` | `number` | (integer) the wanted number of points in the curve |

#### Returns

[`Curve3`](Curve3.md)

the created Curve3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:854

___

### CreateHermiteSpline

▸ `Static` **CreateHermiteSpline**(`p1`, `t1`, `p2`, `t2`, `nbPoints`): [`Curve3`](Curve3.md)

Returns a Curve3 object along a Hermite Spline curve : https://doc.babylonjs.com/how_to/how_to_use_curve3#hermite-spline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `p1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the origin point of the Hermite Spline |
| `t1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the tangent vector at the origin point |
| `p2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the end point of the Hermite Spline |
| `t2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the tangent vector at the end point |
| `nbPoints` | `number` | (integer) the wanted number of points in the curve |

#### Returns

[`Curve3`](Curve3.md)

the created Curve3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:876

___

### CreateQuadraticBezier

▸ `Static` **CreateQuadraticBezier**(`v0`, `v1`, `v2`, `nbPoints`): [`Curve3`](Curve3.md)

Returns a Curve3 object along a Quadratic Bezier curve : https://doc.babylonjs.com/how_to/how_to_use_curve3#quadratic-bezier-curve

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the origin point of the Quadratic Bezier |
| `v1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the control point |
| `v2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | (Vector3) the end point of the Quadratic Bezier |
| `nbPoints` | `number` | (integer) the wanted number of points in the curve |

#### Returns

[`Curve3`](Curve3.md)

the created Curve3

#### Defined in

packages/dev/core/src/Maths/math.path.ts:832

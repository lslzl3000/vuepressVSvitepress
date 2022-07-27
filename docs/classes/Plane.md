[@dev/core](../README.md) / [Exports](../modules.md) / Plane

# Class: Plane

Represents a plane by the equation ax + by + cz + d = 0

## Table of contents

### Constructors

- [constructor](Plane.md#constructor)

### Properties

- [d](Plane.md#d)
- [normal](Plane.md#normal)
- [\_TmpMatrix](Plane.md#_tmpmatrix)

### Methods

- [asArray](Plane.md#asarray)
- [clone](Plane.md#clone)
- [copyFromPoints](Plane.md#copyfrompoints)
- [dotCoordinate](Plane.md#dotcoordinate)
- [getClassName](Plane.md#getclassname)
- [getHashCode](Plane.md#gethashcode)
- [isFrontFacingTo](Plane.md#isfrontfacingto)
- [normalize](Plane.md#normalize)
- [signedDistanceTo](Plane.md#signeddistanceto)
- [transform](Plane.md#transform)
- [FromArray](Plane.md#fromarray)
- [FromPoints](Plane.md#frompoints)
- [FromPositionAndNormal](Plane.md#frompositionandnormal)
- [SignedDistanceToPlaneFromPositionAndNormal](Plane.md#signeddistancetoplanefrompositionandnormal)

## Constructors

### constructor

• **new Plane**(`a`, `b`, `c`, `d`)

Creates a Plane object according to the given floats a, b, c, d and the plane equation : ax + by + cz + d = 0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | `number` | a component of the plane |
| `b` | `number` | b component of the plane |
| `c` | `number` | c component of the plane |
| `d` | `number` | d component of the plane |

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:25

## Properties

### d

• **d**: `number`

d component of the plane

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:17

___

### normal

• **normal**: [`Vector3`](Vector3.md)

Normal of the plane (a,b,c)

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:13

___

### \_TmpMatrix

▪ `Static` `Private` **\_TmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:8

## Methods

### asArray

▸ **asArray**(): `number`[]

#### Returns

`number`[]

the plane coordinates as a new array of 4 elements [a, b, c, d].

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:33

___

### clone

▸ **clone**(): [`Plane`](Plane.md)

#### Returns

[`Plane`](Plane.md)

a new plane copied from the current Plane.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:41

___

### copyFromPoints

▸ **copyFromPoints**(`point1`, `point2`, `point3`): [`Plane`](Plane.md)

Updates the current Plane from the plane defined by the three given points.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | one of the points used to construct the plane |
| `point2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | one of the points used to construct the plane |
| `point3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | one of the points used to construct the plane |

#### Returns

[`Plane`](Plane.md)

the updated Plane.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:113

___

### dotCoordinate

▸ **dotCoordinate**(`point`): `number`

Compute the dot product between the point and the plane normal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point to calculate the dot product with |

#### Returns

`number`

the dot product (float) of the point coordinates and the plane normal.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:102

___

### getClassName

▸ **getClassName**(): `string`

#### Returns

`string`

the string "Plane".

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:47

___

### getHashCode

▸ **getHashCode**(): `number`

#### Returns

`number`

the Plane hash code.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:53

___

### isFrontFacingTo

▸ **isFrontFacingTo**(`direction`, `epsilon`): `boolean`

Checks if the plane is facing a given direction (meaning if the plane's normal is pointing in the opposite direction of the given vector).
Note that for this function to work as expected you should make sure that:
  - direction and the plane normal are normalized
  - epsilon is a number just bigger than -1, something like -0.99 for eg

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the direction to check if the plane is facing |
| `epsilon` | `number` | value the dot product is compared against (returns true if dot = epsilon) |

#### Returns

`boolean`

True if the plane is facing the given direction

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:149

___

### normalize

▸ **normalize**(): [`Plane`](Plane.md)

Normalize the current Plane in place.

#### Returns

[`Plane`](Plane.md)

the updated Plane.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:62

___

### signedDistanceTo

▸ **signedDistanceTo**(`point`): `number`

Calculates the distance to a point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point to calculate distance to |

#### Returns

`number`

the signed distance (float) from the given point to the Plane.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:159

___

### transform

▸ **transform**(`transformation`): [`Plane`](Plane.md)

Applies a transformation the plane and returns the result

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | the transformation matrix to be applied to the plane |

#### Returns

[`Plane`](Plane.md)

a new Plane as the result of the transformation of the current Plane by the given matrix.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:80

___

### FromArray

▸ `Static` **FromArray**(`array`): [`Plane`](Plane.md)

Creates a plane from an  array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | the array to create a plane from |

#### Returns

[`Plane`](Plane.md)

a new Plane from the given array.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:169

___

### FromPoints

▸ `Static` **FromPoints**(`point1`, `point2`, `point3`): [`Plane`](Plane.md)

Creates a plane from three points

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point used to create the plane |
| `point2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point used to create the plane |
| `point3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point used to create the plane |

#### Returns

[`Plane`](Plane.md)

a new Plane defined by the three given points.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:179

___

### FromPositionAndNormal

▸ `Static` **FromPositionAndNormal**(`origin`, `normal`): [`Plane`](Plane.md)

Creates a plane from an origin point and a normal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | origin of the plane to be constructed |
| `normal` | [`Vector3`](Vector3.md) | normal of the plane to be constructed |

#### Returns

[`Plane`](Plane.md)

a new Plane the normal vector to this plane at the given origin point.
Note : the vector "normal" is updated because normalized.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:191

___

### SignedDistanceToPlaneFromPositionAndNormal

▸ `Static` **SignedDistanceToPlaneFromPositionAndNormal**(`origin`, `normal`, `point`): `number`

Calculates the distance from a plane and a point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | origin of the plane to be constructed |
| `normal` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | normal of the plane to be constructed |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point to calculate distance to |

#### Returns

`number`

the signed distance between the plane defined by the normal vector at the "origin"" point and the given other point.

#### Defined in

packages/dev/core/src/Maths/math.plane.ts:206

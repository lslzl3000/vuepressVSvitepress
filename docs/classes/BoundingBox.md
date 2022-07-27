[@dev/core](../README.md) / [Exports](../modules.md) / BoundingBox

# Class: BoundingBox

Class used to store bounding box information

## Implements

- [`ICullable`](../interfaces/ICullable.md)

## Table of contents

### Constructors

- [constructor](BoundingBox.md#constructor)

### Properties

- [\_worldMatrix](BoundingBox.md#_worldmatrix)
- [center](BoundingBox.md#center)
- [centerWorld](BoundingBox.md#centerworld)
- [directions](BoundingBox.md#directions)
- [extendSize](BoundingBox.md#extendsize)
- [extendSizeWorld](BoundingBox.md#extendsizeworld)
- [maximum](BoundingBox.md#maximum)
- [maximumWorld](BoundingBox.md#maximumworld)
- [minimum](BoundingBox.md#minimum)
- [minimumWorld](BoundingBox.md#minimumworld)
- [vectors](BoundingBox.md#vectors)
- [vectorsWorld](BoundingBox.md#vectorsworld)
- [\_TmpVector3](BoundingBox.md#_tmpvector3)

### Methods

- [dispose](BoundingBox.md#dispose)
- [getWorldMatrix](BoundingBox.md#getworldmatrix)
- [intersectsMinMax](BoundingBox.md#intersectsminmax)
- [intersectsPoint](BoundingBox.md#intersectspoint)
- [intersectsSphere](BoundingBox.md#intersectssphere)
- [isCompletelyInFrustum](BoundingBox.md#iscompletelyinfrustum)
- [isInFrustum](BoundingBox.md#isinfrustum)
- [reConstruct](BoundingBox.md#reconstruct)
- [scale](BoundingBox.md#scale)
- [Intersects](BoundingBox.md#intersects)
- [IntersectsSphere](BoundingBox.md#intersectssphere-1)
- [IsCompletelyInFrustum](BoundingBox.md#iscompletelyinfrustum-1)
- [IsInFrustum](BoundingBox.md#isinfrustum-1)

## Constructors

### constructor

• **new BoundingBox**(`min`, `max`, `worldMatrix?`)

Creates a new bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the minimum vector (in local space) |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the maximum vector (in local space) |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:80

## Properties

### \_worldMatrix

• `Private` **\_worldMatrix**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:61

___

### center

• `Readonly` **center**: [`Vector3`](Vector3.md)

Gets the center of the bounding box in local space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:23

___

### centerWorld

• `Readonly` **centerWorld**: [`Vector3`](Vector3.md)

Gets the center of the bounding box in world space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:27

___

### directions

• `Readonly` **directions**: [`Vector3`](Vector3.md)[]

Gets the OBB (object bounding box) directions

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:39

___

### extendSize

• `Readonly` **extendSize**: [`Vector3`](Vector3.md)

Gets the extend size in local space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:31

___

### extendSizeWorld

• `Readonly` **extendSizeWorld**: [`Vector3`](Vector3.md)

Gets the extend size in world space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:35

___

### maximum

• `Readonly` **maximum**: [`Vector3`](Vector3.md)

Gets the maximum vector in local space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:59

___

### maximumWorld

• `Readonly` **maximumWorld**: [`Vector3`](Vector3.md)

Gets the maximum vector in world space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:51

___

### minimum

• `Readonly` **minimum**: [`Vector3`](Vector3.md)

Gets the minimum vector in local space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:55

___

### minimumWorld

• `Readonly` **minimumWorld**: [`Vector3`](Vector3.md)

Gets the minimum vector in world space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:47

___

### vectors

• `Readonly` **vectors**: [`Vector3`](Vector3.md)[]

Gets the 8 vectors representing the bounding box in local space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:19

___

### vectorsWorld

• `Readonly` **vectorsWorld**: [`Vector3`](Vector3.md)[]

Gets the 8 vectors representing the bounding box in world space

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:43

___

### \_TmpVector3

▪ `Static` `Private` `Readonly` **\_TmpVector3**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:62

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the resources of the class

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:294

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

Gets the world matrix of the bounding box

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

a matrix

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:146

___

### intersectsMinMax

▸ **intersectsMinMax**(`min`, `max`): `boolean`

Tests if the bounding box intersects with a box defined by a min and max vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the min vector to use |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the max vector to use |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:261

___

### intersectsPoint

▸ **intersectsPoint**(`point`): `boolean`

Tests if a point is inside the bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the point to test |

#### Returns

`boolean`

true if the point is inside the bounding box

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:217

___

### intersectsSphere

▸ **intersectsSphere**(`sphere`): `boolean`

Tests if the bounding box intersects with a bounding sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sphere` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingSphere`](BoundingSphere.md) | defines the sphere to test |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:251

___

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`frustumPlanes`): `boolean`

Tests if the bounding box is entirely inside the frustum planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if there is an inclusion

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isCompletelyInFrustum](../interfaces/ICullable.md#iscompletelyinfrustum)

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:208

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

Tests if the bounding box is intersecting the frustum planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if there is an intersection

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isInFrustum](../interfaces/ICullable.md#isinfrustum)

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:199

___

### reConstruct

▸ **reConstruct**(`min`, `max`, `worldMatrix?`): `void`

Recreates the entire bounding box from scratch as if we call the constructor in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new minimum vector (in local space) |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new maximum vector (in local space) |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:92

___

### scale

▸ **scale**(`factor`): [`BoundingBox`](BoundingBox.md)

Scale the current bounding box by applying a scale factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `factor` | `number` | defines the scale factor to apply |

#### Returns

[`BoundingBox`](BoundingBox.md)

the current bounding box

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:126

___

### Intersects

▸ `Static` **Intersects**(`box0`, `box1`): `boolean`

Tests if two bounding boxes are intersections

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `box0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingBox`](BoundingBox.md) | defines the first box to test |
| `box1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingBox`](BoundingBox.md) | defines the second box to test |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:307

___

### IntersectsSphere

▸ `Static` **IntersectsSphere**(`minPoint`, `maxPoint`, `sphereCenter`, `sphereRadius`): `boolean`

Tests if a bounding box defines by a min/max vectors intersects a sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minPoint` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the minimum vector of the bounding box |
| `maxPoint` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the maximum vector of the bounding box |
| `sphereCenter` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the sphere center |
| `sphereRadius` | `number` | defines the sphere radius |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:319

___

### IsCompletelyInFrustum

▸ `Static` **IsCompletelyInFrustum**(`boundingVectors`, `frustumPlanes`): `boolean`

Tests if a bounding box defined with 8 vectors is entirely inside frustum planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `boundingVectors` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)[] | defines an array of 8 vectors representing a bounding box |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if there is an inclusion

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:332

___

### IsInFrustum

▸ `Static` **IsInFrustum**(`boundingVectors`, `frustumPlanes`): `boolean`

Tests if a bounding box defined with 8 vectors intersects frustum planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `boundingVectors` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)[] | defines an array of 8 vectors representing a bounding box |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Culling/boundingBox.ts:350

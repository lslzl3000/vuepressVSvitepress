[@dev/core](../README.md) / [Exports](../modules.md) / BoundingSphere

# Class: BoundingSphere

Class used to store bounding sphere information

## Table of contents

### Constructors

- [constructor](BoundingSphere.md#constructor)

### Properties

- [\_worldMatrix](BoundingSphere.md#_worldmatrix)
- [center](BoundingSphere.md#center)
- [centerWorld](BoundingSphere.md#centerworld)
- [maximum](BoundingSphere.md#maximum)
- [minimum](BoundingSphere.md#minimum)
- [radius](BoundingSphere.md#radius)
- [radiusWorld](BoundingSphere.md#radiusworld)
- [\_TmpVector3](BoundingSphere.md#_tmpvector3)

### Methods

- [getWorldMatrix](BoundingSphere.md#getworldmatrix)
- [intersectsPoint](BoundingSphere.md#intersectspoint)
- [isCenterInFrustum](BoundingSphere.md#iscenterinfrustum)
- [isInFrustum](BoundingSphere.md#isinfrustum)
- [reConstruct](BoundingSphere.md#reconstruct)
- [scale](BoundingSphere.md#scale)
- [CreateFromCenterAndRadius](BoundingSphere.md#createfromcenterandradius)
- [Intersects](BoundingSphere.md#intersects)

## Constructors

### constructor

• **new BoundingSphere**(`min`, `max`, `worldMatrix?`)

Creates a new bounding sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the minimum vector (in local space) |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the maximum vector (in local space) |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:44

## Properties

### \_worldMatrix

• `Private` **\_worldMatrix**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:35

___

### center

• `Readonly` **center**: [`Vector3`](Vector3.md)

Gets the center of the bounding sphere in local space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:13

___

### centerWorld

• `Readonly` **centerWorld**: [`Vector3`](Vector3.md)

Gets the center of the bounding sphere in world space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:21

___

### maximum

• `Readonly` **maximum**: [`Vector3`](Vector3.md)

Gets the maximum vector in local space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:33

___

### minimum

• `Readonly` **minimum**: [`Vector3`](Vector3.md)

Gets the minimum vector in local space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:29

___

### radius

• **radius**: `number`

Radius of the bounding sphere in local space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:17

___

### radiusWorld

• **radiusWorld**: `number`

Radius of the bounding sphere in world space

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:25

___

### \_TmpVector3

▪ `Static` `Private` `Readonly` **\_TmpVector3**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:36

## Methods

### getWorldMatrix

▸ **getWorldMatrix**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

Gets the world matrix of the bounding box

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

a matrix

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:87

___

### intersectsPoint

▸ **intersectsPoint**(`point`): `boolean`

Tests if a point is inside the bounding sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the point to test |

#### Returns

`boolean`

true if the point is inside the bounding sphere

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:145

___

### isCenterInFrustum

▸ **isCenterInFrustum**(`frustumPlanes`): `boolean`

Tests if the bounding sphere center is in between the frustum planes.
Used for optimistic fast inclusion.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if the sphere center is in between the frustum planes

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:130

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

Tests if the bounding sphere is intersecting the frustum planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | defines the frustum planes to test |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:113

___

### reConstruct

▸ **reConstruct**(`min`, `max`, `worldMatrix?`): `void`

Recreates the entire bounding sphere from scratch as if we call the constructor in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new minimum vector (in local space) |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new maximum vector (in local space) |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:54

___

### scale

▸ **scale**(`factor`): [`BoundingSphere`](BoundingSphere.md)

Scale the current bounding sphere by applying a scale factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `factor` | `number` | defines the scale factor to apply |

#### Returns

[`BoundingSphere`](BoundingSphere.md)

the current bounding box

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:71

___

### CreateFromCenterAndRadius

▸ `Static` **CreateFromCenterAndRadius**(`center`, `radius`, `matrix?`): [`BoundingSphere`](BoundingSphere.md)

Creates a sphere from a center and a radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `center` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | The center |
| `radius` | `number` | radius |
| `matrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | Optional worldMatrix |

#### Returns

[`BoundingSphere`](BoundingSphere.md)

The sphere

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:179

___

### Intersects

▸ `Static` **Intersects**(`sphere0`, `sphere1`): `boolean`

Checks if two sphere intersect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sphere0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingSphere`](BoundingSphere.md) | sphere 0 |
| `sphere1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingSphere`](BoundingSphere.md) | sphere 1 |

#### Returns

`boolean`

true if the spheres intersect

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingSphere.ts:161

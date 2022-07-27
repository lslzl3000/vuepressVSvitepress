[@dev/core](../README.md) / [Exports](../modules.md) / BoundingInfo

# Class: BoundingInfo

Info for a bounding data of a mesh

## Implements

- [`ICullable`](../interfaces/ICullable.md)

## Table of contents

### Constructors

- [constructor](BoundingInfo.md#constructor)

### Properties

- [\_isLocked](BoundingInfo.md#_islocked)
- [boundingBox](BoundingInfo.md#boundingbox)
- [boundingSphere](BoundingInfo.md#boundingsphere)
- [\_TmpVector3](BoundingInfo.md#_tmpvector3)

### Accessors

- [diagonalLength](BoundingInfo.md#diagonallength)
- [isLocked](BoundingInfo.md#islocked)
- [maximum](BoundingInfo.md#maximum)
- [minimum](BoundingInfo.md#minimum)

### Methods

- [centerOn](BoundingInfo.md#centeron)
- [encapsulate](BoundingInfo.md#encapsulate)
- [encapsulateBoundingInfo](BoundingInfo.md#encapsulateboundinginfo)
- [intersects](BoundingInfo.md#intersects)
- [intersectsPoint](BoundingInfo.md#intersectspoint)
- [isCompletelyInFrustum](BoundingInfo.md#iscompletelyinfrustum)
- [isInFrustum](BoundingInfo.md#isinfrustum)
- [reConstruct](BoundingInfo.md#reconstruct)
- [scale](BoundingInfo.md#scale)
- [update](BoundingInfo.md#update)

## Constructors

### constructor

• **new BoundingInfo**(`minimum`, `maximum`, `worldMatrix?`)

Constructs bounding info

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minimum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | min vector of the bounding box/sphere |
| `maximum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | max vector of the bounding box/sphere |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:75

## Properties

### \_isLocked

• `Private` **\_isLocked**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:65

___

### boundingBox

• `Readonly` **boundingBox**: [`BoundingBox`](BoundingBox.md)

Bounding box for the mesh

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:59

___

### boundingSphere

• `Readonly` **boundingSphere**: [`BoundingSphere`](BoundingSphere.md)

Bounding sphere for the mesh

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:63

___

### \_TmpVector3

▪ `Static` `Private` `Readonly` **\_TmpVector3**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:67

## Accessors

### diagonalLength

• `get` **diagonalLength**(): `number`

Gets the world distance between the min and max points of the bounding box

#### Returns

`number`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:213

___

### isLocked

• `get` **isLocked**(): `boolean`

If the info is locked and won't be updated to avoid perf overhead

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:108

• `set` **isLocked**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:112

___

### maximum

• `get` **maximum**(): [`Vector3`](Vector3.md)

max vector of the bounding box/sphere

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:101

___

### minimum

• `get` **minimum**(): [`Vector3`](Vector3.md)

min vector of the bounding box/sphere

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:94

## Methods

### centerOn

▸ **centerOn**(`center`, `extend`): [`BoundingInfo`](BoundingInfo.md)

Recreate the bounding info to be centered around a specific point given a specific extend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `center` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | New center of the bounding info |
| `extend` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | New extend of the bounding info |

#### Returns

[`BoundingInfo`](BoundingInfo.md)

the current bounding info

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:135

___

### encapsulate

▸ **encapsulate**(`point`): [`BoundingInfo`](BoundingInfo.md)

Grows the bounding info to include the given point.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | The point that will be included in the current bounding info |

#### Returns

[`BoundingInfo`](BoundingInfo.md)

the current bounding info

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:150

___

### encapsulateBoundingInfo

▸ **encapsulateBoundingInfo**(`toEncapsulate`): [`BoundingInfo`](BoundingInfo.md)

Grows the bounding info to encapsulate the given bounding info.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toEncapsulate` | [`BoundingInfo`](BoundingInfo.md) | The bounding info that will be encapsulated in the current bounding info |

#### Returns

[`BoundingInfo`](BoundingInfo.md)

the current bounding info

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:163

___

### intersects

▸ **intersects**(`boundingInfo`, `precise`): `boolean`

Checks if another bounding info intersects the bounding box and bounding sphere or the mesh

**`See`**

https://doc.babylonjs.com/babylon101/intersect_collisions_-_mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `boundingInfo` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`BoundingInfo`](BoundingInfo.md) | the bounding info to check intersection with |
| `precise` | `boolean` | if the intersection should be done using OBB |

#### Returns

`boolean`

if the bounding info intersects

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:265

___

### intersectsPoint

▸ **intersectsPoint**(`point`): `boolean`

Checks if a point is inside the bounding box and bounding sphere or the mesh

**`See`**

https://doc.babylonjs.com/babylon101/intersect_collisions_-_mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the point to check intersection with |

#### Returns

`boolean`

if the point intersects

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:242

___

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`frustumPlanes`): `boolean`

Checks if a cullable object (mesh...) is in the camera frustum
Unlike isInFrustum this checks the full bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | Camera near/planes |

#### Returns

`boolean`

true if the object is in frustum otherwise false

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isCompletelyInFrustum](../interfaces/ICullable.md#iscompletelyinfrustum)

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:225

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`, `strategy?`): `boolean`

Returns `true` if the bounding info is within the frustum defined by the passed array of planes.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `frustumPlanes` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Plane`](Plane.md)[] | `undefined` | defines the frustum to test |
| `strategy` | `number` | `Constants.MESHES_CULLINGSTRATEGY_STANDARD` | defines the strategy to use for the culling (default is BABYLON.AbstractMesh.CULLINGSTRATEGY_STANDARD) |

#### Returns

`boolean`

true if the bounding info is in the frustum planes

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isInFrustum](../interfaces/ICullable.md#isinfrustum)

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:188

___

### reConstruct

▸ **reConstruct**(`min`, `max`, `worldMatrix?`): `void`

Recreates the entire bounding info from scratch as if we call the constructor in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new minimum vector (in local space) |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the new maximum vector (in local space) |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:86

___

### scale

▸ **scale**(`factor`): [`BoundingInfo`](BoundingInfo.md)

Scale the current bounding info by applying a scale factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `factor` | `number` | defines the scale factor to apply |

#### Returns

[`BoundingInfo`](BoundingInfo.md)

the current bounding info

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:175

___

### update

▸ **update**(`world`): `void`

Updates the bounding sphere and box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | world matrix to be used to update |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/boundingInfo.ts:121

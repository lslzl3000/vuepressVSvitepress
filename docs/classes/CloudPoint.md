[@dev/core](../README.md) / [Exports](../modules.md) / CloudPoint

# Class: CloudPoint

Represents one particle of a points cloud system.

## Table of contents

### Constructors

- [constructor](CloudPoint.md#constructor)

### Properties

- [\_group](CloudPoint.md#_group)
- [color](CloudPoint.md#color)
- [groupId](CloudPoint.md#groupid)
- [idx](CloudPoint.md#idx)
- [idxInGroup](CloudPoint.md#idxingroup)
- [parentId](CloudPoint.md#parentid)
- [pivot](CloudPoint.md#pivot)
- [position](CloudPoint.md#position)
- [rotation](CloudPoint.md#rotation)
- [rotationQuaternion](CloudPoint.md#rotationquaternion)
- [translateFromPivot](CloudPoint.md#translatefrompivot)
- [uv](CloudPoint.md#uv)
- [velocity](CloudPoint.md#velocity)

### Accessors

- [quaternion](CloudPoint.md#quaternion)
- [size](CloudPoint.md#size)

### Methods

- [intersectsMesh](CloudPoint.md#intersectsmesh)

## Constructors

### constructor

• **new CloudPoint**(`particleIndex`, `group`, `groupId`, `idxInGroup`, `pcs`)

Creates a Point Cloud object.
Don't create particles manually, use instead the PCS internal tools like _addParticle()

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particleIndex` | `number` | (integer) is the particle index in the PCS pool. It's also the particle identifier. |
| `group` | [`PointsGroup`](PointsGroup.md) | (PointsGroup) is the group the particle belongs to |
| `groupId` | `number` | (integer) is the group identifier in the PCS. |
| `idxInGroup` | `number` | (integer) is the index of the particle in the current point group (ex: the 10th point of addPoints(30)) |
| `pcs` | [`PointsCloudSystem`](PointsCloudSystem.md) | defines the PCS it is associated to |

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:105

## Properties

### \_group

• **\_group**: [`PointsGroup`](PointsGroup.md)

Group this particle belongs to

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:61

___

### color

• **color**: [`Nullable`](../modules.md#nullable)[`Color4`](Color4.md)

The color of the particle

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:18

___

### groupId

• **groupId**: `number` = `0`

Group id of this particle

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:65

___

### idx

• **idx**: `number` = `0`

particle global index

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:14

___

### idxInGroup

• **idxInGroup**: `number` = `0`

Index of the particle in its group id (Internal use)

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:69

___

### parentId

• **parentId**: [`Nullable`](../modules.md#nullable)`number` = `null`

Parent particle Id, if any.
Default null.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:90

___

### pivot

• **pivot**: [`Vector3`](Vector3.md)

The pivot point in the particle local space.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:42

___

### position

• **position**: [`Vector3`](Vector3.md)

The world space position of the particle.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:22

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

The world space rotation of the particle. (Not use if rotationQuaternion is set)

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:26

___

### rotationQuaternion

• **rotationQuaternion**: [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

The world space rotation quaternion of the particle.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:30

___

### translateFromPivot

• **translateFromPivot**: `boolean` = `false`

Must the particle be translated from its pivot point in its local space ?
In this case, the pivot point is set at the origin of the particle local space and the particle is translated.
Default : false

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:48

___

### uv

• **uv**: [`Nullable`](../modules.md#nullable)[`Vector2`](Vector2.md)

The uv of the particle.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:34

___

### velocity

• **velocity**: [`Vector3`](Vector3.md)

The current speed of the particle.

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:38

## Accessors

### quaternion

• `get` **quaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Legacy support, changed quaternion to rotationQuaternion

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:130

• `set` **quaternion**(`q`): `void`

Legacy support, changed quaternion to rotationQuaternion

#### Parameters

| Name | Type |
| :------ | :------ |
| `q` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:137

___

### size

• `get` **size**(): [`Vector3`](Vector3.md)

get point size

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:116

• `set` **size**(`scale`): `void`

Set point size

#### Parameters

| Name | Type |
| :------ | :------ |
| `scale` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:123

## Methods

### intersectsMesh

▸ **intersectsMesh**(`target`, `isSphere`): `boolean`

Returns a boolean. True if the particle intersects a mesh, else false
The intersection is computed on the particle position and Axis Aligned Bounding Box (AABB) or Sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Mesh`](Mesh.md) | is the object (point or mesh) what the intersection is computed against |
| `isSphere` | `boolean` | is boolean flag when false (default) bounding box of mesh is used, when true the bounding sphere is used |

#### Returns

`boolean`

true if it intersects

#### Defined in

packages/dev/core/src/Particles/cloudPoint.ts:148

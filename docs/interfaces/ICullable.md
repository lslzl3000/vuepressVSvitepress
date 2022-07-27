[@dev/core](../README.md) / [Exports](../modules.md) / ICullable

# Interface: ICullable

Interface for cullable objects

**`See`**

https://doc.babylonjs.com/babylon101/materials#back-face-culling

## Implemented by

- [`AbstractMesh`](../classes/AbstractMesh.md)
- [`BoundingBox`](../classes/BoundingBox.md)
- [`BoundingInfo`](../classes/BoundingInfo.md)
- [`SubMesh`](../classes/SubMesh.md)

## Table of contents

### Methods

- [isCompletelyInFrustum](ICullable.md#iscompletelyinfrustum)
- [isInFrustum](ICullable.md#isinfrustum)

## Methods

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`frustumPlanes`): `boolean`

Checks if a cullable object (mesh...) is in the camera frustum
Unlike isInFrustum this checks the full bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](../classes/Plane.md)[] | Camera near/planes |

#### Returns

`boolean`

true if the object is in frustum otherwise false

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingInfo.ts:49

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

Checks if the object or part of the object is in the frustum

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](../classes/Plane.md)[] | Camera near/planes |

#### Returns

`boolean`

true if the object is in frustum otherwise false

#### Defined in

https://github.com/babylon.js/core/src/Culling/boundingInfo.ts:42

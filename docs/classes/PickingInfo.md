[@dev/core](../README.md) / [Exports](../modules.md) / PickingInfo

# Class: PickingInfo

Information about the result of picking within a scene

**`See`**

https://doc.babylonjs.com/divingDeeper/mesh/interactions/picking_collisions

## Table of contents

### Constructors

- [constructor](PickingInfo.md#constructor)

### Properties

- [aimTransform](PickingInfo.md#aimtransform)
- [bu](PickingInfo.md#bu)
- [bv](PickingInfo.md#bv)
- [distance](PickingInfo.md#distance)
- [faceId](PickingInfo.md#faceid)
- [gripTransform](PickingInfo.md#griptransform)
- [hit](PickingInfo.md#hit)
- [originMesh](PickingInfo.md#originmesh)
- [pickedMesh](PickingInfo.md#pickedmesh)
- [pickedPoint](PickingInfo.md#pickedpoint)
- [pickedSprite](PickingInfo.md#pickedsprite)
- [ray](PickingInfo.md#ray)
- [subMeshFaceId](PickingInfo.md#submeshfaceid)
- [subMeshId](PickingInfo.md#submeshid)
- [thinInstanceIndex](PickingInfo.md#thininstanceindex)

### Methods

- [getNormal](PickingInfo.md#getnormal)
- [getTextureCoordinates](PickingInfo.md#gettexturecoordinates)

## Constructors

### constructor

• **new PickingInfo**()

## Properties

### aimTransform

• **aimTransform**: [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) = `null`

The aim-space transform of the input used for picking, if it is an XR input source.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:59

___

### bu

• **bu**: `number` = `0`

(See getTextureCoordinates) The barycentric U coordinate that is used when calculating the texture coordinates of the collision.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:35

___

### bv

• **bv**: `number` = `0`

(See getTextureCoordinates) The barycentric V coordinate that is used when calculating the texture coordinates of the collision.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:37

___

### distance

• **distance**: `number` = `0`

Distance away where the pick collided

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:25

___

### faceId

• **faceId**: `number` = `-1`

The index of the face on the mesh that was picked, or the index of the Line if the picked Mesh is a LinesMesh

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:39

___

### gripTransform

• **gripTransform**: [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) = `null`

The grip-space transform of the input used for picking, if it is an XR input source.
Some XR sources, such as input coming from head mounted displays, do not have this.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:64

___

### hit

• **hit**: `boolean` = `false`

If the pick collided with an object

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:21

___

### originMesh

• **originMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

If a mesh was used to do the picking (eg. 6dof controller) as a "near interaction", this will be populated.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:55

___

### pickedMesh

• **pickedMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

The mesh corresponding the the pick collision

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:33

___

### pickedPoint

• **pickedPoint**: [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) = `null`

The location of pick collision

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:29

___

### pickedSprite

• **pickedSprite**: [`Nullable`](../modules.md#nullable)[`Sprite`](Sprite.md) = `null`

If a sprite was picked, this will be the sprite the pick collided with

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:45

___

### ray

• **ray**: [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md) = `null`

The ray that was used to perform the picking.

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:51

___

### subMeshFaceId

• **subMeshFaceId**: `number` = `-1`

The index of the face on the subMesh that was picked, or the index of the Line if the picked Mesh is a LinesMesh

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:41

___

### subMeshId

• **subMeshId**: `number` = `0`

Id of the the submesh that was picked

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:43

___

### thinInstanceIndex

• **thinInstanceIndex**: `number` = `-1`

If we are picking a mesh with thin instance, this will give you the picked thin instance

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:47

## Methods

### getNormal

▸ **getNormal**(`useWorldCoordinates?`, `useVerticesNormals?`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the normal corresponding to the face the pick collided with

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `useWorldCoordinates` | `boolean` | `false` | If the resulting normal should be relative to the world (default: false) |
| `useVerticesNormals` | `boolean` | `true` | If the vertices normals should be used to calculate the normal instead of the normal map |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

The normal corresponding to the face the pick collided with

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:72

___

### getTextureCoordinates

▸ **getTextureCoordinates**(): [`Nullable`](../modules.md#nullable)[`Vector2`](Vector2.md)

Gets the texture coordinates of where the pick occurred

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector2`](Vector2.md)

the vector containing the coordinates of the texture

#### Defined in

https://github.com/babylon.js/core/src/Collisions/pickingInfo.ts:135

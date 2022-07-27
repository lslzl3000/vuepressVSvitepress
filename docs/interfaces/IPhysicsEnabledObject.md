[@dev/core](../README.md) / [Exports](../modules.md) / IPhysicsEnabledObject

# Interface: IPhysicsEnabledObject

Interface for a physics-enabled object

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Table of contents

### Properties

- [parent](IPhysicsEnabledObject.md#parent)
- [position](IPhysicsEnabledObject.md#position)
- [rotation](IPhysicsEnabledObject.md#rotation)
- [rotationQuaternion](IPhysicsEnabledObject.md#rotationquaternion)
- [scaling](IPhysicsEnabledObject.md#scaling)

### Methods

- [computeWorldMatrix](IPhysicsEnabledObject.md#computeworldmatrix)
- [getAbsolutePivotPoint](IPhysicsEnabledObject.md#getabsolutepivotpoint)
- [getAbsolutePosition](IPhysicsEnabledObject.md#getabsoluteposition)
- [getBoundingInfo](IPhysicsEnabledObject.md#getboundinginfo)
- [getChildMeshes](IPhysicsEnabledObject.md#getchildmeshes)
- [getClassName](IPhysicsEnabledObject.md#getclassname)
- [getIndices](IPhysicsEnabledObject.md#getindices)
- [getScene](IPhysicsEnabledObject.md#getscene)
- [getVerticesData](IPhysicsEnabledObject.md#getverticesdata)
- [getWorldMatrix](IPhysicsEnabledObject.md#getworldmatrix)
- [rotate](IPhysicsEnabledObject.md#rotate)
- [setAbsolutePosition](IPhysicsEnabledObject.md#setabsoluteposition)
- [translate](IPhysicsEnabledObject.md#translate)

## Properties

### parent

• `Optional` **parent**: `any`

The parent of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:110

___

### position

• **position**: [`Vector3`](../classes/Vector3.md)

The position of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:94

___

### rotation

• `Optional` **rotation**: [`Vector3`](../classes/Vector3.md)

The rotation of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:106

___

### rotationQuaternion

• **rotationQuaternion**: [`Nullable`](../modules.md#nullable)[`Quaternion`](../classes/Quaternion.md)

The rotation of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:98

___

### scaling

• **scaling**: [`Vector3`](../classes/Vector3.md)

The scale of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:102

## Methods

### computeWorldMatrix

▸ **computeWorldMatrix**(`force`): [`Matrix`](../classes/Matrix.md)

Computes the world matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force` | `boolean` | Specifies if the world matrix should be computed by force |

#### Returns

[`Matrix`](../classes/Matrix.md)

A world matrix

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:121

___

### getAbsolutePivotPoint

▸ **getAbsolutePivotPoint**(): [`Vector3`](../classes/Vector3.md)

Gets the absolute pivot point from the mesh

#### Returns

[`Vector3`](../classes/Vector3.md)

the absolute pivot point

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:158

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](../classes/Vector3.md)

Gets the absolute position from the mesh

#### Returns

[`Vector3`](../classes/Vector3.md)

the absolute position

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:153

___

### getBoundingInfo

▸ **getBoundingInfo**(): [`BoundingInfo`](../classes/BoundingInfo.md)

The bounding info of the physics-enabled object

#### Returns

[`BoundingInfo`](../classes/BoundingInfo.md)

The bounding info of the physics-enabled object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:115

___

### getChildMeshes

▸ `Optional` **getChildMeshes**(`directDescendantsOnly?`): [`AbstractMesh`](../classes/AbstractMesh.md)[]

Gets the child meshes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | Specifies if only direct-descendants should be obtained |

#### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)[]

An array of abstract meshes

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:132

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the mesh

#### Returns

`string`

The class name

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:185

___

### getIndices

▸ `Optional` **getIndices**(): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Gets the indices from the mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

A nullable array of index arrays

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:143

___

### getScene

▸ `Optional` **getScene**(): [`Scene`](../classes/Scene.md)

Gets the scene from the mesh

#### Returns

[`Scene`](../classes/Scene.md)

the indices array or null

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:148

___

### getVerticesData

▸ **getVerticesData**(`kind`): [`Nullable`](../modules.md#nullable)`number`[] \| `Float32Array`

Gets the vertex data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | The type of vertex data |

#### Returns

[`Nullable`](../modules.md#nullable)`number`[] \| `Float32Array`

A nullable array of numbers, or a float32 array

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:138

___

### getWorldMatrix

▸ `Optional` **getWorldMatrix**(): [`Matrix`](../classes/Matrix.md)

Gets the world matrix

#### Returns

[`Matrix`](../classes/Matrix.md)

A world matrix

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:126

___

### rotate

▸ **rotate**(`axis`, `amount`, `space?`): [`TransformNode`](../classes/TransformNode.md)

Rotates the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](../classes/Vector3.md) | The axis of rotation |
| `amount` | `number` | The amount of rotation |
| `space?` | [`Space`](../enums/Space.md) | The space of the rotation |

#### Returns

[`TransformNode`](../classes/TransformNode.md)

The rotation transform node

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:166

___

### setAbsolutePosition

▸ **setAbsolutePosition**(`absolutePosition`): [`TransformNode`](../classes/TransformNode.md)

Sets the absolute position of the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `absolutePosition` | [`Vector3`](../classes/Vector3.md) | The absolute position of the mesh |

#### Returns

[`TransformNode`](../classes/TransformNode.md)

The transform node

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:180

___

### translate

▸ **translate**(`axis`, `distance`, `space?`): [`TransformNode`](../classes/TransformNode.md)

Translates the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](../classes/Vector3.md) | The axis of translation |
| `distance` | `number` | The distance of translation |
| `space?` | [`Space`](../enums/Space.md) | The space of the translation |

#### Returns

[`TransformNode`](../classes/TransformNode.md)

The transform node

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:174

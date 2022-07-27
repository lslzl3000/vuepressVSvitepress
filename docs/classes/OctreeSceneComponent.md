[@dev/core](../README.md) / [Exports](../modules.md) / OctreeSceneComponent

# Class: OctreeSceneComponent

Defines the octree scene component responsible to manage any octrees
in a given scene.

## Table of contents

### Constructors

- [constructor](OctreeSceneComponent.md#constructor)

### Properties

- [\_tempRay](OctreeSceneComponent.md#_tempray)
- [checksIsEnabled](OctreeSceneComponent.md#checksisenabled)
- [name](OctreeSceneComponent.md#name)
- [scene](OctreeSceneComponent.md#scene)

### Methods

- [dispose](OctreeSceneComponent.md#dispose)
- [getActiveMeshCandidates](OctreeSceneComponent.md#getactivemeshcandidates)
- [getActiveSubMeshCandidates](OctreeSceneComponent.md#getactivesubmeshcandidates)
- [getCollidingSubMeshCandidates](OctreeSceneComponent.md#getcollidingsubmeshcandidates)
- [getIntersectingSubMeshCandidates](OctreeSceneComponent.md#getintersectingsubmeshcandidates)
- [rebuild](OctreeSceneComponent.md#rebuild)
- [register](OctreeSceneComponent.md#register)

## Constructors

### constructor

• **new OctreeSceneComponent**(`scene?`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:143

## Properties

### \_tempRay

• `Private` **\_tempRay**: [`Ray`](Ray.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:205

___

### checksIsEnabled

• `Readonly` **checksIsEnabled**: ``true``

Indicates if the meshes have been checked to make sure they are isEnabled()

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:137

___

### name

• `Readonly` **name**: ``"Octree"``

The component name help to identify the component in the list of scene components.

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:127

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:132

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:249

___

### getActiveMeshCandidates

▸ **getActiveMeshCandidates**(): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

Return the list of active meshes

#### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

the list of active meshes

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:184

___

### getActiveSubMeshCandidates

▸ **getActiveSubMeshCandidates**(`mesh`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Return the list of active sub meshes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to get the candidates sub meshes from |

#### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

the list of active sub meshes

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:197

___

### getCollidingSubMeshCandidates

▸ **getCollidingSubMeshCandidates**(`mesh`, `collider`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Return the list of sub meshes colliding with a collider

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to find the submesh for |
| `collider` | `Collider` | defines the collider to evaluate the collision against |

#### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

the list of colliding sub meshes

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:228

___

### getIntersectingSubMeshCandidates

▸ **getIntersectingSubMeshCandidates**(`mesh`, `localRay`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Return the list of sub meshes intersecting with a given local ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to find the submesh for |
| `localRay` | [`Ray`](Ray.md) | defines the ray in local space |

#### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

the list of intersecting sub meshes

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:212

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:242

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:160

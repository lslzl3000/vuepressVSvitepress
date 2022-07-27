[@dev/core](../README.md) / [Exports](../modules.md) / AttachToBoxBehavior

# Class: AttachToBoxBehavior

A behavior that when attached to a mesh will will place a specified node on the meshes face pointing towards the camera

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`Mesh`](Mesh.md)

## Table of contents

### Constructors

- [constructor](AttachToBoxBehavior.md#constructor)

### Properties

- [\_faceVectors](AttachToBoxBehavior.md#_facevectors)
- [\_lookAtTmpMatrix](AttachToBoxBehavior.md#_lookattmpmatrix)
- [\_onRenderObserver](AttachToBoxBehavior.md#_onrenderobserver)
- [\_scene](AttachToBoxBehavior.md#_scene)
- [\_target](AttachToBoxBehavior.md#_target)
- [\_tmpMatrix](AttachToBoxBehavior.md#_tmpmatrix)
- [\_tmpVector](AttachToBoxBehavior.md#_tmpvector)
- [\_zeroVector](AttachToBoxBehavior.md#_zerovector)
- [distanceAwayFromBottomOfFace](AttachToBoxBehavior.md#distanceawayfrombottomofface)
- [distanceAwayFromFace](AttachToBoxBehavior.md#distanceawayfromface)
- [name](AttachToBoxBehavior.md#name)

### Methods

- [\_closestFace](AttachToBoxBehavior.md#_closestface)
- [\_lookAtToRef](AttachToBoxBehavior.md#_lookattoref)
- [attach](AttachToBoxBehavior.md#attach)
- [detach](AttachToBoxBehavior.md#detach)
- [init](AttachToBoxBehavior.md#init)

## Constructors

### constructor

• **new AttachToBoxBehavior**(`_ui`)

Creates the AttachToBoxBehavior, used to attach UI to the closest face of the box to a camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_ui` | [`TransformNode`](TransformNode.md) | The transform node that should be attached to the mesh |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:50

## Properties

### \_faceVectors

• `Private` **\_faceVectors**: `FaceDirectionInfo`[]

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:32

___

### \_lookAtTmpMatrix

• `Private` **\_lookAtTmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:84

___

### \_onRenderObserver

• `Private` **\_onRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:42

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:41

___

### \_target

• `Private` **\_target**: [`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:40

___

### \_tmpMatrix

• `Private` **\_tmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:43

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:44

___

### \_zeroVector

• `Private` **\_zeroVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:83

___

### distanceAwayFromBottomOfFace

• **distanceAwayFromBottomOfFace**: `number` = `0.15`

The distance from the bottom of the face that the UI should be attached to (default: 0.15)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:31

___

### distanceAwayFromFace

• **distanceAwayFromFace**: `number` = `0.15`

The distance away from the face of the mesh that the UI should be attached to (default: 0.15)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:27

___

### name

• **name**: `string` = `"AttachToBoxBehavior"`

The name of the behavior

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:23

## Methods

### \_closestFace

▸ `Private` **_closestFace**(`targetDirection`): `FaceDirectionInfo`

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetDirection` | [`Vector3`](Vector3.md) |

#### Returns

`FaceDirectionInfo`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:61

___

### \_lookAtToRef

▸ `Private` **_lookAtToRef**(`pos`, `up?`, `ref`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pos` | [`Vector3`](Vector3.md) |
| `up` | [`Vector3`](Vector3.md) |
| `ref` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:85

___

### attach

▸ **attach**(`target`): `void`

Attaches the AttachToBoxBehavior to the passed in mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Mesh`](Mesh.md) | The mesh that the specified node will be attached to |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:95

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:176

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/attachToBoxBehavior.ts:57

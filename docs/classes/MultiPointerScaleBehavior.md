[@dev/core](../README.md) / [Exports](../modules.md) / MultiPointerScaleBehavior

# Class: MultiPointerScaleBehavior

A behavior that when attached to a mesh will allow the mesh to be scaled

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`Mesh`](Mesh.md)

## Table of contents

### Constructors

- [constructor](MultiPointerScaleBehavior.md#constructor)

### Properties

- [\_dragBehaviorA](MultiPointerScaleBehavior.md#_dragbehaviora)
- [\_dragBehaviorB](MultiPointerScaleBehavior.md#_dragbehaviorb)
- [\_initialScale](MultiPointerScaleBehavior.md#_initialscale)
- [\_ownerNode](MultiPointerScaleBehavior.md#_ownernode)
- [\_sceneRenderObserver](MultiPointerScaleBehavior.md#_scenerenderobserver)
- [\_startDistance](MultiPointerScaleBehavior.md#_startdistance)
- [\_targetScale](MultiPointerScaleBehavior.md#_targetscale)

### Accessors

- [name](MultiPointerScaleBehavior.md#name)

### Methods

- [\_getCurrentDistance](MultiPointerScaleBehavior.md#_getcurrentdistance)
- [attach](MultiPointerScaleBehavior.md#attach)
- [detach](MultiPointerScaleBehavior.md#detach)
- [init](MultiPointerScaleBehavior.md#init)

## Constructors

### constructor

• **new MultiPointerScaleBehavior**()

Instantiate a new behavior that when attached to a mesh will allow the mesh to be scaled

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:24

## Properties

### \_dragBehaviorA

• `Private` **\_dragBehaviorA**: [`PointerDragBehavior`](PointerDragBehavior.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:13

___

### \_dragBehaviorB

• `Private` **\_dragBehaviorB**: [`PointerDragBehavior`](PointerDragBehavior.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:14

___

### \_initialScale

• `Private` **\_initialScale**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:16

___

### \_ownerNode

• `Private` **\_ownerNode**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:18

___

### \_sceneRenderObserver

• `Private` **\_sceneRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:19

___

### \_startDistance

• `Private` **\_startDistance**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:15

___

### \_targetScale

• `Private` **\_targetScale**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:17

## Accessors

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:34

## Methods

### \_getCurrentDistance

▸ `Private` **_getCurrentDistance**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:43

___

### attach

▸ **attach**(`ownerNode`): `void`

Attaches the scale behavior the passed in mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`Mesh`](Mesh.md) | The mesh that will be scaled around once attached |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:51

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:102

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/multiPointerScaleBehavior.ts:41

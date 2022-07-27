[@dev/core](../README.md) / [Exports](../modules.md) / SixDofDragBehavior

# Class: SixDofDragBehavior

A behavior that when attached to a mesh will allow the mesh to be dragged around based on directions and origin of the pointer's ray

## Hierarchy

- [`BaseSixDofDragBehavior`](BaseSixDofDragBehavior.md)

  ↳ **`SixDofDragBehavior`**

## Table of contents

### Constructors

- [constructor](SixDofDragBehavior.md#constructor)

### Properties

- [\_dragType](SixDofDragBehavior.md#_dragtype)
- [\_dragging](SixDofDragBehavior.md#_dragging)
- [\_moving](SixDofDragBehavior.md#_moving)
- [\_ownerNode](SixDofDragBehavior.md#_ownernode)
- [\_scene](SixDofDragBehavior.md#_scene)
- [\_sceneRenderObserver](SixDofDragBehavior.md#_scenerenderobserver)
- [\_startingOrientation](SixDofDragBehavior.md#_startingorientation)
- [\_startingPosition](SixDofDragBehavior.md#_startingposition)
- [\_startingScaling](SixDofDragBehavior.md#_startingscaling)
- [\_targetOrientation](SixDofDragBehavior.md#_targetorientation)
- [\_targetPosition](SixDofDragBehavior.md#_targetposition)
- [\_targetScaling](SixDofDragBehavior.md#_targetscaling)
- [\_virtualMeshesInfo](SixDofDragBehavior.md#_virtualmeshesinfo)
- [\_virtualTransformNode](SixDofDragBehavior.md#_virtualtransformnode)
- [allowMultiPointer](SixDofDragBehavior.md#allowmultipointer)
- [currentDraggingPointerIds](SixDofDragBehavior.md#currentdraggingpointerids)
- [detachCameraControls](SixDofDragBehavior.md#detachcameracontrols)
- [disableMovement](SixDofDragBehavior.md#disablemovement)
- [dragDeltaRatio](SixDofDragBehavior.md#dragdeltaratio)
- [draggableMeshes](SixDofDragBehavior.md#draggablemeshes)
- [faceCameraOnDragStart](SixDofDragBehavior.md#facecameraondragstart)
- [onDragEndObservable](SixDofDragBehavior.md#ondragendobservable)
- [onDragObservable](SixDofDragBehavior.md#ondragobservable)
- [onDragStartObservable](SixDofDragBehavior.md#ondragstartobservable)
- [onPositionChangedObservable](SixDofDragBehavior.md#onpositionchangedobservable)
- [rotateAroundYOnly](SixDofDragBehavior.md#rotatearoundyonly)
- [rotateDraggedObject](SixDofDragBehavior.md#rotatedraggedobject)
- [rotateWithMotionController](SixDofDragBehavior.md#rotatewithmotioncontroller)
- [zDragFactor](SixDofDragBehavior.md#zdragfactor)
- [\_virtualScene](SixDofDragBehavior.md#_virtualscene)

### Accessors

- [\_pointerCamera](SixDofDragBehavior.md#_pointercamera)
- [currentDraggingPointerID](SixDofDragBehavior.md#currentdraggingpointerid)
- [currentDraggingPointerId](SixDofDragBehavior.md#currentdraggingpointerid-1)
- [isMoving](SixDofDragBehavior.md#ismoving)
- [name](SixDofDragBehavior.md#name)

### Methods

- [\_getPositionOffsetAround](SixDofDragBehavior.md#_getpositionoffsetaround)
- [\_onePointerPositionUpdated](SixDofDragBehavior.md#_onepointerpositionupdated)
- [\_resetVirtualMeshesPosition](SixDofDragBehavior.md#_resetvirtualmeshesposition)
- [\_targetDrag](SixDofDragBehavior.md#_targetdrag)
- [\_targetDragEnd](SixDofDragBehavior.md#_targetdragend)
- [\_targetDragStart](SixDofDragBehavior.md#_targetdragstart)
- [\_twoPointersPositionUpdated](SixDofDragBehavior.md#_twopointerspositionupdated)
- [attach](SixDofDragBehavior.md#attach)
- [detach](SixDofDragBehavior.md#detach)
- [init](SixDofDragBehavior.md#init)

## Constructors

### constructor

• **new SixDofDragBehavior**()

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[constructor](BaseSixDofDragBehavior.md#constructor)

## Properties

### \_dragType

• `Protected` **\_dragType**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `DRAG` | `number` |
| `DRAG_WITH_CONTROLLER` | `number` |
| `NEAR_DRAG` | `number` |
| `NONE` | `number` |

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_dragType](BaseSixDofDragBehavior.md#_dragtype)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:52

___

### \_dragging

• `Protected` **\_dragging**: `number`

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_dragging](BaseSixDofDragBehavior.md#_dragging)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:62

___

### \_moving

• `Protected` **\_moving**: `boolean` = `false`

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_moving](BaseSixDofDragBehavior.md#_moving)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:60

___

### \_ownerNode

• `Protected` **\_ownerNode**: [`TransformNode`](TransformNode.md)

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_ownerNode](BaseSixDofDragBehavior.md#_ownernode)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:61

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_scene](BaseSixDofDragBehavior.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:59

___

### \_sceneRenderObserver

• `Private` **\_sceneRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:15

___

### \_startingOrientation

• `Protected` **\_startingOrientation**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:22

___

### \_startingPosition

• `Protected` **\_startingPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:21

___

### \_startingScaling

• `Protected` **\_startingScaling**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:23

___

### \_targetOrientation

• `Protected` **\_targetOrientation**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:19

___

### \_targetPosition

• `Protected` **\_targetPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:18

___

### \_targetScaling

• `Protected` **\_targetScaling**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:20

___

### \_virtualMeshesInfo

• `Protected` **\_virtualMeshesInfo**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: `VirtualMeshInfo`

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_virtualMeshesInfo](BaseSixDofDragBehavior.md#_virtualmeshesinfo)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:45

___

### \_virtualTransformNode

• `Private` **\_virtualTransformNode**: [`TransformNode`](TransformNode.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:16

___

### allowMultiPointer

• **allowMultiPointer**: `boolean` = `true`

Should the behavior allow simultaneous pointers to interact with the owner node.

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[allowMultiPointer](BaseSixDofDragBehavior.md#allowmultipointer)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:125

___

### currentDraggingPointerIds

• **currentDraggingPointerIds**: `number`[] = `[]`

In case of multipointer interaction, all pointer ids currently active are stored here

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[currentDraggingPointerIds](BaseSixDofDragBehavior.md#currentdraggingpointerids)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:91

___

### detachCameraControls

• **detachCameraControls**: `boolean` = `true`

/**
 * If camera controls should be detached during the drag

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[detachCameraControls](BaseSixDofDragBehavior.md#detachcameracontrols)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:107

___

### disableMovement

• **disableMovement**: `boolean` = `false`

Use this flag to update the target but not move the owner node towards the target

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:60

___

### dragDeltaRatio

• **dragDeltaRatio**: `number` = `0.2`

The distance towards the target drag position to move each frame. This can be useful to avoid jitter. Set this to 1 for no delay. (Default: 0.2)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:33

___

### draggableMeshes

• **draggableMeshes**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] = `null`

The list of child meshes that can receive drag events
If `null`, all child meshes will receive drag event

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[draggableMeshes](BaseSixDofDragBehavior.md#draggablemeshes)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:68

___

### faceCameraOnDragStart

• **faceCameraOnDragStart**: `boolean` = `false`

Should the object rotate towards the camera when we start dragging it

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:65

___

### onDragEndObservable

• **onDragEndObservable**: [`Observable`](Observable.md){}

Fires each time a drag ends (eg. mouse release after drag)

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[onDragEndObservable](BaseSixDofDragBehavior.md#ondragendobservable)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:120

___

### onDragObservable

• **onDragObservable**: [`Observable`](Observable.md){ `delta`: [`Vector3`](Vector3.md) ; `pickInfo`: [`PickingInfo`](PickingInfo.md) ; `position`: [`Vector3`](Vector3.md)  }

Fires each time a drag happens

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[onDragObservable](BaseSixDofDragBehavior.md#ondragobservable)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:116

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md){ `position`: [`Vector3`](Vector3.md)  }

Fires each time a drag starts

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[onDragStartObservable](BaseSixDofDragBehavior.md#ondragstartobservable)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:112

___

### onPositionChangedObservable

• **onPositionChangedObservable**: [`Observable`](Observable.md){ `position`: [`Vector3`](Vector3.md)  }

Fires when position is updated

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:28

___

### rotateAroundYOnly

• **rotateAroundYOnly**: `boolean` = `false`

If `rotateDraggedObject` is set to `true`, this parameter determines if we are only rotating around the y axis (yaw)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:43

___

### rotateDraggedObject

• **rotateDraggedObject**: `boolean` = `true`

If the object should rotate to face the drag origin

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:38

___

### rotateWithMotionController

• **rotateWithMotionController**: `boolean` = `true`

Should the behavior rotate 1:1 with the motion controller, when one is used.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:48

___

### zDragFactor

• **zDragFactor**: `number` = `3`

How much faster the object should move when the controller is moving towards it. This is useful to bring objects that are far away from the user to them faster. Set this to 0 to avoid any speed increase. (Default: 3)

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[zDragFactor](BaseSixDofDragBehavior.md#zdragfactor)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:73

___

### \_virtualScene

▪ `Static` `Protected` **\_virtualScene**: [`Scene`](Scene.md)

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_virtualScene](BaseSixDofDragBehavior.md#_virtualscene)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:42

## Accessors

### \_pointerCamera

• `Private` `get` **_pointerCamera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

In the case of multiple active cameras, the cameraToUseForPointers should be used if set instead of active camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Inherited from

BaseSixDofDragBehavior.\_pointerCamera

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:149

___

### currentDraggingPointerID

• `get` **currentDraggingPointerID**(): `number`

Get or set the currentDraggingPointerId

**`Deprecated`**

Please use currentDraggingPointerId instead

#### Returns

`number`

#### Inherited from

BaseSixDofDragBehavior.currentDraggingPointerID

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:97

• `set` **currentDraggingPointerID**(`currentDraggingPointerID`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentDraggingPointerID` | `number` |

#### Returns

`void`

#### Inherited from

BaseSixDofDragBehavior.currentDraggingPointerID

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:100

___

### currentDraggingPointerId

• `get` **currentDraggingPointerId**(): `number`

The id of the pointer that is currently interacting with the behavior (-1 when no pointer is active)

#### Returns

`number`

#### Inherited from

BaseSixDofDragBehavior.currentDraggingPointerId

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:77

• `set` **currentDraggingPointerId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseSixDofDragBehavior.currentDraggingPointerId

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:84

___

### isMoving

• `get` **isMoving**(): `boolean`

Returns true if the attached mesh is currently moving with this behavior

#### Returns

`boolean`

#### Inherited from

BaseSixDofDragBehavior.isMoving

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:137

___

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Overrides

BaseSixDofDragBehavior.name

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:53

## Methods

### \_getPositionOffsetAround

▸ `Private` **_getPositionOffsetAround**(`transformationLocalOrigin`, `scaling`, `rotation`): [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `transformationLocalOrigin` | [`Vector3`](Vector3.md) |
| `scaling` | `number` |
| `rotation` | [`Quaternion`](Quaternion.md) |

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:100

___

### \_onePointerPositionUpdated

▸ `Private` **_onePointerPositionUpdated**(`worldDeltaPosition`, `worldDeltaRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `worldDeltaPosition` | [`Vector3`](Vector3.md) |
| `worldDeltaRotation` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:118

___

### \_resetVirtualMeshesPosition

▸ `Protected` **_resetVirtualMeshesPosition**(): `void`

#### Returns

`void`

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_resetVirtualMeshesPosition](BaseSixDofDragBehavior.md#_resetvirtualmeshesposition)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:182

___

### \_targetDrag

▸ `Protected` **_targetDrag**(`worldDeltaPosition`, `worldDeltaRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `worldDeltaPosition` | [`Vector3`](Vector3.md) |
| `worldDeltaRotation` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Overrides

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_targetDrag](BaseSixDofDragBehavior.md#_targetdrag)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:220

___

### \_targetDragEnd

▸ `Protected` **_targetDragEnd**(): `void`

#### Returns

`void`

#### Overrides

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_targetDragEnd](BaseSixDofDragBehavior.md#_targetdragend)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:228

___

### \_targetDragStart

▸ `Protected` **_targetDragStart**(): `void`

#### Returns

`void`

#### Overrides

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[_targetDragStart](BaseSixDofDragBehavior.md#_targetdragstart)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:176

___

### \_twoPointersPositionUpdated

▸ `Private` **_twoPointersPositionUpdated**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:139

___

### attach

▸ **attach**(`ownerNode`): `void`

Attaches the six DoF drag behavior

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`Mesh`](Mesh.md) | The mesh that will be dragged around once attached |

#### Returns

`void`

#### Overrides

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[attach](BaseSixDofDragBehavior.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:71

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Overrides

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[detach](BaseSixDofDragBehavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/sixDofDragBehavior.ts:242

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Inherited from

[BaseSixDofDragBehavior](BaseSixDofDragBehavior.md).[init](BaseSixDofDragBehavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:144

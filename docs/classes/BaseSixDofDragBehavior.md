[@dev/core](../README.md) / [Exports](../modules.md) / BaseSixDofDragBehavior

# Class: BaseSixDofDragBehavior

Base behavior for six degrees of freedom interactions in XR experiences.
Creates virtual meshes that are dragged around
And observables for position/rotation changes

## Hierarchy

- **`BaseSixDofDragBehavior`**

  ↳ [`SixDofDragBehavior`](SixDofDragBehavior.md)

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`Mesh`](Mesh.md)

## Table of contents

### Constructors

- [constructor](BaseSixDofDragBehavior.md#constructor)

### Properties

- [\_attachedToElement](BaseSixDofDragBehavior.md#_attachedtoelement)
- [\_dragType](BaseSixDofDragBehavior.md#_dragtype)
- [\_dragging](BaseSixDofDragBehavior.md#_dragging)
- [\_moving](BaseSixDofDragBehavior.md#_moving)
- [\_ownerNode](BaseSixDofDragBehavior.md#_ownernode)
- [\_pointerObserver](BaseSixDofDragBehavior.md#_pointerobserver)
- [\_scene](BaseSixDofDragBehavior.md#_scene)
- [\_tmpQuaternion](BaseSixDofDragBehavior.md#_tmpquaternion)
- [\_tmpVector](BaseSixDofDragBehavior.md#_tmpvector)
- [\_virtualMeshesInfo](BaseSixDofDragBehavior.md#_virtualmeshesinfo)
- [allowMultiPointer](BaseSixDofDragBehavior.md#allowmultipointer)
- [currentDraggingPointerIds](BaseSixDofDragBehavior.md#currentdraggingpointerids)
- [detachCameraControls](BaseSixDofDragBehavior.md#detachcameracontrols)
- [draggableMeshes](BaseSixDofDragBehavior.md#draggablemeshes)
- [onDragEndObservable](BaseSixDofDragBehavior.md#ondragendobservable)
- [onDragObservable](BaseSixDofDragBehavior.md#ondragobservable)
- [onDragStartObservable](BaseSixDofDragBehavior.md#ondragstartobservable)
- [zDragFactor](BaseSixDofDragBehavior.md#zdragfactor)
- [\_virtualScene](BaseSixDofDragBehavior.md#_virtualscene)

### Accessors

- [\_pointerCamera](BaseSixDofDragBehavior.md#_pointercamera)
- [currentDraggingPointerID](BaseSixDofDragBehavior.md#currentdraggingpointerid)
- [currentDraggingPointerId](BaseSixDofDragBehavior.md#currentdraggingpointerid-1)
- [isMoving](BaseSixDofDragBehavior.md#ismoving)
- [name](BaseSixDofDragBehavior.md#name)

### Methods

- [\_applyZOffset](BaseSixDofDragBehavior.md#_applyzoffset)
- [\_createVirtualMeshInfo](BaseSixDofDragBehavior.md#_createvirtualmeshinfo)
- [\_pointerUpdate2D](BaseSixDofDragBehavior.md#_pointerupdate2d)
- [\_pointerUpdateXR](BaseSixDofDragBehavior.md#_pointerupdatexr)
- [\_resetVirtualMeshesPosition](BaseSixDofDragBehavior.md#_resetvirtualmeshesposition)
- [\_targetDrag](BaseSixDofDragBehavior.md#_targetdrag)
- [\_targetDragEnd](BaseSixDofDragBehavior.md#_targetdragend)
- [\_targetDragStart](BaseSixDofDragBehavior.md#_targetdragstart)
- [attach](BaseSixDofDragBehavior.md#attach)
- [detach](BaseSixDofDragBehavior.md#detach)
- [init](BaseSixDofDragBehavior.md#init)

## Constructors

### constructor

• **new BaseSixDofDragBehavior**()

## Properties

### \_attachedToElement

• `Private` **\_attachedToElement**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:44

___

### \_dragType

• `Protected` **\_dragType**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `DRAG` | `number` |
| `DRAG_WITH_CONTROLLER` | `number` |
| `NEAR_DRAG` | `number` |
| `NONE` | `number` |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:52

___

### \_dragging

• `Protected` **\_dragging**: `number`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:62

___

### \_moving

• `Protected` **\_moving**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:60

___

### \_ownerNode

• `Protected` **\_ownerNode**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:61

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:43

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:59

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:50

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:49

___

### \_virtualMeshesInfo

• `Protected` **\_virtualMeshesInfo**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: `VirtualMeshInfo`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:45

___

### allowMultiPointer

• **allowMultiPointer**: `boolean` = `true`

Should the behavior allow simultaneous pointers to interact with the owner node.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:125

___

### currentDraggingPointerIds

• **currentDraggingPointerIds**: `number`[] = `[]`

In case of multipointer interaction, all pointer ids currently active are stored here

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:91

___

### detachCameraControls

• **detachCameraControls**: `boolean` = `true`

/**
 * If camera controls should be detached during the drag

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:107

___

### draggableMeshes

• **draggableMeshes**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] = `null`

The list of child meshes that can receive drag events
If `null`, all child meshes will receive drag event

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:68

___

### onDragEndObservable

• **onDragEndObservable**: [`Observable`](Observable.md){}

Fires each time a drag ends (eg. mouse release after drag)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:120

___

### onDragObservable

• **onDragObservable**: [`Observable`](Observable.md){ `delta`: [`Vector3`](Vector3.md) ; `pickInfo`: [`PickingInfo`](PickingInfo.md) ; `position`: [`Vector3`](Vector3.md)  }

Fires each time a drag happens

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:116

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md){ `position`: [`Vector3`](Vector3.md)  }

Fires each time a drag starts

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:112

___

### zDragFactor

• **zDragFactor**: `number` = `3`

How much faster the object should move when the controller is moving towards it. This is useful to bring objects that are far away from the user to them faster. Set this to 0 to avoid any speed increase. (Default: 3)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:73

___

### \_virtualScene

▪ `Static` `Protected` **\_virtualScene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:42

## Accessors

### \_pointerCamera

• `Private` `get` **_pointerCamera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

In the case of multiple active cameras, the cameraToUseForPointers should be used if set instead of active camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:149

___

### currentDraggingPointerID

• `get` **currentDraggingPointerID**(): `number`

Get or set the currentDraggingPointerId

**`Deprecated`**

Please use currentDraggingPointerId instead

#### Returns

`number`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:97

• `set` **currentDraggingPointerID**(`currentDraggingPointerID`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentDraggingPointerID` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:100

___

### currentDraggingPointerId

• `get` **currentDraggingPointerId**(): `number`

The id of the pointer that is currently interacting with the behavior (-1 when no pointer is active)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:77

• `set` **currentDraggingPointerId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:84

___

### isMoving

• `get` **isMoving**(): `boolean`

Returns true if the attached mesh is currently moving with this behavior

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:137

___

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:130

## Methods

### \_applyZOffset

▸ `Private` **_applyZOffset**(`node`, `localOriginDragDifference`, `zDragFactor`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`TransformNode`](TransformNode.md) |
| `localOriginDragDifference` | `number` |
| `zDragFactor` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:444

___

### \_createVirtualMeshInfo

▸ `Private` **_createVirtualMeshInfo**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `dragMesh` | [`AbstractMesh`](AbstractMesh.md) |
| `dragging` | `boolean` |
| `lastDragPosition` | [`Vector3`](Vector3.md) |
| `lastOriginPosition` | [`Vector3`](Vector3.md) |
| `moving` | `boolean` |
| `originMesh` | [`AbstractMesh`](AbstractMesh.md) |
| `pivotMesh` | [`AbstractMesh`](AbstractMesh.md) |
| `startingOrientation` | [`Quaternion`](Quaternion.md) |
| `startingPivotOrientation` | [`Quaternion`](Quaternion.md) |
| `startingPivotPosition` | [`Vector3`](Vector3.md) |
| `startingPosition` | [`Vector3`](Vector3.md) |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:157

___

### \_pointerUpdate2D

▸ `Private` **_pointerUpdate2D**(`ray`, `pointerId`, `zDragFactor`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ray` | [`Ray`](Ray.md) |
| `pointerId` | `number` |
| `zDragFactor` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:199

___

### \_pointerUpdateXR

▸ `Private` **_pointerUpdateXR**(`controllerAimTransform`, `controllerGripTransform`, `pointerId`, `zDragFactor`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controllerAimTransform` | [`TransformNode`](TransformNode.md) |
| `controllerGripTransform` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) |
| `pointerId` | `number` |
| `zDragFactor` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:229

___

### \_resetVirtualMeshesPosition

▸ `Protected` **_resetVirtualMeshesPosition**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:182

___

### \_targetDrag

▸ `Protected` **_targetDrag**(`worldDeltaPosition`, `worldDeltaRotation`, `pointerId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `worldDeltaPosition` | [`Vector3`](Vector3.md) |
| `worldDeltaRotation` | [`Quaternion`](Quaternion.md) |
| `pointerId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:457

___

### \_targetDragEnd

▸ `Protected` **_targetDragEnd**(`pointerId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointerId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:461

___

### \_targetDragStart

▸ `Protected` **_targetDragStart**(`worldPosition`, `worldRotation`, `pointerId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `worldPosition` | [`Vector3`](Vector3.md) |
| `worldRotation` | [`Quaternion`](Quaternion.md) |
| `pointerId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:453

___

### attach

▸ **attach**(`ownerNode`): `void`

Attaches the scale behavior the passed in mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`TransformNode`](TransformNode.md) | The mesh that will be scaled around once attached |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:281

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:468

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/baseSixDofDragBehavior.ts:144

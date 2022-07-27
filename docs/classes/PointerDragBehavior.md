[@dev/core](../README.md) / [Exports](../modules.md) / PointerDragBehavior

# Class: PointerDragBehavior

A behavior that when attached to a mesh will allow the mesh to be dragged around the screen based on pointer events

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`AbstractMesh`](AbstractMesh.md)

## Table of contents

### Constructors

- [constructor](PointerDragBehavior.md#constructor)

### Properties

- [\_activeDragButton](PointerDragBehavior.md#_activedragbutton)
- [\_alternatePickedPoint](PointerDragBehavior.md#_alternatepickedpoint)
- [\_attachedToElement](PointerDragBehavior.md#_attachedtoelement)
- [\_beforeRenderObserver](PointerDragBehavior.md#_beforerenderobserver)
- [\_debugMode](PointerDragBehavior.md#_debugmode)
- [\_dragDelta](PointerDragBehavior.md#_dragdelta)
- [\_dragPlane](PointerDragBehavior.md#_dragplane)
- [\_enabled](PointerDragBehavior.md#_enabled)
- [\_lastPointerRay](PointerDragBehavior.md#_lastpointerray)
- [\_localAxis](PointerDragBehavior.md#_localaxis)
- [\_lookAt](PointerDragBehavior.md#_lookat)
- [\_moving](PointerDragBehavior.md#_moving)
- [\_options](PointerDragBehavior.md#_options)
- [\_pointA](PointerDragBehavior.md#_pointa)
- [\_pointC](PointerDragBehavior.md#_pointc)
- [\_pointerObserver](PointerDragBehavior.md#_pointerobserver)
- [\_scene](PointerDragBehavior.md#_scene)
- [\_startDragRay](PointerDragBehavior.md#_startdragray)
- [\_targetPosition](PointerDragBehavior.md#_targetposition)
- [\_tmpVector](PointerDragBehavior.md#_tmpvector)
- [\_useAlternatePickedPointAboveMaxDragAngleDragSpeed](PointerDragBehavior.md#_usealternatepickedpointabovemaxdragangledragspeed)
- [\_worldDragAxis](PointerDragBehavior.md#_worlddragaxis)
- [attachedNode](PointerDragBehavior.md#attachednode)
- [currentDraggingPointerId](PointerDragBehavior.md#currentdraggingpointerid)
- [detachCameraControls](PointerDragBehavior.md#detachcameracontrols)
- [dragButtons](PointerDragBehavior.md#dragbuttons)
- [dragDeltaRatio](PointerDragBehavior.md#dragdeltaratio)
- [dragging](PointerDragBehavior.md#dragging)
- [lastDragPosition](PointerDragBehavior.md#lastdragposition)
- [maxDragAngle](PointerDragBehavior.md#maxdragangle)
- [moveAttached](PointerDragBehavior.md#moveattached)
- [onDragEndObservable](PointerDragBehavior.md#ondragendobservable)
- [onDragObservable](PointerDragBehavior.md#ondragobservable)
- [onDragStartObservable](PointerDragBehavior.md#ondragstartobservable)
- [onEnabledObservable](PointerDragBehavior.md#onenabledobservable)
- [startAndReleaseDragOnPointerEvents](PointerDragBehavior.md#startandreleasedragonpointerevents)
- [updateDragPlane](PointerDragBehavior.md#updatedragplane)
- [useObjectOrientationForDragging](PointerDragBehavior.md#useobjectorientationfordragging)
- [\_AnyMouseId](PointerDragBehavior.md#_anymouseid)
- [\_PlaneScene](PointerDragBehavior.md#_planescene)

### Accessors

- [currentDraggingPointerID](PointerDragBehavior.md#currentdraggingpointerid-1)
- [enabled](PointerDragBehavior.md#enabled)
- [name](PointerDragBehavior.md#name)
- [options](PointerDragBehavior.md#options)

### Methods

- [\_moveDrag](PointerDragBehavior.md#_movedrag)
- [\_pickWithRayOnDragPlane](PointerDragBehavior.md#_pickwithrayondragplane)
- [\_startDrag](PointerDragBehavior.md#_startdrag)
- [\_updateDragPlanePosition](PointerDragBehavior.md#_updatedragplaneposition)
- [attach](PointerDragBehavior.md#attach)
- [detach](PointerDragBehavior.md#detach)
- [init](PointerDragBehavior.md#init)
- [releaseDrag](PointerDragBehavior.md#releasedrag)
- [startDrag](PointerDragBehavior.md#startdrag)
- [validateDrag](PointerDragBehavior.md#validatedrag)

## Constructors

### constructor

• **new PointerDragBehavior**(`options?`)

Creates a pointer drag behavior that can be attached to a mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Object` | The drag axis or normal of the plane that will be dragged across. If no options are specified the drag plane will always face the ray's origin (eg. camera) |
| `options.dragAxis?` | [`Vector3`](Vector3.md) |  |
| `options.dragPlaneNormal?` | [`Vector3`](Vector3.md) |  |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:156

## Properties

### \_activeDragButton

• `Private` **\_activeDragButton**: `number` = `-1`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:33

___

### \_alternatePickedPoint

• `Private` **\_alternatePickedPoint**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:193

___

### \_attachedToElement

• `Private` **\_attachedToElement**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:196

___

### \_beforeRenderObserver

• `Private` **\_beforeRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:30

___

### \_debugMode

• `Private` **\_debugMode**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:77

___

### \_dragDelta

• `Private` **\_dragDelta**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:411

___

### \_dragPlane

• `Private` **\_dragPlane**: [`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:27

___

### \_enabled

• `Private` **\_enabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:118

___

### \_lastPointerRay

• `Private` **\_lastPointerRay**: `Object` = `{}`

#### Index signature

▪ [key: `number`]: [`Ray`](Ray.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:351

___

### \_localAxis

• `Private` **\_localAxis**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:498

___

### \_lookAt

• `Private` **\_lookAt**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:499

___

### \_moving

• `Private` **\_moving**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:78

___

### \_options

• `Private` **\_options**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `dragAxis?` | [`Vector3`](Vector3.md) |
| `dragPlaneNormal?` | [`Vector3`](Vector3.md) |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:134

___

### \_pointA

• `Private` **\_pointA**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:496

___

### \_pointC

• `Private` **\_pointC**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:497

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:29

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:28

___

### \_startDragRay

• `Private` **\_startDragRay**: [`Ray`](Ray.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:350

___

### \_targetPosition

• `Private` **\_targetPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:195

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:192

___

### \_useAlternatePickedPointAboveMaxDragAngleDragSpeed

• `Private` **\_useAlternatePickedPointAboveMaxDragAngleDragSpeed**: `number` = `-1.1`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:32

___

### \_worldDragAxis

• `Private` **\_worldDragAxis**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:194

___

### attachedNode

• **attachedNode**: [`AbstractMesh`](AbstractMesh.md)

Abstract mesh the behavior is set on

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:26

___

### currentDraggingPointerId

• **currentDraggingPointerId**: `number` = `-1`

The id of the pointer that is currently interacting with the behavior (-1 when no pointer is active)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:59

___

### detachCameraControls

• **detachCameraControls**: `boolean` = `true`

If camera controls should be detached during the drag

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:127

___

### dragButtons

• **dragButtons**: `number`[]

Butttons that can be used to initiate a drag

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:41

___

### dragDeltaRatio

• **dragDeltaRatio**: `number` = `0.2`

The distance towards the target drag position to move each frame. This can be useful to avoid jitter. Set this to 1 for no delay. (Default: 0.2)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:71

___

### dragging

• **dragging**: `boolean` = `false`

If the behavior is currently in a dragging state

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:67

___

### lastDragPosition

• **lastDragPosition**: [`Vector3`](Vector3.md)

The last position where the pointer hit the drag plane in world space

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:63

___

### maxDragAngle

• **maxDragAngle**: `number` = `0`

The maximum tolerated angle between the drag plane and dragging pointer rays to trigger pointer events. Set to 0 to allow any angle (default: 0)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:37

___

### moveAttached

• **moveAttached**: `boolean` = `true`

If the attached mesh should be moved when dragged

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:103

___

### onDragEndObservable

• **onDragEndObservable**: [`Observable`](Observable.md){ `dragPlanePoint`: [`Vector3`](Vector3.md) ; `pointerId`: `number`  }

Fires each time a drag ends (eg. mouse release after drag)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:94

___

### onDragObservable

• **onDragObservable**: [`Observable`](Observable.md){ `delta`: [`Vector3`](Vector3.md) ; `dragDistance`: `number` ; `dragPlaneNormal`: [`Vector3`](Vector3.md) ; `dragPlanePoint`: [`Vector3`](Vector3.md) ; `pointerId`: `number`  }

Fires each time the attached mesh is dragged with the pointer
 * delta between last drag position and current drag position in world space
 * dragDistance along the drag axis
 * dragPlaneNormal normal of the current drag plane used during the drag
 * dragPlanePoint in world space where the drag intersects the drag plane

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:86

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md){ `dragPlanePoint`: [`Vector3`](Vector3.md) ; `pointerId`: `number`  }

Fires each time a drag begins (eg. mouse down on mesh)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:90

___

### onEnabledObservable

• **onEnabledObservable**: [`Observable`](Observable.md)`boolean`

Fires each time behavior enabled state changes

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:98

___

### startAndReleaseDragOnPointerEvents

• **startAndReleaseDragOnPointerEvents**: `boolean` = `true`

If pointer events should start and release the drag (Default: true)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:123

___

### updateDragPlane

• **updateDragPlane**: `boolean` = `true`

If the drag plane orientation should be updated during the dragging (Default: true)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:75

___

### useObjectOrientationForDragging

• **useObjectOrientationForDragging**: `boolean` = `true`

If set, the drag plane/axis will be rotated based on the attached mesh's world rotation (Default: true)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:132

___

### \_AnyMouseId

▪ `Static` `Private` **\_AnyMouseId**: `number` = `-2`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:22

___

### \_PlaneScene

▪ `Static` `Private` **\_PlaneScene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:31

## Accessors

### currentDraggingPointerID

• `get` **currentDraggingPointerID**(): `number`

Get or set the currentDraggingPointerId

**`Deprecated`**

Please use currentDraggingPointerId instead

#### Returns

`number`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:50

• `set` **currentDraggingPointerID**(`currentDraggingPointerID`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentDraggingPointerID` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:53

___

### enabled

• `get` **enabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:115

• `set` **enabled**(`value`): `void`

If the drag behavior will react to drag events (Default: true)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:108

___

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:183

___

### options

• `get` **options**(): `Object`

Gets the options used by the behavior

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `dragAxis?` | [`Vector3`](Vector3.md) |
| `dragPlaneNormal?` | [`Vector3`](Vector3.md) |

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:139

• `set` **options**(`options`): `void`

Sets the options used by the behavior

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Object` |
| `options.dragAxis?` | [`Vector3`](Vector3.md) |
| `options.dragPlaneNormal?` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:146

## Methods

### \_moveDrag

▸ `Protected` **_moveDrag**(`ray`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ray` | [`Ray`](Ray.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:412

___

### \_pickWithRayOnDragPlane

▸ `Private` **_pickWithRayOnDragPlane**(`ray`): ``null`` \| [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `ray` | [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md) |

#### Returns

``null`` \| [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:452

___

### \_startDrag

▸ `Protected` **_startDrag**(`pointerId`, `fromRay?`, `startPickedPoint?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointerId` | `number` |
| `fromRay?` | [`Ray`](Ray.md) |
| `startPickedPoint?` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:372

___

### \_updateDragPlanePosition

▸ `Private` **_updateDragPlanePosition**(`ray`, `dragPlanePosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ray` | [`Ray`](Ray.md) |
| `dragPlanePosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:501

___

### attach

▸ **attach**(`ownerNode`, `predicate?`): `void`

Attaches the drag behavior the passed in mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`AbstractMesh`](AbstractMesh.md) | The mesh that will be dragged around once attached |
| `predicate?` | (`m`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate to use for pick filtering |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:202

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:549

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:190

___

### releaseDrag

▸ **releaseDrag**(): `void`

Force release the drag action by code.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:325

___

### startDrag

▸ **startDrag**(`pointerId?`, `fromRay?`, `startPickedPoint?`): `void`

Simulates the start of a pointer drag event on the behavior

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `pointerId` | `number` | `PointerDragBehavior._AnyMouseId` | pointerID of the pointer that should be simulated (Default: Any mouse pointer ID) |
| `fromRay?` | [`Ray`](Ray.md) | `undefined` | initial ray of the pointer to be simulated (Default: Ray from camera to attached mesh) |
| `startPickedPoint?` | [`Vector3`](Vector3.md) | `undefined` | picked point of the pointer to be simulated (Default: attached mesh position) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:358

___

### validateDrag

▸ **validateDrag**(`targetPosition`): `boolean`

Predicate to determine if it is valid to move the object to a new position when it is moved

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetPosition` | [`Vector3`](Vector3.md) |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/pointerDragBehavior.ts:176

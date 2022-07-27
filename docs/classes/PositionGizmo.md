[@dev/core](../README.md) / [Exports](../modules.md) / PositionGizmo

# Class: PositionGizmo

Gizmo that enables dragging a mesh along 3 axis

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`PositionGizmo`**

## Table of contents

### Constructors

- [constructor](PositionGizmo.md#constructor)

### Properties

- [\_customMeshSet](PositionGizmo.md#_custommeshset)
- [\_gizmoAxisCache](PositionGizmo.md#_gizmoaxiscache)
- [\_interactionsEnabled](PositionGizmo.md#_interactionsenabled)
- [\_isHovered](PositionGizmo.md#_ishovered)
- [\_meshAttached](PositionGizmo.md#_meshattached)
- [\_nodeAttached](PositionGizmo.md#_nodeattached)
- [\_observables](PositionGizmo.md#_observables)
- [\_planarGizmoEnabled](PositionGizmo.md#_planargizmoenabled)
- [\_rootMesh](PositionGizmo.md#_rootmesh)
- [\_scaleRatio](PositionGizmo.md#_scaleratio)
- [\_snapDistance](PositionGizmo.md#_snapdistance)
- [\_updateGizmoRotationToMatchAttachedMesh](PositionGizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](PositionGizmo.md#gizmolayer)
- [onDragEndObservable](PositionGizmo.md#ondragendobservable)
- [onDragStartObservable](PositionGizmo.md#ondragstartobservable)
- [updateGizmoPositionToMatchAttachedMesh](PositionGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](PositionGizmo.md#updatescale)
- [xGizmo](PositionGizmo.md#xgizmo)
- [xPlaneGizmo](PositionGizmo.md#xplanegizmo)
- [yGizmo](PositionGizmo.md#ygizmo)
- [yPlaneGizmo](PositionGizmo.md#yplanegizmo)
- [zGizmo](PositionGizmo.md#zgizmo)
- [zPlaneGizmo](PositionGizmo.md#zplanegizmo)
- [PreserveScaling](PositionGizmo.md#preservescaling)

### Accessors

- [attachedMesh](PositionGizmo.md#attachedmesh)
- [attachedNode](PositionGizmo.md#attachednode)
- [customRotationQuaternion](PositionGizmo.md#customrotationquaternion)
- [isHovered](PositionGizmo.md#ishovered)
- [planarGizmoEnabled](PositionGizmo.md#planargizmoenabled)
- [scaleRatio](PositionGizmo.md#scaleratio)
- [snapDistance](PositionGizmo.md#snapdistance)
- [updateGizmoRotationToMatchAttachedMesh](PositionGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](PositionGizmo.md#_attachednodechanged)
- [\_handlePivot](PositionGizmo.md#_handlepivot)
- [\_matrixChanged](PositionGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](PositionGizmo.md#_setgizmomeshmaterial)
- [\_update](PositionGizmo.md#_update)
- [addToAxisCache](PositionGizmo.md#addtoaxiscache)
- [dispose](PositionGizmo.md#dispose)
- [setCustomMesh](PositionGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](PositionGizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new PositionGizmo**(`gizmoLayer?`, `thickness?`, `gizmoManager?`)

Creates a PositionGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |
| `thickness` | `number` | `1` | display gizmo axis thickness |
| `gizmoManager?` | [`GizmoManager`](GizmoManager.md) | `undefined` |  |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:114

## Properties

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:89

___

### \_gizmoAxisCache

• `Private` **\_gizmoAxisCache**: `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md)

Node Caching for quick lookup

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:55

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_interactionsEnabled](Gizmo.md#_interactionsenabled)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:153

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:60

___

### \_meshAttached

• `Private` **\_meshAttached**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

private variables

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:49

___

### \_nodeAttached

• `Private` **\_nodeAttached**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:50

___

### \_observables

• `Private` **\_observables**: [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)[] = `[]`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:52

___

### \_planarGizmoEnabled

• `Private` **\_planarGizmoEnabled**: `boolean` = `false`

If set to true, planar drag is enabled

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:65

___

### \_rootMesh

• **\_rootMesh**: [`Mesh`](Mesh.md)

The root mesh of the gizmo

#### Inherited from

[Gizmo](Gizmo.md).[_rootMesh](Gizmo.md#_rootmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:48

___

### \_scaleRatio

• `Protected` **\_scaleRatio**: `number` = `1`

Ratio for the scale of the gizmo (Default: 1)

#### Inherited from

[Gizmo](Gizmo.md).[_scaleRatio](Gizmo.md#_scaleratio)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:55

___

### \_snapDistance

• `Private` **\_snapDistance**: `number`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:51

___

### \_updateGizmoRotationToMatchAttachedMesh

• `Protected` **\_updateGizmoRotationToMatchAttachedMesh**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_updateGizmoRotationToMatchAttachedMesh](Gizmo.md#_updategizmorotationtomatchattachedmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:134

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Inherited from

[Gizmo](Gizmo.md).[gizmoLayer](Gizmo.md#gizmolayer)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:171

___

### onDragEndObservable

• **onDragEndObservable**: [`Observable`](Observable.md)`unknown`

Fires an event when any of it's sub gizmos are released from dragging

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:60

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md)`unknown`

Fires an event when any of it's sub gizmos are dragged

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:58

___

### updateGizmoPositionToMatchAttachedMesh

• **updateGizmoPositionToMatchAttachedMesh**: `boolean` = `true`

If set the gizmo's position will be updated to match the attached mesh each frame (Default: true)

#### Inherited from

[Gizmo](Gizmo.md).[updateGizmoPositionToMatchAttachedMesh](Gizmo.md#updategizmopositiontomatchattachedmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:148

___

### updateScale

• **updateScale**: `boolean` = `true`

When set, the gizmo will always appear the same size no matter where the camera is (default: true)

#### Inherited from

[Gizmo](Gizmo.md).[updateScale](Gizmo.md#updatescale)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:152

___

### xGizmo

• **xGizmo**: [`AxisDragGizmo`](AxisDragGizmo.md)

Internal gizmo used for interactions on the x axis

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:24

___

### xPlaneGizmo

• **xPlaneGizmo**: [`PlaneDragGizmo`](PlaneDragGizmo.md)

Internal gizmo used for interactions on the yz plane

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:36

___

### yGizmo

• **yGizmo**: [`AxisDragGizmo`](AxisDragGizmo.md)

Internal gizmo used for interactions on the y axis

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:28

___

### yPlaneGizmo

• **yPlaneGizmo**: [`PlaneDragGizmo`](PlaneDragGizmo.md)

Internal gizmo used for interactions on the xz plane

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:40

___

### zGizmo

• **zGizmo**: [`AxisDragGizmo`](AxisDragGizmo.md)

Internal gizmo used for interactions on the z axis

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:32

___

### zPlaneGizmo

• **zPlaneGizmo**: [`PlaneDragGizmo`](PlaneDragGizmo.md)

Internal gizmo used for interactions on the xy plane

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:44

___

### PreserveScaling

▪ `Static` **PreserveScaling**: `boolean` = `false`

When enabled, any gizmo operation will perserve scaling sign. Default is off.
Only valid for TransformNode derived classes (Mesh, AbstractMesh, ...)

#### Inherited from

[Gizmo](Gizmo.md).[PreserveScaling](Gizmo.md#preservescaling)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:66

## Accessors

### attachedMesh

• `get` **attachedMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Mesh that the gizmo will be attached to. (eg. on a drag gizmo the mesh that will be dragged)
* When set, interactions will be enabled

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Overrides

Gizmo.attachedMesh

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:67

• `set` **attachedMesh**(`mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Overrides

Gizmo.attachedMesh

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:70

___

### attachedNode

• `get` **attachedNode**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Node that the gizmo will be attached to. (eg. on a drag gizmo the mesh, bone or NodeTransform that will be dragged)
* When set, interactions will be enabled

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Overrides

Gizmo.attachedNode

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:82

• `set` **attachedNode**(`node`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Overrides

Gizmo.attachedNode

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:85

___

### customRotationQuaternion

• `get` **customRotationQuaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

posture that the gizmo will be display
When set null, default value will be used (Quaternion(0, 0, 0, 1))

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Inherited from

Gizmo.customRotationQuaternion

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:185

• `set` **customRotationQuaternion**(`customRotationQuaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `customRotationQuaternion` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Inherited from

Gizmo.customRotationQuaternion

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:189

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovering a gizmo mesh

#### Returns

`boolean`

#### Overrides

Gizmo.isHovered

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:100

___

### planarGizmoEnabled

• `get` **planarGizmoEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:162

• `set` **planarGizmoEnabled**(`value`): `void`

If the planar drag gizmo is enabled
setting this will enable/disable XY, XZ and YZ planes regardless of individual gizmo settings.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:147

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Overrides

Gizmo.scaleRatio

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:204

• `set` **scaleRatio**(`value`): `void`

Ratio for the scale of the gizmo (Default: 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

Gizmo.scaleRatio

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:196

___

### snapDistance

• `get` **snapDistance**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:189

• `set` **snapDistance**(`value`): `void`

Drag distance in babylon units that the gizmo will snap to when dragged (Default: 0)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:181

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Overrides

Gizmo.updateGizmoRotationToMatchAttachedMesh

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:174

• `set` **updateGizmoRotationToMatchAttachedMesh**(`value`): `void`

If set the gizmo's rotation will be updated to match the attached mesh each frame (Default: true)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

Gizmo.updateGizmoRotationToMatchAttachedMesh

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:166

## Methods

### \_attachedNodeChanged

▸ `Protected` **_attachedNodeChanged**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_attachedNodeChanged](Gizmo.md#_attachednodechanged)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:155

___

### \_handlePivot

▸ `Protected` **_handlePivot**(): `void`

Handle position/translation when using an attached node using pivot

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_handlePivot](Gizmo.md#_handlepivot)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:251

___

### \_matrixChanged

▸ `Protected` **_matrixChanged**(): `void`

computes the rotation/scaling/position of the transform once the Node world matrix has changed.

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_matrixChanged](Gizmo.md#_matrixchanged)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:266

___

### \_setGizmoMeshMaterial

▸ `Protected` **_setGizmoMeshMaterial**(`gizmoMeshes`, `material`): `void`

refresh gizmo mesh material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gizmoMeshes` | [`Mesh`](Mesh.md)[] |  |
| `material` | [`StandardMaterial`](StandardMaterial.md) | material to apply |

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_setGizmoMeshMaterial](Gizmo.md#_setgizmomeshmaterial)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:385

___

### \_update

▸ `Protected` **_update**(): `void`

Updates the gizmo to match the attached mesh's position/rotation

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_update](Gizmo.md#_update)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:196

___

### addToAxisCache

▸ **addToAxisCache**(`mesh`, `cache`): `void`

Builds Gizmo Axis Cache to enable features such as hover state preservation and graying out other axis during manipulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | Axis gizmo mesh |
| `cache` | [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md) | Gizmo axis definition used for reactive gizmo UI |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:213

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:220

___

### setCustomMesh

▸ **setCustomMesh**(): `void`

CustomMeshes are not supported by this gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[setCustomMesh](Gizmo.md#setcustommesh)

#### Defined in

packages/dev/core/src/Gizmos/positionGizmo.ts:236

___

### GizmoAxisPointerObserver

▸ `Static` **GizmoAxisPointerObserver**(`gizmoLayer`, `gizmoAxisCache`): [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

Subscribes to pointer up, down, and hover events. Used for responsive gizmos.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | The utility layer the gizmo will be added to |
| `gizmoAxisCache` | `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md) | Gizmo axis definition used for reactive gizmo UI |

#### Returns

[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

pointerObserver

#### Inherited from

[Gizmo](Gizmo.md).[GizmoAxisPointerObserver](Gizmo.md#gizmoaxispointerobserver)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:402

[@dev/core](../README.md) / [Exports](../modules.md) / RotationGizmo

# Class: RotationGizmo

Gizmo that enables rotating a mesh along 3 axis

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`RotationGizmo`**

## Table of contents

### Constructors

- [constructor](RotationGizmo.md#constructor)

### Properties

- [\_customMeshSet](RotationGizmo.md#_custommeshset)
- [\_gizmoAxisCache](RotationGizmo.md#_gizmoaxiscache)
- [\_interactionsEnabled](RotationGizmo.md#_interactionsenabled)
- [\_isHovered](RotationGizmo.md#_ishovered)
- [\_meshAttached](RotationGizmo.md#_meshattached)
- [\_nodeAttached](RotationGizmo.md#_nodeattached)
- [\_observables](RotationGizmo.md#_observables)
- [\_rootMesh](RotationGizmo.md#_rootmesh)
- [\_scaleRatio](RotationGizmo.md#_scaleratio)
- [\_updateGizmoRotationToMatchAttachedMesh](RotationGizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](RotationGizmo.md#gizmolayer)
- [onDragEndObservable](RotationGizmo.md#ondragendobservable)
- [onDragStartObservable](RotationGizmo.md#ondragstartobservable)
- [updateGizmoPositionToMatchAttachedMesh](RotationGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](RotationGizmo.md#updatescale)
- [xGizmo](RotationGizmo.md#xgizmo)
- [yGizmo](RotationGizmo.md#ygizmo)
- [zGizmo](RotationGizmo.md#zgizmo)
- [PreserveScaling](RotationGizmo.md#preservescaling)

### Accessors

- [attachedMesh](RotationGizmo.md#attachedmesh)
- [attachedNode](RotationGizmo.md#attachednode)
- [customRotationQuaternion](RotationGizmo.md#customrotationquaternion)
- [isHovered](RotationGizmo.md#ishovered)
- [scaleRatio](RotationGizmo.md#scaleratio)
- [snapDistance](RotationGizmo.md#snapdistance)
- [updateGizmoRotationToMatchAttachedMesh](RotationGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](RotationGizmo.md#_attachednodechanged)
- [\_checkBillboardTransform](RotationGizmo.md#_checkbillboardtransform)
- [\_handlePivot](RotationGizmo.md#_handlepivot)
- [\_matrixChanged](RotationGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](RotationGizmo.md#_setgizmomeshmaterial)
- [\_update](RotationGizmo.md#_update)
- [addToAxisCache](RotationGizmo.md#addtoaxiscache)
- [dispose](RotationGizmo.md#dispose)
- [setCustomMesh](RotationGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](RotationGizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new RotationGizmo**(`gizmoLayer?`, `tessellation?`, `useEulerRotation?`, `thickness?`, `gizmoManager?`, `options?`)

Creates a RotationGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |
| `tessellation` | `number` | `32` | Amount of tessellation to be used when creating rotation circles |
| `useEulerRotation` | `boolean` | `false` | Use and update Euler angle instead of quaternion |
| `thickness` | `number` | `1` | display gizmo axis thickness |
| `gizmoManager?` | [`GizmoManager`](GizmoManager.md) | `undefined` | Gizmo manager |
| `options?` | [`RotationGizmoOptions`](../interfaces/RotationGizmoOptions.md) | `undefined` | More options |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:141

## Properties

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:89

___

### \_gizmoAxisCache

• `Private` **\_gizmoAxisCache**: `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md)

Node Caching for quick lookup

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:81

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_interactionsEnabled](Gizmo.md#_interactionsenabled)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:153

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:60

___

### \_meshAttached

• `Private` **\_meshAttached**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:76

___

### \_nodeAttached

• `Private` **\_nodeAttached**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:77

___

### \_observables

• `Private` **\_observables**: [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:78

___

### \_rootMesh

• **\_rootMesh**: [`Mesh`](Mesh.md)

The root mesh of the gizmo

#### Inherited from

[Gizmo](Gizmo.md).[_rootMesh](Gizmo.md#_rootmesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:48

___

### \_scaleRatio

• `Protected` **\_scaleRatio**: `number` = `1`

Ratio for the scale of the gizmo (Default: 1)

#### Inherited from

[Gizmo](Gizmo.md).[_scaleRatio](Gizmo.md#_scaleratio)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:55

___

### \_updateGizmoRotationToMatchAttachedMesh

• `Protected` **\_updateGizmoRotationToMatchAttachedMesh**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_updateGizmoRotationToMatchAttachedMesh](Gizmo.md#_updategizmorotationtomatchattachedmesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:134

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Inherited from

[Gizmo](Gizmo.md).[gizmoLayer](Gizmo.md#gizmolayer)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:171

___

### onDragEndObservable

• **onDragEndObservable**: [`Observable`](Observable.md)`unknown`

Fires an event when any of it's sub gizmos are released from dragging

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:74

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md)`unknown`

Fires an event when any of it's sub gizmos are dragged

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:72

___

### updateGizmoPositionToMatchAttachedMesh

• **updateGizmoPositionToMatchAttachedMesh**: `boolean` = `true`

If set the gizmo's position will be updated to match the attached mesh each frame (Default: true)

#### Inherited from

[Gizmo](Gizmo.md).[updateGizmoPositionToMatchAttachedMesh](Gizmo.md#updategizmopositiontomatchattachedmesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:148

___

### updateScale

• **updateScale**: `boolean` = `true`

When set, the gizmo will always appear the same size no matter where the camera is (default: true)

#### Inherited from

[Gizmo](Gizmo.md).[updateScale](Gizmo.md#updatescale)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:152

___

### xGizmo

• **xGizmo**: [`PlaneRotationGizmo`](PlaneRotationGizmo.md)

Internal gizmo used for interactions on the x axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:61

___

### yGizmo

• **yGizmo**: [`PlaneRotationGizmo`](PlaneRotationGizmo.md)

Internal gizmo used for interactions on the y axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:65

___

### zGizmo

• **zGizmo**: [`PlaneRotationGizmo`](PlaneRotationGizmo.md)

Internal gizmo used for interactions on the z axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:69

___

### PreserveScaling

▪ `Static` **PreserveScaling**: `boolean` = `false`

When enabled, any gizmo operation will perserve scaling sign. Default is off.
Only valid for TransformNode derived classes (Mesh, AbstractMesh, ...)

#### Inherited from

[Gizmo](Gizmo.md).[PreserveScaling](Gizmo.md#preservescaling)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:66

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:83

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:86

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:99

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:102

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:185

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:189

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovering a gizmo mesh

#### Returns

`boolean`

#### Overrides

Gizmo.isHovered

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:124

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Overrides

Gizmo.scaleRatio

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:217

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:210

___

### snapDistance

• `get` **snapDistance**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:203

• `set` **snapDistance**(`value`): `void`

Drag distance in babylon units that the gizmo will snap to when dragged (Default: 0)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:196

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Overrides

Gizmo.updateGizmoRotationToMatchAttachedMesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:189

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:182

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:155

___

### \_checkBillboardTransform

▸ `Protected` **_checkBillboardTransform**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:115

___

### \_handlePivot

▸ `Protected` **_handlePivot**(): `void`

Handle position/translation when using an attached node using pivot

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_handlePivot](Gizmo.md#_handlepivot)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:251

___

### \_matrixChanged

▸ `Protected` **_matrixChanged**(): `void`

computes the rotation/scaling/position of the transform once the Node world matrix has changed.

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_matrixChanged](Gizmo.md#_matrixchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:266

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:385

___

### \_update

▸ `Protected` **_update**(): `void`

Updates the gizmo to match the attached mesh's position/rotation

#### Returns

`void`

#### Inherited from

[Gizmo](Gizmo.md).[_update](Gizmo.md#_update)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:196

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

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:226

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:233

___

### setCustomMesh

▸ **setCustomMesh**(): `void`

CustomMeshes are not supported by this gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[setCustomMesh](Gizmo.md#setcustommesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/rotationGizmo.ts:247

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:402

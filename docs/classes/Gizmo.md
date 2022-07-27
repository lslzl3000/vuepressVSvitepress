[@dev/core](../README.md) / [Exports](../modules.md) / Gizmo

# Class: Gizmo

Renders gizmos on top of an existing scene which provide controls for position, rotation, etc.

## Hierarchy

- **`Gizmo`**

  ↳ [`AxisDragGizmo`](AxisDragGizmo.md)

  ↳ [`AxisScaleGizmo`](AxisScaleGizmo.md)

  ↳ [`BoundingBoxGizmo`](BoundingBoxGizmo.md)

  ↳ [`PlaneRotationGizmo`](PlaneRotationGizmo.md)

  ↳ [`PositionGizmo`](PositionGizmo.md)

  ↳ [`RotationGizmo`](RotationGizmo.md)

  ↳ [`ScaleGizmo`](ScaleGizmo.md)

  ↳ [`LightGizmo`](LightGizmo.md)

  ↳ [`CameraGizmo`](CameraGizmo.md)

  ↳ [`PlaneDragGizmo`](PlaneDragGizmo.md)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](Gizmo.md#constructor)

### Properties

- [\_attachedMesh](Gizmo.md#_attachedmesh)
- [\_attachedNode](Gizmo.md#_attachednode)
- [\_beforeRenderObserver](Gizmo.md#_beforerenderobserver)
- [\_customMeshSet](Gizmo.md#_custommeshset)
- [\_customRotationQuaternion](Gizmo.md#_customrotationquaternion)
- [\_interactionsEnabled](Gizmo.md#_interactionsenabled)
- [\_isHovered](Gizmo.md#_ishovered)
- [\_rightHandtoLeftHandMatrix](Gizmo.md#_righthandtolefthandmatrix)
- [\_rootMesh](Gizmo.md#_rootmesh)
- [\_scaleRatio](Gizmo.md#_scaleratio)
- [\_tempMatrix1](Gizmo.md#_tempmatrix1)
- [\_tempMatrix2](Gizmo.md#_tempmatrix2)
- [\_tempQuaternion](Gizmo.md#_tempquaternion)
- [\_tempVector](Gizmo.md#_tempvector)
- [\_tempVector2](Gizmo.md#_tempvector2)
- [\_updateGizmoRotationToMatchAttachedMesh](Gizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](Gizmo.md#gizmolayer)
- [updateGizmoPositionToMatchAttachedMesh](Gizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](Gizmo.md#updatescale)
- [PreserveScaling](Gizmo.md#preservescaling)

### Accessors

- [attachedMesh](Gizmo.md#attachedmesh)
- [attachedNode](Gizmo.md#attachednode)
- [customRotationQuaternion](Gizmo.md#customrotationquaternion)
- [isHovered](Gizmo.md#ishovered)
- [scaleRatio](Gizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](Gizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](Gizmo.md#_attachednodechanged)
- [\_handlePivot](Gizmo.md#_handlepivot)
- [\_matrixChanged](Gizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](Gizmo.md#_setgizmomeshmaterial)
- [\_update](Gizmo.md#_update)
- [dispose](Gizmo.md#dispose)
- [setCustomMesh](Gizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](Gizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new Gizmo**(`gizmoLayer?`)

Creates a gizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:169

## Properties

### \_attachedMesh

• `Private` **\_attachedMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:49

___

### \_attachedNode

• `Private` **\_attachedNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:50

___

### \_beforeRenderObserver

• `Private` **\_beforeRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:157

___

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:89

___

### \_customRotationQuaternion

• `Private` **\_customRotationQuaternion**: [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:51

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:153

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:60

___

### \_rightHandtoLeftHandMatrix

• `Private` **\_rightHandtoLeftHandMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:163

___

### \_rootMesh

• **\_rootMesh**: [`Mesh`](Mesh.md)

The root mesh of the gizmo

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:48

___

### \_scaleRatio

• `Protected` **\_scaleRatio**: `number` = `1`

Ratio for the scale of the gizmo (Default: 1)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:55

___

### \_tempMatrix1

• `Private` **\_tempMatrix1**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:161

___

### \_tempMatrix2

• `Private` **\_tempMatrix2**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:162

___

### \_tempQuaternion

• `Private` **\_tempQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:158

___

### \_tempVector

• `Private` **\_tempVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:159

___

### \_tempVector2

• `Private` **\_tempVector2**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:160

___

### \_updateGizmoRotationToMatchAttachedMesh

• `Protected` **\_updateGizmoRotationToMatchAttachedMesh**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:134

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:171

___

### updateGizmoPositionToMatchAttachedMesh

• **updateGizmoPositionToMatchAttachedMesh**: `boolean` = `true`

If set the gizmo's position will be updated to match the attached mesh each frame (Default: true)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:148

___

### updateScale

• **updateScale**: `boolean` = `true`

When set, the gizmo will always appear the same size no matter where the camera is (default: true)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:152

___

### PreserveScaling

▪ `Static` **PreserveScaling**: `boolean` = `false`

When enabled, any gizmo operation will perserve scaling sign. Default is off.
Only valid for TransformNode derived classes (Mesh, AbstractMesh, ...)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:66

## Accessors

### attachedMesh

• `get` **attachedMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Mesh that the gizmo will be attached to. (eg. on a drag gizmo the mesh that will be dragged)
* When set, interactions will be enabled

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:94

• `set` **attachedMesh**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:97

___

### attachedNode

• `get` **attachedNode**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Node that the gizmo will be attached to. (eg. on a drag gizmo the mesh, bone or NodeTransform that will be dragged)
* When set, interactions will be enabled

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:109

• `set` **attachedNode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:112

___

### customRotationQuaternion

• `get` **customRotationQuaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

posture that the gizmo will be display
When set null, default value will be used (Quaternion(0, 0, 0, 1))

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:185

• `set` **customRotationQuaternion**(`customRotationQuaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `customRotationQuaternion` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:189

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovered a gizmo mesh

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:82

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:75

• `set` **scaleRatio**(`value`): `void`

Ratio for the scale of the gizmo (Default: 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:71

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:142

• `set` **updateGizmoRotationToMatchAttachedMesh**(`value`): `void`

If set the gizmo's rotation will be updated to match the attached mesh each frame (Default: true)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:139

## Methods

### \_attachedNodeChanged

▸ `Protected` **_attachedNodeChanged**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:155

___

### \_handlePivot

▸ `Protected` **_handlePivot**(): `void`

Handle position/translation when using an attached node using pivot

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:251

___

### \_matrixChanged

▸ `Protected` **_matrixChanged**(): `void`

computes the rotation/scaling/position of the transform once the Node world matrix has changed.

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:385

___

### \_update

▸ `Protected` **_update**(): `void`

Updates the gizmo to match the attached mesh's position/rotation

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:196

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:468

___

### setCustomMesh

▸ **setCustomMesh**(`mesh`): `void`

Disposes and replaces the current meshes in the gizmo with the specified mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to replace the default mesh of the gizmo |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:123

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

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:402

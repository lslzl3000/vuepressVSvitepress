[@dev/core](../README.md) / [Exports](../modules.md) / AxisScaleGizmo

# Class: AxisScaleGizmo

Single axis scale gizmo

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`AxisScaleGizmo`**

## Table of contents

### Constructors

- [constructor](AxisScaleGizmo.md#constructor)

### Properties

- [\_coloredMaterial](AxisScaleGizmo.md#_coloredmaterial)
- [\_customMeshSet](AxisScaleGizmo.md#_custommeshset)
- [\_disableMaterial](AxisScaleGizmo.md#_disablematerial)
- [\_dragging](AxisScaleGizmo.md#_dragging)
- [\_gizmoMesh](AxisScaleGizmo.md#_gizmomesh)
- [\_hoverMaterial](AxisScaleGizmo.md#_hovermaterial)
- [\_interactionsEnabled](AxisScaleGizmo.md#_interactionsenabled)
- [\_isEnabled](AxisScaleGizmo.md#_isenabled)
- [\_isHovered](AxisScaleGizmo.md#_ishovered)
- [\_parent](AxisScaleGizmo.md#_parent)
- [\_pointerObserver](AxisScaleGizmo.md#_pointerobserver)
- [\_rootMesh](AxisScaleGizmo.md#_rootmesh)
- [\_scaleRatio](AxisScaleGizmo.md#_scaleratio)
- [\_tmpMatrix](AxisScaleGizmo.md#_tmpmatrix)
- [\_tmpMatrix2](AxisScaleGizmo.md#_tmpmatrix2)
- [\_tmpVector](AxisScaleGizmo.md#_tmpvector)
- [\_updateGizmoRotationToMatchAttachedMesh](AxisScaleGizmo.md#_updategizmorotationtomatchattachedmesh)
- [dragBehavior](AxisScaleGizmo.md#dragbehavior)
- [dragScale](AxisScaleGizmo.md#dragscale)
- [gizmoLayer](AxisScaleGizmo.md#gizmolayer)
- [onSnapObservable](AxisScaleGizmo.md#onsnapobservable)
- [sensitivity](AxisScaleGizmo.md#sensitivity)
- [snapDistance](AxisScaleGizmo.md#snapdistance)
- [uniformScaling](AxisScaleGizmo.md#uniformscaling)
- [updateGizmoPositionToMatchAttachedMesh](AxisScaleGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](AxisScaleGizmo.md#updatescale)
- [PreserveScaling](AxisScaleGizmo.md#preservescaling)

### Accessors

- [attachedMesh](AxisScaleGizmo.md#attachedmesh)
- [attachedNode](AxisScaleGizmo.md#attachednode)
- [customRotationQuaternion](AxisScaleGizmo.md#customrotationquaternion)
- [isEnabled](AxisScaleGizmo.md#isenabled)
- [isHovered](AxisScaleGizmo.md#ishovered)
- [scaleRatio](AxisScaleGizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](AxisScaleGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](AxisScaleGizmo.md#_attachednodechanged)
- [\_createGizmoMesh](AxisScaleGizmo.md#_creategizmomesh)
- [\_handlePivot](AxisScaleGizmo.md#_handlepivot)
- [\_matrixChanged](AxisScaleGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](AxisScaleGizmo.md#_setgizmomeshmaterial)
- [\_update](AxisScaleGizmo.md#_update)
- [dispose](AxisScaleGizmo.md#dispose)
- [setCustomMesh](AxisScaleGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](AxisScaleGizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new AxisScaleGizmo**(`dragAxis`, `color?`, `gizmoLayer?`, `parent?`, `thickness?`)

Creates an AxisScaleGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `dragAxis` | [`Vector3`](Vector3.md) | `undefined` | The axis which the gizmo will be able to scale on |
| `color` | [`Color3`](Color3.md) | `undefined` | The color of the gizmo |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |
| `parent` | [`Nullable`](../modules.md#nullable)[`ScaleGizmo`](ScaleGizmo.md) | `null` |  |
| `thickness` | `number` | `1` | display gizmo axis thickness |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:72

## Properties

### \_coloredMaterial

• `Private` **\_coloredMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:56

___

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:89

___

### \_disableMaterial

• `Private` **\_disableMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:58

___

### \_dragging

• `Private` **\_dragging**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:59

___

### \_gizmoMesh

• `Private` **\_gizmoMesh**: [`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:55

___

### \_hoverMaterial

• `Private` **\_hoverMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:57

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_interactionsEnabled](Gizmo.md#_interactionsenabled)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:153

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:52

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:60

___

### \_parent

• `Private` **\_parent**: [`Nullable`](../modules.md#nullable)[`ScaleGizmo`](ScaleGizmo.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:53

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:29

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

### \_tmpMatrix

• `Private` **\_tmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:61

___

### \_tmpMatrix2

• `Private` **\_tmpMatrix2**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:62

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:60

___

### \_updateGizmoRotationToMatchAttachedMesh

• `Protected` **\_updateGizmoRotationToMatchAttachedMesh**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_updateGizmoRotationToMatchAttachedMesh](Gizmo.md#_updategizmorotationtomatchattachedmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:134

___

### dragBehavior

• **dragBehavior**: [`PointerDragBehavior`](PointerDragBehavior.md)

Drag behavior responsible for the gizmos dragging interactions

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:28

___

### dragScale

• **dragScale**: `number` = `1`

The magnitude of the drag strength (scaling factor)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:50

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Inherited from

[Gizmo](Gizmo.md).[gizmoLayer](Gizmo.md#gizmolayer)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:171

___

### onSnapObservable

• **onSnapObservable**: [`Observable`](Observable.md){ `snapDistance`: `number`  }

Event that fires each time the gizmo snaps to a new location.
* snapDistance is the the change in distance

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:38

___

### sensitivity

• **sensitivity**: `number` = `1`

Custom sensitivity value for the drag strength

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:46

___

### snapDistance

• **snapDistance**: `number` = `0`

Scale distance in babylon units that the gizmo will snap to when dragged (Default: 0)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:33

___

### uniformScaling

• **uniformScaling**: `boolean` = `false`

If the scaling operation should be done on all axis (default: false)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:42

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

#### Inherited from

Gizmo.attachedMesh

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:94

• `set` **attachedMesh**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Inherited from

Gizmo.attachedMesh

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:97

___

### attachedNode

• `get` **attachedNode**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Node that the gizmo will be attached to. (eg. on a drag gizmo the mesh, bone or NodeTransform that will be dragged)
* When set, interactions will be enabled

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

Gizmo.attachedNode

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:109

• `set` **attachedNode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Inherited from

Gizmo.attachedNode

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:112

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

### isEnabled

• `get` **isEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:279

• `set` **isEnabled**(`value`): `void`

If the gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:267

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovered a gizmo mesh

#### Returns

`boolean`

#### Inherited from

Gizmo.isHovered

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:82

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Inherited from

Gizmo.scaleRatio

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

#### Inherited from

Gizmo.scaleRatio

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:71

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Gizmo.updateGizmoRotationToMatchAttachedMesh

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

#### Inherited from

Gizmo.updateGizmoRotationToMatchAttachedMesh

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

#### Overrides

[Gizmo](Gizmo.md).[_attachedNodeChanged](Gizmo.md#_attachednodechanged)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:258

___

### \_createGizmoMesh

▸ `Private` **_createGizmoMesh**(`parentMesh`, `thickness`, `isCollider?`): `Object`

Create Geometry for Gizmo

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `parentMesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `thickness` | `number` | `undefined` |
| `isCollider` | `boolean` | `false` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `arrowMesh` | [`Mesh`](Mesh.md) |
| `arrowTail` | [`Mesh`](Mesh.md) |

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:229

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

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:286

___

### setCustomMesh

▸ **setCustomMesh**(`mesh`, `useGizmoMaterial?`): `void`

Disposes and replaces the current meshes in the gizmo with the specified mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | `undefined` | The mesh to replace the default mesh of the gizmo |
| `useGizmoMaterial` | `boolean` | `false` | If the gizmo's default material should be used (default: false) |

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[setCustomMesh](Gizmo.md#setcustommesh)

#### Defined in

packages/dev/core/src/Gizmos/axisScaleGizmo.ts:306

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

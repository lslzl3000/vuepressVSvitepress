[@dev/core](../README.md) / [Exports](../modules.md) / ScaleGizmo

# Class: ScaleGizmo

Gizmo that enables scaling a mesh along 3 axis

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`ScaleGizmo`**

## Table of contents

### Constructors

- [constructor](ScaleGizmo.md#constructor)

### Properties

- [\_coloredMaterial](ScaleGizmo.md#_coloredmaterial)
- [\_customMeshSet](ScaleGizmo.md#_custommeshset)
- [\_disableMaterial](ScaleGizmo.md#_disablematerial)
- [\_gizmoAxisCache](ScaleGizmo.md#_gizmoaxiscache)
- [\_hoverMaterial](ScaleGizmo.md#_hovermaterial)
- [\_interactionsEnabled](ScaleGizmo.md#_interactionsenabled)
- [\_isHovered](ScaleGizmo.md#_ishovered)
- [\_meshAttached](ScaleGizmo.md#_meshattached)
- [\_nodeAttached](ScaleGizmo.md#_nodeattached)
- [\_observables](ScaleGizmo.md#_observables)
- [\_octahedron](ScaleGizmo.md#_octahedron)
- [\_rootMesh](ScaleGizmo.md#_rootmesh)
- [\_scaleRatio](ScaleGizmo.md#_scaleratio)
- [\_sensitivity](ScaleGizmo.md#_sensitivity)
- [\_snapDistance](ScaleGizmo.md#_snapdistance)
- [\_uniformScalingMesh](ScaleGizmo.md#_uniformscalingmesh)
- [\_updateGizmoRotationToMatchAttachedMesh](ScaleGizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](ScaleGizmo.md#gizmolayer)
- [onDragEndObservable](ScaleGizmo.md#ondragendobservable)
- [onDragStartObservable](ScaleGizmo.md#ondragstartobservable)
- [uniformScaleGizmo](ScaleGizmo.md#uniformscalegizmo)
- [updateGizmoPositionToMatchAttachedMesh](ScaleGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](ScaleGizmo.md#updatescale)
- [xGizmo](ScaleGizmo.md#xgizmo)
- [yGizmo](ScaleGizmo.md#ygizmo)
- [zGizmo](ScaleGizmo.md#zgizmo)
- [PreserveScaling](ScaleGizmo.md#preservescaling)

### Accessors

- [attachedMesh](ScaleGizmo.md#attachedmesh)
- [attachedNode](ScaleGizmo.md#attachednode)
- [customRotationQuaternion](ScaleGizmo.md#customrotationquaternion)
- [isHovered](ScaleGizmo.md#ishovered)
- [scaleRatio](ScaleGizmo.md#scaleratio)
- [sensitivity](ScaleGizmo.md#sensitivity)
- [snapDistance](ScaleGizmo.md#snapdistance)
- [updateGizmoRotationToMatchAttachedMesh](ScaleGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](ScaleGizmo.md#_attachednodechanged)
- [\_createUniformScaleMesh](ScaleGizmo.md#_createuniformscalemesh)
- [\_handlePivot](ScaleGizmo.md#_handlepivot)
- [\_matrixChanged](ScaleGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](ScaleGizmo.md#_setgizmomeshmaterial)
- [\_update](ScaleGizmo.md#_update)
- [addToAxisCache](ScaleGizmo.md#addtoaxiscache)
- [dispose](ScaleGizmo.md#dispose)
- [setCustomMesh](ScaleGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](ScaleGizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new ScaleGizmo**(`gizmoLayer?`, `thickness?`, `gizmoManager?`)

Creates a ScaleGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |
| `thickness` | `number` | `1` | display gizmo axis thickness |
| `gizmoManager?` | [`GizmoManager`](GizmoManager.md) | `undefined` |  |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:106

## Properties

### \_coloredMaterial

• `Private` **\_coloredMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:46

___

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:89

___

### \_disableMaterial

• `Private` **\_disableMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:48

___

### \_gizmoAxisCache

• `Private` **\_gizmoAxisCache**: `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md)

Node Caching for quick lookup

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:52

___

### \_hoverMaterial

• `Private` **\_hoverMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:47

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

• `Private` **\_meshAttached**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:40

___

### \_nodeAttached

• `Private` **\_nodeAttached**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:41

___

### \_observables

• `Private` **\_observables**: [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:49

___

### \_octahedron

• `Private` **\_octahedron**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:44

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

### \_sensitivity

• `Private` **\_sensitivity**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:45

___

### \_snapDistance

• `Private` **\_snapDistance**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:42

___

### \_uniformScalingMesh

• `Private` **\_uniformScalingMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:43

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:57

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md)`unknown`

Fires an event when any of it's sub gizmos are dragged

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:55

___

### uniformScaleGizmo

• **uniformScaleGizmo**: [`AxisScaleGizmo`](AxisScaleGizmo.md)

Internal gizmo used to scale all axis equally

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:38

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

• **xGizmo**: [`AxisScaleGizmo`](AxisScaleGizmo.md)

Internal gizmo used for interactions on the x axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:25

___

### yGizmo

• **yGizmo**: [`AxisScaleGizmo`](AxisScaleGizmo.md)

Internal gizmo used for interactions on the y axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:29

___

### zGizmo

• **zGizmo**: [`AxisScaleGizmo`](AxisScaleGizmo.md)

Internal gizmo used for interactions on the z axis

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:33

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:59

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:62

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:74

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:77

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:92

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Overrides

Gizmo.scaleRatio

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:216

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:208

___

### sensitivity

• `get` **sensitivity**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:231

• `set` **sensitivity**(`value`): `void`

Sensitivity factor for dragging (Default: 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:223

___

### snapDistance

• `get` **snapDistance**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:201

• `set` **snapDistance**(`value`): `void`

Drag distance in babylon units that the gizmo will snap to when dragged (Default: 0)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:193

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Overrides

Gizmo.updateGizmoRotationToMatchAttachedMesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:186

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:174

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

### \_createUniformScaleMesh

▸ `Private` **_createUniformScaleMesh**(): [`AxisScaleGizmo`](AxisScaleGizmo.md)

Create Geometry for Gizmo

#### Returns

[`AxisScaleGizmo`](AxisScaleGizmo.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:135

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

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:240

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/scaleGizmo.ts:247

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

#### Inherited from

[Gizmo](Gizmo.md).[setCustomMesh](Gizmo.md#setcustommesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:123

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

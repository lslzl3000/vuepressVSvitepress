[@dev/core](../README.md) / [Exports](../modules.md) / CameraGizmo

# Class: CameraGizmo

Gizmo that enables viewing a camera

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`CameraGizmo`**

## Table of contents

### Constructors

- [constructor](CameraGizmo.md#constructor)

### Properties

- [\_camera](CameraGizmo.md#_camera)
- [\_cameraLinesMesh](CameraGizmo.md#_cameralinesmesh)
- [\_cameraMesh](CameraGizmo.md#_cameramesh)
- [\_customMeshSet](CameraGizmo.md#_custommeshset)
- [\_interactionsEnabled](CameraGizmo.md#_interactionsenabled)
- [\_invProjection](CameraGizmo.md#_invprojection)
- [\_isHovered](CameraGizmo.md#_ishovered)
- [\_material](CameraGizmo.md#_material)
- [\_pointerObserver](CameraGizmo.md#_pointerobserver)
- [\_rootMesh](CameraGizmo.md#_rootmesh)
- [\_scaleRatio](CameraGizmo.md#_scaleratio)
- [\_updateGizmoRotationToMatchAttachedMesh](CameraGizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](CameraGizmo.md#gizmolayer)
- [onClickedObservable](CameraGizmo.md#onclickedobservable)
- [updateGizmoPositionToMatchAttachedMesh](CameraGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](CameraGizmo.md#updatescale)
- [PreserveScaling](CameraGizmo.md#preservescaling)
- [\_Scale](CameraGizmo.md#_scale)

### Accessors

- [attachedMesh](CameraGizmo.md#attachedmesh)
- [attachedNode](CameraGizmo.md#attachednode)
- [camera](CameraGizmo.md#camera)
- [customRotationQuaternion](CameraGizmo.md#customrotationquaternion)
- [displayFrustum](CameraGizmo.md#displayfrustum)
- [isHovered](CameraGizmo.md#ishovered)
- [material](CameraGizmo.md#material)
- [scaleRatio](CameraGizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](CameraGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](CameraGizmo.md#_attachednodechanged)
- [\_handlePivot](CameraGizmo.md#_handlepivot)
- [\_matrixChanged](CameraGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](CameraGizmo.md#_setgizmomeshmaterial)
- [dispose](CameraGizmo.md#dispose)
- [setCustomMesh](CameraGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](CameraGizmo.md#gizmoaxispointerobserver)
- [\_CreateCameraFrustum](CameraGizmo.md#_createcamerafrustum)
- [\_CreateCameraMesh](CameraGizmo.md#_createcameramesh)

## Constructors

### constructor

• **new CameraGizmo**(`gizmoLayer?`)

Creates a CameraGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:37

## Properties

### \_camera

• `Private` **\_camera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:55

___

### \_cameraLinesMesh

• `Private` **\_cameraLinesMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:24

___

### \_cameraMesh

• `Private` **\_cameraMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:23

___

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:89

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_interactionsEnabled](Gizmo.md#_interactionsenabled)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:153

___

### \_invProjection

• `Private` **\_invProjection**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:143

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:60

___

### \_material

• `Private` **\_material**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:25

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:26

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

### onClickedObservable

• **onClickedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Event that fires each time the gizmo is clicked

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:31

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

### PreserveScaling

▪ `Static` **PreserveScaling**: `boolean` = `false`

When enabled, any gizmo operation will perserve scaling sign. Default is off.
Only valid for TransformNode derived classes (Mesh, AbstractMesh, ...)

#### Inherited from

[Gizmo](Gizmo.md).[PreserveScaling](Gizmo.md#preservescaling)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:66

___

### \_Scale

▪ `Static` `Private` **\_Scale**: `number` = `0.05`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:142

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:94

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:97

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:109

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:112

___

### camera

• `get` **camera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:106

• `set` **camera**(`camera`): `void`

The camera that the gizmo is attached to

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:68

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

### displayFrustum

• `get` **displayFrustum**(): `boolean`

Gets or sets a boolean indicating if frustum lines must be rendered (true by default))

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:58

• `set` **displayFrustum**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:61

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovered a gizmo mesh

#### Returns

`boolean`

#### Inherited from

Gizmo.isHovered

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:82

___

### material

• `get` **material**(): [`StandardMaterial`](StandardMaterial.md)

Gets the material used to render the camera gizmo

#### Returns

[`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:113

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Inherited from

Gizmo.scaleRatio

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:75

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:71

___

### updateGizmoRotationToMatchAttachedMesh

• `get` **updateGizmoRotationToMatchAttachedMesh**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Gizmo.updateGizmoRotationToMatchAttachedMesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:142

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

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:139

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

### dispose

▸ **dispose**(): `void`

Disposes of the camera gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:148

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

___

### \_CreateCameraFrustum

▸ `Static` `Private` **_CreateCameraFrustum**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:194

___

### \_CreateCameraMesh

▸ `Static` `Private` **_CreateCameraMesh**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/cameraGizmo.ts:161

[@dev/core](../README.md) / [Exports](../modules.md) / PlaneRotationGizmo

# Class: PlaneRotationGizmo

Single plane rotation gizmo

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`PlaneRotationGizmo`**

## Table of contents

### Constructors

- [constructor](PlaneRotationGizmo.md#constructor)

### Properties

- [\_angles](PlaneRotationGizmo.md#_angles)
- [\_coloredMaterial](PlaneRotationGizmo.md#_coloredmaterial)
- [\_customMeshSet](PlaneRotationGizmo.md#_custommeshset)
- [\_disableMaterial](PlaneRotationGizmo.md#_disablematerial)
- [\_dragging](PlaneRotationGizmo.md#_dragging)
- [\_gizmoMesh](PlaneRotationGizmo.md#_gizmomesh)
- [\_hoverMaterial](PlaneRotationGizmo.md#_hovermaterial)
- [\_interactionsEnabled](PlaneRotationGizmo.md#_interactionsenabled)
- [\_isEnabled](PlaneRotationGizmo.md#_isenabled)
- [\_isHovered](PlaneRotationGizmo.md#_ishovered)
- [\_parent](PlaneRotationGizmo.md#_parent)
- [\_pointerObserver](PlaneRotationGizmo.md#_pointerobserver)
- [\_rootMesh](PlaneRotationGizmo.md#_rootmesh)
- [\_rotationDisplayPlane](PlaneRotationGizmo.md#_rotationdisplayplane)
- [\_rotationShaderMaterial](PlaneRotationGizmo.md#_rotationshadermaterial)
- [\_scaleRatio](PlaneRotationGizmo.md#_scaleratio)
- [\_updateGizmoRotationToMatchAttachedMesh](PlaneRotationGizmo.md#_updategizmorotationtomatchattachedmesh)
- [angle](PlaneRotationGizmo.md#angle)
- [dragBehavior](PlaneRotationGizmo.md#dragbehavior)
- [gizmoLayer](PlaneRotationGizmo.md#gizmolayer)
- [onSnapObservable](PlaneRotationGizmo.md#onsnapobservable)
- [snapDistance](PlaneRotationGizmo.md#snapdistance)
- [updateGizmoPositionToMatchAttachedMesh](PlaneRotationGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](PlaneRotationGizmo.md#updatescale)
- [MaxDragAngle](PlaneRotationGizmo.md#maxdragangle)
- [PreserveScaling](PlaneRotationGizmo.md#preservescaling)
- [\_RotationGizmoFragmentShader](PlaneRotationGizmo.md#_rotationgizmofragmentshader)
- [\_RotationGizmoVertexShader](PlaneRotationGizmo.md#_rotationgizmovertexshader)

### Accessors

- [attachedMesh](PlaneRotationGizmo.md#attachedmesh)
- [attachedNode](PlaneRotationGizmo.md#attachednode)
- [customRotationQuaternion](PlaneRotationGizmo.md#customrotationquaternion)
- [isEnabled](PlaneRotationGizmo.md#isenabled)
- [isHovered](PlaneRotationGizmo.md#ishovered)
- [scaleRatio](PlaneRotationGizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](PlaneRotationGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](PlaneRotationGizmo.md#_attachednodechanged)
- [\_createGizmoMesh](PlaneRotationGizmo.md#_creategizmomesh)
- [\_handlePivot](PlaneRotationGizmo.md#_handlepivot)
- [\_matrixChanged](PlaneRotationGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](PlaneRotationGizmo.md#_setgizmomeshmaterial)
- [\_update](PlaneRotationGizmo.md#_update)
- [dispose](PlaneRotationGizmo.md#dispose)
- [setCustomMesh](PlaneRotationGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](PlaneRotationGizmo.md#gizmoaxispointerobserver)

## Constructors

### constructor

• **new PlaneRotationGizmo**(`planeNormal`, `color?`, `gizmoLayer?`, `tessellation?`, `parent?`, `useEulerRotation?`, `thickness?`)

Creates a PlaneRotationGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `planeNormal` | [`Vector3`](Vector3.md) | `undefined` | The normal of the plane which the gizmo will be able to rotate on |
| `color` | [`Color3`](Color3.md) | `undefined` | The color of the gizmo |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |
| `tessellation` | `number` | `32` | Amount of tessellation to be used when creating rotation circles |
| `parent` | [`Nullable`](../modules.md#nullable)[`RotationGizmo`](RotationGizmo.md) | `null` |  |
| `useEulerRotation` | `boolean` | `false` | Use and update Euler angle instead of quaternion |
| `thickness` | `number` | `1` | display gizmo axis thickness |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:116

## Properties

### \_angles

• `Private` **\_angles**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:61

___

### \_coloredMaterial

• `Private` **\_coloredMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:55

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

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:57

___

### \_dragging

• `Private` **\_dragging**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:60

___

### \_gizmoMesh

• `Private` **\_gizmoMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:58

___

### \_hoverMaterial

• `Private` **\_hoverMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:56

___

### \_interactionsEnabled

• `Protected` **\_interactionsEnabled**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_interactionsEnabled](Gizmo.md#_interactionsenabled)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:153

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:53

___

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:60

___

### \_parent

• `Private` **\_parent**: [`Nullable`](../modules.md#nullable)[`RotationGizmo`](RotationGizmo.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:54

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:30

___

### \_rootMesh

• **\_rootMesh**: [`Mesh`](Mesh.md)

The root mesh of the gizmo

#### Inherited from

[Gizmo](Gizmo.md).[_rootMesh](Gizmo.md#_rootmesh)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:48

___

### \_rotationDisplayPlane

• `Private` **\_rotationDisplayPlane**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:59

___

### \_rotationShaderMaterial

• `Private` **\_rotationShaderMaterial**: [`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:104

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

### angle

• **angle**: `number` = `0`

Accumulated relative angle value for rotation on the axis. Reset to 0 when a dragStart occurs

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:51

___

### dragBehavior

• **dragBehavior**: [`PointerDragBehavior`](PointerDragBehavior.md)

Drag behavior responsible for the gizmos dragging interactions

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:29

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Inherited from

[Gizmo](Gizmo.md).[gizmoLayer](Gizmo.md#gizmolayer)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:171

___

### onSnapObservable

• **onSnapObservable**: [`Observable`](Observable.md){ `snapDistance`: `number`  }

Event that fires each time the gizmo snaps to a new location.
* snapDistance is the the change in distance

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:40

___

### snapDistance

• **snapDistance**: `number` = `0`

Rotation distance in radians that the gizmo will snap to (Default: 0)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:35

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

### MaxDragAngle

▪ `Static` **MaxDragAngle**: `number`

The maximum angle between the camera and the rotation allowed for interaction
If a rotation plane appears 'flat', a lower value allows interaction.

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:46

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

### \_RotationGizmoFragmentShader

▪ `Static` `Private` **\_RotationGizmoFragmentShader**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:75

___

### \_RotationGizmoVertexShader

▪ `Static` `Private` **\_RotationGizmoVertexShader**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:63

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

### isEnabled

• `get` **isEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:392

• `set` **isEnabled**(`value`): `void`

If the gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:382

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

#### Overrides

[Gizmo](Gizmo.md).[_attachedNodeChanged](Gizmo.md#_attachednodechanged)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:373

___

### \_createGizmoMesh

▸ `Private` **_createGizmoMesh**(`parentMesh`, `thickness`, `tessellation`): `Object`

Create Geometry for Gizmo

#### Parameters

| Name | Type |
| :------ | :------ |
| `parentMesh` | [`AbstractMesh`](AbstractMesh.md) |
| `thickness` | `number` |
| `tessellation` | `number` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `collider` | [`Mesh`](Mesh.md) |
| `rotationMesh` | [`Mesh`](Mesh.md) |

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:342

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

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/planeRotationGizmo.ts:398

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

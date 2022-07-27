[@dev/core](../README.md) / [Exports](../modules.md) / LightGizmo

# Class: LightGizmo

Gizmo that enables viewing a light

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`LightGizmo`**

## Table of contents

### Constructors

- [constructor](LightGizmo.md#constructor)

### Properties

- [\_attachedMeshParent](LightGizmo.md#_attachedmeshparent)
- [\_cachedForward](LightGizmo.md#_cachedforward)
- [\_cachedPosition](LightGizmo.md#_cachedposition)
- [\_customMeshSet](LightGizmo.md#_custommeshset)
- [\_interactionsEnabled](LightGizmo.md#_interactionsenabled)
- [\_isHovered](LightGizmo.md#_ishovered)
- [\_light](LightGizmo.md#_light)
- [\_lightMesh](LightGizmo.md#_lightmesh)
- [\_material](LightGizmo.md#_material)
- [\_pointerObserver](LightGizmo.md#_pointerobserver)
- [\_rootMesh](LightGizmo.md#_rootmesh)
- [\_scaleRatio](LightGizmo.md#_scaleratio)
- [\_updateGizmoRotationToMatchAttachedMesh](LightGizmo.md#_updategizmorotationtomatchattachedmesh)
- [gizmoLayer](LightGizmo.md#gizmolayer)
- [onClickedObservable](LightGizmo.md#onclickedobservable)
- [updateGizmoPositionToMatchAttachedMesh](LightGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](LightGizmo.md#updatescale)
- [PreserveScaling](LightGizmo.md#preservescaling)
- [\_Scale](LightGizmo.md#_scale)

### Accessors

- [attachedMesh](LightGizmo.md#attachedmesh)
- [attachedNode](LightGizmo.md#attachednode)
- [customRotationQuaternion](LightGizmo.md#customrotationquaternion)
- [isHovered](LightGizmo.md#ishovered)
- [light](LightGizmo.md#light)
- [material](LightGizmo.md#material)
- [scaleRatio](LightGizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](LightGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](LightGizmo.md#_attachednodechanged)
- [\_handlePivot](LightGizmo.md#_handlepivot)
- [\_matrixChanged](LightGizmo.md#_matrixchanged)
- [\_setGizmoMeshMaterial](LightGizmo.md#_setgizmomeshmaterial)
- [dispose](LightGizmo.md#dispose)
- [setCustomMesh](LightGizmo.md#setcustommesh)
- [GizmoAxisPointerObserver](LightGizmo.md#gizmoaxispointerobserver)
- [\_CreateDirectionalLightMesh](LightGizmo.md#_createdirectionallightmesh)
- [\_CreateHemisphericLightMesh](LightGizmo.md#_createhemisphericlightmesh)
- [\_CreateLightLines](LightGizmo.md#_createlightlines)
- [\_CreatePointLightMesh](LightGizmo.md#_createpointlightmesh)
- [\_CreateSpotLightMesh](LightGizmo.md#_createspotlightmesh)

## Constructors

### constructor

• **new LightGizmo**(`gizmoLayer?`)

Creates a LightGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | The utility layer the gizmo will be added to |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:44

## Properties

### \_attachedMeshParent

• `Private` **\_attachedMeshParent**: [`TransformNode`](TransformNode.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:32

___

### \_cachedForward

• `Private` **\_cachedForward**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:31

___

### \_cachedPosition

• `Private` **\_cachedPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:30

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

### \_isHovered

• `Protected` **\_isHovered**: `boolean` = `false`

boolean updated by pointermove when a gizmo mesh is hovered

#### Inherited from

[Gizmo](Gizmo.md).[_isHovered](Gizmo.md#_ishovered)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:60

___

### \_light

• `Private` **\_light**: [`Nullable`](../modules.md#nullable)[`Light`](Light.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:65

___

### \_lightMesh

• `Private` **\_lightMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:28

___

### \_material

• `Private` **\_material**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:29

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:33

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

• **onClickedObservable**: [`Observable`](Observable.md)[`Light`](Light.md)

Event that fires each time the gizmo is clicked

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:38

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

▪ `Static` `Private` **\_Scale**: `number` = `0.007`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:193

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

Override attachedNode because lightgizmo only support attached mesh
It will return the attached mesh (if any) and setting an attached node will log
a warning

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Overrides

Gizmo.attachedNode

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:72

• `set` **attachedNode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Overrides

Gizmo.attachedNode

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:75

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

True when the mouse pointer is hovered a gizmo mesh

#### Returns

`boolean`

#### Inherited from

Gizmo.isHovered

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:82

___

### light

• `get` **light**(): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:134

• `set` **light**(`light`): `void`

The light that the gizmo is attached to

#### Parameters

| Name | Type |
| :------ | :------ |
| `light` | [`Nullable`](../modules.md#nullable)[`Light`](Light.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:82

___

### material

• `get` **material**(): [`StandardMaterial`](StandardMaterial.md)

Gets the material used to render the light gizmo

#### Returns

[`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:141

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

Disposes of the light gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:271

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

### \_CreateDirectionalLightMesh

▸ `Static` `Private` **_CreateDirectionalLightMesh**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:326

___

### \_CreateHemisphericLightMesh

▸ `Static` `Private` **_CreateHemisphericLightMesh**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:279

___

### \_CreateLightLines

▸ `Static` `Private` **_CreateLightLines**(`levels`, `scene`): [`Mesh`](Mesh.md)

Creates the lines for a light mesh

#### Parameters

| Name | Type |
| :------ | :------ |
| `levels` | `number` |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:200

___

### \_CreatePointLightMesh

▸ `Static` `Private` **_CreatePointLightMesh**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:295

___

### \_CreateSpotLightMesh

▸ `Static` `Private` **_CreateSpotLightMesh**(`scene`): [`Mesh`](Mesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/lightGizmo.ts:309

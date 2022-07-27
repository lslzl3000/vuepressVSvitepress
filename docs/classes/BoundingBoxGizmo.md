[@dev/core](../README.md) / [Exports](../modules.md) / BoundingBoxGizmo

# Class: BoundingBoxGizmo

Bounding box gizmo

## Hierarchy

- [`Gizmo`](Gizmo.md)

  ↳ **`BoundingBoxGizmo`**

## Table of contents

### Constructors

- [constructor](BoundingBoxGizmo.md#constructor)

### Properties

- [\_anchorMesh](BoundingBoxGizmo.md#_anchormesh)
- [\_axisFactor](BoundingBoxGizmo.md#_axisfactor)
- [\_boundingDimensions](BoundingBoxGizmo.md#_boundingdimensions)
- [\_coloredMaterial](BoundingBoxGizmo.md#_coloredmaterial)
- [\_customMeshSet](BoundingBoxGizmo.md#_custommeshset)
- [\_dragMesh](BoundingBoxGizmo.md#_dragmesh)
- [\_existingMeshScale](BoundingBoxGizmo.md#_existingmeshscale)
- [\_hoverColoredMaterial](BoundingBoxGizmo.md#_hovercoloredmaterial)
- [\_interactionsEnabled](BoundingBoxGizmo.md#_interactionsenabled)
- [\_isHovered](BoundingBoxGizmo.md#_ishovered)
- [\_lineBoundingBox](BoundingBoxGizmo.md#_lineboundingbox)
- [\_pointerDragBehavior](BoundingBoxGizmo.md#_pointerdragbehavior)
- [\_pointerObserver](BoundingBoxGizmo.md#_pointerobserver)
- [\_renderObserver](BoundingBoxGizmo.md#_renderobserver)
- [\_rootMesh](BoundingBoxGizmo.md#_rootmesh)
- [\_rotateSpheresParent](BoundingBoxGizmo.md#_rotatespheresparent)
- [\_scaleBoxesParent](BoundingBoxGizmo.md#_scaleboxesparent)
- [\_scaleDragSpeed](BoundingBoxGizmo.md#_scaledragspeed)
- [\_scaleRatio](BoundingBoxGizmo.md#_scaleratio)
- [\_tmpQuaternion](BoundingBoxGizmo.md#_tmpquaternion)
- [\_tmpRotationMatrix](BoundingBoxGizmo.md#_tmprotationmatrix)
- [\_tmpVector](BoundingBoxGizmo.md#_tmpvector)
- [\_updateGizmoRotationToMatchAttachedMesh](BoundingBoxGizmo.md#_updategizmorotationtomatchattachedmesh)
- [fixedDragMeshBoundsSize](BoundingBoxGizmo.md#fixeddragmeshboundssize)
- [fixedDragMeshScreenSize](BoundingBoxGizmo.md#fixeddragmeshscreensize)
- [fixedDragMeshScreenSizeDistanceFactor](BoundingBoxGizmo.md#fixeddragmeshscreensizedistancefactor)
- [gizmoLayer](BoundingBoxGizmo.md#gizmolayer)
- [ignoreChildren](BoundingBoxGizmo.md#ignorechildren)
- [includeChildPredicate](BoundingBoxGizmo.md#includechildpredicate)
- [onDragStartObservable](BoundingBoxGizmo.md#ondragstartobservable)
- [onRotationSphereDragEndObservable](BoundingBoxGizmo.md#onrotationspheredragendobservable)
- [onRotationSphereDragObservable](BoundingBoxGizmo.md#onrotationspheredragobservable)
- [onScaleBoxDragEndObservable](BoundingBoxGizmo.md#onscaleboxdragendobservable)
- [onScaleBoxDragObservable](BoundingBoxGizmo.md#onscaleboxdragobservable)
- [rotationSphereSize](BoundingBoxGizmo.md#rotationspheresize)
- [scaleBoxSize](BoundingBoxGizmo.md#scaleboxsize)
- [scalePivot](BoundingBoxGizmo.md#scalepivot)
- [updateGizmoPositionToMatchAttachedMesh](BoundingBoxGizmo.md#updategizmopositiontomatchattachedmesh)
- [updateScale](BoundingBoxGizmo.md#updatescale)
- [PreserveScaling](BoundingBoxGizmo.md#preservescaling)

### Accessors

- [attachedMesh](BoundingBoxGizmo.md#attachedmesh)
- [attachedNode](BoundingBoxGizmo.md#attachednode)
- [axisFactor](BoundingBoxGizmo.md#axisfactor)
- [customRotationQuaternion](BoundingBoxGizmo.md#customrotationquaternion)
- [isHovered](BoundingBoxGizmo.md#ishovered)
- [scaleDragSpeed](BoundingBoxGizmo.md#scaledragspeed)
- [scaleRatio](BoundingBoxGizmo.md#scaleratio)
- [updateGizmoRotationToMatchAttachedMesh](BoundingBoxGizmo.md#updategizmorotationtomatchattachedmesh)

### Methods

- [\_attachedNodeChanged](BoundingBoxGizmo.md#_attachednodechanged)
- [\_handlePivot](BoundingBoxGizmo.md#_handlepivot)
- [\_matrixChanged](BoundingBoxGizmo.md#_matrixchanged)
- [\_selectNode](BoundingBoxGizmo.md#_selectnode)
- [\_setGizmoMeshMaterial](BoundingBoxGizmo.md#_setgizmomeshmaterial)
- [\_update](BoundingBoxGizmo.md#_update)
- [\_updateDummy](BoundingBoxGizmo.md#_updatedummy)
- [\_updateRotationSpheres](BoundingBoxGizmo.md#_updaterotationspheres)
- [\_updateScaleBoxes](BoundingBoxGizmo.md#_updatescaleboxes)
- [dispose](BoundingBoxGizmo.md#dispose)
- [enableDragBehavior](BoundingBoxGizmo.md#enabledragbehavior)
- [getScaleBoxes](BoundingBoxGizmo.md#getscaleboxes)
- [setColor](BoundingBoxGizmo.md#setcolor)
- [setCustomMesh](BoundingBoxGizmo.md#setcustommesh)
- [setEnabledRotationAxis](BoundingBoxGizmo.md#setenabledrotationaxis)
- [setEnabledScaling](BoundingBoxGizmo.md#setenabledscaling)
- [updateBoundingBox](BoundingBoxGizmo.md#updateboundingbox)
- [GizmoAxisPointerObserver](BoundingBoxGizmo.md#gizmoaxispointerobserver)
- [MakeNotPickableAndWrapInBoundingBox](BoundingBoxGizmo.md#makenotpickableandwrapinboundingbox)

## Constructors

### constructor

• **new BoundingBoxGizmo**(`color?`, `gizmoLayer?`)

Creates an BoundingBoxGizmo

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | `undefined` | The color of the gizmo |
| `gizmoLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultKeepDepthUtilityLayer` | The utility layer the gizmo will be added to |

#### Overrides

[Gizmo](Gizmo.md).[constructor](Gizmo.md#constructor)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:182

## Properties

### \_anchorMesh

• `Private` **\_anchorMesh**: [`AbstractMesh`](AbstractMesh.md)

Mesh used as a pivot to rotate the attached node

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:153

___

### \_axisFactor

• `Private` **\_axisFactor**: [`Vector3`](Vector3.md)

Scale factor used for masking some axis

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:97

___

### \_boundingDimensions

• `Private` **\_boundingDimensions**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:31

___

### \_coloredMaterial

• `Private` **\_coloredMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:161

___

### \_customMeshSet

• `Protected` **\_customMeshSet**: `boolean` = `false`

If a custom mesh has been set (Default: false)

#### Inherited from

[Gizmo](Gizmo.md).[_customMeshSet](Gizmo.md#_custommeshset)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:89

___

### \_dragMesh

• `Private` **\_dragMesh**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:158

___

### \_existingMeshScale

• `Private` **\_existingMeshScale**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:155

___

### \_hoverColoredMaterial

• `Private` **\_hoverColoredMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:162

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

### \_lineBoundingBox

• `Private` **\_lineBoundingBox**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:28

___

### \_pointerDragBehavior

• `Private` **\_pointerDragBehavior**: [`PointerDragBehavior`](PointerDragBehavior.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:159

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:33

___

### \_renderObserver

• `Private` **\_renderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:32

___

### \_rootMesh

• **\_rootMesh**: [`Mesh`](Mesh.md)

The root mesh of the gizmo

#### Inherited from

[Gizmo](Gizmo.md).[_rootMesh](Gizmo.md#_rootmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:48

___

### \_rotateSpheresParent

• `Private` **\_rotateSpheresParent**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:29

___

### \_scaleBoxesParent

• `Private` **\_scaleBoxesParent**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:30

___

### \_scaleDragSpeed

• `Private` **\_scaleDragSpeed**: `number` = `0.2`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:34

___

### \_scaleRatio

• `Protected` **\_scaleRatio**: `number` = `1`

Ratio for the scale of the gizmo (Default: 1)

#### Inherited from

[Gizmo](Gizmo.md).[_scaleRatio](Gizmo.md#_scaleratio)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:55

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:36

___

### \_tmpRotationMatrix

• `Private` **\_tmpRotationMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:38

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:37

___

### \_updateGizmoRotationToMatchAttachedMesh

• `Protected` **\_updateGizmoRotationToMatchAttachedMesh**: `boolean` = `true`

#### Inherited from

[Gizmo](Gizmo.md).[_updateGizmoRotationToMatchAttachedMesh](Gizmo.md#_updategizmorotationtomatchattachedmesh)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:134

___

### fixedDragMeshBoundsSize

• **fixedDragMeshBoundsSize**: `boolean` = `false`

If set, the rotation spheres and scale boxes will increase in size based on the size of the bounding box
Note : fixedDragMeshScreenSize takes precedence over fixedDragMeshBoundsSize if both are true

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:65

___

### fixedDragMeshScreenSize

• **fixedDragMeshScreenSize**: `boolean` = `false`

If set, the rotation spheres and scale boxes will increase in size based on the distance away from the camera to have a consistent screen size (Default: false)
Note : fixedDragMeshScreenSize takes precedence over fixedDragMeshBoundsSize if both are true

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:60

___

### fixedDragMeshScreenSizeDistanceFactor

• **fixedDragMeshScreenSizeDistanceFactor**: `number` = `10`

The distance away from the object which the draggable meshes should appear world sized when fixedDragMeshScreenSize is set to true (default: 10)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:69

___

### gizmoLayer

• **gizmoLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md) = `UtilityLayerRenderer.DefaultUtilityLayer`

#### Inherited from

[Gizmo](Gizmo.md).[gizmoLayer](Gizmo.md#gizmolayer)

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:171

___

### ignoreChildren

• **ignoreChildren**: `boolean` = `false`

If child meshes should be ignored when calculating the bounding box. This should be set to true to avoid perf hits with heavily nested meshes (Default: false)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:42

___

### includeChildPredicate

• **includeChildPredicate**: [`Nullable`](../modules.md#nullable)(`abstractMesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` = `null`

Returns true if a descendant should be included when computing the bounding box. When null, all descendants are included. If ignoreChildren is set this will be ignored. (Default: null)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:46

___

### onDragStartObservable

• **onDragStartObservable**: [`Observable`](Observable.md){}

Fired when a rotation sphere or scale box is dragged

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:73

___

### onRotationSphereDragEndObservable

• **onRotationSphereDragEndObservable**: [`Observable`](Observable.md){}

Fired when a rotation sphere drag is ended

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:89

___

### onRotationSphereDragObservable

• **onRotationSphereDragObservable**: [`Observable`](Observable.md){}

Fired when a rotation sphere is dragged

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:85

___

### onScaleBoxDragEndObservable

• **onScaleBoxDragEndObservable**: [`Observable`](Observable.md){}

Fired when a scale box drag is ended

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:81

___

### onScaleBoxDragObservable

• **onScaleBoxDragObservable**: [`Observable`](Observable.md){}

Fired when a scale box is dragged

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:77

___

### rotationSphereSize

• **rotationSphereSize**: `number` = `0.1`

The size of the rotation spheres attached to the bounding box (Default: 0.1)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:51

___

### scaleBoxSize

• **scaleBoxSize**: `number` = `0.1`

The size of the scale boxes attached to the bounding box (Default: 0.1)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:55

___

### scalePivot

• **scalePivot**: [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) = `null`

Relative bounding box pivot used when scaling the attached node. When null object with scale from the opposite corner. 0.5,0.5,0.5 for center and 0.5,0,0.5 for bottom (Default: null)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:93

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

### axisFactor

• `get` **axisFactor**(): [`Vector3`](Vector3.md)

Gets the axis factor

#### Returns

[`Vector3`](Vector3.md)

the Vector3 factor value

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:130

• `set` **axisFactor**(`factor`): `void`

Sets the axis factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `factor` | [`Vector3`](Vector3.md) | the Vector3 value |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:103

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

True when the mouse pointer is hovered a gizmo mesh

#### Returns

`boolean`

#### Inherited from

Gizmo.isHovered

#### Defined in

packages/dev/core/src/Gizmos/gizmo.ts:82

___

### scaleDragSpeed

• `get` **scaleDragSpeed**(): `number`

Gets scale drag speed

#### Returns

`number`

the scale speed number

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:146

• `set` **scaleDragSpeed**(`value`): `void`

Sets scale drag speed value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | the new speed value |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:138

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
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[_attachedNodeChanged](Gizmo.md#_attachednodechanged)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:517

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

### \_selectNode

▸ `Private` **_selectNode**(`selectedMesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `selectedMesh` | [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:539

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

### \_updateDummy

▸ `Private` **_updateDummy**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:727

___

### \_updateRotationSpheres

▸ `Private` **_updateRotationSpheres**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:617

___

### \_updateScaleBoxes

▸ `Private` **_updateScaleBoxes**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:662

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[dispose](Gizmo.md#dispose)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:749

___

### enableDragBehavior

▸ **enableDragBehavior**(): `void`

Enables a pointer drag behavior on the bounding box of the gizmo

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:738

___

### getScaleBoxes

▸ **getScaleBoxes**(): [`AbstractMesh`](AbstractMesh.md)[]

returns an array containing all boxes used for scaling (in increasing x, y and z orders)

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:550

___

### setColor

▸ **setColor**(`color`): `void`

Sets the color of the bounding box gizmo

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | the color to set |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:168

___

### setCustomMesh

▸ **setCustomMesh**(): `void`

CustomMeshes are not supported by this gizmo

#### Returns

`void`

#### Overrides

[Gizmo](Gizmo.md).[setCustomMesh](Gizmo.md#setcustommesh)

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:817

___

### setEnabledRotationAxis

▸ **setEnabledRotationAxis**(`axis`): `void`

Enables rotation on the specified axis and disables rotation on the others

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | `string` | The list of axis that should be enabled (eg. "xy" or "xyz") |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:699

___

### setEnabledScaling

▸ **setEnabledScaling**(`enable`, `homogeneousScaling?`): `void`

Enables/disables scaling

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `enable` | `boolean` | `undefined` | if scaling should be enabled |
| `homogeneousScaling` | `boolean` | `false` | defines if scaling should only be homogeneous |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:716

___

### updateBoundingBox

▸ **updateBoundingBox**(): `void`

Updates the bounding box information for the Gizmo

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:557

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

___

### MakeNotPickableAndWrapInBoundingBox

▸ `Static` **MakeNotPickableAndWrapInBoundingBox**(`mesh`): [`Mesh`](Mesh.md)

Makes a mesh not pickable and wraps the mesh inside of a bounding box mesh that is pickable. (This is useful to avoid picking within complex geometry)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | the mesh to wrap in the bounding box mesh and make not pickable |

#### Returns

[`Mesh`](Mesh.md)

the bounding box mesh with the passed in mesh as a child

#### Defined in

packages/dev/core/src/Gizmos/boundingBoxGizmo.ts:766

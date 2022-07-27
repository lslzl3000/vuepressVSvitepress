[@dev/core](../README.md) / [Exports](../modules.md) / GizmoManager

# Class: GizmoManager

Helps setup gizmo's in the scene to rotate/scale/position nodes

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](GizmoManager.md#constructor)

### Properties

- [\_attachedMesh](GizmoManager.md#_attachedmesh)
- [\_attachedNode](GizmoManager.md#_attachednode)
- [\_boundingBoxColor](GizmoManager.md#_boundingboxcolor)
- [\_defaultKeepDepthUtilityLayer](GizmoManager.md#_defaultkeepdepthutilitylayer)
- [\_defaultUtilityLayer](GizmoManager.md#_defaultutilitylayer)
- [\_gizmoAxisCache](GizmoManager.md#_gizmoaxiscache)
- [\_gizmosEnabled](GizmoManager.md#_gizmosenabled)
- [\_pointerObservers](GizmoManager.md#_pointerobservers)
- [\_scaleRatio](GizmoManager.md#_scaleratio)
- [\_thickness](GizmoManager.md#_thickness)
- [attachableMeshes](GizmoManager.md#attachablemeshes)
- [attachableNodes](GizmoManager.md#attachablenodes)
- [boundingBoxDragBehavior](GizmoManager.md#boundingboxdragbehavior)
- [clearGizmoOnEmptyPointerEvent](GizmoManager.md#cleargizmoonemptypointerevent)
- [enableAutoPicking](GizmoManager.md#enableautopicking)
- [gizmos](GizmoManager.md#gizmos)
- [onAttachedToMeshObservable](GizmoManager.md#onattachedtomeshobservable)
- [onAttachedToNodeObservable](GizmoManager.md#onattachedtonodeobservable)
- [usePointerToAttachGizmos](GizmoManager.md#usepointertoattachgizmos)

### Accessors

- [boundingBoxGizmoEnabled](GizmoManager.md#boundingboxgizmoenabled)
- [isHovered](GizmoManager.md#ishovered)
- [keepDepthUtilityLayer](GizmoManager.md#keepdepthutilitylayer)
- [positionGizmoEnabled](GizmoManager.md#positiongizmoenabled)
- [rotationGizmoEnabled](GizmoManager.md#rotationgizmoenabled)
- [scaleGizmoEnabled](GizmoManager.md#scalegizmoenabled)
- [scaleRatio](GizmoManager.md#scaleratio)
- [utilityLayer](GizmoManager.md#utilitylayer)

### Methods

- [\_attachToMeshPointerObserver](GizmoManager.md#_attachtomeshpointerobserver)
- [addToAxisCache](GizmoManager.md#addtoaxiscache)
- [attachToMesh](GizmoManager.md#attachtomesh)
- [attachToNode](GizmoManager.md#attachtonode)
- [dispose](GizmoManager.md#dispose)

## Constructors

### constructor

• **new GizmoManager**(`_scene`, `thickness?`, `utilityLayer?`, `keepDepthUtilityLayer?`)

Instantiates a gizmo manager

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `_scene` | [`Scene`](Scene.md) | `undefined` | the scene to overlay the gizmos on top of |
| `thickness` | `number` | `1` | display gizmo axis thickness |
| `utilityLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultUtilityLayer` | the layer where gizmos are rendered |
| `keepDepthUtilityLayer` | [`UtilityLayerRenderer`](UtilityLayerRenderer.md) | `UtilityLayerRenderer.DefaultKeepDepthUtilityLayer` | the layer where occluded gizmos are rendered |

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:126

## Properties

### \_attachedMesh

• `Private` **\_attachedMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:48

___

### \_attachedNode

• `Private` **\_attachedNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:49

___

### \_boundingBoxColor

• `Private` **\_boundingBoxColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:50

___

### \_defaultKeepDepthUtilityLayer

• `Private` **\_defaultKeepDepthUtilityLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:52

___

### \_defaultUtilityLayer

• `Private` **\_defaultUtilityLayer**: [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:51

___

### \_gizmoAxisCache

• `Private` **\_gizmoAxisCache**: `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md)

Node Caching for quick lookup

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:57

___

### \_gizmosEnabled

• `Private` **\_gizmosEnabled**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `boundingBoxGizmo` | `boolean` |
| `positionGizmo` | `boolean` |
| `rotationGizmo` | `boolean` |
| `scaleGizmo` | `boolean` |

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:46

___

### \_pointerObservers

• `Private` **\_pointerObservers**: [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:47

___

### \_scaleRatio

• `Private` **\_scaleRatio**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:54

___

### \_thickness

• `Private` **\_thickness**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:53

___

### attachableMeshes

• **attachableMeshes**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] = `null`

Array of meshes which will have the gizmo attached when a pointer selected them. If null, all meshes are attachable. (Default: null)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:65

___

### attachableNodes

• **attachableNodes**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md)[] = `null`

Array of nodes which will have the gizmo attached when a pointer selected them. If null, all nodes are attachable. (Default: null)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:69

___

### boundingBoxDragBehavior

• **boundingBoxDragBehavior**: [`SixDofDragBehavior`](SixDofDragBehavior.md)

When bounding box gizmo is enabled, this can be used to track drag/end events

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:61

___

### clearGizmoOnEmptyPointerEvent

• **clearGizmoOnEmptyPointerEvent**: `boolean` = `false`

When true, the gizmo will be detached from the current object when a pointer down occurs with an empty picked mesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:35

___

### enableAutoPicking

• **enableAutoPicking**: `boolean` = `true`

When true (default), picking to attach a new mesh is enabled. This works in sync with inspector autopicking.

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:38

___

### gizmos

• **gizmos**: `Object`

Gizmo's created by the gizmo manager, gizmo will be null until gizmo has been enabled for the first time

#### Type declaration

| Name | Type |
| :------ | :------ |
| `boundingBoxGizmo` | [`Nullable`](../modules.md#nullable)[`BoundingBoxGizmo`](BoundingBoxGizmo.md) |
| `positionGizmo` | [`Nullable`](../modules.md#nullable)[`PositionGizmo`](PositionGizmo.md) |
| `rotationGizmo` | [`Nullable`](../modules.md#nullable)[`RotationGizmo`](RotationGizmo.md) |
| `scaleGizmo` | [`Nullable`](../modules.md#nullable)[`ScaleGizmo`](ScaleGizmo.md) |

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:27

___

### onAttachedToMeshObservable

• **onAttachedToMeshObservable**: [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Fires an event when the manager is attached to a mesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:41

___

### onAttachedToNodeObservable

• **onAttachedToNodeObservable**: [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Fires an event when the manager is attached to a node

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:44

___

### usePointerToAttachGizmos

• **usePointerToAttachGizmos**: `boolean` = `true`

If pointer events should perform attaching/detaching a gizmo, if false this can be done manually via attachToMesh/attachToNode. (Default: true)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:73

## Accessors

### boundingBoxGizmoEnabled

• `get` **boundingBoxGizmoEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:335

• `set` **boundingBoxGizmoEnabled**(`value`): `void`

If the boundingBox gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:309

___

### isHovered

• `get` **isHovered**(): `boolean`

True when the mouse pointer is hovering a gizmo mesh

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:92

___

### keepDepthUtilityLayer

• `get` **keepDepthUtilityLayer**(): [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

Utility layer that the bounding box gizmo belongs to

#### Returns

[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:78

___

### positionGizmoEnabled

• `get` **positionGizmoEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:263

• `set` **positionGizmoEnabled**(`value`): `void`

If the position gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:248

___

### rotationGizmoEnabled

• `get` **rotationGizmoEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:284

• `set` **rotationGizmoEnabled**(`value`): `void`

If the rotation gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:269

___

### scaleGizmoEnabled

• `get` **scaleGizmoEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:303

• `set` **scaleGizmoEnabled**(`value`): `void`

If the scale gizmo is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:290

___

### scaleRatio

• `get` **scaleRatio**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:115

• `set` **scaleRatio**(`value`): `void`

Ratio for the scale of the gizmo (Default: 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:107

___

### utilityLayer

• `get` **utilityLayer**(): [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

Utility layer that all gizmos besides bounding box belong to

#### Returns

[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:85

## Methods

### \_attachToMeshPointerObserver

▸ `Private` **_attachToMeshPointerObserver**(`scene`): [`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

Subscribes to pointer down events, for attaching and detaching mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene layer the observer will be added to |

#### Returns

[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:147

___

### addToAxisCache

▸ **addToAxisCache**(`gizmoAxisCache`): `void`

Builds Gizmo Axis Cache to enable features such as hover state preservation and graying out other axis during manipulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gizmoAxisCache` | `Map`[`Mesh`](Mesh.md), [`GizmoAxisCache`](../interfaces/GizmoAxisCache.md) | Gizmo axis definition used for reactive gizmo UI |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:343

___

### attachToMesh

▸ **attachToMesh**(`mesh`): `void`

Attaches a set of gizmos to the specified mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | The mesh the gizmo's should be attached to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:199

___

### attachToNode

▸ **attachToNode**(`node`): `void`

Attaches a set of gizmos to the specified node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | The node the gizmo's should be attached to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:224

___

### dispose

▸ **dispose**(): `void`

Disposes of the gizmo manager

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmoManager.ts:354

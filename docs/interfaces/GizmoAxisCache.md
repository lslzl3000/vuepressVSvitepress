[@dev/core](../README.md) / [Exports](../modules.md) / GizmoAxisCache

# Interface: GizmoAxisCache

Cache built by each axis. Used for managing state between all elements of gizmo for enhanced UI

## Table of contents

### Properties

- [active](GizmoAxisCache.md#active)
- [colliderMeshes](GizmoAxisCache.md#collidermeshes)
- [disableMaterial](GizmoAxisCache.md#disablematerial)
- [dragBehavior](GizmoAxisCache.md#dragbehavior)
- [gizmoMeshes](GizmoAxisCache.md#gizmomeshes)
- [hoverMaterial](GizmoAxisCache.md#hovermaterial)
- [material](GizmoAxisCache.md#material)

## Properties

### active

• **active**: `boolean`

Used to indicate Active state of the Gizmo

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:37

___

### colliderMeshes

• **colliderMeshes**: [`Mesh`](../classes/Mesh.md)[]

Mesh used to detect user interaction with Gizmo

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:29

___

### disableMaterial

• **disableMaterial**: [`StandardMaterial`](../classes/StandardMaterial.md)

Material used to indicate disabled state of the Gizmo

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:35

___

### dragBehavior

• **dragBehavior**: [`PointerDragBehavior`](../classes/PointerDragBehavior.md)

DragBehavior

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:39

___

### gizmoMeshes

• **gizmoMeshes**: [`Mesh`](../classes/Mesh.md)[]

Mesh used to render the Gizmo

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:27

___

### hoverMaterial

• **hoverMaterial**: [`StandardMaterial`](../classes/StandardMaterial.md)

Material used to indicate hover state of the Gizmo

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:33

___

### material

• **material**: [`StandardMaterial`](../classes/StandardMaterial.md)

Material used to indicate color of gizmo mesh

#### Defined in

https://github.com/babylon.js/core/src/Gizmos/gizmo.ts:31

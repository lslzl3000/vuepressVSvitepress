[@dev/core](../README.md) / [Exports](../modules.md) / OutlineRenderer

# Class: OutlineRenderer

This class is responsible to draw the outline/overlay of meshes.
It should not be used directly but through the available method on mesh.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](OutlineRenderer.md#constructor)

### Properties

- [\_engine](OutlineRenderer.md#_engine)
- [\_passIdForDrawWrapper](OutlineRenderer.md#_passidfordrawwrapper)
- [\_savedDepthWrite](OutlineRenderer.md#_saveddepthwrite)
- [name](OutlineRenderer.md#name)
- [scene](OutlineRenderer.md#scene)
- [zOffset](OutlineRenderer.md#zoffset)
- [zOffsetUnits](OutlineRenderer.md#zoffsetunits)
- [\_StencilReference](OutlineRenderer.md#_stencilreference)

### Methods

- [\_afterRenderingMesh](OutlineRenderer.md#_afterrenderingmesh)
- [\_beforeRenderingMesh](OutlineRenderer.md#_beforerenderingmesh)
- [dispose](OutlineRenderer.md#dispose)
- [isReady](OutlineRenderer.md#isready)
- [rebuild](OutlineRenderer.md#rebuild)
- [register](OutlineRenderer.md#register)
- [render](OutlineRenderer.md#render)

## Constructors

### constructor

• **new OutlineRenderer**(`scene`)

Instantiates a new outline renderer. (There could be only one per scene).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene it belongs to |

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:127

## Properties

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:119

___

### \_passIdForDrawWrapper

• `Private` **\_passIdForDrawWrapper**: `number`[]

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:121

___

### \_savedDepthWrite

• `Private` **\_savedDepthWrite**: `boolean`

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:120

___

### name

• **name**: `string` = `SceneComponentConstants.NAME_OUTLINERENDERER`

The name of the component. Each component must have a unique name.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:102

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:107

___

### zOffset

• **zOffset**: `number` = `1`

Defines a zOffset default Factor to prevent zFighting between the overlay and the mesh.

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:112

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `4`

Defines a zOffset default Unit to prevent zFighting between the overlay and the mesh.

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:117

___

### \_StencilReference

▪ `Static` `Private` **\_StencilReference**: `number` = `0x04`

Stencil value used to avoid outline being seen within the mesh when the mesh is transparent

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:98

## Methods

### \_afterRenderingMesh

▸ `Private` **_afterRenderingMesh**(`mesh`, `subMesh`, `batch`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `batch` | `_InstancesBatch` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:429

___

### \_beforeRenderingMesh

▸ `Private` **_beforeRenderingMesh**(`mesh`, `subMesh`, `batch`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `batch` | `_InstancesBatch` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:394

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:156

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`, `renderPassId?`): `boolean`

Returns whether or not the outline renderer is ready for a given submesh.
All the dependencies e.g. submeshes, texture, effect... mus be ready

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | Defines the submesh to check readiness for |
| `useInstances` | `boolean` | Defines whether wee are trying to render instances or not |
| `renderPassId?` | `number` | Render pass id to use to render the mesh |

#### Returns

`boolean`

true if ready otherwise false

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:255

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:149

___

### register

▸ **register**(): `void`

Register the component to one instance of a scene.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:140

___

### render

▸ **render**(`subMesh`, `batch`, `useOverlay?`, `renderPassId?`): `void`

Renders the outline in the canvas.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | `undefined` | Defines the sumesh to render |
| `batch` | `_InstancesBatch` | `undefined` | Defines the batch of meshes in case of instances |
| `useOverlay` | `boolean` | `false` | Defines if the rendering is for the overlay or the outline |
| `renderPassId?` | `number` | `undefined` | Render pass id to use to render the mesh |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:169

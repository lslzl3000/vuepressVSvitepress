[@dev/core](../README.md) / [Exports](../modules.md) / PrePassRendererSceneComponent

# Class: PrePassRendererSceneComponent

Defines the Geometry Buffer scene component responsible to manage a G-Buffer useful
in several rendering techniques.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](PrePassRendererSceneComponent.md#constructor)

### Properties

- [name](PrePassRendererSceneComponent.md#name)
- [scene](PrePassRendererSceneComponent.md#scene)

### Methods

- [\_afterCameraDraw](PrePassRendererSceneComponent.md#_aftercameradraw)
- [\_afterRenderTargetDraw](PrePassRendererSceneComponent.md#_afterrendertargetdraw)
- [\_afterRenderingMeshStage](PrePassRendererSceneComponent.md#_afterrenderingmeshstage)
- [\_beforeCameraDraw](PrePassRendererSceneComponent.md#_beforecameradraw)
- [\_beforeClearStage](PrePassRendererSceneComponent.md#_beforeclearstage)
- [\_beforeRenderTargetClearStage](PrePassRendererSceneComponent.md#_beforerendertargetclearstage)
- [\_beforeRenderTargetDraw](PrePassRendererSceneComponent.md#_beforerendertargetdraw)
- [\_beforeRenderingMeshStage](PrePassRendererSceneComponent.md#_beforerenderingmeshstage)
- [dispose](PrePassRendererSceneComponent.md#dispose)
- [rebuild](PrePassRendererSceneComponent.md#rebuild)
- [register](PrePassRendererSceneComponent.md#register)

## Constructors

### constructor

• **new PrePassRendererSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:101

## Properties

### name

• `Readonly` **name**: ``"PrePassRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:90

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:95

## Methods

### \_afterCameraDraw

▸ `Private` **_afterCameraDraw**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:151

___

### \_afterRenderTargetDraw

▸ `Private` **_afterRenderTargetDraw**(`renderTarget`, `faceIndex?`, `layer?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTarget` | [`RenderTargetTexture`](RenderTargetTexture.md) |
| `faceIndex?` | `number` |
| `layer?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:128

___

### \_afterRenderingMeshStage

▸ `Private` **_afterRenderingMeshStage**(`mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:176

___

### \_beforeCameraDraw

▸ `Private` **_beforeCameraDraw**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:144

___

### \_beforeClearStage

▸ `Private` **_beforeClearStage**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:157

___

### \_beforeRenderTargetClearStage

▸ `Private` **_beforeRenderTargetClearStage**(`renderTarget`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTarget` | [`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:134

___

### \_beforeRenderTargetDraw

▸ `Private` **_beforeRenderTargetDraw**(`renderTarget`, `faceIndex?`, `layer?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTarget` | [`RenderTargetTexture`](RenderTargetTexture.md) |
| `faceIndex?` | `number` |
| `layer?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:121

___

### \_beforeRenderingMeshStage

▸ `Private` **_beforeRenderingMeshStage**(`mesh`, `subMesh`, `batch`, `effect`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `batch` | `_InstancesBatch` |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:164

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:199

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

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:188

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:108

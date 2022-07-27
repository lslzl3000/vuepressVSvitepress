[@dev/core](../README.md) / [Exports](../modules.md) / DepthRenderer

# Class: DepthRenderer

This represents a depth renderer in Babylon.
A depth renderer will render to it's depth map every frame which can be displayed or used in post processing

## Table of contents

### Constructors

- [constructor](DepthRenderer.md#constructor)

### Properties

- [\_camera](DepthRenderer.md#_camera)
- [\_clearColor](DepthRenderer.md#_clearcolor)
- [\_depthMap](DepthRenderer.md#_depthmap)
- [\_scene](DepthRenderer.md#_scene)
- [\_storeNonLinearDepth](DepthRenderer.md#_storenonlineardepth)
- [enabled](DepthRenderer.md#enabled)
- [forceDepthWriteTransparentMeshes](DepthRenderer.md#forcedepthwritetransparentmeshes)
- [isPacked](DepthRenderer.md#ispacked)
- [useOnlyInActiveCamera](DepthRenderer.md#useonlyinactivecamera)

### Methods

- [dispose](DepthRenderer.md#dispose)
- [getDepthMap](DepthRenderer.md#getdepthmap)
- [isReady](DepthRenderer.md#isready)
- [setMaterialForRendering](DepthRenderer.md#setmaterialforrendering)

## Constructors

### constructor

• **new DepthRenderer**(`scene`, `type?`, `camera?`, `storeNonLinearDepth?`, `samplingMode?`)

Instantiates a depth renderer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the renderer belongs to |
| `type` | `number` | `Constants.TEXTURETYPE_FLOAT` | The texture type of the depth map (default: Engine.TEXTURETYPE_FLOAT) |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `null` | The camera to be used to render the depth map (default: scene's active camera) |
| `storeNonLinearDepth` | `boolean` | `false` | Defines whether the depth is stored linearly like in Babylon Shadows or directly like glFragCoord.z |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | The sampling mode to be used with the render target (Linear, Nearest...) |

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:74

## Properties

### \_camera

• `Private` **\_camera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:34

___

### \_clearColor

• `Private` `Readonly` **\_clearColor**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:29

___

### \_depthMap

• `Private` **\_depthMap**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:27

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:26

___

### \_storeNonLinearDepth

• `Private` `Readonly` **\_storeNonLinearDepth**: `boolean`

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:28

___

### enabled

• **enabled**: `boolean` = `true`

Enable or disable the depth renderer. When disabled, the depth texture is not updated

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:37

___

### forceDepthWriteTransparentMeshes

• **forceDepthWriteTransparentMeshes**: `boolean` = `false`

Force writing the transparent objects into the depth map

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:40

___

### isPacked

• `Readonly` **isPacked**: `boolean`

Get if the depth renderer is using packed depth or not

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:32

___

### useOnlyInActiveCamera

• **useOnlyInActiveCamera**: `boolean` = `false`

Specifies that the depth renderer will only be used within
the camera it is created for.
This can help forcing its rendering during the camera processing.

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:47

## Methods

### dispose

▸ **dispose**(): `void`

Disposes of the depth renderer.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:501

___

### getDepthMap

▸ **getDepthMap**(): [`RenderTargetTexture`](RenderTargetTexture.md)

Gets the texture which the depth map will be written to.

#### Returns

[`RenderTargetTexture`](RenderTargetTexture.md)

The depth map texture

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:494

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`): `boolean`

Creates the depth rendering effect and checks if the effect is ready.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | The submesh to be used to render the depth map of |
| `useInstances` | `boolean` | If multiple world instances should be used |

#### Returns

`boolean`

if the depth renderer is ready to render the depth map

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:335

___

### setMaterialForRendering

▸ **setMaterialForRendering**(`mesh`, `material?`): `void`

Sets a specific material to be used to render a mesh/a list of meshes by the depth renderer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) \| [`AbstractMesh`](AbstractMesh.md)[] | mesh or array of meshes |
| `material?` | [`Material`](Material.md) | material to use by the depth render when rendering the mesh(es). If undefined is passed, the specific material created by the depth renderer will be used. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthRenderer.ts:62

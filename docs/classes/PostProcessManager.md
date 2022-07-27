[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessManager

# Class: PostProcessManager

PostProcessManager is used to manage one or more post processes or post process pipelines
See https://doc.babylonjs.com/how_to/how_to_use_postprocesses

## Table of contents

### Constructors

- [constructor](PostProcessManager.md#constructor)

### Properties

- [\_indexBuffer](PostProcessManager.md#_indexbuffer)
- [\_scene](PostProcessManager.md#_scene)
- [\_vertexBuffers](PostProcessManager.md#_vertexbuffers)

### Methods

- [\_buildIndexBuffer](PostProcessManager.md#_buildindexbuffer)
- [\_prepareBuffers](PostProcessManager.md#_preparebuffers)
- [directRender](PostProcessManager.md#directrender)
- [dispose](PostProcessManager.md#dispose)

## Constructors

### constructor

• **new PostProcessManager**(`scene`)

Creates a new instance PostProcess

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene that the post process is associated with. |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:24

## Properties

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:17

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:16

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:18

## Methods

### \_buildIndexBuffer

▸ `Private` **_buildIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:45

___

### \_prepareBuffers

▸ `Private` **_prepareBuffers**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:28

___

### directRender

▸ **directRender**(`postProcesses`, `targetTexture?`, `forceFullscreenViewport?`, `faceIndex?`, `lodLevel?`, `doNotBindFrambuffer?`): `void`

Manually render a set of post processes to a texture.
Please note, the frame buffer won't be unbound after the call in case you have more render to do.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `postProcesses` | [`PostProcess`](PostProcess.md)[] | `undefined` | An array of post processes to be run. |
| `targetTexture` | [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) | `null` | The render target wrapper to render to. |
| `forceFullscreenViewport` | `boolean` | `false` | force gl.viewport to be full screen eg. 0,0,textureWidth,textureHeight |
| `faceIndex` | `number` | `0` | defines the face to render to if a cubemap is defined as the target |
| `lodLevel` | `number` | `0` | defines which lod of the texture to render to |
| `doNotBindFrambuffer` | `boolean` | `false` | If set to true, assumes that the framebuffer has been bound previously |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:109

___

### dispose

▸ **dispose**(): `void`

Disposes of the post process manager.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcessManager.ts:228

[@dev/core](../README.md) / [Exports](../modules.md) / RenderTargetWrapper

# Class: RenderTargetWrapper

Wrapper around a render target (either single or multi textures)

## Table of contents

### Constructors

- [constructor](RenderTargetWrapper.md#constructor)

### Properties

- [\_engine](RenderTargetWrapper.md#_engine)
- [\_isCube](RenderTargetWrapper.md#_iscube)
- [\_isMulti](RenderTargetWrapper.md#_ismulti)
- [\_size](RenderTargetWrapper.md#_size)
- [\_textures](RenderTargetWrapper.md#_textures)

### Accessors

- [depthStencilTexture](RenderTargetWrapper.md#depthstenciltexture)
- [depthStencilTextureWithStencil](RenderTargetWrapper.md#depthstenciltexturewithstencil)
- [height](RenderTargetWrapper.md#height)
- [is2DArray](RenderTargetWrapper.md#is2darray)
- [isCube](RenderTargetWrapper.md#iscube)
- [isMulti](RenderTargetWrapper.md#ismulti)
- [layers](RenderTargetWrapper.md#layers)
- [samples](RenderTargetWrapper.md#samples)
- [size](RenderTargetWrapper.md#size)
- [texture](RenderTargetWrapper.md#texture)
- [textures](RenderTargetWrapper.md#textures)
- [width](RenderTargetWrapper.md#width)

### Methods

- [\_cloneRenderTargetWrapper](RenderTargetWrapper.md#_clonerendertargetwrapper)
- [\_swapRenderTargetWrapper](RenderTargetWrapper.md#_swaprendertargetwrapper)
- [createDepthStencilTexture](RenderTargetWrapper.md#createdepthstenciltexture)
- [dispose](RenderTargetWrapper.md#dispose)
- [releaseTextures](RenderTargetWrapper.md#releasetextures)
- [setSamples](RenderTargetWrapper.md#setsamples)
- [setTexture](RenderTargetWrapper.md#settexture)
- [setTextures](RenderTargetWrapper.md#settextures)

## Constructors

### constructor

• **new RenderTargetWrapper**(`isMulti`, `isCube`, `size`, `engine`)

Initializes the render target wrapper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `isMulti` | `boolean` | true if the wrapper is a multi render target |
| `isCube` | `boolean` | true if the wrapper should render to a cube texture |
| `size` | `TextureSize` | size of the render target (width/height/layers) |
| `engine` | [`ThinEngine`](ThinEngine.md) | engine used to create the render target |

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:148

## Properties

### \_engine

• `Protected` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:22

___

### \_isCube

• `Private` **\_isCube**: `boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:24

___

### \_isMulti

• `Private` **\_isMulti**: `boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:25

___

### \_size

• `Private` **\_size**: `TextureSize`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:23

___

### \_textures

• `Private` **\_textures**: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)[] = `null`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:26

## Accessors

### depthStencilTexture

• `get` **depthStencilTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Gets the depth/stencil texture (if created by a createDepthStencilTexture() call)

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:43

___

### depthStencilTextureWithStencil

• `get` **depthStencilTextureWithStencil**(): `boolean`

Indicates if the depth/stencil texture has a stencil aspect

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:50

___

### height

• `get` **height**(): `number`

Gets the height of the render target wrapper

#### Returns

`number`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:92

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Defines if the render target wrapper is for a single or an array of textures

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:71

___

### isCube

• `get` **isCube**(): `boolean`

Defines if the render target wrapper is for a cube texture or if false a 2d texture

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:57

___

### isMulti

• `get` **isMulti**(): `boolean`

Defines if the render target wrapper is for a single or multi target render wrapper

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:64

___

### layers

• `get` **layers**(): `number`

Gets the number of layers of the render target wrapper (only used if is2DArray is true)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:99

___

### samples

• `get` **samples**(): `number`

Gets the sample count of the render target

#### Returns

`number`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:120

___

### size

• `get` **size**(): `number`

Gets the size of the render target wrapper (used for cubes, as width=height in this case)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:78

___

### texture

• `get` **texture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Gets the render texture. If this is a multi render target, gets the first texture

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:106

___

### textures

• `get` **textures**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)[]

Gets the list of render textures. If we are not in a multi render target, the list will be null (use the texture getter instead)

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)[]

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:113

___

### width

• `get` **width**(): `number`

Gets the width of the render target wrapper

#### Returns

`number`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:85

## Methods

### \_cloneRenderTargetWrapper

▸ `Protected` **_cloneRenderTargetWrapper**(): [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:250

___

### \_swapRenderTargetWrapper

▸ `Protected` **_swapRenderTargetWrapper**(`target`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | [`RenderTargetWrapper`](RenderTargetWrapper.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:318

___

### createDepthStencilTexture

▸ **createDepthStencilTexture**(`comparisonFunction?`, `bilinearFiltering?`, `generateStencil?`, `samples?`, `format?`): [`InternalTexture`](InternalTexture.md)

Creates the depth/stencil texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `comparisonFunction` | `number` | `0` | Comparison function to use for the texture |
| `bilinearFiltering` | `boolean` | `true` | true if bilinear filtering should be used when sampling the texture |
| `generateStencil` | `boolean` | `false` | true if the stencil aspect should also be created |
| `samples` | `number` | `1` | sample count to use when creating the texture |
| `format` | `number` | `Constants.TEXTUREFORMAT_DEPTH32_FLOAT` | format of the depth texture |

#### Returns

[`InternalTexture`](InternalTexture.md)

the depth/stencil created texture

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:196

___

### dispose

▸ **dispose**(`disposeOnlyFramebuffers?`): `void`

Disposes the whole render target wrapper

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposeOnlyFramebuffers` | `boolean` | `false` | true if only the frame buffers should be released (used for the WebGL engine). If false, all the textures will also be released |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:374

___

### releaseTextures

▸ **releaseTextures**(): `void`

Releases the internal render textures

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:361

___

### setSamples

▸ **setSamples**(`value`, `initializeBuffers?`, `force?`): `number`

Sets the sample count of the render target

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `value` | `number` | `undefined` | sample count |
| `initializeBuffers` | `boolean` | `true` | If set to true, the engine will make an initializing call to drawBuffers (only used when isMulti=true). |
| `force` | `boolean` | `false` | true to force calling the update sample count engine function even if the current sample count is equal to value |

#### Returns

`number`

the sample count that has been set

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:131

___

### setTexture

▸ **setTexture**(`texture`, `index?`, `disposePrevious?`): `void`

Set a texture in the textures array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | the texture to set |
| `index` | `number` | `0` | the index in the textures array to set |
| `disposePrevious` | `boolean` | `true` | If this function should dispose the previous texture |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:176

___

### setTextures

▸ **setTextures**(`textures`): `void`

Sets the render target texture(s)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `textures` | ``null`` \| [`InternalTexture`](InternalTexture.md) \| [`InternalTexture`](InternalTexture.md)[] | texture(s) to set |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/renderTargetWrapper.ts:160

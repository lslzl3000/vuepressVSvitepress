[@dev/core](../README.md) / [Exports](../modules.md) / ThinRenderTargetTexture

# Class: ThinRenderTargetTexture

This is a tiny helper class to wrap a RenderTargetWrapper in a texture
usable as the input of an effect.

## Hierarchy

- [`ThinTexture`](ThinTexture.md)

  ↳ **`ThinRenderTargetTexture`**

## Implements

- [`IRenderTargetTexture`](../interfaces/IRenderTargetTexture.md)

## Table of contents

### Constructors

- [constructor](ThinRenderTargetTexture.md#constructor)

### Properties

- [\_engine](ThinRenderTargetTexture.md#_engine)
- [\_renderTarget](ThinRenderTargetTexture.md#_rendertarget)
- [\_renderTargetOptions](ThinRenderTargetTexture.md#_rendertargetoptions)
- [\_size](ThinRenderTargetTexture.md#_size)
- [\_wrapU](ThinRenderTargetTexture.md#_wrapu)
- [\_wrapV](ThinRenderTargetTexture.md#_wrapv)
- [anisotropicFilteringLevel](ThinRenderTargetTexture.md#anisotropicfilteringlevel)
- [delayLoadState](ThinRenderTargetTexture.md#delayloadstate)
- [wrapR](ThinRenderTargetTexture.md#wrapr)

### Accessors

- [coordinatesMode](ThinRenderTargetTexture.md#coordinatesmode)
- [is2DArray](ThinRenderTargetTexture.md#is2darray)
- [is3D](ThinRenderTargetTexture.md#is3d)
- [isCube](ThinRenderTargetTexture.md#iscube)
- [renderTarget](ThinRenderTargetTexture.md#rendertarget)
- [samplingMode](ThinRenderTargetTexture.md#samplingmode)
- [wrapU](ThinRenderTargetTexture.md#wrapu)
- [wrapV](ThinRenderTargetTexture.md#wrapv)

### Methods

- [delayLoad](ThinRenderTargetTexture.md#delayload)
- [dispose](ThinRenderTargetTexture.md#dispose)
- [getBaseSize](ThinRenderTargetTexture.md#getbasesize)
- [getClassName](ThinRenderTargetTexture.md#getclassname)
- [getInternalTexture](ThinRenderTargetTexture.md#getinternaltexture)
- [getSize](ThinRenderTargetTexture.md#getsize)
- [isReady](ThinRenderTargetTexture.md#isready)
- [releaseInternalTexture](ThinRenderTargetTexture.md#releaseinternaltexture)
- [resize](ThinRenderTargetTexture.md#resize)
- [updateSamplingMode](ThinRenderTargetTexture.md#updatesamplingmode)

## Constructors

### constructor

• **new ThinRenderTargetTexture**(`engine`, `size`, `options`)

Instantiates a new ThinRenderTargetTexture.
Tiny helper class to wrap a RenderTargetWrapper in a texture.
This can be used as an internal texture wrapper in ThinEngine to benefit from the cache and to hold on the associated RTT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | Define the internalTexture to wrap |
| `size` | `TextureSize` | Define the size of the RTT to create |
| `options` | `RenderTargetCreationOptions` | Define rendertarget options |

#### Overrides

[ThinTexture](ThinTexture.md).[constructor](ThinTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:34

## Properties

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[ThinTexture](ThinTexture.md).[_engine](ThinTexture.md#_engine)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:144

___

### \_renderTarget

• `Private` **\_renderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) = `null`

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:16

___

### \_renderTargetOptions

• `Private` `Readonly` **\_renderTargetOptions**: `RenderTargetCreationOptions`

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:14

___

### \_size

• `Private` **\_size**: `TextureSize`

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:17

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ThinTexture](ThinTexture.md).[_wrapU](ThinTexture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ThinTexture](ThinTexture.md).[_wrapV](ThinTexture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `4`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[ThinTexture](ThinTexture.md).[anisotropicFilteringLevel](ThinTexture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:61

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[ThinTexture](ThinTexture.md).[delayLoadState](ThinTexture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Inherited from

[ThinTexture](ThinTexture.md).[wrapR](ThinTexture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:54

## Accessors

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Inherited from

ThinTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:72

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ThinTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:117

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ThinTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:125

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ThinTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:98

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ThinTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:106

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ThinTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:79

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ThinTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:87

___

### renderTarget

• `get` **renderTarget**(): [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

Gets the render target wrapper associated with this render target

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Implementation of

[IRenderTargetTexture](../interfaces/IRenderTargetTexture.md).[renderTarget](../interfaces/IRenderTargetTexture.md#rendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:22

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

ThinTexture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### wrapU

• `get` **wrapU**(): `number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

`number`

#### Inherited from

ThinTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:23

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ThinTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:27

___

### wrapV

• `get` **wrapV**(): `number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

`number`

#### Inherited from

ThinTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:39

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ThinTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:43

## Methods

### delayLoad

▸ **delayLoad**(): `void`

Triggers the load sequence in delayed load mode.

#### Returns

`void`

#### Inherited from

[ThinTexture](ThinTexture.md).[delayLoad](ThinTexture.md#delayload)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:182

___

### dispose

▸ **dispose**(`disposeOnlyFramebuffers?`): `void`

Dispose the texture and release its associated resources.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `disposeOnlyFramebuffers` | `boolean` | `false` |

#### Returns

`void`

#### Overrides

[ThinTexture](ThinTexture.md).[dispose](ThinTexture.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:80

___

### getBaseSize

▸ **getBaseSize**(): [`ISize`](../interfaces/ISize.md)

Get the base size of the texture.
It can be different from the size if the texture has been resized for POT for instance

#### Returns

[`ISize`](../interfaces/ISize.md)

the base size

#### Inherited from

[ThinTexture](ThinTexture.md).[getBaseSize](ThinTexture.md#getbasesize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the texture.

#### Returns

`string`

"ThinRenderTargetTexture"

#### Overrides

[ThinTexture](ThinTexture.md).[getClassName](ThinTexture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:72

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Overrides

[ThinTexture](ThinTexture.md).[getInternalTexture](ThinTexture.md#getinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:64

___

### getSize

▸ **getSize**(): [`ISize`](../interfaces/ISize.md)

Get the size of the texture.

#### Returns

[`ISize`](../interfaces/ISize.md)

the texture size.

#### Inherited from

[ThinTexture](ThinTexture.md).[getSize](ThinTexture.md#getsize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:196

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Inherited from

[ThinTexture](ThinTexture.md).[isReady](ThinTexture.md#isready)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:166

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[ThinTexture](ThinTexture.md).[releaseInternalTexture](ThinTexture.md#releaseinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:284

___

### resize

▸ **resize**(`size`): `void`

Resize the texture to a new desired size.
Be careful as it will recreate all the data in the new texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `TextureSize` | Define the new size. It can be:    - a number for squared texture,    - an object containing { width: number, height: number } |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/thinRenderTargetTexture.ts:48

___

### updateSamplingMode

▸ **updateSamplingMode**(`samplingMode`): `void`

Update the sampling mode of the texture.
Default is Trilinear mode.

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 1     | NEAREST_SAMPLINGMODE or NEAREST_NEAREST_MIPLINEAR  | Nearest is: mag = nearest, min = nearest, mip = linear |
| 2     | BILINEAR_SAMPLINGMODE or LINEAR_LINEAR_MIPNEAREST | Bilinear is: mag = linear, min = linear, mip = nearest |
| 3     | TRILINEAR_SAMPLINGMODE or LINEAR_LINEAR_MIPLINEAR | Trilinear is: mag = linear, min = linear, mip = linear |
| 4     | NEAREST_NEAREST_MIPNEAREST |             |
| 5    | NEAREST_LINEAR_MIPNEAREST |             |
| 6    | NEAREST_LINEAR_MIPLINEAR |             |
| 7    | NEAREST_LINEAR |             |
| 8    | NEAREST_NEAREST |             |
| 9   | LINEAR_NEAREST_MIPNEAREST |             |
| 10   | LINEAR_NEAREST_MIPLINEAR |             |
| 11   | LINEAR_LINEAR |             |
| 12   | LINEAR_NEAREST |             |

   > _mag_: magnification filter (close to the viewer)
   > _min_: minification filter (far from the viewer)
   > _mip_: filter used between mip map levels

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `samplingMode` | `number` | Define the new sampling mode of the texture |

#### Returns

`void`

#### Inherited from

[ThinTexture](ThinTexture.md).[updateSamplingMode](ThinTexture.md#updatesamplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:275

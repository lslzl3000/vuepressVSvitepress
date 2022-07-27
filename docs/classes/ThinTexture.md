[@dev/core](../README.md) / [Exports](../modules.md) / ThinTexture

# Class: ThinTexture

Base class of all the textures in babylon.
It groups all the common properties required to work with Thin Engine.

## Hierarchy

- **`ThinTexture`**

  ↳ [`BaseTexture`](BaseTexture.md)

  ↳ [`ThinRenderTargetTexture`](ThinRenderTargetTexture.md)

## Table of contents

### Constructors

- [constructor](ThinTexture.md#constructor)

### Properties

- [\_cachedBaseSize](ThinTexture.md#_cachedbasesize)
- [\_cachedSize](ThinTexture.md#_cachedsize)
- [\_engine](ThinTexture.md#_engine)
- [\_wrapU](ThinTexture.md#_wrapu)
- [\_wrapV](ThinTexture.md#_wrapv)
- [anisotropicFilteringLevel](ThinTexture.md#anisotropicfilteringlevel)
- [delayLoadState](ThinTexture.md#delayloadstate)
- [wrapR](ThinTexture.md#wrapr)

### Accessors

- [coordinatesMode](ThinTexture.md#coordinatesmode)
- [is2DArray](ThinTexture.md#is2darray)
- [is3D](ThinTexture.md#is3d)
- [isCube](ThinTexture.md#iscube)
- [samplingMode](ThinTexture.md#samplingmode)
- [wrapU](ThinTexture.md#wrapu)
- [wrapV](ThinTexture.md#wrapv)

### Methods

- [delayLoad](ThinTexture.md#delayload)
- [dispose](ThinTexture.md#dispose)
- [getBaseSize](ThinTexture.md#getbasesize)
- [getClassName](ThinTexture.md#getclassname)
- [getInternalTexture](ThinTexture.md#getinternaltexture)
- [getSize](ThinTexture.md#getsize)
- [isReady](ThinTexture.md#isready)
- [releaseInternalTexture](ThinTexture.md#releaseinternaltexture)
- [updateSamplingMode](ThinTexture.md#updatesamplingmode)

## Constructors

### constructor

• **new ThinTexture**(`internalTexture`)

Instantiates a new ThinTexture.
Base class of all the textures in babylon.
This can be used as an internal texture wrapper in ThinEngine to benefit from the cache

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `internalTexture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | Define the internalTexture to wrap |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:155

## Properties

### \_cachedBaseSize

• `Private` **\_cachedBaseSize**: [`ISize`](../interfaces/ISize.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:147

___

### \_cachedSize

• `Private` **\_cachedSize**: [`ISize`](../interfaces/ISize.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:146

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:144

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:31

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `4`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:61

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:66

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:54

## Accessors

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:72

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:117

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:125

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:98

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:106

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:79

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:87

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:243

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:23

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:27

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:39

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:43

## Methods

### delayLoad

▸ **delayLoad**(): `void`

Triggers the load sequence in delayed load mode.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:182

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:294

___

### getBaseSize

▸ **getBaseSize**(): [`ISize`](../interfaces/ISize.md)

Get the base size of the texture.
It can be different from the size if the texture has been resized for POT for instance

#### Returns

[`ISize`](../interfaces/ISize.md)

the base size

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the texture.

#### Returns

`string`

"ThinTexture"

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:137

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:188

___

### getSize

▸ **getSize**(): [`ISize`](../interfaces/ISize.md)

Get the size of the texture.

#### Returns

[`ISize`](../interfaces/ISize.md)

the texture size.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:196

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:166

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:284

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:275

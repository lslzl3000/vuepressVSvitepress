[@dev/core](../README.md) / [Exports](../modules.md) / ColorGradingTexture

# Class: ColorGradingTexture

This represents a color grading texture. This acts as a lookup table LUT, useful during post process
It can help converting any input color in a desired output one. This can then be used to create effects
from sepia, black and white to sixties or futuristic rendering...

The only supported format is currently 3dl.
More information on LUT: https://en.wikipedia.org/wiki/3D_lookup_table

## Hierarchy

- [`BaseTexture`](BaseTexture.md)

  ↳ **`ColorGradingTexture`**

## Table of contents

### Constructors

- [constructor](ColorGradingTexture.md#constructor)

### Properties

- [\_coordinatesIndex](ColorGradingTexture.md#_coordinatesindex)
- [\_coordinatesMode](ColorGradingTexture.md#_coordinatesmode)
- [\_engine](ColorGradingTexture.md#_engine)
- [\_errorObject](ColorGradingTexture.md#_errorobject)
- [\_loadingError](ColorGradingTexture.md#_loadingerror)
- [\_onLoad](ColorGradingTexture.md#_onload)
- [\_scene](ColorGradingTexture.md#_scene)
- [\_textureMatrix](ColorGradingTexture.md#_texturematrix)
- [\_wrapU](ColorGradingTexture.md#_wrapu)
- [\_wrapV](ColorGradingTexture.md#_wrapv)
- [animations](ColorGradingTexture.md#animations)
- [anisotropicFilteringLevel](ColorGradingTexture.md#anisotropicfilteringlevel)
- [delayLoadState](ColorGradingTexture.md#delayloadstate)
- [invertZ](ColorGradingTexture.md#invertz)
- [isRenderTarget](ColorGradingTexture.md#isrendertarget)
- [level](ColorGradingTexture.md#level)
- [metadata](ColorGradingTexture.md#metadata)
- [name](ColorGradingTexture.md#name)
- [onDisposeObservable](ColorGradingTexture.md#ondisposeobservable)
- [reservedDataStore](ColorGradingTexture.md#reserveddatastore)
- [sphericalPolynomial](ColorGradingTexture.md#sphericalpolynomial)
- [uniqueId](ColorGradingTexture.md#uniqueid)
- [url](ColorGradingTexture.md#url)
- [wrapR](ColorGradingTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](ColorGradingTexture.md#default_anisotropic_filtering_level)
- [\_NoneEmptyLineRegex](ColorGradingTexture.md#_noneemptylineregex)

### Accessors

- [canRescale](ColorGradingTexture.md#canrescale)
- [coordinatesIndex](ColorGradingTexture.md#coordinatesindex)
- [coordinatesMode](ColorGradingTexture.md#coordinatesmode)
- [errorObject](ColorGradingTexture.md#errorobject)
- [gammaSpace](ColorGradingTexture.md#gammaspace)
- [getAlphaFromRGB](ColorGradingTexture.md#getalphafromrgb)
- [hasAlpha](ColorGradingTexture.md#hasalpha)
- [irradianceTexture](ColorGradingTexture.md#irradiancetexture)
- [is2DArray](ColorGradingTexture.md#is2darray)
- [is3D](ColorGradingTexture.md#is3d)
- [isBlocking](ColorGradingTexture.md#isblocking)
- [isCube](ColorGradingTexture.md#iscube)
- [isRGBD](ColorGradingTexture.md#isrgbd)
- [linearSpecularLOD](ColorGradingTexture.md#linearspecularlod)
- [loadingError](ColorGradingTexture.md#loadingerror)
- [lodGenerationOffset](ColorGradingTexture.md#lodgenerationoffset)
- [lodGenerationScale](ColorGradingTexture.md#lodgenerationscale)
- [noMipmap](ColorGradingTexture.md#nomipmap)
- [onDispose](ColorGradingTexture.md#ondispose)
- [samplingMode](ColorGradingTexture.md#samplingmode)
- [textureFormat](ColorGradingTexture.md#textureformat)
- [textureType](ColorGradingTexture.md#texturetype)
- [uid](ColorGradingTexture.md#uid)
- [wrapU](ColorGradingTexture.md#wrapu)
- [wrapV](ColorGradingTexture.md#wrapv)

### Methods

- [\_load3dlTexture](ColorGradingTexture.md#_load3dltexture)
- [\_loadTexture](ColorGradingTexture.md#_loadtexture)
- [\_markAllSubMeshesAsTexturesDirty](ColorGradingTexture.md#_markallsubmeshesastexturesdirty)
- [\_triggerOnLoad](ColorGradingTexture.md#_triggeronload)
- [checkTransformsAreIdentical](ColorGradingTexture.md#checktransformsareidentical)
- [clone](ColorGradingTexture.md#clone)
- [delayLoad](ColorGradingTexture.md#delayload)
- [dispose](ColorGradingTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](ColorGradingTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](ColorGradingTexture.md#getbasesize)
- [getClassName](ColorGradingTexture.md#getclassname)
- [getInternalTexture](ColorGradingTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](ColorGradingTexture.md#getreflectiontexturematrix)
- [getScene](ColorGradingTexture.md#getscene)
- [getSize](ColorGradingTexture.md#getsize)
- [getTextureMatrix](ColorGradingTexture.md#gettexturematrix)
- [isReady](ColorGradingTexture.md#isready)
- [isReadyOrNotBlocking](ColorGradingTexture.md#isreadyornotblocking)
- [readPixels](ColorGradingTexture.md#readpixels)
- [releaseInternalTexture](ColorGradingTexture.md#releaseinternaltexture)
- [scale](ColorGradingTexture.md#scale)
- [serialize](ColorGradingTexture.md#serialize)
- [toString](ColorGradingTexture.md#tostring)
- [updateSamplingMode](ColorGradingTexture.md#updatesamplingmode)
- [Parse](ColorGradingTexture.md#parse)
- [WhenAllReady](ColorGradingTexture.md#whenallready)

## Constructors

### constructor

• **new ColorGradingTexture**(`url`, `sceneOrEngine`, `onLoad?`)

Instantiates a ColorGradingTexture from the following parameters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | The location of the color grading data (currently only supporting 3dl) |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene or engine the texture will be used in |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | defines a callback triggered when the texture has been loaded |

#### Overrides

[BaseTexture](BaseTexture.md).[constructor](BaseTexture.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:42

## Properties

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[BaseTexture](BaseTexture.md).[_coordinatesIndex](BaseTexture.md#_coordinatesindex)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_coordinatesMode](BaseTexture.md#_coordinatesmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:126

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_engine](BaseTexture.md#_engine)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:144

___

### \_errorObject

• `Protected` `Optional` **\_errorObject**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `exception?` | `any` |
| `message?` | `string` |

#### Inherited from

[BaseTexture](BaseTexture.md).[_errorObject](BaseTexture.md#_errorobject)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:483

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[BaseTexture](BaseTexture.md).[_loadingError](BaseTexture.md#_loadingerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:482

___

### \_onLoad

• `Private` **\_onLoad**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:33

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_scene](BaseTexture.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:466

___

### \_textureMatrix

• `Private` **\_textureMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:32

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_wrapU](BaseTexture.md#_wrapu)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_wrapV](BaseTexture.md#_wrapv)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[BaseTexture](BaseTexture.md).[animations](BaseTexture.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[BaseTexture](BaseTexture.md).[anisotropicFilteringLevel](BaseTexture.md#anisotropicfilteringlevel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:205

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[BaseTexture](BaseTexture.md).[delayLoadState](BaseTexture.md#delayloadstate)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:66

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[BaseTexture](BaseTexture.md).[invertZ](BaseTexture.md#invertz)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[BaseTexture](BaseTexture.md).[isRenderTarget](BaseTexture.md#isrendertarget)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[BaseTexture](BaseTexture.md).[level](BaseTexture.md#level)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[BaseTexture](BaseTexture.md).[metadata](BaseTexture.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[BaseTexture](BaseTexture.md).[name](BaseTexture.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:42

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[BaseTexture](BaseTexture.md).[onDisposeObservable](BaseTexture.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:452

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[BaseTexture](BaseTexture.md).[reservedDataStore](BaseTexture.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:53

___

### sphericalPolynomial

• **sphericalPolynomial**: [`Nullable`](../modules.md#nullable)[`SphericalPolynomial`](SphericalPolynomial.md)

Get the polynomial representation of the texture data.
This is mainly use as a fast way to recover IBL Diffuse irradiance data.

**`See`**

https://learnopengl.com/PBR/IBL/Diffuse-irradiance

#### Inherited from

[BaseTexture](BaseTexture.md).[sphericalPolynomial](BaseTexture.md#sphericalpolynomial)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[BaseTexture](BaseTexture.md).[uniqueId](BaseTexture.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: `string`

The texture URL.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:25

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Inherited from

[BaseTexture](BaseTexture.md).[wrapR](BaseTexture.md#wrapr)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:197

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[BaseTexture](BaseTexture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](BaseTexture.md#default_anisotropic_filtering_level)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:30

___

### \_NoneEmptyLineRegex

▪ `Static` `Private` **\_NoneEmptyLineRegex**: `RegExp`

Empty line regex stored for GC.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:30

## Accessors

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

BaseTexture.canRescale

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

BaseTexture.coordinatesIndex

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:121

• `set` **coordinatesIndex**(`value`): `void`

Define the UV channel to use starting from 0 and defaulting to 0.
This is part of the texture as textures usually maps to one uv set.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.coordinatesIndex

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:110

___

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Inherited from

BaseTexture.coordinatesMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:155

• `set` **coordinatesMode**(`value`): `void`

How a texture is mapped.

| Value | Type                                | Description |
| ----- | ----------------------------------- | ----------- |
| 0     | EXPLICIT_MODE                       |             |
| 1     | SPHERICAL_MODE                      |             |
| 2     | PLANAR_MODE                         |             |
| 3     | CUBIC_MODE                          |             |
| 4     | PROJECTION_MODE                     |             |
| 5     | SKYBOX_MODE                         |             |
| 6     | INVCUBIC_MODE                       |             |
| 7     | EQUIRECTANGULAR_MODE                |             |
| 8     | FIXED_EQUIRECTANGULAR_MODE          |             |
| 9     | FIXED_EQUIRECTANGULAR_MIRRORED_MODE |             |

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.coordinatesMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

BaseTexture.errorObject

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:498

___

### gammaSpace

• `get` **gammaSpace**(): `boolean`

Define if the texture contains data in gamma space (most of the png/jpg aside bump).
HDR texture are usually stored in linear space.
This only impacts the PBR and Background materials

#### Returns

`boolean`

#### Inherited from

BaseTexture.gammaSpace

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:274

• `set` **gammaSpace**(`gamma`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamma` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.gammaSpace

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

BaseTexture.getAlphaFromRGB

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:92

• `set` **getAlphaFromRGB**(`value`): `void`

Defines if the alpha value should be determined via the rgb values.
If true the luminance of the pixel might be used to find the corresponding alpha value.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.getAlphaFromRGB

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

BaseTexture.hasAlpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:71

• `set` **hasAlpha**(`value`): `void`

Define if the texture is having a usable alpha value (can be use for transparency or glossiness for instance).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.hasAlpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:60

___

### irradianceTexture

• `get` **irradianceTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

In case a better definition than spherical harmonics is required for the diffuse part of the environment.
You can set the irradiance texture to rely on a texture instead of the spherical approach.
This texture need to have the same characteristics than its parent (Cube vs 2d, coordinates mode, Gamma/Linear, RGBD).

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

BaseTexture.irradianceTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:393

• `set` **irradianceTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Inherited from

BaseTexture.irradianceTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.is2DArray

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:251

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.is2DArray

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.is3D

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:231

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.is3D

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:240

___

### isBlocking

• `get` **isBlocking**(): `boolean`

Define if the texture is preventing a material to render or not.
If not and the texture is not ready, the engine will use a default black texture instead.

#### Returns

`boolean`

#### Inherited from

BaseTexture.isBlocking

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:475

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.isCube

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:211

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.isCube

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

BaseTexture.isRGBD

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:307

• `set` **isRGBD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.isRGBD

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:310

___

### linearSpecularLOD

• `get` **linearSpecularLOD**(): `boolean`

With prefiltered texture, defined if the specular generation is based on a linear ramp.
By default we are using a log2 of the linear roughness helping to keep a better resolution for
average roughness values.

#### Returns

`boolean`

#### Inherited from

BaseTexture.linearSpecularLOD

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:374

• `set` **linearSpecularLOD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

BaseTexture.linearSpecularLOD

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

BaseTexture.loadingError

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

BaseTexture.lodGenerationOffset

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:338

• `set` **lodGenerationOffset**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.lodGenerationOffset

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

BaseTexture.lodGenerationScale

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:355

• `set` **lodGenerationScale**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.lodGenerationScale

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:363

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

BaseTexture.noMipmap

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:325

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Callback triggered when the texture has been disposed.
Kept for back compatibility, you can use the onDisposeObservable instead.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

BaseTexture.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:459

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

BaseTexture.samplingMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

BaseTexture.textureFormat

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

BaseTexture.textureType

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

BaseTexture.uid

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:416

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

BaseTexture.wrapU

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:166

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.wrapU

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:170

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

BaseTexture.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:181

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

BaseTexture.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_load3dlTexture

▸ `Private` **_load3dlTexture**(): [`InternalTexture`](InternalTexture.md)

Occurs when the file being loaded is a .3dl LUT file.

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:92

___

### \_loadTexture

▸ `Private` **_loadTexture**(): `void`

Starts the loading process of the texture.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:244

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[_markAllSubMeshesAsTexturesDirty](BaseTexture.md#_markallsubmeshesastexturesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:670

___

### \_triggerOnLoad

▸ `Private` **_triggerOnLoad**(): `void`

Fires the onload event from the constructor if requested.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:75

___

### checkTransformsAreIdentical

▸ **checkTransformsAreIdentical**(`texture`): `boolean`

Checks if the texture has the same transform matrix than another texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) | texture to check against |

#### Returns

`boolean`

true if the transforms are the same, else false

#### Inherited from

[BaseTexture](BaseTexture.md).[checkTransformsAreIdentical](BaseTexture.md#checktransformsareidentical)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:554

___

### clone

▸ **clone**(): [`ColorGradingTexture`](ColorGradingTexture.md)

Clones the color grading texture.

#### Returns

[`ColorGradingTexture`](ColorGradingTexture.md)

#### Overrides

[BaseTexture](BaseTexture.md).[clone](BaseTexture.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:253

___

### delayLoad

▸ **delayLoad**(): `void`

Called during delayed load for textures.

#### Returns

`void`

#### Overrides

[BaseTexture](BaseTexture.md).[delayLoad](BaseTexture.md#delayload)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:265

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[dispose](BaseTexture.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:807

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[forceSphericalPolynomialsRecompute](BaseTexture.md#forcesphericalpolynomialsrecompute)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.polynomial.ts:19

___

### getBaseSize

▸ **getBaseSize**(): [`ISize`](../interfaces/ISize.md)

Get the base size of the texture.
It can be different from the size if the texture has been resized for POT for instance

#### Returns

[`ISize`](../interfaces/ISize.md)

the base size

#### Inherited from

[BaseTexture](BaseTexture.md).[getBaseSize](BaseTexture.md#getbasesize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the texture.

#### Returns

`string`

"BaseTexture"

#### Inherited from

[BaseTexture](BaseTexture.md).[getClassName](BaseTexture.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:440

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Inherited from

[BaseTexture](BaseTexture.md).[getInternalTexture](BaseTexture.md#getinternaltexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Get the texture reflection matrix used to rotate/transform the reflection.

#### Returns

[`Matrix`](Matrix.md)

the reflection matrix

#### Inherited from

[BaseTexture](BaseTexture.md).[getReflectionTextureMatrix](BaseTexture.md#getreflectiontexturematrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:570

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

#### Inherited from

[BaseTexture](BaseTexture.md).[getScene](BaseTexture.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:540

___

### getSize

▸ **getSize**(): [`ISize`](../interfaces/ISize.md)

Get the size of the texture.

#### Returns

[`ISize`](../interfaces/ISize.md)

the texture size.

#### Inherited from

[BaseTexture](BaseTexture.md).[getSize](BaseTexture.md#getsize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:196

___

### getTextureMatrix

▸ **getTextureMatrix**(): [`Matrix`](Matrix.md)

Returns the texture matrix used in most of the material.
This is not used in color grading but keep for troubleshooting purpose (easily swap diffuse by colorgrading to look in).

#### Returns

[`Matrix`](Matrix.md)

#### Overrides

[BaseTexture](BaseTexture.md).[getTextureMatrix](BaseTexture.md#gettexturematrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:85

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Inherited from

[BaseTexture](BaseTexture.md).[isReady](BaseTexture.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:166

___

### isReadyOrNotBlocking

▸ **isReadyOrNotBlocking**(): `boolean`

Get if the texture is ready to be consumed (either it is ready or it is not blocking)

#### Returns

`boolean`

true if ready, not blocking or if there was an error loading the texture

#### Inherited from

[BaseTexture](BaseTexture.md).[isReadyOrNotBlocking](BaseTexture.md#isreadyornotblocking)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:578

___

### readPixels

▸ **readPixels**(`faceIndex?`, `level?`, `buffer?`, `flushRenderer?`, `noDataConversion?`, `x?`, `y?`, `width?`, `height?`): [`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

Reads the pixels stored in the webgl texture and returns them as an ArrayBuffer.
This will returns an RGBA array buffer containing either in values (0-255) or
float values (0-1) depending of the underlying buffer type.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `faceIndex` | `number` | `0` | defines the face of the texture to read (in case of cube texture) |
| `level` | `number` | `0` | defines the LOD level of the texture to read (in case of Mip Maps) |
| `buffer` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `null` | defines a user defined buffer to fill with data (can be null) |
| `flushRenderer` | `boolean` | `true` | true to flush the renderer from the pending commands before reading the pixels |
| `noDataConversion` | `boolean` | `false` | false to convert the data to Uint8Array (if texture type is UNSIGNED_BYTE) or to Float32Array (if texture type is anything but UNSIGNED_BYTE). If true, the type of the generated buffer (if buffer==null) will depend on the type of the texture |
| `x` | `number` | `0` | defines the region x coordinates to start reading from (default to 0) |
| `y` | `number` | `0` | defines the region y coordinates to start reading from (default to 0) |
| `width` | `number` | `Number.MAX_VALUE` | defines the region width to read from (default to the texture size at level) |
| `height` | `number` | `Number.MAX_VALUE` | defines the region width to read from (default to the texture size at level) |

#### Returns

[`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

The Array buffer promise containing the pixels data.

#### Inherited from

[BaseTexture](BaseTexture.md).[readPixels](BaseTexture.md#readpixels)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[releaseInternalTexture](BaseTexture.md#releaseinternaltexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:284

___

### scale

▸ **scale**(`ratio`): `void`

Scales the texture if is `canRescale()`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ratio` | `number` | the resize factor we want to use to rescale |

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[scale](BaseTexture.md#scale)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:587

___

### serialize

▸ **serialize**(): `any`

Serializes the LUT texture to json format.

#### Returns

`any`

#### Overrides

[BaseTexture](BaseTexture.md).[serialize](BaseTexture.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:297

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

#### Inherited from

[BaseTexture](BaseTexture.md).[toString](BaseTexture.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:432

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

[BaseTexture](BaseTexture.md).[updateSamplingMode](BaseTexture.md#updatesamplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:275

___

### Parse

▸ `Static` **Parse**(`parsedTexture`, `scene`): [`Nullable`](../modules.md#nullable)[`ColorGradingTexture`](ColorGradingTexture.md)

Parses a color grading texture serialized by Babylon.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTexture` | `any` | The texture information being parsedTexture |
| `scene` | [`Scene`](Scene.md) | The scene to load the texture in |

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorGradingTexture`](ColorGradingTexture.md)

A color grading texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/colorGradingTexture.ts:284

___

### WhenAllReady

▸ `Static` **WhenAllReady**(`textures`, `callback`): `void`

Helper function to be called back once a list of texture contains only ready textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `textures` | [`BaseTexture`](BaseTexture.md)[] | Define the list of textures to wait for |
| `callback` | () => `void` | Define the callback triggered once the entire list will be ready |

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[WhenAllReady](BaseTexture.md#whenallready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:864

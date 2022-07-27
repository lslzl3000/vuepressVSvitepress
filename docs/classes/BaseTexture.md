[@dev/core](../README.md) / [Exports](../modules.md) / BaseTexture

# Class: BaseTexture

Base class of all the textures in babylon.
It groups all the common properties the materials, post process, lights... might need
in order to make a correct use of the texture.

## Hierarchy

- [`ThinTexture`](ThinTexture.md)

  ↳ **`BaseTexture`**

  ↳↳ [`ColorGradingTexture`](ColorGradingTexture.md)

  ↳↳ [`CubeTexture`](CubeTexture.md)

  ↳↳ [`EquiRectangularCubeTexture`](EquiRectangularCubeTexture.md)

  ↳↳ [`HDRCubeTexture`](HDRCubeTexture.md)

  ↳↳ [`HtmlElementTexture`](HtmlElementTexture.md)

  ↳↳ [`Texture`](Texture.md)

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](BaseTexture.md#constructor)

### Properties

- [\_coordinatesIndex](BaseTexture.md#_coordinatesindex)
- [\_coordinatesMode](BaseTexture.md#_coordinatesmode)
- [\_engine](BaseTexture.md#_engine)
- [\_errorObject](BaseTexture.md#_errorobject)
- [\_gammaSpace](BaseTexture.md#_gammaspace)
- [\_getAlphaFromRGB](BaseTexture.md#_getalphafromrgb)
- [\_hasAlpha](BaseTexture.md#_hasalpha)
- [\_isCube](BaseTexture.md#_iscube)
- [\_loadingError](BaseTexture.md#_loadingerror)
- [\_onDisposeObserver](BaseTexture.md#_ondisposeobserver)
- [\_scene](BaseTexture.md#_scene)
- [\_wrapU](BaseTexture.md#_wrapu)
- [\_wrapV](BaseTexture.md#_wrapv)
- [animations](BaseTexture.md#animations)
- [anisotropicFilteringLevel](BaseTexture.md#anisotropicfilteringlevel)
- [delayLoadState](BaseTexture.md#delayloadstate)
- [invertZ](BaseTexture.md#invertz)
- [isRenderTarget](BaseTexture.md#isrendertarget)
- [level](BaseTexture.md#level)
- [metadata](BaseTexture.md#metadata)
- [name](BaseTexture.md#name)
- [onDisposeObservable](BaseTexture.md#ondisposeobservable)
- [reservedDataStore](BaseTexture.md#reserveddatastore)
- [sphericalPolynomial](BaseTexture.md#sphericalpolynomial)
- [uniqueId](BaseTexture.md#uniqueid)
- [wrapR](BaseTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](BaseTexture.md#default_anisotropic_filtering_level)

### Accessors

- [canRescale](BaseTexture.md#canrescale)
- [coordinatesIndex](BaseTexture.md#coordinatesindex)
- [coordinatesMode](BaseTexture.md#coordinatesmode)
- [errorObject](BaseTexture.md#errorobject)
- [gammaSpace](BaseTexture.md#gammaspace)
- [getAlphaFromRGB](BaseTexture.md#getalphafromrgb)
- [hasAlpha](BaseTexture.md#hasalpha)
- [irradianceTexture](BaseTexture.md#irradiancetexture)
- [is2DArray](BaseTexture.md#is2darray)
- [is3D](BaseTexture.md#is3d)
- [isBlocking](BaseTexture.md#isblocking)
- [isCube](BaseTexture.md#iscube)
- [isRGBD](BaseTexture.md#isrgbd)
- [linearSpecularLOD](BaseTexture.md#linearspecularlod)
- [loadingError](BaseTexture.md#loadingerror)
- [lodGenerationOffset](BaseTexture.md#lodgenerationoffset)
- [lodGenerationScale](BaseTexture.md#lodgenerationscale)
- [noMipmap](BaseTexture.md#nomipmap)
- [onDispose](BaseTexture.md#ondispose)
- [samplingMode](BaseTexture.md#samplingmode)
- [textureFormat](BaseTexture.md#textureformat)
- [textureType](BaseTexture.md#texturetype)
- [uid](BaseTexture.md#uid)
- [wrapU](BaseTexture.md#wrapu)
- [wrapV](BaseTexture.md#wrapv)

### Methods

- [\_markAllSubMeshesAsTexturesDirty](BaseTexture.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](BaseTexture.md#checktransformsareidentical)
- [clone](BaseTexture.md#clone)
- [delayLoad](BaseTexture.md#delayload)
- [dispose](BaseTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](BaseTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](BaseTexture.md#getbasesize)
- [getClassName](BaseTexture.md#getclassname)
- [getInternalTexture](BaseTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](BaseTexture.md#getreflectiontexturematrix)
- [getScene](BaseTexture.md#getscene)
- [getSize](BaseTexture.md#getsize)
- [getTextureMatrix](BaseTexture.md#gettexturematrix)
- [isReady](BaseTexture.md#isready)
- [isReadyOrNotBlocking](BaseTexture.md#isreadyornotblocking)
- [readPixels](BaseTexture.md#readpixels)
- [releaseInternalTexture](BaseTexture.md#releaseinternaltexture)
- [scale](BaseTexture.md#scale)
- [serialize](BaseTexture.md#serialize)
- [toString](BaseTexture.md#tostring)
- [updateSamplingMode](BaseTexture.md#updatesamplingmode)
- [WhenAllReady](BaseTexture.md#whenallready)
- [\_IsScene](BaseTexture.md#_isscene)

## Constructors

### constructor

• **new BaseTexture**(`sceneOrEngine?`)

Instantiates a new BaseTexture.
Base class of all the textures in babylon.
It groups all the common properties the materials, post process, lights... might need
in order to make a correct use of the texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sceneOrEngine?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | Define the scene or engine the texture belongs to |

#### Overrides

[ThinTexture](ThinTexture.md).[constructor](ThinTexture.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:514

## Properties

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:126

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[ThinTexture](ThinTexture.md).[_engine](ThinTexture.md#_engine)

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:483

___

### \_gammaSpace

• `Private` **\_gammaSpace**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:268

___

### \_getAlphaFromRGB

• `Private` **\_getAlphaFromRGB**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:76

___

### \_hasAlpha

• `Private` **\_hasAlpha**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:56

___

### \_isCube

• `Private` **\_isCube**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:207

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:482

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:454

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:466

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ThinTexture](ThinTexture.md).[_wrapU](ThinTexture.md#_wrapu)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ThinTexture](ThinTexture.md).[_wrapV](ThinTexture.md#_wrapv)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Overrides

[ThinTexture](ThinTexture.md).[anisotropicFilteringLevel](ThinTexture.md#anisotropicfilteringlevel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:205

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[ThinTexture](ThinTexture.md).[delayLoadState](ThinTexture.md#delayloadstate)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:66

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:42

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:452

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:53

___

### sphericalPolynomial

• **sphericalPolynomial**: [`Nullable`](../modules.md#nullable)[`SphericalPolynomial`](SphericalPolynomial.md)

Get the polynomial representation of the texture data.
This is mainly use as a fast way to recover IBL Diffuse irradiance data.

**`See`**

https://learnopengl.com/PBR/IBL/Diffuse-irradiance

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:36

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Overrides

[ThinTexture](ThinTexture.md).[wrapR](ThinTexture.md#wrapr)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:197

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:30

## Accessors

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:110

___

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Overrides

ThinTexture.coordinatesMode

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

#### Overrides

ThinTexture.coordinatesMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:274

• `set` **gammaSpace**(`gamma`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamma` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:393

• `set` **irradianceTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Overrides

ThinTexture.is2DArray

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:251

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

ThinTexture.is2DArray

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Overrides

ThinTexture.is3D

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:231

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

ThinTexture.is3D

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:240

___

### isBlocking

• `get` **isBlocking**(): `boolean`

Define if the texture is preventing a material to render or not.
If not and the texture is not ready, the engine will use a default black texture instead.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:475

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Overrides

ThinTexture.isCube

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:211

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

ThinTexture.isCube

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:307

• `set` **isRGBD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:374

• `set` **linearSpecularLOD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:338

• `set` **lodGenerationOffset**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:355

• `set` **lodGenerationScale**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:363

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:459

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

ThinTexture.samplingMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

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

#### Overrides

ThinTexture.wrapU

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:166

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

ThinTexture.wrapU

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

#### Overrides

ThinTexture.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:181

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

ThinTexture.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:670

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:554

___

### clone

▸ **clone**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Clones the texture.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the cloned texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:641

___

### delayLoad

▸ **delayLoad**(): `void`

Triggers the load sequence in delayed load mode.

#### Returns

`void`

#### Inherited from

[ThinTexture](ThinTexture.md).[delayLoad](ThinTexture.md#delayload)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:182

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Overrides

[ThinTexture](ThinTexture.md).[dispose](ThinTexture.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:807

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

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

[ThinTexture](ThinTexture.md).[getBaseSize](ThinTexture.md#getbasesize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the texture.

#### Returns

`string`

"BaseTexture"

#### Overrides

[ThinTexture](ThinTexture.md).[getClassName](ThinTexture.md#getclassname)

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

[ThinTexture](ThinTexture.md).[getInternalTexture](ThinTexture.md#getinternaltexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Get the texture reflection matrix used to rotate/transform the reflection.

#### Returns

[`Matrix`](Matrix.md)

the reflection matrix

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:570

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

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

[ThinTexture](ThinTexture.md).[getSize](ThinTexture.md#getsize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:196

___

### getTextureMatrix

▸ **getTextureMatrix**(): [`Matrix`](Matrix.md)

Get the texture transform matrix used to offset tile the texture for instance.

#### Returns

[`Matrix`](Matrix.md)

the transformation matrix

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:562

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

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:166

___

### isReadyOrNotBlocking

▸ **isReadyOrNotBlocking**(): `boolean`

Get if the texture is ready to be consumed (either it is ready or it is not blocking)

#### Returns

`boolean`

true if ready, not blocking or if there was an error loading the texture

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[ThinTexture](ThinTexture.md).[releaseInternalTexture](ThinTexture.md#releaseinternaltexture)

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:587

___

### serialize

▸ **serialize**(): `any`

Serialize the texture into a JSON representation that can be parsed later on.

#### Returns

`any`

the JSON representation of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:846

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

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

[ThinTexture](ThinTexture.md).[updateSamplingMode](ThinTexture.md#updatesamplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:275

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:864

___

### \_IsScene

▸ `Static` `Private` **_IsScene**(`sceneOrEngine`): sceneOrEngine is Scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) |

#### Returns

sceneOrEngine is Scene

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:896

[@dev/core](../README.md) / [Exports](../modules.md) / RawCubeTexture

# Class: RawCubeTexture

Raw cube texture where the raw buffers are passed in

## Hierarchy

- [`CubeTexture`](CubeTexture.md)

  ↳ **`RawCubeTexture`**

## Table of contents

### Constructors

- [constructor](RawCubeTexture.md#constructor)

### Properties

- [\_coordinatesIndex](RawCubeTexture.md#_coordinatesindex)
- [\_coordinatesMode](RawCubeTexture.md#_coordinatesmode)
- [\_engine](RawCubeTexture.md#_engine)
- [\_errorObject](RawCubeTexture.md#_errorobject)
- [\_forcedExtension](RawCubeTexture.md#_forcedextension)
- [\_loadingError](RawCubeTexture.md#_loadingerror)
- [\_rotationY](RawCubeTexture.md#_rotationy)
- [\_scene](RawCubeTexture.md#_scene)
- [\_wrapU](RawCubeTexture.md#_wrapu)
- [\_wrapV](RawCubeTexture.md#_wrapv)
- [animations](RawCubeTexture.md#animations)
- [anisotropicFilteringLevel](RawCubeTexture.md#anisotropicfilteringlevel)
- [boundingBoxPosition](RawCubeTexture.md#boundingboxposition)
- [delayLoadState](RawCubeTexture.md#delayloadstate)
- [invertZ](RawCubeTexture.md#invertz)
- [isRenderTarget](RawCubeTexture.md#isrendertarget)
- [level](RawCubeTexture.md#level)
- [metadata](RawCubeTexture.md#metadata)
- [name](RawCubeTexture.md#name)
- [onDisposeObservable](RawCubeTexture.md#ondisposeobservable)
- [onLoadObservable](RawCubeTexture.md#onloadobservable)
- [reservedDataStore](RawCubeTexture.md#reserveddatastore)
- [sphericalPolynomial](RawCubeTexture.md#sphericalpolynomial)
- [uniqueId](RawCubeTexture.md#uniqueid)
- [url](RawCubeTexture.md#url)
- [wrapR](RawCubeTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](RawCubeTexture.md#default_anisotropic_filtering_level)

### Accessors

- [boundingBoxSize](RawCubeTexture.md#boundingboxsize)
- [canRescale](RawCubeTexture.md#canrescale)
- [coordinatesIndex](RawCubeTexture.md#coordinatesindex)
- [coordinatesMode](RawCubeTexture.md#coordinatesmode)
- [errorObject](RawCubeTexture.md#errorobject)
- [forcedExtension](RawCubeTexture.md#forcedextension)
- [gammaSpace](RawCubeTexture.md#gammaspace)
- [getAlphaFromRGB](RawCubeTexture.md#getalphafromrgb)
- [hasAlpha](RawCubeTexture.md#hasalpha)
- [irradianceTexture](RawCubeTexture.md#irradiancetexture)
- [is2DArray](RawCubeTexture.md#is2darray)
- [is3D](RawCubeTexture.md#is3d)
- [isBlocking](RawCubeTexture.md#isblocking)
- [isCube](RawCubeTexture.md#iscube)
- [isRGBD](RawCubeTexture.md#isrgbd)
- [linearSpecularLOD](RawCubeTexture.md#linearspecularlod)
- [loadingError](RawCubeTexture.md#loadingerror)
- [lodGenerationOffset](RawCubeTexture.md#lodgenerationoffset)
- [lodGenerationScale](RawCubeTexture.md#lodgenerationscale)
- [noMipmap](RawCubeTexture.md#nomipmap)
- [onDispose](RawCubeTexture.md#ondispose)
- [rotationY](RawCubeTexture.md#rotationy)
- [samplingMode](RawCubeTexture.md#samplingmode)
- [textureFormat](RawCubeTexture.md#textureformat)
- [textureType](RawCubeTexture.md#texturetype)
- [uid](RawCubeTexture.md#uid)
- [wrapU](RawCubeTexture.md#wrapu)
- [wrapV](RawCubeTexture.md#wrapv)

### Methods

- [\_markAllSubMeshesAsTexturesDirty](RawCubeTexture.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](RawCubeTexture.md#checktransformsareidentical)
- [clone](RawCubeTexture.md#clone)
- [delayLoad](RawCubeTexture.md#delayload)
- [dispose](RawCubeTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](RawCubeTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](RawCubeTexture.md#getbasesize)
- [getClassName](RawCubeTexture.md#getclassname)
- [getInternalTexture](RawCubeTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](RawCubeTexture.md#getreflectiontexturematrix)
- [getScene](RawCubeTexture.md#getscene)
- [getSize](RawCubeTexture.md#getsize)
- [getTextureMatrix](RawCubeTexture.md#gettexturematrix)
- [isReady](RawCubeTexture.md#isready)
- [isReadyOrNotBlocking](RawCubeTexture.md#isreadyornotblocking)
- [readPixels](RawCubeTexture.md#readpixels)
- [releaseInternalTexture](RawCubeTexture.md#releaseinternaltexture)
- [scale](RawCubeTexture.md#scale)
- [serialize](RawCubeTexture.md#serialize)
- [setReflectionTextureMatrix](RawCubeTexture.md#setreflectiontexturematrix)
- [toString](RawCubeTexture.md#tostring)
- [update](RawCubeTexture.md#update)
- [updateRGBDAsync](RawCubeTexture.md#updatergbdasync)
- [updateSamplingMode](RawCubeTexture.md#updatesamplingmode)
- [updateURL](RawCubeTexture.md#updateurl)
- [CreateFromImages](RawCubeTexture.md#createfromimages)
- [CreateFromPrefilteredData](RawCubeTexture.md#createfromprefiltereddata)
- [Parse](RawCubeTexture.md#parse)
- [WhenAllReady](RawCubeTexture.md#whenallready)

## Constructors

### constructor

• **new RawCubeTexture**(`scene`, `data`, `size`, `format?`, `type?`, `generateMipMaps?`, `invertY?`, `samplingMode?`, `compression?`)

Creates a cube texture where the raw buffers are passed in.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the scene the texture is attached to |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView`[] | `undefined` | defines the array of data to use to create each face |
| `size` | `number` | `undefined` | defines the size of the textures |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | defines the format of the data |
| `type` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the type of the data (like Engine.TEXTURETYPE_UNSIGNED_INT) |
| `generateMipMaps` | `boolean` | `false` | defines if the engine should generate the mip levels |
| `invertY` | `boolean` | `false` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | `Constants.TEXTURE_TRILINEAR_SAMPLINGMODE` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compression used (null by default) |

#### Overrides

[CubeTexture](CubeTexture.md).[constructor](CubeTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/rawCubeTexture.ts:28

## Properties

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[CubeTexture](CubeTexture.md).[_coordinatesIndex](CubeTexture.md#_coordinatesindex)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[CubeTexture](CubeTexture.md).[_coordinatesMode](CubeTexture.md#_coordinatesmode)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:126

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[CubeTexture](CubeTexture.md).[_engine](CubeTexture.md#_engine)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:144

___

### \_errorObject

• `Protected` `Optional` **\_errorObject**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `exception?` | `any` |
| `message?` | `string` |

#### Inherited from

[CubeTexture](CubeTexture.md).[_errorObject](CubeTexture.md#_errorobject)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:483

___

### \_forcedExtension

• `Protected` **\_forcedExtension**: [`Nullable`](../modules.md#nullable)`string` = `null`

#### Inherited from

[CubeTexture](CubeTexture.md).[_forcedExtension](CubeTexture.md#_forcedextension)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:99

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[CubeTexture](CubeTexture.md).[_loadingError](CubeTexture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_rotationY

• `Protected` **\_rotationY**: `number` = `0`

#### Inherited from

[CubeTexture](CubeTexture.md).[_rotationY](CubeTexture.md#_rotationy)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:68

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[CubeTexture](CubeTexture.md).[_scene](CubeTexture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[CubeTexture](CubeTexture.md).[_wrapU](CubeTexture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[CubeTexture](CubeTexture.md).[_wrapV](CubeTexture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[CubeTexture](CubeTexture.md).[animations](CubeTexture.md#animations)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[CubeTexture](CubeTexture.md).[anisotropicFilteringLevel](CubeTexture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:205

___

### boundingBoxPosition

• **boundingBoxPosition**: [`Vector3`](Vector3.md)

Gets or sets the center of the bounding box associated with the cube texture.
It must define where the camera used to render the texture was set

**`See`**

https://doc.babylonjs.com/how_to/reflect#using-local-cubemap-mode

#### Inherited from

[CubeTexture](CubeTexture.md).[boundingBoxPosition](CubeTexture.md#boundingboxposition)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:40

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[CubeTexture](CubeTexture.md).[delayLoadState](CubeTexture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[CubeTexture](CubeTexture.md).[invertZ](CubeTexture.md#invertz)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[CubeTexture](CubeTexture.md).[isRenderTarget](CubeTexture.md#isrendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[CubeTexture](CubeTexture.md).[level](CubeTexture.md#level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[CubeTexture](CubeTexture.md).[metadata](CubeTexture.md#metadata)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[CubeTexture](CubeTexture.md).[name](CubeTexture.md#name)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:42

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[CubeTexture](CubeTexture.md).[onDisposeObservable](CubeTexture.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:452

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`CubeTexture`](CubeTexture.md)

Observable triggered once the texture has been loaded.

#### Inherited from

[CubeTexture](CubeTexture.md).[onLoadObservable](CubeTexture.md#onloadobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:27

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[CubeTexture](CubeTexture.md).[reservedDataStore](CubeTexture.md#reserveddatastore)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:53

___

### sphericalPolynomial

• **sphericalPolynomial**: [`Nullable`](../modules.md#nullable)[`SphericalPolynomial`](SphericalPolynomial.md)

Get the polynomial representation of the texture data.
This is mainly use as a fast way to recover IBL Diffuse irradiance data.

**`See`**

https://learnopengl.com/PBR/IBL/Diffuse-irradiance

#### Inherited from

[CubeTexture](CubeTexture.md).[sphericalPolynomial](CubeTexture.md#sphericalpolynomial)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[CubeTexture](CubeTexture.md).[uniqueId](CubeTexture.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: `string`

The url of the texture

#### Inherited from

[CubeTexture](CubeTexture.md).[url](CubeTexture.md#url)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:33

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Inherited from

[CubeTexture](CubeTexture.md).[wrapR](CubeTexture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:197

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[CubeTexture](CubeTexture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](CubeTexture.md#default_anisotropic_filtering_level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:30

## Accessors

### boundingBoxSize

• `get` **boundingBoxSize**(): [`Vector3`](Vector3.md)

Returns the bounding box size

**`See`**

https://doc.babylonjs.com/how_to/reflect#using-local-cubemap-mode

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

CubeTexture.boundingBoxSize

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:64

• `set` **boundingBoxSize**(`value`): `void`

Gets or sets the size of the bounding box associated with the cube texture
When defined, the cubemap will switch to local mode

**`See`**

https://community.arm.com/graphics/b/blog/posts/reflections-based-on-local-cubemaps-in-unity

**`Example`**

```ts
https://www.babylonjs-playground.com/#RNASML
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

CubeTexture.boundingBoxSize

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:50

___

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

CubeTexture.canRescale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

CubeTexture.coordinatesIndex

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:121

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

CubeTexture.coordinatesIndex

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:110

___

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Inherited from

CubeTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:155

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

CubeTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

CubeTexture.errorObject

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:498

___

### forcedExtension

• `get` **forcedExtension**(): [`Nullable`](../modules.md#nullable)`string`

Gets the forced extension (if any)

#### Returns

[`Nullable`](../modules.md#nullable)`string`

#### Inherited from

CubeTexture.forcedExtension

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:104

___

### gammaSpace

• `get` **gammaSpace**(): `boolean`

Define if the texture contains data in gamma space (most of the png/jpg aside bump).
HDR texture are usually stored in linear space.
This only impacts the PBR and Background materials

#### Returns

`boolean`

#### Inherited from

CubeTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:274

• `set` **gammaSpace**(`gamma`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamma` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

CubeTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:92

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

CubeTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

CubeTexture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:71

• `set` **hasAlpha**(`value`): `void`

Define if the texture is having a usable alpha value (can be use for transparency or glossiness for instance).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:60

___

### irradianceTexture

• `get` **irradianceTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

In case a better definition than spherical harmonics is required for the diffuse part of the environment.
You can set the irradiance texture to rely on a texture instead of the spherical approach.
This texture need to have the same characteristics than its parent (Cube vs 2d, coordinates mode, Gamma/Linear, RGBD).

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

CubeTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:393

• `set` **irradianceTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Inherited from

CubeTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

CubeTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:251

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

CubeTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:231

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:240

___

### isBlocking

• `get` **isBlocking**(): `boolean`

Define if the texture is preventing a material to render or not.
If not and the texture is not ready, the engine will use a default black texture instead.

#### Returns

`boolean`

#### Inherited from

CubeTexture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:475

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

CubeTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:211

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

CubeTexture.isRGBD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:307

• `set` **isRGBD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.isRGBD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:310

___

### linearSpecularLOD

• `get` **linearSpecularLOD**(): `boolean`

With prefiltered texture, defined if the specular generation is based on a linear ramp.
By default we are using a log2 of the linear roughness helping to keep a better resolution for
average roughness values.

#### Returns

`boolean`

#### Inherited from

CubeTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:374

• `set` **linearSpecularLOD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

CubeTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

CubeTexture.loadingError

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

CubeTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:338

• `set` **lodGenerationOffset**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

CubeTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

CubeTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:355

• `set` **lodGenerationScale**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

CubeTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:363

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

CubeTexture.noMipmap

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:88

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

CubeTexture.onDispose

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:459

___

### rotationY

• `get` **rotationY**(): `number`

Gets texture matrix rotation angle around Y axis radians.

#### Returns

`number`

#### Inherited from

CubeTexture.rotationY

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:81

• `set` **rotationY**(`value`): `void`

Sets texture matrix rotation angle around Y axis in radians.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

CubeTexture.rotationY

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:73

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

CubeTexture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

CubeTexture.textureFormat

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

CubeTexture.textureType

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

CubeTexture.uid

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:416

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

CubeTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:166

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

CubeTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:170

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

CubeTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:181

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

CubeTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[_markAllSubMeshesAsTexturesDirty](CubeTexture.md#_markallsubmeshesastexturesdirty)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:670

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

[CubeTexture](CubeTexture.md).[checkTransformsAreIdentical](CubeTexture.md#checktransformsareidentical)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:554

___

### clone

▸ **clone**(): [`CubeTexture`](CubeTexture.md)

Clones the raw cube texture.

#### Returns

[`CubeTexture`](CubeTexture.md)

a new cube texture

#### Overrides

[CubeTexture](CubeTexture.md).[clone](CubeTexture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/rawCubeTexture.ts:72

___

### delayLoad

▸ **delayLoad**(`forcedExtension?`): `void`

Delays loading of the cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forcedExtension?` | `string` | defines the extension to use |

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[delayLoad](CubeTexture.md#delayload)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:303

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[dispose](CubeTexture.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:807

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[forceSphericalPolynomialsRecompute](CubeTexture.md#forcesphericalpolynomialsrecompute)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:19

___

### getBaseSize

▸ **getBaseSize**(): [`ISize`](../interfaces/ISize.md)

Get the base size of the texture.
It can be different from the size if the texture has been resized for POT for instance

#### Returns

[`ISize`](../interfaces/ISize.md)

the base size

#### Inherited from

[CubeTexture](CubeTexture.md).[getBaseSize](CubeTexture.md#getbasesize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name of the texture useful for serialization or dynamic coding.

#### Returns

`string`

"CubeTexture"

#### Inherited from

[CubeTexture](CubeTexture.md).[getClassName](CubeTexture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:220

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Inherited from

[CubeTexture](CubeTexture.md).[getInternalTexture](CubeTexture.md#getinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Returns the reflection texture matrix

#### Returns

[`Matrix`](Matrix.md)

the reflection texture matrix

#### Inherited from

[CubeTexture](CubeTexture.md).[getReflectionTextureMatrix](CubeTexture.md#getreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:319

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

#### Inherited from

[CubeTexture](CubeTexture.md).[getScene](CubeTexture.md#getscene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:540

___

### getSize

▸ **getSize**(): [`ISize`](../interfaces/ISize.md)

Get the size of the texture.

#### Returns

[`ISize`](../interfaces/ISize.md)

the texture size.

#### Inherited from

[CubeTexture](CubeTexture.md).[getSize](CubeTexture.md#getsize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:196

___

### getTextureMatrix

▸ **getTextureMatrix**(): [`Matrix`](Matrix.md)

Get the texture transform matrix used to offset tile the texture for instance.

#### Returns

[`Matrix`](Matrix.md)

the transformation matrix

#### Inherited from

[CubeTexture](CubeTexture.md).[getTextureMatrix](CubeTexture.md#gettexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:562

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Inherited from

[CubeTexture](CubeTexture.md).[isReady](CubeTexture.md#isready)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:166

___

### isReadyOrNotBlocking

▸ **isReadyOrNotBlocking**(): `boolean`

Get if the texture is ready to be consumed (either it is ready or it is not blocking)

#### Returns

`boolean`

true if ready, not blocking or if there was an error loading the texture

#### Inherited from

[CubeTexture](CubeTexture.md).[isReadyOrNotBlocking](CubeTexture.md#isreadyornotblocking)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:578

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

[CubeTexture](CubeTexture.md).[readPixels](CubeTexture.md#readpixels)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[releaseInternalTexture](CubeTexture.md#releaseinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:284

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

[CubeTexture](CubeTexture.md).[scale](CubeTexture.md#scale)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:587

___

### serialize

▸ **serialize**(): `any`

Serialize the texture into a JSON representation that can be parsed later on.

#### Returns

`any`

the JSON representation of the texture

#### Inherited from

[CubeTexture](CubeTexture.md).[serialize](CubeTexture.md#serialize)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:846

___

### setReflectionTextureMatrix

▸ **setReflectionTextureMatrix**(`value`): `void`

Sets the reflection texture matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Matrix`](Matrix.md) | Reflection texture matrix |

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[setReflectionTextureMatrix](CubeTexture.md#setreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:327

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

#### Inherited from

[CubeTexture](CubeTexture.md).[toString](CubeTexture.md#tostring)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:432

___

### update

▸ **update**(`data`, `format`, `type`, `invertY`, `compression?`): `void`

Updates the raw cube texture.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `ArrayBufferView`[] | `undefined` | defines the data to store |
| `format` | `number` | `undefined` | defines the data format |
| `type` | `number` | `undefined` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compression used (null by default) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/rawCubeTexture.ts:52

___

### updateRGBDAsync

▸ **updateRGBDAsync**(`data`, `sphericalPolynomial?`, `lodScale?`, `lodOffset?`): `Promise``void`

Updates a raw cube texture with RGBD encoded data.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `ArrayBufferView`[][] | `undefined` | defines the array of data [mipmap][face] to use to create each face |
| `sphericalPolynomial` | [`Nullable`](../modules.md#nullable)[`SphericalPolynomial`](SphericalPolynomial.md) | `null` | defines the spherical polynomial for irradiance |
| `lodScale` | `number` | `0.8` | defines the scale applied to environment texture. This manages the range of LOD level used for IBL according to the roughness |
| `lodOffset` | `number` | `0` | defines the offset applied to environment texture. This manages first LOD level used for IBL according to the roughness |

#### Returns

`Promise``void`

a promise that resolves when the operation is complete

#### Defined in

packages/dev/core/src/Materials/Textures/rawCubeTexture.ts:64

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

[CubeTexture](CubeTexture.md).[updateSamplingMode](CubeTexture.md#updatesamplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:275

___

### updateURL

▸ **updateURL**(`url`, `forcedExtension?`, `onLoad?`, `prefiltered?`, `onError?`, `extensions?`, `delayLoad?`, `files?`): `void`

Update the url (and optional buffer) of this texture if url was null during construction.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | the url of the texture |
| `forcedExtension?` | `string` | `undefined` | defines the extension to use |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | callback called when the texture is loaded  (defaults to null) |
| `prefiltered` | `boolean` | `false` | Defines whether the updated texture is prefiltered or not |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` | callback called if there was an error during the loading process (defaults to null) |
| `extensions` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the suffixes add to the picture name in case six images are in use like _px.jpg... |
| `delayLoad` | `boolean` | `false` | defines if the texture should be loaded now (false by default) |
| `files` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the six files to load for the different faces in that order: px, py, pz, nx, ny, nz |

#### Returns

`void`

#### Inherited from

[CubeTexture](CubeTexture.md).[updateURL](CubeTexture.md#updateurl)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:235

___

### CreateFromImages

▸ `Static` **CreateFromImages**(`files`, `scene`, `noMipmap?`): [`CubeTexture`](CubeTexture.md)

Creates a cube texture from an array of image urls

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `files` | `string`[] | defines an array of image urls |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `noMipmap?` | `boolean` | specifies if mip maps are not used |

#### Returns

[`CubeTexture`](CubeTexture.md)

a cube texture

#### Inherited from

[CubeTexture](CubeTexture.md).[CreateFromImages](CubeTexture.md#createfromimages)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:126

___

### CreateFromPrefilteredData

▸ `Static` **CreateFromPrefilteredData**(`url`, `scene`, `forcedExtension?`, `createPolynomials?`): [`CubeTexture`](CubeTexture.md)

Creates and return a texture created from prefilterd data by tools like IBL Baker or Lys.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | defines the url of the prefiltered texture |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the scene the texture is attached to |
| `forcedExtension` | `any` | `null` | defines the extension of the file if different from the url |
| `createPolynomials` | `boolean` | `true` | defines whether or not to create polynomial harmonics from the texture data if necessary |

#### Returns

[`CubeTexture`](CubeTexture.md)

the prefiltered texture

#### Inherited from

[CubeTexture](CubeTexture.md).[CreateFromPrefilteredData](CubeTexture.md#createfromprefiltereddata)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:142

___

### Parse

▸ `Static` **Parse**(`parsedTexture`, `scene`, `rootUrl`): [`CubeTexture`](CubeTexture.md)

Parses text to create a cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTexture` | `any` | define the serialized text to read from |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root url of the cube texture |

#### Returns

[`CubeTexture`](CubeTexture.md)

a cube texture

#### Inherited from

[CubeTexture](CubeTexture.md).[Parse](CubeTexture.md#parse)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:413

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

[CubeTexture](CubeTexture.md).[WhenAllReady](CubeTexture.md#whenallready)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:864

[@dev/core](../README.md) / [Exports](../modules.md) / CubeTexture

# Class: CubeTexture

Class for creating a cube texture

## Hierarchy

- [`BaseTexture`](BaseTexture.md)

  ↳ **`CubeTexture`**

  ↳↳ [`RawCubeTexture`](RawCubeTexture.md)

## Table of contents

### Constructors

- [constructor](CubeTexture.md#constructor)

### Properties

- [\_boundingBoxSize](CubeTexture.md#_boundingboxsize)
- [\_coordinatesIndex](CubeTexture.md#_coordinatesindex)
- [\_coordinatesMode](CubeTexture.md#_coordinatesmode)
- [\_createPolynomials](CubeTexture.md#_createpolynomials)
- [\_delayedOnError](CubeTexture.md#_delayedonerror)
- [\_delayedOnLoad](CubeTexture.md#_delayedonload)
- [\_engine](CubeTexture.md#_engine)
- [\_errorObject](CubeTexture.md#_errorobject)
- [\_extensions](CubeTexture.md#_extensions)
- [\_forcedExtension](CubeTexture.md#_forcedextension)
- [\_format](CubeTexture.md#_format)
- [\_loaderOptions](CubeTexture.md#_loaderoptions)
- [\_loadingError](CubeTexture.md#_loadingerror)
- [\_lodOffset](CubeTexture.md#_lodoffset)
- [\_lodScale](CubeTexture.md#_lodscale)
- [\_noMipmap](CubeTexture.md#_nomipmap)
- [\_rotationY](CubeTexture.md#_rotationy)
- [\_scene](CubeTexture.md#_scene)
- [\_textureMatrix](CubeTexture.md#_texturematrix)
- [\_useSRGBBuffer](CubeTexture.md#_usesrgbbuffer)
- [\_wrapU](CubeTexture.md#_wrapu)
- [\_wrapV](CubeTexture.md#_wrapv)
- [animations](CubeTexture.md#animations)
- [anisotropicFilteringLevel](CubeTexture.md#anisotropicfilteringlevel)
- [boundingBoxPosition](CubeTexture.md#boundingboxposition)
- [delayLoadState](CubeTexture.md#delayloadstate)
- [invertZ](CubeTexture.md#invertz)
- [isRenderTarget](CubeTexture.md#isrendertarget)
- [level](CubeTexture.md#level)
- [metadata](CubeTexture.md#metadata)
- [name](CubeTexture.md#name)
- [onDisposeObservable](CubeTexture.md#ondisposeobservable)
- [onLoadObservable](CubeTexture.md#onloadobservable)
- [reservedDataStore](CubeTexture.md#reserveddatastore)
- [sphericalPolynomial](CubeTexture.md#sphericalpolynomial)
- [uniqueId](CubeTexture.md#uniqueid)
- [url](CubeTexture.md#url)
- [wrapR](CubeTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](CubeTexture.md#default_anisotropic_filtering_level)

### Accessors

- [boundingBoxSize](CubeTexture.md#boundingboxsize)
- [canRescale](CubeTexture.md#canrescale)
- [coordinatesIndex](CubeTexture.md#coordinatesindex)
- [coordinatesMode](CubeTexture.md#coordinatesmode)
- [errorObject](CubeTexture.md#errorobject)
- [forcedExtension](CubeTexture.md#forcedextension)
- [gammaSpace](CubeTexture.md#gammaspace)
- [getAlphaFromRGB](CubeTexture.md#getalphafromrgb)
- [hasAlpha](CubeTexture.md#hasalpha)
- [irradianceTexture](CubeTexture.md#irradiancetexture)
- [is2DArray](CubeTexture.md#is2darray)
- [is3D](CubeTexture.md#is3d)
- [isBlocking](CubeTexture.md#isblocking)
- [isCube](CubeTexture.md#iscube)
- [isRGBD](CubeTexture.md#isrgbd)
- [linearSpecularLOD](CubeTexture.md#linearspecularlod)
- [loadingError](CubeTexture.md#loadingerror)
- [lodGenerationOffset](CubeTexture.md#lodgenerationoffset)
- [lodGenerationScale](CubeTexture.md#lodgenerationscale)
- [noMipmap](CubeTexture.md#nomipmap)
- [onDispose](CubeTexture.md#ondispose)
- [rotationY](CubeTexture.md#rotationy)
- [samplingMode](CubeTexture.md#samplingmode)
- [textureFormat](CubeTexture.md#textureformat)
- [textureType](CubeTexture.md#texturetype)
- [uid](CubeTexture.md#uid)
- [wrapU](CubeTexture.md#wrapu)
- [wrapV](CubeTexture.md#wrapv)

### Methods

- [\_loadTexture](CubeTexture.md#_loadtexture)
- [\_markAllSubMeshesAsTexturesDirty](CubeTexture.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](CubeTexture.md#checktransformsareidentical)
- [clone](CubeTexture.md#clone)
- [delayLoad](CubeTexture.md#delayload)
- [dispose](CubeTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](CubeTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](CubeTexture.md#getbasesize)
- [getClassName](CubeTexture.md#getclassname)
- [getInternalTexture](CubeTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](CubeTexture.md#getreflectiontexturematrix)
- [getScene](CubeTexture.md#getscene)
- [getSize](CubeTexture.md#getsize)
- [getTextureMatrix](CubeTexture.md#gettexturematrix)
- [isReady](CubeTexture.md#isready)
- [isReadyOrNotBlocking](CubeTexture.md#isreadyornotblocking)
- [readPixels](CubeTexture.md#readpixels)
- [releaseInternalTexture](CubeTexture.md#releaseinternaltexture)
- [scale](CubeTexture.md#scale)
- [serialize](CubeTexture.md#serialize)
- [setReflectionTextureMatrix](CubeTexture.md#setreflectiontexturematrix)
- [toString](CubeTexture.md#tostring)
- [updateSamplingMode](CubeTexture.md#updatesamplingmode)
- [updateURL](CubeTexture.md#updateurl)
- [CreateFromImages](CubeTexture.md#createfromimages)
- [CreateFromPrefilteredData](CubeTexture.md#createfromprefiltereddata)
- [Parse](CubeTexture.md#parse)
- [WhenAllReady](CubeTexture.md#whenallready)

## Constructors

### constructor

• **new CubeTexture**(`rootUrl`, `sceneOrEngine`, `extensions?`, `noMipmap?`, `files?`, `onLoad?`, `onError?`, `format?`, `prefiltered?`, `forcedExtension?`, `createPolynomials?`, `lodScale?`, `lodOffset?`, `loaderOptions?`, `useSRGBBuffer?`)

Creates a cube texture to use with reflection for instance. It can be based upon dds or six images as well
as prefiltered data.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rootUrl` | `string` | `undefined` | defines the url of the texture or the root name of the six images |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | defines the scene or engine the texture is attached to |
| `extensions` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the suffixes add to the picture name in case six images are in use like _px.jpg... |
| `noMipmap` | `boolean` | `false` | defines if mipmaps should be created or not |
| `files` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the six files to load for the different faces in that order: px, py, pz, nx, ny, nz |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | defines a callback triggered at the end of the file load if no errors occurred |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` | defines a callback triggered in case of error during load |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | defines the internal format to use for the texture once loaded |
| `prefiltered` | `boolean` | `false` | defines whether or not the texture is created from prefiltered data |
| `forcedExtension` | `any` | `null` | defines the extensions to use (force a special type of file to load) in case it is different from the file name |
| `createPolynomials` | `boolean` | `false` | defines whether or not to create polynomial harmonics from the texture data if necessary |
| `lodScale` | `number` | `0.8` | defines the scale applied to environment texture. This manages the range of LOD level used for IBL according to the roughness |
| `lodOffset` | `number` | `0` | defines the offset applied to environment texture. This manages first LOD level used for IBL according to the roughness |
| `loaderOptions?` | `any` | `undefined` | options to be passed to the loader |
| `useSRGBBuffer?` | `boolean` | `undefined` | Defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU) (default: false) |

#### Overrides

[BaseTexture](BaseTexture.md).[constructor](BaseTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:173

## Properties

### \_boundingBoxSize

• `Private` **\_boundingBoxSize**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:42

___

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[BaseTexture](BaseTexture.md).[_coordinatesIndex](BaseTexture.md#_coordinatesindex)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_coordinatesMode](BaseTexture.md#_coordinatesmode)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:126

___

### \_createPolynomials

• `Private` **\_createPolynomials**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:115

___

### \_delayedOnError

• `Private` **\_delayedOnError**: [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:20

___

### \_delayedOnLoad

• `Private` **\_delayedOnLoad**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:19

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_engine](BaseTexture.md#_engine)

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

[BaseTexture](BaseTexture.md).[_errorObject](BaseTexture.md#_errorobject)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:483

___

### \_extensions

• `Private` **\_extensions**: [`Nullable`](../modules.md#nullable)`string`[] = `null`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:109

___

### \_forcedExtension

• `Protected` **\_forcedExtension**: [`Nullable`](../modules.md#nullable)`string` = `null`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:99

___

### \_format

• `Private` **\_format**: `number`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:114

___

### \_loaderOptions

• `Private` **\_loaderOptions**: `any`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:116

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[BaseTexture](BaseTexture.md).[_loadingError](BaseTexture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_lodOffset

• `Private` **\_lodOffset**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:22

___

### \_lodScale

• `Private` **\_lodScale**: `number` = `0.8`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:21

___

### \_noMipmap

• `Private` **\_noMipmap**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:92

___

### \_rotationY

• `Protected` **\_rotationY**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:68

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_scene](BaseTexture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_textureMatrix

• `Private` **\_textureMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:112

___

### \_useSRGBBuffer

• `Private` `Optional` **\_useSRGBBuffer**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:117

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_wrapU](BaseTexture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[BaseTexture](BaseTexture.md).[_wrapV](BaseTexture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[BaseTexture](BaseTexture.md).[animations](BaseTexture.md#animations)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[BaseTexture](BaseTexture.md).[anisotropicFilteringLevel](BaseTexture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:205

___

### boundingBoxPosition

• **boundingBoxPosition**: [`Vector3`](Vector3.md)

Gets or sets the center of the bounding box associated with the cube texture.
It must define where the camera used to render the texture was set

**`See`**

https://doc.babylonjs.com/how_to/reflect#using-local-cubemap-mode

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:40

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[BaseTexture](BaseTexture.md).[delayLoadState](BaseTexture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[BaseTexture](BaseTexture.md).[invertZ](BaseTexture.md#invertz)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[BaseTexture](BaseTexture.md).[isRenderTarget](BaseTexture.md#isrendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[BaseTexture](BaseTexture.md).[level](BaseTexture.md#level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[BaseTexture](BaseTexture.md).[metadata](BaseTexture.md#metadata)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[BaseTexture](BaseTexture.md).[name](BaseTexture.md#name)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:42

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[BaseTexture](BaseTexture.md).[onDisposeObservable](BaseTexture.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:452

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`CubeTexture`](CubeTexture.md)

Observable triggered once the texture has been loaded.

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:27

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[BaseTexture](BaseTexture.md).[reservedDataStore](BaseTexture.md#reserveddatastore)

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

[BaseTexture](BaseTexture.md).[sphericalPolynomial](BaseTexture.md#sphericalpolynomial)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[BaseTexture](BaseTexture.md).[uniqueId](BaseTexture.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: `string`

The url of the texture

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

[BaseTexture](BaseTexture.md).[wrapR](BaseTexture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:197

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[BaseTexture](BaseTexture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](BaseTexture.md#default_anisotropic_filtering_level)

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

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:50

___

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

BaseTexture.canRescale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

BaseTexture.coordinatesIndex

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

BaseTexture.coordinatesIndex

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

BaseTexture.coordinatesMode

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

BaseTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

BaseTexture.errorObject

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:498

___

### forcedExtension

• `get` **forcedExtension**(): [`Nullable`](../modules.md#nullable)`string`

Gets the forced extension (if any)

#### Returns

[`Nullable`](../modules.md#nullable)`string`

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

BaseTexture.gammaSpace

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

BaseTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

BaseTexture.getAlphaFromRGB

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

BaseTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

BaseTexture.hasAlpha

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

BaseTexture.hasAlpha

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

BaseTexture.irradianceTexture

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

BaseTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.is2DArray

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

BaseTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.is3D

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

BaseTexture.is3D

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

BaseTexture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:475

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

BaseTexture.isCube

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

BaseTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

BaseTexture.isRGBD

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

BaseTexture.isRGBD

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

BaseTexture.linearSpecularLOD

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

BaseTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

BaseTexture.loadingError

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

BaseTexture.lodGenerationOffset

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

BaseTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

BaseTexture.lodGenerationScale

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

BaseTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:363

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Overrides

BaseTexture.noMipmap

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

BaseTexture.onDispose

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:459

___

### rotationY

• `get` **rotationY**(): `number`

Gets texture matrix rotation angle around Y axis radians.

#### Returns

`number`

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

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:73

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

BaseTexture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

BaseTexture.textureFormat

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

BaseTexture.textureType

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

BaseTexture.uid

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

BaseTexture.wrapU

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

BaseTexture.wrapU

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

BaseTexture.wrapV

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

BaseTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_loadTexture

▸ `Private` **_loadTexture**(`onLoad?`, `onError?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:339

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[_markAllSubMeshesAsTexturesDirty](BaseTexture.md#_markallsubmeshesastexturesdirty)

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

[BaseTexture](BaseTexture.md).[checkTransformsAreIdentical](BaseTexture.md#checktransformsareidentical)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:554

___

### clone

▸ **clone**(): [`CubeTexture`](CubeTexture.md)

Makes a clone, or deep copy, of the cube texture

#### Returns

[`CubeTexture`](CubeTexture.md)

a new cube texture

#### Overrides

[BaseTexture](BaseTexture.md).[clone](BaseTexture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:463

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

#### Overrides

[BaseTexture](BaseTexture.md).[delayLoad](BaseTexture.md#delayload)

#### Defined in

packages/dev/core/src/Materials/Textures/cubeTexture.ts:303

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[dispose](BaseTexture.md#dispose)

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

[BaseTexture](BaseTexture.md).[forceSphericalPolynomialsRecompute](BaseTexture.md#forcesphericalpolynomialsrecompute)

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

[BaseTexture](BaseTexture.md).[getBaseSize](BaseTexture.md#getbasesize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name of the texture useful for serialization or dynamic coding.

#### Returns

`string`

"CubeTexture"

#### Overrides

[BaseTexture](BaseTexture.md).[getClassName](BaseTexture.md#getclassname)

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

[BaseTexture](BaseTexture.md).[getInternalTexture](BaseTexture.md#getinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Returns the reflection texture matrix

#### Returns

[`Matrix`](Matrix.md)

the reflection texture matrix

#### Overrides

[BaseTexture](BaseTexture.md).[getReflectionTextureMatrix](BaseTexture.md#getreflectiontexturematrix)

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

[BaseTexture](BaseTexture.md).[getScene](BaseTexture.md#getscene)

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

[BaseTexture](BaseTexture.md).[getSize](BaseTexture.md#getsize)

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

[BaseTexture](BaseTexture.md).[getTextureMatrix](BaseTexture.md#gettexturematrix)

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

[BaseTexture](BaseTexture.md).[isReady](BaseTexture.md#isready)

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

[BaseTexture](BaseTexture.md).[isReadyOrNotBlocking](BaseTexture.md#isreadyornotblocking)

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

[BaseTexture](BaseTexture.md).[readPixels](BaseTexture.md#readpixels)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[releaseInternalTexture](BaseTexture.md#releaseinternaltexture)

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

[BaseTexture](BaseTexture.md).[scale](BaseTexture.md#scale)

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

[BaseTexture](BaseTexture.md).[serialize](BaseTexture.md#serialize)

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

[BaseTexture](BaseTexture.md).[toString](BaseTexture.md#tostring)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:432

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

[BaseTexture](BaseTexture.md).[WhenAllReady](BaseTexture.md#whenallready)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:864

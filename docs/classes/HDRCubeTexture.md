[@dev/core](../README.md) / [Exports](../modules.md) / HDRCubeTexture

# Class: HDRCubeTexture

This represents a texture coming from an HDR input.

The only supported format is currently panorama picture stored in RGBE format.
Example of such files can be found on Poly Haven: https://polyhaven.com/hdris

## Hierarchy

- [`BaseTexture`](BaseTexture.md)

  ↳ **`HDRCubeTexture`**

## Table of contents

### Constructors

- [constructor](HDRCubeTexture.md#constructor)

### Properties

- [\_boundingBoxSize](HDRCubeTexture.md#_boundingboxsize)
- [\_coordinatesIndex](HDRCubeTexture.md#_coordinatesindex)
- [\_coordinatesMode](HDRCubeTexture.md#_coordinatesmode)
- [\_engine](HDRCubeTexture.md#_engine)
- [\_errorObject](HDRCubeTexture.md#_errorobject)
- [\_generateHarmonics](HDRCubeTexture.md#_generateharmonics)
- [\_isBlocking](HDRCubeTexture.md#_isblocking)
- [\_loadingError](HDRCubeTexture.md#_loadingerror)
- [\_noMipmap](HDRCubeTexture.md#_nomipmap)
- [\_onError](HDRCubeTexture.md#_onerror)
- [\_onLoad](HDRCubeTexture.md#_onload)
- [\_prefilterOnLoad](HDRCubeTexture.md#_prefilteronload)
- [\_rotationY](HDRCubeTexture.md#_rotationy)
- [\_scene](HDRCubeTexture.md#_scene)
- [\_size](HDRCubeTexture.md#_size)
- [\_textureMatrix](HDRCubeTexture.md#_texturematrix)
- [\_wrapU](HDRCubeTexture.md#_wrapu)
- [\_wrapV](HDRCubeTexture.md#_wrapv)
- [animations](HDRCubeTexture.md#animations)
- [anisotropicFilteringLevel](HDRCubeTexture.md#anisotropicfilteringlevel)
- [boundingBoxPosition](HDRCubeTexture.md#boundingboxposition)
- [delayLoadState](HDRCubeTexture.md#delayloadstate)
- [invertZ](HDRCubeTexture.md#invertz)
- [isRenderTarget](HDRCubeTexture.md#isrendertarget)
- [level](HDRCubeTexture.md#level)
- [metadata](HDRCubeTexture.md#metadata)
- [name](HDRCubeTexture.md#name)
- [onDisposeObservable](HDRCubeTexture.md#ondisposeobservable)
- [onLoadObservable](HDRCubeTexture.md#onloadobservable)
- [reservedDataStore](HDRCubeTexture.md#reserveddatastore)
- [sphericalPolynomial](HDRCubeTexture.md#sphericalpolynomial)
- [uniqueId](HDRCubeTexture.md#uniqueid)
- [url](HDRCubeTexture.md#url)
- [wrapR](HDRCubeTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](HDRCubeTexture.md#default_anisotropic_filtering_level)
- [\_FacesMapping](HDRCubeTexture.md#_facesmapping)

### Accessors

- [boundingBoxSize](HDRCubeTexture.md#boundingboxsize)
- [canRescale](HDRCubeTexture.md#canrescale)
- [coordinatesIndex](HDRCubeTexture.md#coordinatesindex)
- [coordinatesMode](HDRCubeTexture.md#coordinatesmode)
- [errorObject](HDRCubeTexture.md#errorobject)
- [gammaSpace](HDRCubeTexture.md#gammaspace)
- [getAlphaFromRGB](HDRCubeTexture.md#getalphafromrgb)
- [hasAlpha](HDRCubeTexture.md#hasalpha)
- [irradianceTexture](HDRCubeTexture.md#irradiancetexture)
- [is2DArray](HDRCubeTexture.md#is2darray)
- [is3D](HDRCubeTexture.md#is3d)
- [isBlocking](HDRCubeTexture.md#isblocking)
- [isCube](HDRCubeTexture.md#iscube)
- [isRGBD](HDRCubeTexture.md#isrgbd)
- [linearSpecularLOD](HDRCubeTexture.md#linearspecularlod)
- [loadingError](HDRCubeTexture.md#loadingerror)
- [lodGenerationOffset](HDRCubeTexture.md#lodgenerationoffset)
- [lodGenerationScale](HDRCubeTexture.md#lodgenerationscale)
- [noMipmap](HDRCubeTexture.md#nomipmap)
- [onDispose](HDRCubeTexture.md#ondispose)
- [rotationY](HDRCubeTexture.md#rotationy)
- [samplingMode](HDRCubeTexture.md#samplingmode)
- [textureFormat](HDRCubeTexture.md#textureformat)
- [textureType](HDRCubeTexture.md#texturetype)
- [uid](HDRCubeTexture.md#uid)
- [wrapU](HDRCubeTexture.md#wrapu)
- [wrapV](HDRCubeTexture.md#wrapv)

### Methods

- [\_loadTexture](HDRCubeTexture.md#_loadtexture)
- [\_markAllSubMeshesAsTexturesDirty](HDRCubeTexture.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](HDRCubeTexture.md#checktransformsareidentical)
- [clone](HDRCubeTexture.md#clone)
- [delayLoad](HDRCubeTexture.md#delayload)
- [dispose](HDRCubeTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](HDRCubeTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](HDRCubeTexture.md#getbasesize)
- [getClassName](HDRCubeTexture.md#getclassname)
- [getInternalTexture](HDRCubeTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](HDRCubeTexture.md#getreflectiontexturematrix)
- [getScene](HDRCubeTexture.md#getscene)
- [getSize](HDRCubeTexture.md#getsize)
- [getTextureMatrix](HDRCubeTexture.md#gettexturematrix)
- [isReady](HDRCubeTexture.md#isready)
- [isReadyOrNotBlocking](HDRCubeTexture.md#isreadyornotblocking)
- [readPixels](HDRCubeTexture.md#readpixels)
- [releaseInternalTexture](HDRCubeTexture.md#releaseinternaltexture)
- [scale](HDRCubeTexture.md#scale)
- [serialize](HDRCubeTexture.md#serialize)
- [setReflectionTextureMatrix](HDRCubeTexture.md#setreflectiontexturematrix)
- [toString](HDRCubeTexture.md#tostring)
- [updateSamplingMode](HDRCubeTexture.md#updatesamplingmode)
- [Parse](HDRCubeTexture.md#parse)
- [WhenAllReady](HDRCubeTexture.md#whenallready)

## Constructors

### constructor

• **new HDRCubeTexture**(`url`, `sceneOrEngine`, `size`, `noMipmap?`, `generateHarmonics?`, `gammaSpace?`, `prefilterOnLoad?`, `onLoad?`, `onError?`)

Instantiates an HDRTexture from the following parameters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | The location of the HDR raw data (Panorama stored in RGBE format) |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene or engine the texture will be used in |
| `size` | `number` | `undefined` | The cubemap desired size (the more it increases the longer the generation will be) |
| `noMipmap` | `boolean` | `false` | Forces to not generate the mipmap if true |
| `generateHarmonics` | `boolean` | `true` | Specifies whether you want to extract the polynomial harmonics during the generation process |
| `gammaSpace` | `boolean` | `false` | Specifies if the texture will be use in gamma or linear space (the PBR material requires those texture in linear space, but the standard material would require them in Gamma space) |
| `prefilterOnLoad` | `boolean` | `false` | Prefilters HDR texture to allow use of this texture as a PBR reflection texture. |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` |  |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` |  |

#### Overrides

[BaseTexture](BaseTexture.md).[constructor](BaseTexture.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:116

## Properties

### \_boundingBoxSize

• `Private` **\_boundingBoxSize**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:76

___

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

### \_generateHarmonics

• `Private` **\_generateHarmonics**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:28

___

### \_isBlocking

• `Protected` **\_isBlocking**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:41

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[BaseTexture](BaseTexture.md).[_loadingError](BaseTexture.md#_loadingerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:482

___

### \_noMipmap

• `Private` **\_noMipmap**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:29

___

### \_onError

• `Private` **\_onError**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:34

___

### \_onLoad

• `Private` **\_onLoad**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:33

___

### \_prefilterOnLoad

• `Private` **\_prefilterOnLoad**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:30

___

### \_rotationY

• `Protected` **\_rotationY**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:55

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_scene](BaseTexture.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:466

___

### \_size

• `Private` **\_size**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:32

___

### \_textureMatrix

• `Private` **\_textureMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:31

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

### boundingBoxPosition

• **boundingBoxPosition**: [`Vector3`](Vector3.md)

Gets or sets the center of the bounding box associated with the cube texture
It must define where the camera used to render the texture was set

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:74

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

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`HDRCubeTexture`](HDRCubeTexture.md)

Observable triggered once the texture has been loaded.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:101

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

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:39

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

### \_FacesMapping

▪ `Static` `Private` **\_FacesMapping**: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:26

## Accessors

### boundingBoxSize

• `get` **boundingBoxSize**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:94

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

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:84

___

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

Gets whether or not the texture is blocking during loading.

#### Returns

`boolean`

#### Overrides

BaseTexture.isBlocking

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:51

• `set` **isBlocking**(`value`): `void`

Sets whether or not the texture is blocking during loading.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

BaseTexture.isBlocking

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:45

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

### rotationY

• `get` **rotationY**(): `number`

Gets texture matrix rotation angle around Y axis radians.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:66

• `set` **rotationY**(`value`): `void`

Sets texture matrix rotation angle around Y axis in radians.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:59

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

### \_loadTexture

▸ `Private` **_loadTexture**(): `void`

Occurs when the file is raw .hdr file.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:182

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

▸ **clone**(): [`HDRCubeTexture`](HDRCubeTexture.md)

Clones the texture.

#### Returns

[`HDRCubeTexture`](HDRCubeTexture.md)

the cloned texture

#### Overrides

[BaseTexture](BaseTexture.md).[clone](BaseTexture.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:296

___

### delayLoad

▸ **delayLoad**(): `void`

Triggers the load sequence in delayed load mode.

#### Returns

`void`

#### Overrides

[BaseTexture](BaseTexture.md).[delayLoad](BaseTexture.md#delayload)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:310

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Overrides

[BaseTexture](BaseTexture.md).[dispose](BaseTexture.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:350

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

Get the current class name of the texture useful for serialization or dynamic coding.

#### Returns

`string`

"HDRCubeTexture"

#### Overrides

[BaseTexture](BaseTexture.md).[getClassName](BaseTexture.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:175

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

#### Overrides

[BaseTexture](BaseTexture.md).[getReflectionTextureMatrix](BaseTexture.md#getreflectiontexturematrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:327

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

Get the texture transform matrix used to offset tile the texture for instance.

#### Returns

[`Matrix`](Matrix.md)

the transformation matrix

#### Inherited from

[BaseTexture](BaseTexture.md).[getTextureMatrix](BaseTexture.md#gettexturematrix)

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

Serialize the texture into a JSON representation that can be parsed later on.

#### Returns

`any`

the JSON representation of the texture

#### Overrides

[BaseTexture](BaseTexture.md).[serialize](BaseTexture.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:393

___

### setReflectionTextureMatrix

▸ **setReflectionTextureMatrix**(`value`): `void`

Set the texture reflection matrix used to rotate/transform the reflection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Matrix`](Matrix.md) | Define the reflection matrix to set |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:335

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

▸ `Static` **Parse**(`parsedTexture`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`HDRCubeTexture`](HDRCubeTexture.md)

Parses a JSON representation of an HDR Texture in order to create the texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTexture` | `any` | Define the JSON representation |
| `scene` | [`Scene`](Scene.md) | Define the scene the texture should be created in |
| `rootUrl` | `string` | Define the root url in case we need to load relative dependencies |

#### Returns

[`Nullable`](../modules.md#nullable)[`HDRCubeTexture`](HDRCubeTexture.md)

the newly created texture after parsing

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/hdrCubeTexture.ts:362

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

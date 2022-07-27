[@dev/core](../README.md) / [Exports](../modules.md) / EquiRectangularCubeTexture

# Class: EquiRectangularCubeTexture

This represents a texture coming from an equirectangular image supported by the web browser canvas.

## Hierarchy

- [`BaseTexture`](BaseTexture.md)

  ↳ **`EquiRectangularCubeTexture`**

## Table of contents

### Constructors

- [constructor](EquiRectangularCubeTexture.md#constructor)

### Properties

- [\_buffer](EquiRectangularCubeTexture.md#_buffer)
- [\_coordinatesIndex](EquiRectangularCubeTexture.md#_coordinatesindex)
- [\_coordinatesMode](EquiRectangularCubeTexture.md#_coordinatesmode)
- [\_engine](EquiRectangularCubeTexture.md#_engine)
- [\_errorObject](EquiRectangularCubeTexture.md#_errorobject)
- [\_height](EquiRectangularCubeTexture.md#_height)
- [\_loadingError](EquiRectangularCubeTexture.md#_loadingerror)
- [\_noMipmap](EquiRectangularCubeTexture.md#_nomipmap)
- [\_onError](EquiRectangularCubeTexture.md#_onerror)
- [\_onLoad](EquiRectangularCubeTexture.md#_onload)
- [\_scene](EquiRectangularCubeTexture.md#_scene)
- [\_size](EquiRectangularCubeTexture.md#_size)
- [\_width](EquiRectangularCubeTexture.md#_width)
- [\_wrapU](EquiRectangularCubeTexture.md#_wrapu)
- [\_wrapV](EquiRectangularCubeTexture.md#_wrapv)
- [animations](EquiRectangularCubeTexture.md#animations)
- [anisotropicFilteringLevel](EquiRectangularCubeTexture.md#anisotropicfilteringlevel)
- [delayLoadState](EquiRectangularCubeTexture.md#delayloadstate)
- [invertZ](EquiRectangularCubeTexture.md#invertz)
- [isRenderTarget](EquiRectangularCubeTexture.md#isrendertarget)
- [level](EquiRectangularCubeTexture.md#level)
- [metadata](EquiRectangularCubeTexture.md#metadata)
- [name](EquiRectangularCubeTexture.md#name)
- [onDisposeObservable](EquiRectangularCubeTexture.md#ondisposeobservable)
- [reservedDataStore](EquiRectangularCubeTexture.md#reserveddatastore)
- [sphericalPolynomial](EquiRectangularCubeTexture.md#sphericalpolynomial)
- [uniqueId](EquiRectangularCubeTexture.md#uniqueid)
- [url](EquiRectangularCubeTexture.md#url)
- [wrapR](EquiRectangularCubeTexture.md#wrapr)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](EquiRectangularCubeTexture.md#default_anisotropic_filtering_level)
- [\_FacesMapping](EquiRectangularCubeTexture.md#_facesmapping)

### Accessors

- [canRescale](EquiRectangularCubeTexture.md#canrescale)
- [coordinatesIndex](EquiRectangularCubeTexture.md#coordinatesindex)
- [coordinatesMode](EquiRectangularCubeTexture.md#coordinatesmode)
- [errorObject](EquiRectangularCubeTexture.md#errorobject)
- [gammaSpace](EquiRectangularCubeTexture.md#gammaspace)
- [getAlphaFromRGB](EquiRectangularCubeTexture.md#getalphafromrgb)
- [hasAlpha](EquiRectangularCubeTexture.md#hasalpha)
- [irradianceTexture](EquiRectangularCubeTexture.md#irradiancetexture)
- [is2DArray](EquiRectangularCubeTexture.md#is2darray)
- [is3D](EquiRectangularCubeTexture.md#is3d)
- [isBlocking](EquiRectangularCubeTexture.md#isblocking)
- [isCube](EquiRectangularCubeTexture.md#iscube)
- [isRGBD](EquiRectangularCubeTexture.md#isrgbd)
- [linearSpecularLOD](EquiRectangularCubeTexture.md#linearspecularlod)
- [loadingError](EquiRectangularCubeTexture.md#loadingerror)
- [lodGenerationOffset](EquiRectangularCubeTexture.md#lodgenerationoffset)
- [lodGenerationScale](EquiRectangularCubeTexture.md#lodgenerationscale)
- [noMipmap](EquiRectangularCubeTexture.md#nomipmap)
- [onDispose](EquiRectangularCubeTexture.md#ondispose)
- [samplingMode](EquiRectangularCubeTexture.md#samplingmode)
- [textureFormat](EquiRectangularCubeTexture.md#textureformat)
- [textureType](EquiRectangularCubeTexture.md#texturetype)
- [uid](EquiRectangularCubeTexture.md#uid)
- [wrapU](EquiRectangularCubeTexture.md#wrapu)
- [wrapV](EquiRectangularCubeTexture.md#wrapv)

### Methods

- [\_getFloat32ArrayFromArrayBuffer](EquiRectangularCubeTexture.md#_getfloat32arrayfromarraybuffer)
- [\_loadImage](EquiRectangularCubeTexture.md#_loadimage)
- [\_loadTexture](EquiRectangularCubeTexture.md#_loadtexture)
- [\_markAllSubMeshesAsTexturesDirty](EquiRectangularCubeTexture.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](EquiRectangularCubeTexture.md#checktransformsareidentical)
- [clone](EquiRectangularCubeTexture.md#clone)
- [delayLoad](EquiRectangularCubeTexture.md#delayload)
- [dispose](EquiRectangularCubeTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](EquiRectangularCubeTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](EquiRectangularCubeTexture.md#getbasesize)
- [getClassName](EquiRectangularCubeTexture.md#getclassname)
- [getInternalTexture](EquiRectangularCubeTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](EquiRectangularCubeTexture.md#getreflectiontexturematrix)
- [getScene](EquiRectangularCubeTexture.md#getscene)
- [getSize](EquiRectangularCubeTexture.md#getsize)
- [getTextureMatrix](EquiRectangularCubeTexture.md#gettexturematrix)
- [isReady](EquiRectangularCubeTexture.md#isready)
- [isReadyOrNotBlocking](EquiRectangularCubeTexture.md#isreadyornotblocking)
- [readPixels](EquiRectangularCubeTexture.md#readpixels)
- [releaseInternalTexture](EquiRectangularCubeTexture.md#releaseinternaltexture)
- [scale](EquiRectangularCubeTexture.md#scale)
- [serialize](EquiRectangularCubeTexture.md#serialize)
- [toString](EquiRectangularCubeTexture.md#tostring)
- [updateSamplingMode](EquiRectangularCubeTexture.md#updatesamplingmode)
- [WhenAllReady](EquiRectangularCubeTexture.md#whenallready)

## Constructors

### constructor

• **new EquiRectangularCubeTexture**(`url`, `scene`, `size`, `noMipmap?`, `gammaSpace?`, `onLoad?`, `onError?`)

Instantiates an EquiRectangularCubeTexture from the following parameters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | The location of the image |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the texture will be used in |
| `size` | `number` | `undefined` | The cubemap desired size (the more it increases the longer the generation will be) |
| `noMipmap` | `boolean` | `false` | Forces to not generate the mipmap if true |
| `gammaSpace` | `boolean` | `true` | Specifies if the texture will be used in gamma or linear space  (the PBR material requires those textures in linear space, but the standard material would require them in Gamma space) |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | — defines a callback called when texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` | — defines a callback called if there is an error |

#### Overrides

[BaseTexture](BaseTexture.md).[constructor](BaseTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:48

## Properties

### \_buffer

• `Private` **\_buffer**: `ArrayBuffer`

The buffer of the image.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:26

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

### \_height

• `Private` **\_height**: `number`

The height of the input image.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:32

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[BaseTexture](BaseTexture.md).[_loadingError](BaseTexture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_noMipmap

• `Private` **\_noMipmap**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:18

___

### \_onError

• `Private` **\_onError**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:20

___

### \_onLoad

• `Private` **\_onLoad**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:19

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[BaseTexture](BaseTexture.md).[_scene](BaseTexture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_size

• `Private` **\_size**: `number`

The size of the cubemap.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:23

___

### \_width

• `Private` **\_width**: `number`

The width of the input image.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:29

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

The URL to the image.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:35

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

___

### \_FacesMapping

▪ `Static` `Private` **\_FacesMapping**: `string`[]

The six faces of the cube.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:16

## Accessors

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

#### Inherited from

BaseTexture.noMipmap

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:325

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

### \_getFloat32ArrayFromArrayBuffer

▸ `Private` **_getFloat32ArrayFromArrayBuffer**(`buffer`): `Float32Array`

Convert the ArrayBuffer into a Float32Array and drop the transparency channel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | `ArrayBuffer` | The ArrayBuffer that should be converted. |

#### Returns

`Float32Array`

The buffer as Float32Array.

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:171

___

### \_loadImage

▸ `Private` **_loadImage**(`loadTextureCallback`, `onError`): `void`

Load the image data, by putting the image on a canvas and extracting its buffer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `loadTextureCallback` | () => `void` |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:97

___

### \_loadTexture

▸ `Private` **_loadTexture**(): `void`

Convert the image buffer into a cubemap and create a CubeTexture.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:128

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

▸ **clone**(): [`EquiRectangularCubeTexture`](EquiRectangularCubeTexture.md)

Create a clone of the current EquiRectangularCubeTexture and return it.

#### Returns

[`EquiRectangularCubeTexture`](EquiRectangularCubeTexture.md)

A clone of the current EquiRectangularCubeTexture.

#### Overrides

[BaseTexture](BaseTexture.md).[clone](BaseTexture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:198

___

### delayLoad

▸ **delayLoad**(): `void`

Triggers the load sequence in delayed load mode.

#### Returns

`void`

#### Inherited from

[BaseTexture](BaseTexture.md).[delayLoad](BaseTexture.md#delayload)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:182

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

"EquiRectangularCubeTexture"

#### Overrides

[BaseTexture](BaseTexture.md).[getClassName](BaseTexture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/equiRectangularCubeTexture.ts:190

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

Get the texture reflection matrix used to rotate/transform the reflection.

#### Returns

[`Matrix`](Matrix.md)

the reflection matrix

#### Inherited from

[BaseTexture](BaseTexture.md).[getReflectionTextureMatrix](BaseTexture.md#getreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:570

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

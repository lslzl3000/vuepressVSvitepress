[@dev/core](../README.md) / [Exports](../modules.md) / RawTexture2DArray

# Class: RawTexture2DArray

Class used to store 2D array textures containing user data

## Hierarchy

- [`Texture`](Texture.md)

  ↳ **`RawTexture2DArray`**

## Table of contents

### Constructors

- [constructor](RawTexture2DArray.md#constructor)

### Properties

- [\_coordinatesIndex](RawTexture2DArray.md#_coordinatesindex)
- [\_coordinatesMode](RawTexture2DArray.md#_coordinatesmode)
- [\_depth](RawTexture2DArray.md#_depth)
- [\_engine](RawTexture2DArray.md#_engine)
- [\_errorObject](RawTexture2DArray.md#_errorobject)
- [\_format](RawTexture2DArray.md#_format)
- [\_isBlocking](RawTexture2DArray.md#_isblocking)
- [\_loadingError](RawTexture2DArray.md#_loadingerror)
- [\_scene](RawTexture2DArray.md#_scene)
- [\_wrapU](RawTexture2DArray.md#_wrapu)
- [\_wrapV](RawTexture2DArray.md#_wrapv)
- [animations](RawTexture2DArray.md#animations)
- [anisotropicFilteringLevel](RawTexture2DArray.md#anisotropicfilteringlevel)
- [delayLoadState](RawTexture2DArray.md#delayloadstate)
- [format](RawTexture2DArray.md#format)
- [homogeneousRotationInUVTransform](RawTexture2DArray.md#homogeneousrotationinuvtransform)
- [inspectableCustomProperties](RawTexture2DArray.md#inspectablecustomproperties)
- [invertZ](RawTexture2DArray.md#invertz)
- [isRenderTarget](RawTexture2DArray.md#isrendertarget)
- [level](RawTexture2DArray.md#level)
- [metadata](RawTexture2DArray.md#metadata)
- [name](RawTexture2DArray.md#name)
- [onDisposeObservable](RawTexture2DArray.md#ondisposeobservable)
- [onLoadObservable](RawTexture2DArray.md#onloadobservable)
- [reservedDataStore](RawTexture2DArray.md#reserveddatastore)
- [sphericalPolynomial](RawTexture2DArray.md#sphericalpolynomial)
- [uAng](RawTexture2DArray.md#uang)
- [uOffset](RawTexture2DArray.md#uoffset)
- [uRotationCenter](RawTexture2DArray.md#urotationcenter)
- [uScale](RawTexture2DArray.md#uscale)
- [uniqueId](RawTexture2DArray.md#uniqueid)
- [url](RawTexture2DArray.md#url)
- [vAng](RawTexture2DArray.md#vang)
- [vOffset](RawTexture2DArray.md#voffset)
- [vRotationCenter](RawTexture2DArray.md#vrotationcenter)
- [vScale](RawTexture2DArray.md#vscale)
- [wAng](RawTexture2DArray.md#wang)
- [wRotationCenter](RawTexture2DArray.md#wrotationcenter)
- [wrapR](RawTexture2DArray.md#wrapr)
- [BILINEAR\_SAMPLINGMODE](RawTexture2DArray.md#bilinear_samplingmode)
- [CLAMP\_ADDRESSMODE](RawTexture2DArray.md#clamp_addressmode)
- [CUBIC\_MODE](RawTexture2DArray.md#cubic_mode)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](RawTexture2DArray.md#default_anisotropic_filtering_level)
- [EQUIRECTANGULAR\_MODE](RawTexture2DArray.md#equirectangular_mode)
- [EXPLICIT\_MODE](RawTexture2DArray.md#explicit_mode)
- [FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](RawTexture2DArray.md#fixed_equirectangular_mirrored_mode)
- [FIXED\_EQUIRECTANGULAR\_MODE](RawTexture2DArray.md#fixed_equirectangular_mode)
- [ForceSerializeBuffers](RawTexture2DArray.md#forceserializebuffers)
- [INVCUBIC\_MODE](RawTexture2DArray.md#invcubic_mode)
- [LINEAR\_LINEAR](RawTexture2DArray.md#linear_linear)
- [LINEAR\_LINEAR\_MIPLINEAR](RawTexture2DArray.md#linear_linear_miplinear)
- [LINEAR\_LINEAR\_MIPNEAREST](RawTexture2DArray.md#linear_linear_mipnearest)
- [LINEAR\_NEAREST](RawTexture2DArray.md#linear_nearest)
- [LINEAR\_NEAREST\_MIPLINEAR](RawTexture2DArray.md#linear_nearest_miplinear)
- [LINEAR\_NEAREST\_MIPNEAREST](RawTexture2DArray.md#linear_nearest_mipnearest)
- [MIRROR\_ADDRESSMODE](RawTexture2DArray.md#mirror_addressmode)
- [NEAREST\_LINEAR](RawTexture2DArray.md#nearest_linear)
- [NEAREST\_LINEAR\_MIPLINEAR](RawTexture2DArray.md#nearest_linear_miplinear)
- [NEAREST\_LINEAR\_MIPNEAREST](RawTexture2DArray.md#nearest_linear_mipnearest)
- [NEAREST\_NEAREST](RawTexture2DArray.md#nearest_nearest)
- [NEAREST\_NEAREST\_MIPLINEAR](RawTexture2DArray.md#nearest_nearest_miplinear)
- [NEAREST\_NEAREST\_MIPNEAREST](RawTexture2DArray.md#nearest_nearest_mipnearest)
- [NEAREST\_SAMPLINGMODE](RawTexture2DArray.md#nearest_samplingmode)
- [OnTextureLoadErrorObservable](RawTexture2DArray.md#ontextureloaderrorobservable)
- [PLANAR\_MODE](RawTexture2DArray.md#planar_mode)
- [PROJECTION\_MODE](RawTexture2DArray.md#projection_mode)
- [SKYBOX\_MODE](RawTexture2DArray.md#skybox_mode)
- [SPHERICAL\_MODE](RawTexture2DArray.md#spherical_mode)
- [SerializeBuffers](RawTexture2DArray.md#serializebuffers)
- [TRILINEAR\_SAMPLINGMODE](RawTexture2DArray.md#trilinear_samplingmode)
- [UseSerializedUrlIfAny](RawTexture2DArray.md#useserializedurlifany)
- [WRAP\_ADDRESSMODE](RawTexture2DArray.md#wrap_addressmode)

### Accessors

- [canRescale](RawTexture2DArray.md#canrescale)
- [coordinatesIndex](RawTexture2DArray.md#coordinatesindex)
- [coordinatesMode](RawTexture2DArray.md#coordinatesmode)
- [depth](RawTexture2DArray.md#depth)
- [errorObject](RawTexture2DArray.md#errorobject)
- [gammaSpace](RawTexture2DArray.md#gammaspace)
- [getAlphaFromRGB](RawTexture2DArray.md#getalphafromrgb)
- [hasAlpha](RawTexture2DArray.md#hasalpha)
- [invertY](RawTexture2DArray.md#inverty)
- [irradianceTexture](RawTexture2DArray.md#irradiancetexture)
- [is2DArray](RawTexture2DArray.md#is2darray)
- [is3D](RawTexture2DArray.md#is3d)
- [isBlocking](RawTexture2DArray.md#isblocking)
- [isCube](RawTexture2DArray.md#iscube)
- [isRGBD](RawTexture2DArray.md#isrgbd)
- [linearSpecularLOD](RawTexture2DArray.md#linearspecularlod)
- [loadingError](RawTexture2DArray.md#loadingerror)
- [lodGenerationOffset](RawTexture2DArray.md#lodgenerationoffset)
- [lodGenerationScale](RawTexture2DArray.md#lodgenerationscale)
- [mimeType](RawTexture2DArray.md#mimetype)
- [noMipmap](RawTexture2DArray.md#nomipmap)
- [onDispose](RawTexture2DArray.md#ondispose)
- [samplingMode](RawTexture2DArray.md#samplingmode)
- [textureFormat](RawTexture2DArray.md#textureformat)
- [textureType](RawTexture2DArray.md#texturetype)
- [uid](RawTexture2DArray.md#uid)
- [wrapU](RawTexture2DArray.md#wrapu)
- [wrapV](RawTexture2DArray.md#wrapv)

### Methods

- [\_markAllSubMeshesAsTexturesDirty](RawTexture2DArray.md#_markallsubmeshesastexturesdirty)
- [checkTransformsAreIdentical](RawTexture2DArray.md#checktransformsareidentical)
- [clone](RawTexture2DArray.md#clone)
- [dispose](RawTexture2DArray.md#dispose)
- [forceSphericalPolynomialsRecompute](RawTexture2DArray.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](RawTexture2DArray.md#getbasesize)
- [getClassName](RawTexture2DArray.md#getclassname)
- [getInternalTexture](RawTexture2DArray.md#getinternaltexture)
- [getReflectionTextureMatrix](RawTexture2DArray.md#getreflectiontexturematrix)
- [getScene](RawTexture2DArray.md#getscene)
- [getSize](RawTexture2DArray.md#getsize)
- [getTextureMatrix](RawTexture2DArray.md#gettexturematrix)
- [isReady](RawTexture2DArray.md#isready)
- [isReadyOrNotBlocking](RawTexture2DArray.md#isreadyornotblocking)
- [readPixels](RawTexture2DArray.md#readpixels)
- [releaseInternalTexture](RawTexture2DArray.md#releaseinternaltexture)
- [scale](RawTexture2DArray.md#scale)
- [serialize](RawTexture2DArray.md#serialize)
- [toString](RawTexture2DArray.md#tostring)
- [update](RawTexture2DArray.md#update)
- [updateSamplingMode](RawTexture2DArray.md#updatesamplingmode)
- [updateURL](RawTexture2DArray.md#updateurl)
- [CreateFromBase64String](RawTexture2DArray.md#createfrombase64string)
- [CreateRGBATexture](RawTexture2DArray.md#creatergbatexture)
- [LoadFromDataString](RawTexture2DArray.md#loadfromdatastring)
- [Parse](RawTexture2DArray.md#parse)
- [WhenAllReady](RawTexture2DArray.md#whenallready)

## Constructors

### constructor

• **new RawTexture2DArray**(`data`, `width`, `height`, `depth`, `format`, `scene`, `generateMipMaps?`, `invertY?`, `samplingMode?`, `textureType?`)

Create a new RawTexture2DArray

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `ArrayBufferView` | `undefined` | defines the data of the texture |
| `width` | `number` | `undefined` | defines the width of the texture |
| `height` | `number` | `undefined` | defines the height of the texture |
| `depth` | `number` | `undefined` | defines the number of layers of the texture |
| `format` | `number` | `undefined` | defines the texture format to use |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `generateMipMaps` | `boolean` | `true` | defines a boolean indicating if mip levels should be generated (true by default) |
| `invertY` | `boolean` | `false` | defines if texture must be stored with Y axis inverted |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | defines the sampling mode to use (Texture.TRILINEAR_SAMPLINGMODE by default) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the texture Type (Engine.TEXTURETYPE_UNSIGNED_INT, Engine.TEXTURETYPE_FLOAT...) |

#### Overrides

[Texture](Texture.md).[constructor](Texture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:33

## Properties

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[Texture](Texture.md).[_coordinatesIndex](Texture.md#_coordinatesindex)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[Texture](Texture.md).[_coordinatesMode](Texture.md#_coordinatesmode)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:126

___

### \_depth

• `Private` **\_depth**: `number`

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:11

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[Texture](Texture.md).[_engine](Texture.md#_engine)

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

[Texture](Texture.md).[_errorObject](Texture.md#_errorobject)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:483

___

### \_format

• `Protected` **\_format**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Inherited from

[Texture](Texture.md).[_format](Texture.md#_format)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:312

___

### \_isBlocking

• `Protected` **\_isBlocking**: `boolean` = `true`

#### Inherited from

[Texture](Texture.md).[_isBlocking](Texture.md#_isblocking)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:331

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[Texture](Texture.md).[_loadingError](Texture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[Texture](Texture.md).[_scene](Texture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[Texture](Texture.md).[_wrapU](Texture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[Texture](Texture.md).[_wrapV](Texture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[Texture](Texture.md).[animations](Texture.md#animations)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[Texture](Texture.md).[anisotropicFilteringLevel](Texture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:205

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[Texture](Texture.md).[delayLoadState](Texture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### format

• **format**: `number`

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:39

___

### homogeneousRotationInUVTransform

• **homogeneousRotationInUVTransform**: `boolean` = `false`

Sets this property to true to avoid deformations when rotating the texture with non-uniform scaling

#### Inherited from

[Texture](Texture.md).[homogeneousRotationInUVTransform](Texture.md#homogeneousrotationinuvtransform)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:270

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`Nullable`](../modules.md#nullable)[`IInspectable`](../interfaces/IInspectable.md)[] = `null`

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Texture](Texture.md).[inspectableCustomProperties](Texture.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:283

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[Texture](Texture.md).[invertZ](Texture.md#invertz)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[Texture](Texture.md).[isRenderTarget](Texture.md#isrendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[Texture](Texture.md).[level](Texture.md#level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[Texture](Texture.md).[metadata](Texture.md#metadata)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[Texture](Texture.md).[name](Texture.md#name)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:42

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[Texture](Texture.md).[onDisposeObservable](Texture.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:452

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable triggered once the texture has been loaded.

#### Inherited from

[Texture](Texture.md).[onLoadObservable](Texture.md#onloadobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:329

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Texture](Texture.md).[reservedDataStore](Texture.md#reserveddatastore)

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

[Texture](Texture.md).[sphericalPolynomial](Texture.md#sphericalpolynomial)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uAng

• **uAng**: `number` = `0`

Define an offset on the texture to rotate around the u coordinates of the UVs
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[Texture](Texture.md).[uAng](Texture.md#uang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:230

___

### uOffset

• **uOffset**: `number` = `0`

Define an offset on the texture to offset the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[Texture](Texture.md).[uOffset](Texture.md#uoffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:201

___

### uRotationCenter

• **uRotationCenter**: `number` = `0.5`

Defines the center of rotation (U)

#### Inherited from

[Texture](Texture.md).[uRotationCenter](Texture.md#urotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:252

___

### uScale

• **uScale**: `number` = `1.0`

Define an offset on the texture to scale the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[Texture](Texture.md).[uScale](Texture.md#uscale)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:215

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[Texture](Texture.md).[uniqueId](Texture.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: [`Nullable`](../modules.md#nullable)`string` = `null`

Define the url of the texture.

#### Inherited from

[Texture](Texture.md).[url](Texture.md#url)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:194

___

### vAng

• **vAng**: `number` = `0`

Define an offset on the texture to rotate around the v coordinates of the UVs
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[Texture](Texture.md).[vAng](Texture.md#vang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:238

___

### vOffset

• **vOffset**: `number` = `0`

Define an offset on the texture to offset the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[Texture](Texture.md).[vOffset](Texture.md#voffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:208

___

### vRotationCenter

• **vRotationCenter**: `number` = `0.5`

Defines the center of rotation (V)

#### Inherited from

[Texture](Texture.md).[vRotationCenter](Texture.md#vrotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:258

___

### vScale

• **vScale**: `number` = `1.0`

Define an offset on the texture to scale the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[Texture](Texture.md).[vScale](Texture.md#vscale)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:222

___

### wAng

• **wAng**: `number` = `0`

Define an offset on the texture to rotate around the w coordinates of the UVs (in case of 3d texture)
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[Texture](Texture.md).[wAng](Texture.md#wang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:246

___

### wRotationCenter

• **wRotationCenter**: `number` = `0.5`

Defines the center of rotation (W)

#### Inherited from

[Texture](Texture.md).[wRotationCenter](Texture.md#wrotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:264

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Inherited from

[Texture](Texture.md).[wrapR](Texture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:197

___

### BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[BILINEAR_SAMPLINGMODE](Texture.md#bilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:129

___

### CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Inherited from

[Texture](Texture.md).[CLAMP_ADDRESSMODE](Texture.md#clamp_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:179

___

### CUBIC\_MODE

▪ `Static` `Readonly` **CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[CUBIC_MODE](Texture.md#cubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:164

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[Texture](Texture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](Texture.md#default_anisotropic_filtering_level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:30

___

### EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Inherited from

[Texture](Texture.md).[EQUIRECTANGULAR_MODE](Texture.md#equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:172

___

### EXPLICIT\_MODE

▪ `Static` `Readonly` **EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Inherited from

[Texture](Texture.md).[EXPLICIT_MODE](Texture.md#explicit_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:158

___

### FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Inherited from

[Texture](Texture.md).[FIXED_EQUIRECTANGULAR_MIRRORED_MODE](Texture.md#fixed_equirectangular_mirrored_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:176

___

### FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Inherited from

[Texture](Texture.md).[FIXED_EQUIRECTANGULAR_MODE](Texture.md#fixed_equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:174

___

### ForceSerializeBuffers

▪ `Static` **ForceSerializeBuffers**: `boolean` = `false`

Gets or sets a general boolean used to indicate that texture buffers must be saved as part of the serialization process.
If no buffer exists, one will be created as base64 string from the internal webgl data.

#### Inherited from

[Texture](Texture.md).[ForceSerializeBuffers](Texture.md#forceserializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:82

___

### INVCUBIC\_MODE

▪ `Static` `Readonly` **INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[INVCUBIC_MODE](Texture.md#invcubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:170

___

### LINEAR\_LINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR](Texture.md#linear_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:153

___

### LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR_MIPLINEAR](Texture.md#linear_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:136

___

### LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR_MIPNEAREST](Texture.md#linear_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:131

___

### LINEAR\_NEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST](Texture.md#linear_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:155

___

### LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST_MIPLINEAR](Texture.md#linear_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:151

___

### LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST_MIPNEAREST](Texture.md#linear_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:149

___

### MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Inherited from

[Texture](Texture.md).[MIRROR_ADDRESSMODE](Texture.md#mirror_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:183

___

### NEAREST\_LINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR](Texture.md#nearest_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:145

___

### NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR_MIPLINEAR](Texture.md#nearest_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:143

___

### NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR_MIPNEAREST](Texture.md#nearest_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:141

___

### NEAREST\_NEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST](Texture.md#nearest_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:147

___

### NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST_MIPLINEAR](Texture.md#nearest_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:126

___

### NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST_MIPNEAREST](Texture.md#nearest_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:139

___

### NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_SAMPLINGMODE](Texture.md#nearest_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:124

___

### OnTextureLoadErrorObservable

▪ `Static` **OnTextureLoadErrorObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

This observable will notify when any texture had a loading error

#### Inherited from

[Texture](Texture.md).[OnTextureLoadErrorObservable](Texture.md#ontextureloaderrorobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:87

___

### PLANAR\_MODE

▪ `Static` `Readonly` **PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Inherited from

[Texture](Texture.md).[PLANAR_MODE](Texture.md#planar_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:162

___

### PROJECTION\_MODE

▪ `Static` `Readonly` **PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Inherited from

[Texture](Texture.md).[PROJECTION_MODE](Texture.md#projection_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:166

___

### SKYBOX\_MODE

▪ `Static` `Readonly` **SKYBOX\_MODE**: ``5``

Inverse Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[SKYBOX_MODE](Texture.md#skybox_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:168

___

### SPHERICAL\_MODE

▪ `Static` `Readonly` **SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Inherited from

[Texture](Texture.md).[SPHERICAL_MODE](Texture.md#spherical_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:160

___

### SerializeBuffers

▪ `Static` **SerializeBuffers**: `boolean` = `true`

Gets or sets a general boolean used to indicate that textures containing direct data (buffers) must be saved as part of the serialization process

#### Inherited from

[Texture](Texture.md).[SerializeBuffers](Texture.md#serializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:76

___

### TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[TRILINEAR_SAMPLINGMODE](Texture.md#trilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:134

___

### UseSerializedUrlIfAny

▪ `Static` **UseSerializedUrlIfAny**: `boolean` = `false`

Gets or sets a boolean which defines if the texture url must be build from the serialized URL instead of just using the name and loading them side by side with the scene file

#### Inherited from

[Texture](Texture.md).[UseSerializedUrlIfAny](Texture.md#useserializedurlifany)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:188

___

### WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Inherited from

[Texture](Texture.md).[WRAP_ADDRESSMODE](Texture.md#wrap_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:181

## Accessors

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

Texture.canRescale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

Texture.coordinatesIndex

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

Texture.coordinatesIndex

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

Texture.coordinatesMode

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

Texture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:144

___

### depth

• `get` **depth**(): `number`

Gets the number of layers of the texture

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:16

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

Texture.errorObject

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

Texture.gammaSpace

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

Texture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Texture.getAlphaFromRGB

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

Texture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Texture.hasAlpha

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

Texture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:60

___

### invertY

• `get` **invertY**(): `boolean`

Gets a boolean indicating if the texture needs to be inverted on the y axis during loading

#### Returns

`boolean`

#### Inherited from

Texture.invertY

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:347

___

### irradianceTexture

• `get` **irradianceTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

In case a better definition than spherical harmonics is required for the diffuse part of the environment.
You can set the irradiance texture to rely on a texture instead of the spherical approach.
This texture need to have the same characteristics than its parent (Cube vs 2d, coordinates mode, Gamma/Linear, RGBD).

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

Texture.irradianceTexture

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

Texture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.is2DArray

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

Texture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.is3D

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

Texture.is3D

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

Texture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:339

• `set` **isBlocking**(`value`): `void`

Is the texture preventing material to render while loading.
If false, a default texture will be used instead of the loading one during the preparation step.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Texture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:336

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.isCube

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

Texture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

Texture.isRGBD

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

Texture.isRGBD

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

Texture.linearSpecularLOD

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

Texture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

Texture.loadingError

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

Texture.lodGenerationOffset

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

Texture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

Texture.lodGenerationScale

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

Texture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:363

___

### mimeType

• `get` **mimeType**(): `undefined` \| `string`

Returns the texture mime type if it was defined by a loader (undefined else)

#### Returns

`undefined` \| `string`

#### Inherited from

Texture.mimeType

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:322

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

Texture.noMipmap

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:275

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

Texture.onDispose

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:459

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

Texture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

Texture.textureFormat

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

Texture.textureType

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

Texture.uid

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

Texture.wrapU

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

Texture.wrapU

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

Texture.wrapV

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

Texture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[_markAllSubMeshesAsTexturesDirty](Texture.md#_markallsubmeshesastexturesdirty)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:670

___

### checkTransformsAreIdentical

▸ **checkTransformsAreIdentical**(`texture`): `boolean`

Checks if the texture has the same transform matrix than another texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) | texture to check against |

#### Returns

`boolean`

true if the transforms are the same, else false

#### Inherited from

[Texture](Texture.md).[checkTransformsAreIdentical](Texture.md#checktransformsareidentical)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:633

___

### clone

▸ **clone**(): [`Texture`](Texture.md)

Clones the texture.

#### Returns

[`Texture`](Texture.md)

the cloned texture

#### Inherited from

[Texture](Texture.md).[clone](Texture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:827

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[dispose](Texture.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:904

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[forceSphericalPolynomialsRecompute](Texture.md#forcesphericalpolynomialsrecompute)

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

[Texture](Texture.md).[getBaseSize](Texture.md#getbasesize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name of the texture useful for serialization or dynamic coding.

#### Returns

`string`

"Texture"

#### Inherited from

[Texture](Texture.md).[getClassName](Texture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:897

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Inherited from

[Texture](Texture.md).[getInternalTexture](Texture.md#getinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Get the current matrix used to apply reflection. This is useful to rotate an environment texture for instance.

#### Returns

[`Matrix`](Matrix.md)

The reflection texture transform

#### Inherited from

[Texture](Texture.md).[getReflectionTextureMatrix](Texture.md#getreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:751

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

#### Inherited from

[Texture](Texture.md).[getScene](Texture.md#getscene)

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

[Texture](Texture.md).[getSize](Texture.md#getsize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:196

___

### getTextureMatrix

▸ **getTextureMatrix**(`uBase?`): [`Matrix`](Matrix.md)

Get the current texture matrix which includes the requested offsetting, tiling and rotation components.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `uBase` | `number` | `1` |

#### Returns

[`Matrix`](Matrix.md)

the transform matrix of the texture.

#### Inherited from

[Texture](Texture.md).[getTextureMatrix](Texture.md#gettexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:651

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Inherited from

[Texture](Texture.md).[isReady](Texture.md#isready)

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

[Texture](Texture.md).[isReadyOrNotBlocking](Texture.md#isreadyornotblocking)

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

[Texture](Texture.md).[readPixels](Texture.md#readpixels)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[releaseInternalTexture](Texture.md#releaseinternaltexture)

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

[Texture](Texture.md).[scale](Texture.md#scale)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:587

___

### serialize

▸ **serialize**(): `any`

Serialize the texture to a JSON representation we can easily use in the respective Parse function.

#### Returns

`any`

The JSON representation of the texture

#### Inherited from

[Texture](Texture.md).[serialize](Texture.md#serialize)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:852

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

#### Inherited from

[Texture](Texture.md).[toString](Texture.md#tostring)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:432

___

### update

▸ **update**(`data`): `void`

Update the texture with new data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | defines the data to store in the texture |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:58

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

[Texture](Texture.md).[updateSamplingMode](Texture.md#updatesamplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:275

___

### updateURL

▸ **updateURL**(`url`, `buffer?`, `onLoad?`, `forcedExtension?`): `void`

Update the url (and optional buffer) of this texture if url was null during construction.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | the url of the texture |
| `buffer` | [`Nullable`](../modules.md#nullable)`string` \| `ArrayBuffer` \| `ArrayBufferView` \| `Blob` \| `HTMLImageElement` | `null` | the buffer of the texture (defaults to null) |
| `onLoad?` | () => `void` | `undefined` | callback called when the texture is loaded  (defaults to null) |
| `forcedExtension?` | `string` | `undefined` | defines the extension to use to pick the right loader |

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[updateURL](Texture.md#updateurl)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:539

___

### CreateFromBase64String

▸ `Static` **CreateFromBase64String**(`data`, `name`, `scene`, `noMipmapOrOptions?`, `invertY?`, `samplingMode?`, `onLoad?`, `onError?`, `format?`, `creationFlags?`): [`Texture`](Texture.md)

Creates a texture from its base 64 representation.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `string` | `undefined` | Define the base64 payload without the data: prefix |
| `name` | `string` | `undefined` | Define the name of the texture in the scene useful fo caching purpose for instance |
| `scene` | [`Scene`](Scene.md) | `undefined` | Define the scene the texture should belong to |
| `noMipmapOrOptions?` | `boolean` \| [`ITextureCreationOptions`](../interfaces/ITextureCreationOptions.md) | `undefined` | defines if the texture will require mip maps or not or set of all options to create the texture |
| `invertY?` | `boolean` | `undefined` | define if the texture needs to be inverted on the y axis during loading |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | define the sampling mode we want for the texture while fetching from it (Texture.NEAREST_SAMPLINGMODE...) |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when the texture has been loaded |
| `onError` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when an error occurred during the loading session |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | define the format of the texture we are trying to load (Engine.TEXTUREFORMAT_RGBA...) |
| `creationFlags?` | `number` | `undefined` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`Texture`](Texture.md)

the created texture

#### Inherited from

[Texture](Texture.md).[CreateFromBase64String](Texture.md#createfrombase64string)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:1057

___

### CreateRGBATexture

▸ `Static` **CreateRGBATexture**(`data`, `width`, `height`, `depth`, `scene`, `generateMipMaps?`, `invertY?`, `samplingMode?`, `type?`): [`RawTexture2DArray`](RawTexture2DArray.md)

Creates a RGBA texture from some data.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `ArrayBufferView` | `undefined` | Define the texture data |
| `width` | `number` | `undefined` | Define the width of the texture |
| `height` | `number` | `undefined` | Define the height of the texture |
| `depth` | `number` | `undefined` | defines the number of layers of the texture |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the scene the texture will belong to |
| `generateMipMaps` | `boolean` | `true` | Define whether or not to create mip maps for the texture |
| `invertY` | `boolean` | `false` | define if the data should be flipped on Y when uploaded to the GPU |
| `samplingMode` | `number` | `Constants.TEXTURE_TRILINEAR_SAMPLINGMODE` | define the texture sampling mode (Texture.xxx_SAMPLINGMODE) |
| `type` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | define the format of the data (int, float... Engine.TEXTURETYPE_xxx) |

#### Returns

[`RawTexture2DArray`](RawTexture2DArray.md)

the RGBA texture

#### Defined in

packages/dev/core/src/Materials/Textures/rawTexture2DArray.ts:78

___

### LoadFromDataString

▸ `Static` **LoadFromDataString**(`name`, `buffer`, `scene`, `deleteBuffer?`, `noMipmapOrOptions?`, `invertY?`, `samplingMode?`, `onLoad?`, `onError?`, `format?`, `creationFlags?`): [`Texture`](Texture.md)

Creates a texture from its data: representation. (data: will be added in case only the payload has been passed in)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Define the name of the texture in the scene useful fo caching purpose for instance |
| `buffer` | `any` | `undefined` | define the buffer to load the texture from in case the texture is loaded from a buffer representation |
| `scene` | [`Scene`](Scene.md) | `undefined` | Define the scene the texture should belong to |
| `deleteBuffer` | `boolean` | `false` | define if the buffer we are loading the texture from should be deleted after load |
| `noMipmapOrOptions?` | `boolean` \| [`ITextureCreationOptions`](../interfaces/ITextureCreationOptions.md) | `undefined` | defines if the texture will require mip maps or not or set of all options to create the texture |
| `invertY` | `boolean` | `true` | define if the texture needs to be inverted on the y axis during loading |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | define the sampling mode we want for the texture while fetching from it (Texture.NEAREST_SAMPLINGMODE...) |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when the texture has been loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` | define a callback triggered when an error occurred during the loading session |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | define the format of the texture we are trying to load (Engine.TEXTUREFORMAT_RGBA...) |
| `creationFlags?` | `number` | `undefined` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`Texture`](Texture.md)

the created texture

#### Inherited from

[Texture](Texture.md).[LoadFromDataString](Texture.md#loadfromdatastring)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:1087

___

### Parse

▸ `Static` **Parse**(`parsedTexture`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Parse the JSON representation of a texture in order to recreate the texture in the given scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTexture` | `any` | Define the JSON representation of the texture |
| `scene` | [`Scene`](Scene.md) | Define the scene the parsed texture should be instantiated in |
| `rootUrl` | `string` | Define the root url of the parsing sequence in the case of relative dependencies |

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The parsed texture if successful

#### Inherited from

[Texture](Texture.md).[Parse](Texture.md#parse)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:920

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

[Texture](Texture.md).[WhenAllReady](Texture.md#whenallready)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:864

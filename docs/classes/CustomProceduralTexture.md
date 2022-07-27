[@dev/core](../README.md) / [Exports](../modules.md) / CustomProceduralTexture

# Class: CustomProceduralTexture

Procedural texturing is a way to programmatically create a texture. There are 2 types of procedural textures: code-only, and code that references some classic 2D images, sometimes called 'refMaps' or 'sampler' images.
Custom Procedural textures are the easiest way to create your own procedural in your application.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures#creating-custom-procedural-textures

## Hierarchy

- [`ProceduralTexture`](ProceduralTexture.md)

  ↳ **`CustomProceduralTexture`**

## Table of contents

### Constructors

- [constructor](CustomProceduralTexture.md#constructor)

### Properties

- [\_animate](CustomProceduralTexture.md#_animate)
- [\_config](CustomProceduralTexture.md#_config)
- [\_coordinatesIndex](CustomProceduralTexture.md#_coordinatesindex)
- [\_coordinatesMode](CustomProceduralTexture.md#_coordinatesmode)
- [\_engine](CustomProceduralTexture.md#_engine)
- [\_errorObject](CustomProceduralTexture.md#_errorobject)
- [\_format](CustomProceduralTexture.md#_format)
- [\_isBlocking](CustomProceduralTexture.md#_isblocking)
- [\_loadingError](CustomProceduralTexture.md#_loadingerror)
- [\_scene](CustomProceduralTexture.md#_scene)
- [\_texturePath](CustomProceduralTexture.md#_texturepath)
- [\_time](CustomProceduralTexture.md#_time)
- [\_wrapU](CustomProceduralTexture.md#_wrapu)
- [\_wrapV](CustomProceduralTexture.md#_wrapv)
- [animations](CustomProceduralTexture.md#animations)
- [anisotropicFilteringLevel](CustomProceduralTexture.md#anisotropicfilteringlevel)
- [autoClear](CustomProceduralTexture.md#autoclear)
- [delayLoadState](CustomProceduralTexture.md#delayloadstate)
- [homogeneousRotationInUVTransform](CustomProceduralTexture.md#homogeneousrotationinuvtransform)
- [inspectableCustomProperties](CustomProceduralTexture.md#inspectablecustomproperties)
- [invertZ](CustomProceduralTexture.md#invertz)
- [isEnabled](CustomProceduralTexture.md#isenabled)
- [isRenderTarget](CustomProceduralTexture.md#isrendertarget)
- [level](CustomProceduralTexture.md#level)
- [metadata](CustomProceduralTexture.md#metadata)
- [name](CustomProceduralTexture.md#name)
- [nodeMaterialSource](CustomProceduralTexture.md#nodematerialsource)
- [onBeforeGenerationObservable](CustomProceduralTexture.md#onbeforegenerationobservable)
- [onDisposeObservable](CustomProceduralTexture.md#ondisposeobservable)
- [onGenerated](CustomProceduralTexture.md#ongenerated)
- [onGeneratedObservable](CustomProceduralTexture.md#ongeneratedobservable)
- [onLoadObservable](CustomProceduralTexture.md#onloadobservable)
- [reservedDataStore](CustomProceduralTexture.md#reserveddatastore)
- [sphericalPolynomial](CustomProceduralTexture.md#sphericalpolynomial)
- [uAng](CustomProceduralTexture.md#uang)
- [uOffset](CustomProceduralTexture.md#uoffset)
- [uRotationCenter](CustomProceduralTexture.md#urotationcenter)
- [uScale](CustomProceduralTexture.md#uscale)
- [uniqueId](CustomProceduralTexture.md#uniqueid)
- [url](CustomProceduralTexture.md#url)
- [vAng](CustomProceduralTexture.md#vang)
- [vOffset](CustomProceduralTexture.md#voffset)
- [vRotationCenter](CustomProceduralTexture.md#vrotationcenter)
- [vScale](CustomProceduralTexture.md#vscale)
- [wAng](CustomProceduralTexture.md#wang)
- [wRotationCenter](CustomProceduralTexture.md#wrotationcenter)
- [wrapR](CustomProceduralTexture.md#wrapr)
- [BILINEAR\_SAMPLINGMODE](CustomProceduralTexture.md#bilinear_samplingmode)
- [CLAMP\_ADDRESSMODE](CustomProceduralTexture.md#clamp_addressmode)
- [CUBIC\_MODE](CustomProceduralTexture.md#cubic_mode)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](CustomProceduralTexture.md#default_anisotropic_filtering_level)
- [EQUIRECTANGULAR\_MODE](CustomProceduralTexture.md#equirectangular_mode)
- [EXPLICIT\_MODE](CustomProceduralTexture.md#explicit_mode)
- [FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](CustomProceduralTexture.md#fixed_equirectangular_mirrored_mode)
- [FIXED\_EQUIRECTANGULAR\_MODE](CustomProceduralTexture.md#fixed_equirectangular_mode)
- [ForceSerializeBuffers](CustomProceduralTexture.md#forceserializebuffers)
- [INVCUBIC\_MODE](CustomProceduralTexture.md#invcubic_mode)
- [LINEAR\_LINEAR](CustomProceduralTexture.md#linear_linear)
- [LINEAR\_LINEAR\_MIPLINEAR](CustomProceduralTexture.md#linear_linear_miplinear)
- [LINEAR\_LINEAR\_MIPNEAREST](CustomProceduralTexture.md#linear_linear_mipnearest)
- [LINEAR\_NEAREST](CustomProceduralTexture.md#linear_nearest)
- [LINEAR\_NEAREST\_MIPLINEAR](CustomProceduralTexture.md#linear_nearest_miplinear)
- [LINEAR\_NEAREST\_MIPNEAREST](CustomProceduralTexture.md#linear_nearest_mipnearest)
- [MIRROR\_ADDRESSMODE](CustomProceduralTexture.md#mirror_addressmode)
- [NEAREST\_LINEAR](CustomProceduralTexture.md#nearest_linear)
- [NEAREST\_LINEAR\_MIPLINEAR](CustomProceduralTexture.md#nearest_linear_miplinear)
- [NEAREST\_LINEAR\_MIPNEAREST](CustomProceduralTexture.md#nearest_linear_mipnearest)
- [NEAREST\_NEAREST](CustomProceduralTexture.md#nearest_nearest)
- [NEAREST\_NEAREST\_MIPLINEAR](CustomProceduralTexture.md#nearest_nearest_miplinear)
- [NEAREST\_NEAREST\_MIPNEAREST](CustomProceduralTexture.md#nearest_nearest_mipnearest)
- [NEAREST\_SAMPLINGMODE](CustomProceduralTexture.md#nearest_samplingmode)
- [OnTextureLoadErrorObservable](CustomProceduralTexture.md#ontextureloaderrorobservable)
- [PLANAR\_MODE](CustomProceduralTexture.md#planar_mode)
- [PROJECTION\_MODE](CustomProceduralTexture.md#projection_mode)
- [SKYBOX\_MODE](CustomProceduralTexture.md#skybox_mode)
- [SPHERICAL\_MODE](CustomProceduralTexture.md#spherical_mode)
- [SerializeBuffers](CustomProceduralTexture.md#serializebuffers)
- [TRILINEAR\_SAMPLINGMODE](CustomProceduralTexture.md#trilinear_samplingmode)
- [UseSerializedUrlIfAny](CustomProceduralTexture.md#useserializedurlifany)
- [WRAP\_ADDRESSMODE](CustomProceduralTexture.md#wrap_addressmode)

### Accessors

- [animate](CustomProceduralTexture.md#animate)
- [canRescale](CustomProceduralTexture.md#canrescale)
- [coordinatesIndex](CustomProceduralTexture.md#coordinatesindex)
- [coordinatesMode](CustomProceduralTexture.md#coordinatesmode)
- [errorObject](CustomProceduralTexture.md#errorobject)
- [gammaSpace](CustomProceduralTexture.md#gammaspace)
- [getAlphaFromRGB](CustomProceduralTexture.md#getalphafromrgb)
- [hasAlpha](CustomProceduralTexture.md#hasalpha)
- [invertY](CustomProceduralTexture.md#inverty)
- [irradianceTexture](CustomProceduralTexture.md#irradiancetexture)
- [is2DArray](CustomProceduralTexture.md#is2darray)
- [is3D](CustomProceduralTexture.md#is3d)
- [isBlocking](CustomProceduralTexture.md#isblocking)
- [isCube](CustomProceduralTexture.md#iscube)
- [isRGBD](CustomProceduralTexture.md#isrgbd)
- [linearSpecularLOD](CustomProceduralTexture.md#linearspecularlod)
- [loadingError](CustomProceduralTexture.md#loadingerror)
- [lodGenerationOffset](CustomProceduralTexture.md#lodgenerationoffset)
- [lodGenerationScale](CustomProceduralTexture.md#lodgenerationscale)
- [mimeType](CustomProceduralTexture.md#mimetype)
- [noMipmap](CustomProceduralTexture.md#nomipmap)
- [onDispose](CustomProceduralTexture.md#ondispose)
- [refreshRate](CustomProceduralTexture.md#refreshrate)
- [samplingMode](CustomProceduralTexture.md#samplingmode)
- [textureFormat](CustomProceduralTexture.md#textureformat)
- [textureType](CustomProceduralTexture.md#texturetype)
- [uid](CustomProceduralTexture.md#uid)
- [wrapU](CustomProceduralTexture.md#wrapu)
- [wrapV](CustomProceduralTexture.md#wrapv)

### Methods

- [\_getDefines](CustomProceduralTexture.md#_getdefines)
- [\_loadJson](CustomProceduralTexture.md#_loadjson)
- [\_markAllSubMeshesAsTexturesDirty](CustomProceduralTexture.md#_markallsubmeshesastexturesdirty)
- [\_setEffect](CustomProceduralTexture.md#_seteffect)
- [checkTransformsAreIdentical](CustomProceduralTexture.md#checktransformsareidentical)
- [clone](CustomProceduralTexture.md#clone)
- [dispose](CustomProceduralTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](CustomProceduralTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](CustomProceduralTexture.md#getbasesize)
- [getClassName](CustomProceduralTexture.md#getclassname)
- [getContent](CustomProceduralTexture.md#getcontent)
- [getEffect](CustomProceduralTexture.md#geteffect)
- [getInternalTexture](CustomProceduralTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](CustomProceduralTexture.md#getreflectiontexturematrix)
- [getRenderSize](CustomProceduralTexture.md#getrendersize)
- [getScene](CustomProceduralTexture.md#getscene)
- [getSize](CustomProceduralTexture.md#getsize)
- [getTextureMatrix](CustomProceduralTexture.md#gettexturematrix)
- [isReady](CustomProceduralTexture.md#isready)
- [isReadyOrNotBlocking](CustomProceduralTexture.md#isreadyornotblocking)
- [readPixels](CustomProceduralTexture.md#readpixels)
- [releaseInternalTexture](CustomProceduralTexture.md#releaseinternaltexture)
- [render](CustomProceduralTexture.md#render)
- [reset](CustomProceduralTexture.md#reset)
- [resetRefreshCounter](CustomProceduralTexture.md#resetrefreshcounter)
- [resize](CustomProceduralTexture.md#resize)
- [scale](CustomProceduralTexture.md#scale)
- [serialize](CustomProceduralTexture.md#serialize)
- [setColor3](CustomProceduralTexture.md#setcolor3)
- [setColor4](CustomProceduralTexture.md#setcolor4)
- [setFloat](CustomProceduralTexture.md#setfloat)
- [setFloats](CustomProceduralTexture.md#setfloats)
- [setFragment](CustomProceduralTexture.md#setfragment)
- [setInt](CustomProceduralTexture.md#setint)
- [setMatrix](CustomProceduralTexture.md#setmatrix)
- [setTexture](CustomProceduralTexture.md#settexture)
- [setVector2](CustomProceduralTexture.md#setvector2)
- [setVector3](CustomProceduralTexture.md#setvector3)
- [toString](CustomProceduralTexture.md#tostring)
- [updateSamplingMode](CustomProceduralTexture.md#updatesamplingmode)
- [updateShaderUniforms](CustomProceduralTexture.md#updateshaderuniforms)
- [updateTextures](CustomProceduralTexture.md#updatetextures)
- [updateURL](CustomProceduralTexture.md#updateurl)
- [CreateFromBase64String](CustomProceduralTexture.md#createfrombase64string)
- [LoadFromDataString](CustomProceduralTexture.md#loadfromdatastring)
- [Parse](CustomProceduralTexture.md#parse)
- [WhenAllReady](CustomProceduralTexture.md#whenallready)

## Constructors

### constructor

• **new CustomProceduralTexture**(`name`, `texturePath`, `size`, `scene`, `fallbackTexture?`, `generateMipMaps?`)

Instantiates a new Custom Procedural Texture.
Procedural texturing is a way to programmatically create a texture. There are 2 types of procedural textures: code-only, and code that references some classic 2D images, sometimes called 'refMaps' or 'sampler' images.
Custom Procedural textures are the easiest way to create your own procedural in your application.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures#creating-custom-procedural-textures

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the texture |
| `texturePath` | `string` | Define the folder path containing all the custom texture related files (config, shaders...) |
| `size` | `number` | Define the size of the texture to create |
| `scene` | [`Scene`](Scene.md) | Define the scene the texture belongs to |
| `fallbackTexture?` | [`Texture`](Texture.md) | Define a fallback texture in case there were issues to create the custom texture |
| `generateMipMaps?` | `boolean` | Define if the texture should creates mip maps or not |

#### Overrides

[ProceduralTexture](ProceduralTexture.md).[constructor](ProceduralTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:31

## Properties

### \_animate

• `Private` **\_animate**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:14

___

### \_config

• `Private` **\_config**: `any`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:16

___

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_coordinatesIndex](ProceduralTexture.md#_coordinatesindex)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_coordinatesMode](ProceduralTexture.md#_coordinatesmode)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:126

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_engine](ProceduralTexture.md#_engine)

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

[ProceduralTexture](ProceduralTexture.md).[_errorObject](ProceduralTexture.md#_errorobject)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:483

___

### \_format

• `Protected` **\_format**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_format](ProceduralTexture.md#_format)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:312

___

### \_isBlocking

• `Protected` **\_isBlocking**: `boolean` = `true`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_isBlocking](ProceduralTexture.md#_isblocking)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:331

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_loadingError](ProceduralTexture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_scene](ProceduralTexture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_texturePath

• `Private` **\_texturePath**: `string`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:17

___

### \_time

• `Private` **\_time**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:15

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_wrapU](ProceduralTexture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_wrapV](ProceduralTexture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[animations](ProceduralTexture.md#animations)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[anisotropicFilteringLevel](ProceduralTexture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:205

___

### autoClear

• **autoClear**: `boolean` = `true`

Define if the texture must be cleared before rendering (default is true)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[autoClear](ProceduralTexture.md#autoclear)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:45

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[delayLoadState](ProceduralTexture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### homogeneousRotationInUVTransform

• **homogeneousRotationInUVTransform**: `boolean` = `false`

Sets this property to true to avoid deformations when rotating the texture with non-uniform scaling

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[homogeneousRotationInUVTransform](ProceduralTexture.md#homogeneousrotationinuvtransform)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:270

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`Nullable`](../modules.md#nullable)[`IInspectable`](../interfaces/IInspectable.md)[] = `null`

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[inspectableCustomProperties](ProceduralTexture.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:283

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[invertZ](ProceduralTexture.md#invertz)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:320

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Define if the texture is enabled or not (disabled texture will not render)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[isEnabled](ProceduralTexture.md#isenabled)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:39

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[isRenderTarget](ProceduralTexture.md#isrendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[level](ProceduralTexture.md#level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[metadata](ProceduralTexture.md#metadata)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[name](ProceduralTexture.md#name)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:42

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets or sets the node material used to create this texture (null if the texture was manually created)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[nodeMaterialSource](ProceduralTexture.md#nodematerialsource)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:65

___

### onBeforeGenerationObservable

• **onBeforeGenerationObservable**: [`Observable`](Observable.md)[`ProceduralTexture`](ProceduralTexture.md)

Event raised before the texture is generated

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[onBeforeGenerationObservable](ProceduralTexture.md#onbeforegenerationobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:60

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[onDisposeObservable](ProceduralTexture.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:452

___

### onGenerated

• **onGenerated**: () => `void`

#### Type declaration

▸ (): `void`

Callback called when the texture is generated

##### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[onGenerated](ProceduralTexture.md#ongenerated)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:50

___

### onGeneratedObservable

• **onGeneratedObservable**: [`Observable`](Observable.md)[`ProceduralTexture`](ProceduralTexture.md)

Event raised when the texture is generated

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[onGeneratedObservable](ProceduralTexture.md#ongeneratedobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:55

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable triggered once the texture has been loaded.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[onLoadObservable](ProceduralTexture.md#onloadobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:329

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[reservedDataStore](ProceduralTexture.md#reserveddatastore)

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

[ProceduralTexture](ProceduralTexture.md).[sphericalPolynomial](ProceduralTexture.md#sphericalpolynomial)

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

[ProceduralTexture](ProceduralTexture.md).[uAng](ProceduralTexture.md#uang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:230

___

### uOffset

• **uOffset**: `number` = `0`

Define an offset on the texture to offset the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[uOffset](ProceduralTexture.md#uoffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:201

___

### uRotationCenter

• **uRotationCenter**: `number` = `0.5`

Defines the center of rotation (U)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[uRotationCenter](ProceduralTexture.md#urotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:252

___

### uScale

• **uScale**: `number` = `1.0`

Define an offset on the texture to scale the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[uScale](ProceduralTexture.md#uscale)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:215

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[uniqueId](ProceduralTexture.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: [`Nullable`](../modules.md#nullable)`string` = `null`

Define the url of the texture.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[url](ProceduralTexture.md#url)

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

[ProceduralTexture](ProceduralTexture.md).[vAng](ProceduralTexture.md#vang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:238

___

### vOffset

• **vOffset**: `number` = `0`

Define an offset on the texture to offset the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[vOffset](ProceduralTexture.md#voffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:208

___

### vRotationCenter

• **vRotationCenter**: `number` = `0.5`

Defines the center of rotation (V)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[vRotationCenter](ProceduralTexture.md#vrotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:258

___

### vScale

• **vScale**: `number` = `1.0`

Define an offset on the texture to scale the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[vScale](ProceduralTexture.md#vscale)

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

[ProceduralTexture](ProceduralTexture.md).[wAng](ProceduralTexture.md#wang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:246

___

### wRotationCenter

• **wRotationCenter**: `number` = `0.5`

Defines the center of rotation (W)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[wRotationCenter](ProceduralTexture.md#wrotationcenter)

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

[ProceduralTexture](ProceduralTexture.md).[wrapR](ProceduralTexture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:197

___

### BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[BILINEAR_SAMPLINGMODE](ProceduralTexture.md#bilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:129

___

### CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[CLAMP_ADDRESSMODE](ProceduralTexture.md#clamp_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:179

___

### CUBIC\_MODE

▪ `Static` `Readonly` **CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[CUBIC_MODE](ProceduralTexture.md#cubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:164

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](ProceduralTexture.md#default_anisotropic_filtering_level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:30

___

### EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[EQUIRECTANGULAR_MODE](ProceduralTexture.md#equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:172

___

### EXPLICIT\_MODE

▪ `Static` `Readonly` **EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[EXPLICIT_MODE](ProceduralTexture.md#explicit_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:158

___

### FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[FIXED_EQUIRECTANGULAR_MIRRORED_MODE](ProceduralTexture.md#fixed_equirectangular_mirrored_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:176

___

### FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[FIXED_EQUIRECTANGULAR_MODE](ProceduralTexture.md#fixed_equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:174

___

### ForceSerializeBuffers

▪ `Static` **ForceSerializeBuffers**: `boolean` = `false`

Gets or sets a general boolean used to indicate that texture buffers must be saved as part of the serialization process.
If no buffer exists, one will be created as base64 string from the internal webgl data.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[ForceSerializeBuffers](ProceduralTexture.md#forceserializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:82

___

### INVCUBIC\_MODE

▪ `Static` `Readonly` **INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[INVCUBIC_MODE](ProceduralTexture.md#invcubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:170

___

### LINEAR\_LINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_LINEAR](ProceduralTexture.md#linear_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:153

___

### LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_LINEAR_MIPLINEAR](ProceduralTexture.md#linear_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:136

___

### LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_LINEAR_MIPNEAREST](ProceduralTexture.md#linear_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:131

___

### LINEAR\_NEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_NEAREST](ProceduralTexture.md#linear_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:155

___

### LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_NEAREST_MIPLINEAR](ProceduralTexture.md#linear_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:151

___

### LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[LINEAR_NEAREST_MIPNEAREST](ProceduralTexture.md#linear_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:149

___

### MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[MIRROR_ADDRESSMODE](ProceduralTexture.md#mirror_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:183

___

### NEAREST\_LINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_LINEAR](ProceduralTexture.md#nearest_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:145

___

### NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_LINEAR_MIPLINEAR](ProceduralTexture.md#nearest_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:143

___

### NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_LINEAR_MIPNEAREST](ProceduralTexture.md#nearest_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:141

___

### NEAREST\_NEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_NEAREST](ProceduralTexture.md#nearest_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:147

___

### NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_NEAREST_MIPLINEAR](ProceduralTexture.md#nearest_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:126

___

### NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_NEAREST_MIPNEAREST](ProceduralTexture.md#nearest_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:139

___

### NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[NEAREST_SAMPLINGMODE](ProceduralTexture.md#nearest_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:124

___

### OnTextureLoadErrorObservable

▪ `Static` **OnTextureLoadErrorObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

This observable will notify when any texture had a loading error

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[OnTextureLoadErrorObservable](ProceduralTexture.md#ontextureloaderrorobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:87

___

### PLANAR\_MODE

▪ `Static` `Readonly` **PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[PLANAR_MODE](ProceduralTexture.md#planar_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:162

___

### PROJECTION\_MODE

▪ `Static` `Readonly` **PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[PROJECTION_MODE](ProceduralTexture.md#projection_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:166

___

### SKYBOX\_MODE

▪ `Static` `Readonly` **SKYBOX\_MODE**: ``5``

Inverse Cubic coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[SKYBOX_MODE](ProceduralTexture.md#skybox_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:168

___

### SPHERICAL\_MODE

▪ `Static` `Readonly` **SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[SPHERICAL_MODE](ProceduralTexture.md#spherical_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:160

___

### SerializeBuffers

▪ `Static` **SerializeBuffers**: `boolean` = `true`

Gets or sets a general boolean used to indicate that textures containing direct data (buffers) must be saved as part of the serialization process

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[SerializeBuffers](ProceduralTexture.md#serializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:76

___

### TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[TRILINEAR_SAMPLINGMODE](ProceduralTexture.md#trilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:134

___

### UseSerializedUrlIfAny

▪ `Static` **UseSerializedUrlIfAny**: `boolean` = `false`

Gets or sets a boolean which defines if the texture url must be build from the serialized URL instead of just using the name and loading them side by side with the scene file

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[UseSerializedUrlIfAny](ProceduralTexture.md#useserializedurlifany)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:188

___

### WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[WRAP_ADDRESSMODE](ProceduralTexture.md#wrap_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:181

## Accessors

### animate

• `get` **animate**(): `boolean`

Define if the texture animates or not.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:168

• `set` **animate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:172

___

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.canRescale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

ProceduralTexture.coordinatesIndex

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

ProceduralTexture.coordinatesIndex

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

ProceduralTexture.coordinatesMode

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

ProceduralTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

ProceduralTexture.errorObject

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

ProceduralTexture.gammaSpace

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

ProceduralTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.getAlphaFromRGB

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

ProceduralTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.hasAlpha

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

ProceduralTexture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:60

___

### invertY

• `get` **invertY**(): `boolean`

Gets a boolean indicating if the texture needs to be inverted on the y axis during loading

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.invertY

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

ProceduralTexture.irradianceTexture

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

ProceduralTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.is2DArray

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

ProceduralTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.is3D

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

ProceduralTexture.is3D

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

ProceduralTexture.isBlocking

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

ProceduralTexture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:336

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.isCube

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

ProceduralTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.isRGBD

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

ProceduralTexture.isRGBD

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

ProceduralTexture.linearSpecularLOD

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

ProceduralTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.loadingError

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

ProceduralTexture.lodGenerationOffset

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

ProceduralTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

ProceduralTexture.lodGenerationScale

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

ProceduralTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:363

___

### mimeType

• `get` **mimeType**(): `undefined` \| `string`

Returns the texture mime type if it was defined by a loader (undefined else)

#### Returns

`undefined` \| `string`

#### Inherited from

ProceduralTexture.mimeType

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:322

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

ProceduralTexture.noMipmap

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

ProceduralTexture.onDispose

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:459

___

### refreshRate

• `get` **refreshRate**(): `number`

Define the refresh rate of the texture or the rendering frequency.
Use 0 to render just once, 1 to render on every frame, 2 to render every two frames and so on...

#### Returns

`number`

#### Inherited from

ProceduralTexture.refreshRate

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:350

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ProceduralTexture.refreshRate

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:355

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

ProceduralTexture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

ProceduralTexture.textureFormat

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

ProceduralTexture.textureType

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

ProceduralTexture.uid

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

ProceduralTexture.wrapU

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

ProceduralTexture.wrapU

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

ProceduralTexture.wrapV

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

ProceduralTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_getDefines

▸ `Protected` **_getDefines**(): `string`

#### Returns

`string`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_getDefines](ProceduralTexture.md#_getdefines)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:269

___

### \_loadJson

▸ `Private` **_loadJson**(`jsonUrl`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `jsonUrl` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:40

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_markAllSubMeshesAsTexturesDirty](ProceduralTexture.md#_markallsubmeshesastexturesdirty)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:670

___

### \_setEffect

▸ **_setEffect**(`effect`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | @hidden* |

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[_setEffect](ProceduralTexture.md#_seteffect)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:204

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

[ProceduralTexture](ProceduralTexture.md).[checkTransformsAreIdentical](ProceduralTexture.md#checktransformsareidentical)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:633

___

### clone

▸ **clone**(): [`ProceduralTexture`](ProceduralTexture.md)

Clone the texture.

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the cloned texture

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[clone](ProceduralTexture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:670

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[dispose](ProceduralTexture.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:687

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[forceSphericalPolynomialsRecompute](ProceduralTexture.md#forcesphericalpolynomialsrecompute)

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

[ProceduralTexture](ProceduralTexture.md).[getBaseSize](ProceduralTexture.md#getbasesize)

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

[ProceduralTexture](ProceduralTexture.md).[getClassName](ProceduralTexture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:897

___

### getContent

▸ **getContent**(): [`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

Gets texture content (Use this function wisely as reading from a texture can be slow)

#### Returns

[`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

an ArrayBufferView promise (Uint8Array or Float32Array)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[getContent](ProceduralTexture.md#getcontent)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:212

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

The effect that is created when initializing the post process.

#### Returns

[`Effect`](Effect.md)

The created effect corresponding the the postprocess.

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[getEffect](ProceduralTexture.md#geteffect)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:196

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[getInternalTexture](ProceduralTexture.md#getinternaltexture)

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

[ProceduralTexture](ProceduralTexture.md).[getReflectionTextureMatrix](ProceduralTexture.md#getreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:751

___

### getRenderSize

▸ **getRenderSize**(): `TextureSize`

Get the size the texture is rendering at.

#### Returns

`TextureSize`

the size (on cube texture it is always squared)

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[getRenderSize](ProceduralTexture.md#getrendersize)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:394

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[getScene](ProceduralTexture.md#getscene)

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

[ProceduralTexture](ProceduralTexture.md).[getSize](ProceduralTexture.md#getsize)

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

[ProceduralTexture](ProceduralTexture.md).[getTextureMatrix](ProceduralTexture.md#gettexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:651

___

### isReady

▸ **isReady**(): `boolean`

Is the texture ready to be used ? (rendered at least once)

#### Returns

`boolean`

true if ready, otherwise, false.

#### Overrides

[ProceduralTexture](ProceduralTexture.md).[isReady](ProceduralTexture.md#isready)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:95

___

### isReadyOrNotBlocking

▸ **isReadyOrNotBlocking**(): `boolean`

Get if the texture is ready to be consumed (either it is ready or it is not blocking)

#### Returns

`boolean`

true if ready, not blocking or if there was an error loading the texture

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[isReadyOrNotBlocking](ProceduralTexture.md#isreadyornotblocking)

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

[ProceduralTexture](ProceduralTexture.md).[readPixels](ProceduralTexture.md#readpixels)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[releaseInternalTexture](ProceduralTexture.md#releaseinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:284

___

### render

▸ **render**(`useCameraPostProcess?`): `void`

Render the texture to its associated render target.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `useCameraPostProcess?` | `boolean` | Define if camera post process should be applied to the texture |

#### Returns

`void`

#### Overrides

[ProceduralTexture](ProceduralTexture.md).[render](ProceduralTexture.md#render)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:115

___

### reset

▸ **reset**(): `void`

Resets the texture in order to recreate its associated resources.
This can be called in case of context loss

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[reset](ProceduralTexture.md#reset)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:265

___

### resetRefreshCounter

▸ **resetRefreshCounter**(): `void`

Resets the refresh counter of the texture and start bak from scratch.
Could be useful to regenerate the texture if it is setup to render only once.

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[resetRefreshCounter](ProceduralTexture.md#resetrefreshcounter)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:334

___

### resize

▸ **resize**(`size`, `generateMipMaps`): `void`

Resize the texture to new value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `TextureSize` | Define the new size the texture should have |
| `generateMipMaps` | `boolean` | Define whether the new texture should create mip maps |

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[resize](ProceduralTexture.md#resize)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:403

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

[ProceduralTexture](ProceduralTexture.md).[scale](ProceduralTexture.md#scale)

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

[ProceduralTexture](ProceduralTexture.md).[serialize](ProceduralTexture.md#serialize)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:852

___

### setColor3

▸ **setColor3**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a vec3 in the shader from a Color3.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color3`](Color3.md) | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setColor3](ProceduralTexture.md#setcolor3)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:485

___

### setColor4

▸ **setColor4**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a vec4 in the shader from a Color4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color4`](Color4.md) | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setColor4](ProceduralTexture.md#setcolor4)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:498

___

### setFloat

▸ **setFloat**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a float in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number` | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setFloat](ProceduralTexture.md#setfloat)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:446

___

### setFloats

▸ **setFloats**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set an array of floats in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setFloats](ProceduralTexture.md#setfloats)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:472

___

### setFragment

▸ **setFragment**(`fragment`): `void`

Set the fragment shader to use in order to render the texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fragment` | `any` | This can be set to a path (into the shader store) or to a json object containing a fragmentElement property. |

#### Returns

`void`

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setFragment](ProceduralTexture.md#setfragment)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:342

___

### setInt

▸ **setInt**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a int in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number` | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setInt](ProceduralTexture.md#setint)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:459

___

### setMatrix

▸ **setMatrix**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a mat4 in the shader from a MAtrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Matrix`](Matrix.md) | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setMatrix](ProceduralTexture.md#setmatrix)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:537

___

### setTexture

▸ **setTexture**(`name`, `texture`): [`ProceduralTexture`](ProceduralTexture.md)

Set a texture in the shader program used to render.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform samplers as defined in the shader |
| `texture` | [`Texture`](Texture.md) | Define the texture to bind to this sampler |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setTexture](ProceduralTexture.md#settexture)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:431

___

### setVector2

▸ **setVector2**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a vec2 in the shader from a Vector2.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Vector2`](Vector2.md) | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setVector2](ProceduralTexture.md#setvector2)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:511

___

### setVector3

▸ **setVector3**(`name`, `value`): [`ProceduralTexture`](ProceduralTexture.md)

Set a vec3 in the shader from a Vector3.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Vector3`](Vector3.md) | Define the value to give to the uniform |

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the texture itself allowing "fluent" like uniform updates

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[setVector3](ProceduralTexture.md#setvector3)

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:524

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

#### Inherited from

[ProceduralTexture](ProceduralTexture.md).[toString](ProceduralTexture.md#tostring)

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

[ProceduralTexture](ProceduralTexture.md).[updateSamplingMode](ProceduralTexture.md#updatesamplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:275

___

### updateShaderUniforms

▸ **updateShaderUniforms**(): `void`

Update the uniform values of the procedural texture in the shader.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:137

___

### updateTextures

▸ **updateTextures**(): `void`

Update the list of dependant textures samplers in the shader.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/customProceduralTexture.ts:128

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

[ProceduralTexture](ProceduralTexture.md).[updateURL](ProceduralTexture.md#updateurl)

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

[ProceduralTexture](ProceduralTexture.md).[CreateFromBase64String](ProceduralTexture.md#createfrombase64string)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:1057

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

[ProceduralTexture](ProceduralTexture.md).[LoadFromDataString](ProceduralTexture.md#loadfromdatastring)

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

[ProceduralTexture](ProceduralTexture.md).[Parse](ProceduralTexture.md#parse)

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

[ProceduralTexture](ProceduralTexture.md).[WhenAllReady](ProceduralTexture.md#whenallready)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:864

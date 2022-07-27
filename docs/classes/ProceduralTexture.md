[@dev/core](../README.md) / [Exports](../modules.md) / ProceduralTexture

# Class: ProceduralTexture

Procedural texturing is a way to programmatically create a texture. There are 2 types of procedural textures: code-only, and code that references some classic 2D images, sometimes calmpler' images.
This is the base class of any Procedural texture and contains most of the shareable code.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures

## Hierarchy

- [`Texture`](Texture.md)

  ↳ **`ProceduralTexture`**

  ↳↳ [`CustomProceduralTexture`](CustomProceduralTexture.md)

  ↳↳ [`NoiseProceduralTexture`](NoiseProceduralTexture.md)

## Table of contents

### Constructors

- [constructor](ProceduralTexture.md#constructor)

### Properties

- [\_cachedDefines](ProceduralTexture.md#_cacheddefines)
- [\_colors3](ProceduralTexture.md#_colors3)
- [\_colors4](ProceduralTexture.md#_colors4)
- [\_contentData](ProceduralTexture.md#_contentdata)
- [\_contentUpdateId](ProceduralTexture.md#_contentupdateid)
- [\_coordinatesIndex](ProceduralTexture.md#_coordinatesindex)
- [\_coordinatesMode](ProceduralTexture.md#_coordinatesmode)
- [\_currentRefreshId](ProceduralTexture.md#_currentrefreshid)
- [\_drawWrapper](ProceduralTexture.md#_drawwrapper)
- [\_engine](ProceduralTexture.md#_engine)
- [\_errorObject](ProceduralTexture.md#_errorobject)
- [\_fallbackTextureUsed](ProceduralTexture.md#_fallbacktextureused)
- [\_floats](ProceduralTexture.md#_floats)
- [\_floatsArrays](ProceduralTexture.md#_floatsarrays)
- [\_format](ProceduralTexture.md#_format)
- [\_fragment](ProceduralTexture.md#_fragment)
- [\_frameId](ProceduralTexture.md#_frameid)
- [\_fullEngine](ProceduralTexture.md#_fullengine)
- [\_indexBuffer](ProceduralTexture.md#_indexbuffer)
- [\_ints](ProceduralTexture.md#_ints)
- [\_isBlocking](ProceduralTexture.md#_isblocking)
- [\_loadingError](ProceduralTexture.md#_loadingerror)
- [\_matrices](ProceduralTexture.md#_matrices)
- [\_refreshRate](ProceduralTexture.md#_refreshrate)
- [\_rtWrapper](ProceduralTexture.md#_rtwrapper)
- [\_samplers](ProceduralTexture.md#_samplers)
- [\_scene](ProceduralTexture.md#_scene)
- [\_size](ProceduralTexture.md#_size)
- [\_textureType](ProceduralTexture.md#_texturetype)
- [\_uniforms](ProceduralTexture.md#_uniforms)
- [\_vectors2](ProceduralTexture.md#_vectors2)
- [\_vectors3](ProceduralTexture.md#_vectors3)
- [\_vertexBuffers](ProceduralTexture.md#_vertexbuffers)
- [\_wrapU](ProceduralTexture.md#_wrapu)
- [\_wrapV](ProceduralTexture.md#_wrapv)
- [animations](ProceduralTexture.md#animations)
- [anisotropicFilteringLevel](ProceduralTexture.md#anisotropicfilteringlevel)
- [autoClear](ProceduralTexture.md#autoclear)
- [delayLoadState](ProceduralTexture.md#delayloadstate)
- [homogeneousRotationInUVTransform](ProceduralTexture.md#homogeneousrotationinuvtransform)
- [inspectableCustomProperties](ProceduralTexture.md#inspectablecustomproperties)
- [invertZ](ProceduralTexture.md#invertz)
- [isEnabled](ProceduralTexture.md#isenabled)
- [isRenderTarget](ProceduralTexture.md#isrendertarget)
- [level](ProceduralTexture.md#level)
- [metadata](ProceduralTexture.md#metadata)
- [name](ProceduralTexture.md#name)
- [nodeMaterialSource](ProceduralTexture.md#nodematerialsource)
- [onBeforeGenerationObservable](ProceduralTexture.md#onbeforegenerationobservable)
- [onDisposeObservable](ProceduralTexture.md#ondisposeobservable)
- [onGenerated](ProceduralTexture.md#ongenerated)
- [onGeneratedObservable](ProceduralTexture.md#ongeneratedobservable)
- [onLoadObservable](ProceduralTexture.md#onloadobservable)
- [reservedDataStore](ProceduralTexture.md#reserveddatastore)
- [sphericalPolynomial](ProceduralTexture.md#sphericalpolynomial)
- [uAng](ProceduralTexture.md#uang)
- [uOffset](ProceduralTexture.md#uoffset)
- [uRotationCenter](ProceduralTexture.md#urotationcenter)
- [uScale](ProceduralTexture.md#uscale)
- [uniqueId](ProceduralTexture.md#uniqueid)
- [url](ProceduralTexture.md#url)
- [vAng](ProceduralTexture.md#vang)
- [vOffset](ProceduralTexture.md#voffset)
- [vRotationCenter](ProceduralTexture.md#vrotationcenter)
- [vScale](ProceduralTexture.md#vscale)
- [wAng](ProceduralTexture.md#wang)
- [wRotationCenter](ProceduralTexture.md#wrotationcenter)
- [wrapR](ProceduralTexture.md#wrapr)
- [BILINEAR\_SAMPLINGMODE](ProceduralTexture.md#bilinear_samplingmode)
- [CLAMP\_ADDRESSMODE](ProceduralTexture.md#clamp_addressmode)
- [CUBIC\_MODE](ProceduralTexture.md#cubic_mode)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](ProceduralTexture.md#default_anisotropic_filtering_level)
- [EQUIRECTANGULAR\_MODE](ProceduralTexture.md#equirectangular_mode)
- [EXPLICIT\_MODE](ProceduralTexture.md#explicit_mode)
- [FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](ProceduralTexture.md#fixed_equirectangular_mirrored_mode)
- [FIXED\_EQUIRECTANGULAR\_MODE](ProceduralTexture.md#fixed_equirectangular_mode)
- [ForceSerializeBuffers](ProceduralTexture.md#forceserializebuffers)
- [INVCUBIC\_MODE](ProceduralTexture.md#invcubic_mode)
- [LINEAR\_LINEAR](ProceduralTexture.md#linear_linear)
- [LINEAR\_LINEAR\_MIPLINEAR](ProceduralTexture.md#linear_linear_miplinear)
- [LINEAR\_LINEAR\_MIPNEAREST](ProceduralTexture.md#linear_linear_mipnearest)
- [LINEAR\_NEAREST](ProceduralTexture.md#linear_nearest)
- [LINEAR\_NEAREST\_MIPLINEAR](ProceduralTexture.md#linear_nearest_miplinear)
- [LINEAR\_NEAREST\_MIPNEAREST](ProceduralTexture.md#linear_nearest_mipnearest)
- [MIRROR\_ADDRESSMODE](ProceduralTexture.md#mirror_addressmode)
- [NEAREST\_LINEAR](ProceduralTexture.md#nearest_linear)
- [NEAREST\_LINEAR\_MIPLINEAR](ProceduralTexture.md#nearest_linear_miplinear)
- [NEAREST\_LINEAR\_MIPNEAREST](ProceduralTexture.md#nearest_linear_mipnearest)
- [NEAREST\_NEAREST](ProceduralTexture.md#nearest_nearest)
- [NEAREST\_NEAREST\_MIPLINEAR](ProceduralTexture.md#nearest_nearest_miplinear)
- [NEAREST\_NEAREST\_MIPNEAREST](ProceduralTexture.md#nearest_nearest_mipnearest)
- [NEAREST\_SAMPLINGMODE](ProceduralTexture.md#nearest_samplingmode)
- [OnTextureLoadErrorObservable](ProceduralTexture.md#ontextureloaderrorobservable)
- [PLANAR\_MODE](ProceduralTexture.md#planar_mode)
- [PROJECTION\_MODE](ProceduralTexture.md#projection_mode)
- [SKYBOX\_MODE](ProceduralTexture.md#skybox_mode)
- [SPHERICAL\_MODE](ProceduralTexture.md#spherical_mode)
- [SerializeBuffers](ProceduralTexture.md#serializebuffers)
- [TRILINEAR\_SAMPLINGMODE](ProceduralTexture.md#trilinear_samplingmode)
- [UseSerializedUrlIfAny](ProceduralTexture.md#useserializedurlifany)
- [WRAP\_ADDRESSMODE](ProceduralTexture.md#wrap_addressmode)

### Accessors

- [canRescale](ProceduralTexture.md#canrescale)
- [coordinatesIndex](ProceduralTexture.md#coordinatesindex)
- [coordinatesMode](ProceduralTexture.md#coordinatesmode)
- [errorObject](ProceduralTexture.md#errorobject)
- [gammaSpace](ProceduralTexture.md#gammaspace)
- [getAlphaFromRGB](ProceduralTexture.md#getalphafromrgb)
- [hasAlpha](ProceduralTexture.md#hasalpha)
- [invertY](ProceduralTexture.md#inverty)
- [irradianceTexture](ProceduralTexture.md#irradiancetexture)
- [is2DArray](ProceduralTexture.md#is2darray)
- [is3D](ProceduralTexture.md#is3d)
- [isBlocking](ProceduralTexture.md#isblocking)
- [isCube](ProceduralTexture.md#iscube)
- [isRGBD](ProceduralTexture.md#isrgbd)
- [linearSpecularLOD](ProceduralTexture.md#linearspecularlod)
- [loadingError](ProceduralTexture.md#loadingerror)
- [lodGenerationOffset](ProceduralTexture.md#lodgenerationoffset)
- [lodGenerationScale](ProceduralTexture.md#lodgenerationscale)
- [mimeType](ProceduralTexture.md#mimetype)
- [noMipmap](ProceduralTexture.md#nomipmap)
- [onDispose](ProceduralTexture.md#ondispose)
- [refreshRate](ProceduralTexture.md#refreshrate)
- [samplingMode](ProceduralTexture.md#samplingmode)
- [textureFormat](ProceduralTexture.md#textureformat)
- [textureType](ProceduralTexture.md#texturetype)
- [uid](ProceduralTexture.md#uid)
- [wrapU](ProceduralTexture.md#wrapu)
- [wrapV](ProceduralTexture.md#wrapv)

### Methods

- [\_checkUniform](ProceduralTexture.md#_checkuniform)
- [\_createIndexBuffer](ProceduralTexture.md#_createindexbuffer)
- [\_createRtWrapper](ProceduralTexture.md#_creatertwrapper)
- [\_getDefines](ProceduralTexture.md#_getdefines)
- [\_markAllSubMeshesAsTexturesDirty](ProceduralTexture.md#_markallsubmeshesastexturesdirty)
- [\_setEffect](ProceduralTexture.md#_seteffect)
- [checkTransformsAreIdentical](ProceduralTexture.md#checktransformsareidentical)
- [clone](ProceduralTexture.md#clone)
- [dispose](ProceduralTexture.md#dispose)
- [forceSphericalPolynomialsRecompute](ProceduralTexture.md#forcesphericalpolynomialsrecompute)
- [getBaseSize](ProceduralTexture.md#getbasesize)
- [getClassName](ProceduralTexture.md#getclassname)
- [getContent](ProceduralTexture.md#getcontent)
- [getEffect](ProceduralTexture.md#geteffect)
- [getInternalTexture](ProceduralTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](ProceduralTexture.md#getreflectiontexturematrix)
- [getRenderSize](ProceduralTexture.md#getrendersize)
- [getScene](ProceduralTexture.md#getscene)
- [getSize](ProceduralTexture.md#getsize)
- [getTextureMatrix](ProceduralTexture.md#gettexturematrix)
- [isReady](ProceduralTexture.md#isready)
- [isReadyOrNotBlocking](ProceduralTexture.md#isreadyornotblocking)
- [readPixels](ProceduralTexture.md#readpixels)
- [releaseInternalTexture](ProceduralTexture.md#releaseinternaltexture)
- [render](ProceduralTexture.md#render)
- [reset](ProceduralTexture.md#reset)
- [resetRefreshCounter](ProceduralTexture.md#resetrefreshcounter)
- [resize](ProceduralTexture.md#resize)
- [scale](ProceduralTexture.md#scale)
- [serialize](ProceduralTexture.md#serialize)
- [setColor3](ProceduralTexture.md#setcolor3)
- [setColor4](ProceduralTexture.md#setcolor4)
- [setFloat](ProceduralTexture.md#setfloat)
- [setFloats](ProceduralTexture.md#setfloats)
- [setFragment](ProceduralTexture.md#setfragment)
- [setInt](ProceduralTexture.md#setint)
- [setMatrix](ProceduralTexture.md#setmatrix)
- [setTexture](ProceduralTexture.md#settexture)
- [setVector2](ProceduralTexture.md#setvector2)
- [setVector3](ProceduralTexture.md#setvector3)
- [toString](ProceduralTexture.md#tostring)
- [updateSamplingMode](ProceduralTexture.md#updatesamplingmode)
- [updateURL](ProceduralTexture.md#updateurl)
- [CreateFromBase64String](ProceduralTexture.md#createfrombase64string)
- [LoadFromDataString](ProceduralTexture.md#loadfromdatastring)
- [Parse](ProceduralTexture.md#parse)
- [WhenAllReady](ProceduralTexture.md#whenallready)

## Constructors

### constructor

• **new ProceduralTexture**(`name`, `size`, `fragment`, `scene`, `fallbackTexture?`, `generateMipMaps?`, `isCube?`, `textureType?`)

Instantiates a new procedural texture.
Procedural texturing is a way to programmatically create a texture. There are 2 types of procedural textures: code-only, and code that references some classic 2D images, sometimes called 'refMaps' or 'sampler' images.
This is the base class of any Procedural texture and contains most of the shareable code.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Define the name of the texture |
| `size` | `TextureSize` | `undefined` | Define the size of the texture to create |
| `fragment` | `any` | `undefined` | Define the fragment shader to use to generate the texture or null if it is defined later |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `undefined` | Define the scene the texture belongs to |
| `fallbackTexture` | [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) | `null` | Define a fallback texture in case there were issues to create the custom texture |
| `generateMipMaps` | `boolean` | `true` | Define if the texture should creates mip maps or not |
| `isCube` | `boolean` | `false` | Define if the texture is a cube texture or not (this will render each faces of the cube) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | The FBO internal texture type |

#### Overrides

[Texture](Texture.md).[constructor](Texture.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:124

## Properties

### \_cachedDefines

• `Private` **\_cachedDefines**: [`Nullable`](../modules.md#nullable)`string` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:103

___

### \_colors3

• `Private` **\_colors3**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:94

___

### \_colors4

• `Private` **\_colors4**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:95

___

### \_contentData

• `Private` **\_contentData**: [`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:106

___

### \_contentUpdateId

• `Private` **\_contentUpdateId**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:105

___

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[Texture](Texture.md).[_coordinatesIndex](Texture.md#_coordinatesindex)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[Texture](Texture.md).[_coordinatesMode](Texture.md#_coordinatesmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:126

___

### \_currentRefreshId

• `Private` **\_currentRefreshId**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:82

___

### \_drawWrapper

• `Private` **\_drawWrapper**: `DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:71

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[Texture](Texture.md).[_engine](Texture.md#_engine)

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

[Texture](Texture.md).[_errorObject](Texture.md#_errorobject)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:483

___

### \_fallbackTextureUsed

• `Private` **\_fallbackTextureUsed**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:100

___

### \_floats

• `Private` **\_floats**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:91

___

### \_floatsArrays

• `Private` **\_floatsArrays**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:93

___

### \_format

• `Protected` **\_format**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Inherited from

[Texture](Texture.md).[_format](Texture.md#_format)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:312

___

### \_fragment

• `Private` **\_fragment**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:89

___

### \_frameId

• `Private` **\_frameId**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:83

___

### \_fullEngine

• `Private` **\_fullEngine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:101

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:86

___

### \_ints

• `Private` **\_ints**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:92

___

### \_isBlocking

• `Protected` **\_isBlocking**: `boolean` = `true`

#### Inherited from

[Texture](Texture.md).[_isBlocking](Texture.md#_isblocking)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:331

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[Texture](Texture.md).[_loadingError](Texture.md#_loadingerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:482

___

### \_matrices

• `Private` **\_matrices**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:98

___

### \_refreshRate

• `Private` **\_refreshRate**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:84

___

### \_rtWrapper

• `Private` **\_rtWrapper**: [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:108

___

### \_samplers

• `Private` **\_samplers**: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:88

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[Texture](Texture.md).[_scene](Texture.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:466

___

### \_size

• `Private` **\_size**: `TextureSize`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:80

___

### \_textureType

• `Private` **\_textureType**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:81

___

### \_uniforms

• `Private` **\_uniforms**: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:87

___

### \_vectors2

• `Private` **\_vectors2**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:96

___

### \_vectors3

• `Private` **\_vectors3**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:97

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:85

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[Texture](Texture.md).[_wrapU](Texture.md#_wrapu)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[Texture](Texture.md).[_wrapV](Texture.md#_wrapv)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:31

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[Texture](Texture.md).[animations](Texture.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[Texture](Texture.md).[anisotropicFilteringLevel](Texture.md#anisotropicfilteringlevel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:205

___

### autoClear

• **autoClear**: `boolean` = `true`

Define if the texture must be cleared before rendering (default is true)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:45

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[Texture](Texture.md).[delayLoadState](Texture.md#delayloadstate)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:66

___

### homogeneousRotationInUVTransform

• **homogeneousRotationInUVTransform**: `boolean` = `false`

Sets this property to true to avoid deformations when rotating the texture with non-uniform scaling

#### Inherited from

[Texture](Texture.md).[homogeneousRotationInUVTransform](Texture.md#homogeneousrotationinuvtransform)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:270

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`Nullable`](../modules.md#nullable)[`IInspectable`](../interfaces/IInspectable.md)[] = `null`

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Texture](Texture.md).[inspectableCustomProperties](Texture.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:283

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[Texture](Texture.md).[invertZ](Texture.md#invertz)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:320

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Define if the texture is enabled or not (disabled texture will not render)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:39

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[Texture](Texture.md).[isRenderTarget](Texture.md#isrendertarget)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[Texture](Texture.md).[level](Texture.md#level)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[Texture](Texture.md).[metadata](Texture.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:48

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[Texture](Texture.md).[name](Texture.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:42

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets or sets the node material used to create this texture (null if the texture was manually created)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:65

___

### onBeforeGenerationObservable

• **onBeforeGenerationObservable**: [`Observable`](Observable.md)[`ProceduralTexture`](ProceduralTexture.md)

Event raised before the texture is generated

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:60

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[Texture](Texture.md).[onDisposeObservable](Texture.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:452

___

### onGenerated

• **onGenerated**: () => `void`

#### Type declaration

▸ (): `void`

Callback called when the texture is generated

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:50

___

### onGeneratedObservable

• **onGeneratedObservable**: [`Observable`](Observable.md)[`ProceduralTexture`](ProceduralTexture.md)

Event raised when the texture is generated

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:55

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable triggered once the texture has been loaded.

#### Inherited from

[Texture](Texture.md).[onLoadObservable](Texture.md#onloadobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:329

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Texture](Texture.md).[reservedDataStore](Texture.md#reserveddatastore)

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

[Texture](Texture.md).[sphericalPolynomial](Texture.md#sphericalpolynomial)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.polynomial.ts:13

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:230

___

### uOffset

• **uOffset**: `number` = `0`

Define an offset on the texture to offset the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[Texture](Texture.md).[uOffset](Texture.md#uoffset)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:201

___

### uRotationCenter

• **uRotationCenter**: `number` = `0.5`

Defines the center of rotation (U)

#### Inherited from

[Texture](Texture.md).[uRotationCenter](Texture.md#urotationcenter)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:252

___

### uScale

• **uScale**: `number` = `1.0`

Define an offset on the texture to scale the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[Texture](Texture.md).[uScale](Texture.md#uscale)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:215

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[Texture](Texture.md).[uniqueId](Texture.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: [`Nullable`](../modules.md#nullable)`string` = `null`

Define the url of the texture.

#### Inherited from

[Texture](Texture.md).[url](Texture.md#url)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:194

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:238

___

### vOffset

• **vOffset**: `number` = `0`

Define an offset on the texture to offset the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[Texture](Texture.md).[vOffset](Texture.md#voffset)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:208

___

### vRotationCenter

• **vRotationCenter**: `number` = `0.5`

Defines the center of rotation (V)

#### Inherited from

[Texture](Texture.md).[vRotationCenter](Texture.md#vrotationcenter)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:258

___

### vScale

• **vScale**: `number` = `1.0`

Define an offset on the texture to scale the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[Texture](Texture.md).[vScale](Texture.md#vscale)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:222

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:246

___

### wRotationCenter

• **wRotationCenter**: `number` = `0.5`

Defines the center of rotation (W)

#### Inherited from

[Texture](Texture.md).[wRotationCenter](Texture.md#wrotationcenter)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:264

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:197

___

### BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[BILINEAR_SAMPLINGMODE](Texture.md#bilinear_samplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:129

___

### CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Inherited from

[Texture](Texture.md).[CLAMP_ADDRESSMODE](Texture.md#clamp_addressmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:179

___

### CUBIC\_MODE

▪ `Static` `Readonly` **CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[CUBIC_MODE](Texture.md#cubic_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:164

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[Texture](Texture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](Texture.md#default_anisotropic_filtering_level)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:30

___

### EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Inherited from

[Texture](Texture.md).[EQUIRECTANGULAR_MODE](Texture.md#equirectangular_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:172

___

### EXPLICIT\_MODE

▪ `Static` `Readonly` **EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Inherited from

[Texture](Texture.md).[EXPLICIT_MODE](Texture.md#explicit_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:158

___

### FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Inherited from

[Texture](Texture.md).[FIXED_EQUIRECTANGULAR_MIRRORED_MODE](Texture.md#fixed_equirectangular_mirrored_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:176

___

### FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Inherited from

[Texture](Texture.md).[FIXED_EQUIRECTANGULAR_MODE](Texture.md#fixed_equirectangular_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:174

___

### ForceSerializeBuffers

▪ `Static` **ForceSerializeBuffers**: `boolean` = `false`

Gets or sets a general boolean used to indicate that texture buffers must be saved as part of the serialization process.
If no buffer exists, one will be created as base64 string from the internal webgl data.

#### Inherited from

[Texture](Texture.md).[ForceSerializeBuffers](Texture.md#forceserializebuffers)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:82

___

### INVCUBIC\_MODE

▪ `Static` `Readonly` **INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[INVCUBIC_MODE](Texture.md#invcubic_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:170

___

### LINEAR\_LINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR](Texture.md#linear_linear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:153

___

### LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR_MIPLINEAR](Texture.md#linear_linear_miplinear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:136

___

### LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[LINEAR_LINEAR_MIPNEAREST](Texture.md#linear_linear_mipnearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:131

___

### LINEAR\_NEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST](Texture.md#linear_nearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:155

___

### LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST_MIPLINEAR](Texture.md#linear_nearest_miplinear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:151

___

### LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Inherited from

[Texture](Texture.md).[LINEAR_NEAREST_MIPNEAREST](Texture.md#linear_nearest_mipnearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:149

___

### MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Inherited from

[Texture](Texture.md).[MIRROR_ADDRESSMODE](Texture.md#mirror_addressmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:183

___

### NEAREST\_LINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR](Texture.md#nearest_linear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:145

___

### NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR_MIPLINEAR](Texture.md#nearest_linear_miplinear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:143

___

### NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Inherited from

[Texture](Texture.md).[NEAREST_LINEAR_MIPNEAREST](Texture.md#nearest_linear_mipnearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:141

___

### NEAREST\_NEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST](Texture.md#nearest_nearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:147

___

### NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST_MIPLINEAR](Texture.md#nearest_nearest_miplinear)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:126

___

### NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Inherited from

[Texture](Texture.md).[NEAREST_NEAREST_MIPNEAREST](Texture.md#nearest_nearest_mipnearest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:139

___

### NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[Texture](Texture.md).[NEAREST_SAMPLINGMODE](Texture.md#nearest_samplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:124

___

### OnTextureLoadErrorObservable

▪ `Static` **OnTextureLoadErrorObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

This observable will notify when any texture had a loading error

#### Inherited from

[Texture](Texture.md).[OnTextureLoadErrorObservable](Texture.md#ontextureloaderrorobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:87

___

### PLANAR\_MODE

▪ `Static` `Readonly` **PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Inherited from

[Texture](Texture.md).[PLANAR_MODE](Texture.md#planar_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:162

___

### PROJECTION\_MODE

▪ `Static` `Readonly` **PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Inherited from

[Texture](Texture.md).[PROJECTION_MODE](Texture.md#projection_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:166

___

### SKYBOX\_MODE

▪ `Static` `Readonly` **SKYBOX\_MODE**: ``5``

Inverse Cubic coordinates mode

#### Inherited from

[Texture](Texture.md).[SKYBOX_MODE](Texture.md#skybox_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:168

___

### SPHERICAL\_MODE

▪ `Static` `Readonly` **SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Inherited from

[Texture](Texture.md).[SPHERICAL_MODE](Texture.md#spherical_mode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:160

___

### SerializeBuffers

▪ `Static` **SerializeBuffers**: `boolean` = `true`

Gets or sets a general boolean used to indicate that textures containing direct data (buffers) must be saved as part of the serialization process

#### Inherited from

[Texture](Texture.md).[SerializeBuffers](Texture.md#serializebuffers)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:76

___

### TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Texture](Texture.md).[TRILINEAR_SAMPLINGMODE](Texture.md#trilinear_samplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:134

___

### UseSerializedUrlIfAny

▪ `Static` **UseSerializedUrlIfAny**: `boolean` = `false`

Gets or sets a boolean which defines if the texture url must be build from the serialized URL instead of just using the name and loading them side by side with the scene file

#### Inherited from

[Texture](Texture.md).[UseSerializedUrlIfAny](Texture.md#useserializedurlifany)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:188

___

### WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Inherited from

[Texture](Texture.md).[WRAP_ADDRESSMODE](Texture.md#wrap_addressmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:181

## Accessors

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can rescale.

#### Returns

`boolean`

#### Inherited from

Texture.canRescale

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:592

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

Texture.coordinatesIndex

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

Texture.coordinatesIndex

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

Texture.coordinatesMode

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

Texture.coordinatesMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:144

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

Texture.errorObject

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

Texture.gammaSpace

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

Texture.gammaSpace

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Texture.getAlphaFromRGB

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

Texture.getAlphaFromRGB

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Texture.hasAlpha

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

Texture.hasAlpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:60

___

### invertY

• `get` **invertY**(): `boolean`

Gets a boolean indicating if the texture needs to be inverted on the y axis during loading

#### Returns

`boolean`

#### Inherited from

Texture.invertY

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:347

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:393

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.is2DArray

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

Texture.is2DArray

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.is3D

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

Texture.is3D

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

Texture.isBlocking

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:339

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:336

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

Texture.isCube

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

Texture.isCube

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

Texture.isRGBD

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

Texture.isRGBD

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

Texture.linearSpecularLOD

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

Texture.linearSpecularLOD

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

Texture.loadingError

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

Texture.lodGenerationOffset

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

Texture.lodGenerationOffset

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

Texture.lodGenerationScale

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

Texture.lodGenerationScale

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:363

___

### mimeType

• `get` **mimeType**(): `undefined` \| `string`

Returns the texture mime type if it was defined by a loader (undefined else)

#### Returns

`undefined` \| `string`

#### Inherited from

Texture.mimeType

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:322

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

Texture.noMipmap

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:275

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:459

___

### refreshRate

• `get` **refreshRate**(): `number`

Define the refresh rate of the texture or the rendering frequency.
Use 0 to render just once, 1 to render on every frame, 2 to render every two frames and so on...

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:350

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:355

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

Texture.samplingMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

Texture.textureFormat

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

Texture.textureType

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

Texture.uid

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

Texture.wrapU

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

Texture.wrapU

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

Texture.wrapV

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

Texture.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_checkUniform

▸ `Private` **_checkUniform**(`uniformName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `uniformName` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:419

___

### \_createIndexBuffer

▸ `Private` **_createIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:230

___

### \_createRtWrapper

▸ `Private` **_createRtWrapper**(`isCube`, `size`, `generateMipMaps`, `textureType`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `isCube` | `boolean` |
| `size` | `TextureSize` |
| `generateMipMaps` | `boolean` |
| `textureType` | `number` |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:172

___

### \_getDefines

▸ `Protected` **_getDefines**(): `string`

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:269

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[_markAllSubMeshesAsTexturesDirty](Texture.md#_markallsubmeshesastexturesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:670

___

### \_setEffect

▸ **_setEffect**(`effect`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | @hidden* |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:204

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:633

___

### clone

▸ **clone**(): [`ProceduralTexture`](ProceduralTexture.md)

Clone the texture.

#### Returns

[`ProceduralTexture`](ProceduralTexture.md)

the cloned texture

#### Overrides

[Texture](Texture.md).[clone](Texture.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:670

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Overrides

[Texture](Texture.md).[dispose](Texture.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:687

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

[Texture](Texture.md).[getBaseSize](Texture.md#getbasesize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:219

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:897

___

### getContent

▸ **getContent**(): [`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

Gets texture content (Use this function wisely as reading from a texture can be slow)

#### Returns

[`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

an ArrayBufferView promise (Uint8Array or Float32Array)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:212

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

The effect that is created when initializing the post process.

#### Returns

[`Effect`](Effect.md)

The created effect corresponding the the postprocess.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:196

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

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:188

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:751

___

### getRenderSize

▸ **getRenderSize**(): `TextureSize`

Get the size the texture is rendering at.

#### Returns

`TextureSize`

the size (on cube texture it is always squared)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:394

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:540

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

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:196

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:651

___

### isReady

▸ **isReady**(): `boolean`

Is the texture ready to be used ? (rendered at least once)

#### Returns

`boolean`

true if ready, otherwise, false.

#### Overrides

[Texture](Texture.md).[isReady](Texture.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:277

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

[Texture](Texture.md).[readPixels](Texture.md#readpixels)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[Texture](Texture.md).[releaseInternalTexture](Texture.md#releaseinternaltexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:284

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:549

___

### reset

▸ **reset**(): `void`

Resets the texture in order to recreate its associated resources.
This can be called in case of context loss

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:265

___

### resetRefreshCounter

▸ **resetRefreshCounter**(): `void`

Resets the refresh counter of the texture and start bak from scratch.
Could be useful to regenerate the texture if it is setup to render only once.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:334

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:403

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:587

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:852

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:485

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:498

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:446

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:472

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:342

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:459

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:537

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:431

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:511

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTexture.ts:524

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

[Texture](Texture.md).[updateSamplingMode](Texture.md#updatesamplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/thinTexture.ts:275

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:539

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:1057

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:1087

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

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:920

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

https://github.com/babylon.js/core/src/Materials/Textures/baseTexture.ts:864

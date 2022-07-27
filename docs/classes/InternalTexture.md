[@dev/core](../README.md) / [Exports](../modules.md) / InternalTexture

# Class: InternalTexture

Class used to store data associated with WebGL texture data for the engine
This class should not be used directly

## Hierarchy

- [`TextureSampler`](TextureSampler.md)

  ↳ **`InternalTexture`**

## Table of contents

### Constructors

- [constructor](InternalTexture.md#constructor)

### Properties

- [\_engine](InternalTexture.md#_engine)
- [\_uniqueId](InternalTexture.md#_uniqueid)
- [baseDepth](InternalTexture.md#basedepth)
- [baseHeight](InternalTexture.md#baseheight)
- [baseWidth](InternalTexture.md#basewidth)
- [depth](InternalTexture.md#depth)
- [format](InternalTexture.md#format)
- [generateMipMaps](InternalTexture.md#generatemipmaps)
- [height](InternalTexture.md#height)
- [invertY](InternalTexture.md#inverty)
- [is2DArray](InternalTexture.md#is2darray)
- [is3D](InternalTexture.md#is3d)
- [isCube](InternalTexture.md#iscube)
- [isMultiview](InternalTexture.md#ismultiview)
- [isReady](InternalTexture.md#isready)
- [onErrorObservable](InternalTexture.md#onerrorobservable)
- [onLoadedObservable](InternalTexture.md#onloadedobservable)
- [onRebuildCallback](InternalTexture.md#onrebuildcallback)
- [samples](InternalTexture.md#samples)
- [samplingMode](InternalTexture.md#samplingmode)
- [type](InternalTexture.md#type)
- [url](InternalTexture.md#url)
- [width](InternalTexture.md#width)

### Accessors

- [anisotropicFilteringLevel](InternalTexture.md#anisotropicfilteringlevel)
- [comparisonFunction](InternalTexture.md#comparisonfunction)
- [source](InternalTexture.md#source)
- [uniqueId](InternalTexture.md#uniqueid)
- [useMipMaps](InternalTexture.md#usemipmaps)
- [wrapR](InternalTexture.md#wrapr)
- [wrapU](InternalTexture.md#wrapu)
- [wrapV](InternalTexture.md#wrapv)

### Methods

- [compareSampler](InternalTexture.md#comparesampler)
- [dispose](InternalTexture.md#dispose)
- [getEngine](InternalTexture.md#getengine)
- [incrementReferences](InternalTexture.md#incrementreferences)
- [setParameters](InternalTexture.md#setparameters)
- [updateSize](InternalTexture.md#updatesize)

## Constructors

### constructor

• **new InternalTexture**(`engine`, `source`, `delayAllocation?`)

Creates a new InternalTexture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | `undefined` | defines the engine to use |
| `source` | [`InternalTextureSource`](../enums/InternalTextureSource.md) | `undefined` | defines the type of data that will be used |
| `delayAllocation` | `boolean` | `false` | if the texture allocation should be delayed (default: false) |

#### Overrides

[TextureSampler](TextureSampler.md).[constructor](TextureSampler.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:286

## Properties

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:254

___

### \_uniqueId

• `Private` **\_uniqueId**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:255

___

### baseDepth

• **baseDepth**: `number` = `0`

Gets the initial depth of the texture (It could be rescaled if the current system does not support non power of two textures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:175

___

### baseHeight

• **baseHeight**: `number` = `0`

Gets the initial height of the texture (It could be rescaled if the current system does not support non power of two textures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:171

___

### baseWidth

• **baseWidth**: `number` = `0`

Gets the initial width of the texture (It could be rescaled if the current system does not support non power of two textures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:167

___

### depth

• **depth**: `number` = `0`

Gets the depth of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:163

___

### format

• **format**: `number` = `-1`

Gets the format of the texture (RGB, RGBA...)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:133

___

### generateMipMaps

• **generateMipMaps**: `boolean` = `false`

Gets a boolean indicating if the texture needs mipmaps generation

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:111

___

### height

• **height**: `number` = `0`

Gets the height of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:159

___

### invertY

• **invertY**: `boolean` = `false`

Gets a boolean indicating if the texture is inverted on Y axis

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:179

___

### is2DArray

• **is2DArray**: `boolean` = `false`

Defines if the texture contains 2D array data

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:97

___

### is3D

• **is3D**: `boolean` = `false`

Defines if the texture contains 3D data

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:93

___

### isCube

• **isCube**: `boolean` = `false`

Defines if the texture is a cube texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:89

___

### isMultiview

• **isMultiview**: `boolean` = `false`

Defines if the texture contains multiview data

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:101

___

### isReady

• **isReady**: `boolean` = `false`

Defines if the texture is ready

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:85

___

### onErrorObservable

• **onErrorObservable**: [`Observable`](Observable.md)`Partial`{ `exception`: `any` ; `message`: `string`  }

Observable called when the texture load is raising an error

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:141

___

### onLoadedObservable

• **onLoadedObservable**: [`Observable`](Observable.md)[`InternalTexture`](InternalTexture.md)

Observable called when the texture is loaded

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:137

___

### onRebuildCallback

• **onRebuildCallback**: [`Nullable`](../modules.md#nullable)(`internalTexture`: [`InternalTexture`](InternalTexture.md)) => { `isAsync`: `boolean` ; `isReady`: `boolean` ; `proxy`: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) \| `Promise`[`InternalTexture`](InternalTexture.md)  } = `null`

If this callback is defined it will be called instead of the default _rebuild function

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:145

___

### samples

• **samples**: `number` = `0`

Gets the number of samples used by the texture (WebGL2+ only)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:125

___

### samplingMode

• **samplingMode**: `number` = `-1`

Gets the sampling mode of the texture

#### Inherited from

[TextureSampler](TextureSampler.md).[samplingMode](TextureSampler.md#samplingmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:11

___

### type

• **type**: `number` = `-1`

Gets the type of the texture (int, float...)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:129

___

### url

• **url**: `string` = `""`

Gets the URL used to load this texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:105

___

### width

• **width**: `number` = `0`

Gets the width of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:155

## Accessors

### anisotropicFilteringLevel

• `get` **anisotropicFilteringLevel**(): [`Nullable`](../modules.md#nullable)`number`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TextureSampler.anisotropicFilteringLevel

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:63

• `set` **anisotropicFilteringLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TextureSampler.anisotropicFilteringLevel

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:67

___

### comparisonFunction

• `get` **comparisonFunction**(): `number`

Gets or sets the comparison function (Constants.LESS, Constants.EQUAL, etc). Set 0 to not use a comparison function

#### Returns

`number`

#### Inherited from

TextureSampler.comparisonFunction

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:74

• `set` **comparisonFunction**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TextureSampler.comparisonFunction

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:78

___

### source

• `get` **source**(): [`InternalTextureSource`](../enums/InternalTextureSource.md)

Gets the data source type of the texture

#### Returns

[`InternalTextureSource`](../enums/InternalTextureSource.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:276

___

### uniqueId

• `get` **uniqueId**(): `number`

Gets the unique id of the internal texture

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:261

___

### useMipMaps

• `get` **useMipMaps**(): `boolean`

Gets a boolean indicating if the texture uses mipmaps
TODO implements useMipMaps as a separate setting from generateMipMaps

#### Returns

`boolean`

#### Overrides

TextureSampler.useMipMaps

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:116

• `set` **useMipMaps**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

TextureSampler.useMipMaps

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:119

___

### wrapR

• `get` **wrapR**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TextureSampler.wrapR

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:50

• `set` **wrapR**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TextureSampler.wrapR

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:54

___

### wrapU

• `get` **wrapU**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TextureSampler.wrapU

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:20

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TextureSampler.wrapU

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:24

___

### wrapV

• `get` **wrapV**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TextureSampler.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:35

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TextureSampler.wrapV

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:39

## Methods

### compareSampler

▸ **compareSampler**(`other`): `boolean`

Compares this sampler with another one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`TextureSampler`](TextureSampler.md) | sampler to compare with |

#### Returns

`boolean`

true if the samplers have the same parametres, else false

#### Inherited from

[TextureSampler](TextureSampler.md).[compareSampler](TextureSampler.md#comparesampler)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:148

___

### dispose

▸ **dispose**(): `void`

Dispose the current allocated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:559

___

### getEngine

▸ **getEngine**(): [`ThinEngine`](ThinEngine.md)

Gets the Engine the texture belongs to.

#### Returns

[`ThinEngine`](ThinEngine.md)

The babylon engine

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:269

___

### incrementReferences

▸ **incrementReferences**(): `void`

Increments the number of references (ie. the number of Texture that point to it)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:301

___

### setParameters

▸ **setParameters**(`wrapU?`, `wrapV?`, `wrapR?`, `anisotropicFilteringLevel?`, `samplingMode?`, `comparisonFunction?`): [`TextureSampler`](TextureSampler.md)

Sets all the parameters of the sampler

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `wrapU` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | u address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `wrapV` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | v address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `wrapR` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | r address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `anisotropicFilteringLevel` | `number` | `1` | anisotropic level (default: 1) |
| `samplingMode` | `number` | `Constants.TEXTURE_BILINEAR_SAMPLINGMODE` | sampling mode (default: Constants.TEXTURE_BILINEAR_SAMPLINGMODE) |
| `comparisonFunction` | `number` | `0` | comparison function (default: 0 - no comparison function) |

#### Returns

[`TextureSampler`](TextureSampler.md)

the current sampler instance

#### Inherited from

[TextureSampler](TextureSampler.md).[setParameters](TextureSampler.md#setparameters)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:125

___

### updateSize

▸ **updateSize**(`width`, `height`, `depth?`): `void`

Change the size of the texture (not the size of the content)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the new width |
| `height` | `number` | `undefined` | defines the new height |
| `depth` | `number` | `1` | defines the new depth (1 by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTexture.ts:311

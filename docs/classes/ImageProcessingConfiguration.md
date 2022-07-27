[@dev/core](../README.md) / [Exports](../modules.md) / ImageProcessingConfiguration

# Class: ImageProcessingConfiguration

This groups together the common properties used for image processing either in direct forward pass
or through post processing effect depending on the use of the image processing pipeline in your scene
or not.

## Table of contents

### Constructors

- [constructor](ImageProcessingConfiguration.md#constructor)

### Properties

- [\_colorCurvesEnabled](ImageProcessingConfiguration.md#_colorcurvesenabled)
- [\_colorGradingBGR](ImageProcessingConfiguration.md#_colorgradingbgr)
- [\_colorGradingEnabled](ImageProcessingConfiguration.md#_colorgradingenabled)
- [\_colorGradingTexture](ImageProcessingConfiguration.md#_colorgradingtexture)
- [\_colorGradingWithGreenDepth](ImageProcessingConfiguration.md#_colorgradingwithgreendepth)
- [\_contrast](ImageProcessingConfiguration.md#_contrast)
- [\_isEnabled](ImageProcessingConfiguration.md#_isenabled)
- [\_toneMappingEnabled](ImageProcessingConfiguration.md#_tonemappingenabled)
- [\_toneMappingType](ImageProcessingConfiguration.md#_tonemappingtype)
- [\_vignetteBlendMode](ImageProcessingConfiguration.md#_vignetteblendmode)
- [\_vignetteEnabled](ImageProcessingConfiguration.md#_vignetteenabled)
- [colorCurves](ImageProcessingConfiguration.md#colorcurves)
- [onUpdateParameters](ImageProcessingConfiguration.md#onupdateparameters)
- [vignetteCameraFov](ImageProcessingConfiguration.md#vignettecamerafov)
- [vignetteCentreX](ImageProcessingConfiguration.md#vignettecentrex)
- [vignetteCentreY](ImageProcessingConfiguration.md#vignettecentrey)
- [vignetteColor](ImageProcessingConfiguration.md#vignettecolor)
- [vignetteStretch](ImageProcessingConfiguration.md#vignettestretch)
- [vignetteWeight](ImageProcessingConfiguration.md#vignetteweight)
- [TONEMAPPING\_ACES](ImageProcessingConfiguration.md#tonemapping_aces)
- [TONEMAPPING\_STANDARD](ImageProcessingConfiguration.md#tonemapping_standard)
- [\_VIGNETTEMODE\_MULTIPLY](ImageProcessingConfiguration.md#_vignettemode_multiply)
- [\_VIGNETTEMODE\_OPAQUE](ImageProcessingConfiguration.md#_vignettemode_opaque)

### Accessors

- [applyByPostProcess](ImageProcessingConfiguration.md#applybypostprocess)
- [colorCurvesEnabled](ImageProcessingConfiguration.md#colorcurvesenabled)
- [colorGradingBGR](ImageProcessingConfiguration.md#colorgradingbgr)
- [colorGradingEnabled](ImageProcessingConfiguration.md#colorgradingenabled)
- [colorGradingTexture](ImageProcessingConfiguration.md#colorgradingtexture)
- [colorGradingWithGreenDepth](ImageProcessingConfiguration.md#colorgradingwithgreendepth)
- [contrast](ImageProcessingConfiguration.md#contrast)
- [exposure](ImageProcessingConfiguration.md#exposure)
- [isEnabled](ImageProcessingConfiguration.md#isenabled)
- [skipFinalColorClamp](ImageProcessingConfiguration.md#skipfinalcolorclamp)
- [toneMappingEnabled](ImageProcessingConfiguration.md#tonemappingenabled)
- [toneMappingType](ImageProcessingConfiguration.md#tonemappingtype)
- [vignetteBlendMode](ImageProcessingConfiguration.md#vignetteblendmode)
- [vignetteEnabled](ImageProcessingConfiguration.md#vignetteenabled)
- [VIGNETTEMODE\_MULTIPLY](ImageProcessingConfiguration.md#vignettemode_multiply)
- [VIGNETTEMODE\_OPAQUE](ImageProcessingConfiguration.md#vignettemode_opaque)

### Methods

- [\_updateParameters](ImageProcessingConfiguration.md#_updateparameters)
- [bind](ImageProcessingConfiguration.md#bind)
- [clone](ImageProcessingConfiguration.md#clone)
- [getClassName](ImageProcessingConfiguration.md#getclassname)
- [isReady](ImageProcessingConfiguration.md#isready)
- [prepareDefines](ImageProcessingConfiguration.md#preparedefines)
- [serialize](ImageProcessingConfiguration.md#serialize)
- [Parse](ImageProcessingConfiguration.md#parse)
- [PrepareSamplers](ImageProcessingConfiguration.md#preparesamplers)
- [PrepareUniforms](ImageProcessingConfiguration.md#prepareuniforms)

## Constructors

### constructor

• **new ImageProcessingConfiguration**()

## Properties

### \_colorCurvesEnabled

• `Private` **\_colorCurvesEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:86

___

### \_colorGradingBGR

• `Private` **\_colorGradingBGR**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:166

___

### \_colorGradingEnabled

• `Private` **\_colorGradingEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:126

___

### \_colorGradingTexture

• `Private` **\_colorGradingTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:106

___

### \_colorGradingWithGreenDepth

• `Private` **\_colorGradingWithGreenDepth**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:146

___

### \_contrast

• `Protected` **\_contrast**: `number` = `1.0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:247

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:388

___

### \_toneMappingEnabled

• `Private` **\_toneMappingEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:207

___

### \_toneMappingType

• `Private` **\_toneMappingType**: `number` = `ImageProcessingConfiguration.TONEMAPPING_STANDARD`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:227

___

### \_vignetteBlendMode

• `Private` **\_vignetteBlendMode**: `number` = `ImageProcessingConfiguration.VIGNETTEMODE_MULTIPLY`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:304

___

### \_vignetteEnabled

• `Private` **\_vignetteEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:324

___

### colorCurves

• **colorCurves**: [`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

Color curves setup used in the effect if colorCurvesEnabled is set to true

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:83

___

### onUpdateParameters

• **onUpdateParameters**: [`Observable`](Observable.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

An event triggered when the configuration changes and requires Shader to Update some parameters.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:410

___

### vignetteCameraFov

• **vignetteCameraFov**: `number` = `0.5`

Camera field of view used by the Vignette effect.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:301

___

### vignetteCentreX

• **vignetteCentreX**: `number` = `0`

Vignette centre X Offset.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:276

___

### vignetteCentreY

• **vignetteCentreY**: `number` = `0`

Vignette centre Y Offset.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:282

___

### vignetteColor

• **vignetteColor**: [`Color4`](Color4.md)

Color of the vignette applied on the screen through the chosen blend mode (vignetteBlendMode)
if vignetteEnabled is set to true.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:295

___

### vignetteStretch

• **vignetteStretch**: `number` = `0`

Vignette stretch size.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:270

___

### vignetteWeight

• **vignetteWeight**: `number` = `1.5`

Vignette weight or intensity of the vignette effect.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:288

___

### TONEMAPPING\_ACES

▪ `Static` `Readonly` **TONEMAPPING\_ACES**: ``1``

ACES Tone mapping (used by default in unreal and unity). This can help getting closer
to other engines rendering to increase portability.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:77

___

### TONEMAPPING\_STANDARD

▪ `Static` `Readonly` **TONEMAPPING\_STANDARD**: ``0``

Default tone mapping applied in BabylonJS.

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:71

___

### \_VIGNETTEMODE\_MULTIPLY

▪ `Static` `Private` **\_VIGNETTEMODE\_MULTIPLY**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:602

___

### \_VIGNETTEMODE\_OPAQUE

▪ `Static` `Private` **\_VIGNETTEMODE\_OPAQUE**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:603

## Accessors

### applyByPostProcess

• `get` **applyByPostProcess**(): `boolean`

Gets whether the image processing is applied through a post process or not.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:372

• `set` **applyByPostProcess**(`value`): `void`

Sets whether the image processing is applied through a post process or not.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:378

___

### colorCurvesEnabled

• `get` **colorCurvesEnabled**(): `boolean`

Gets whether the color curves effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:90

• `set` **colorCurvesEnabled**(`value`): `void`

Sets whether the color curves effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:96

___

### colorGradingBGR

• `get` **colorGradingBGR**(): `boolean`

Gets whether the color grading texture contains BGR values.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:170

• `set` **colorGradingBGR**(`value`): `void`

Sets whether the color grading texture contains BGR values.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:176

___

### colorGradingEnabled

• `get` **colorGradingEnabled**(): `boolean`

Gets whether the color grading effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:130

• `set` **colorGradingEnabled**(`value`): `void`

Sets whether the color grading effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:136

___

### colorGradingTexture

• `get` **colorGradingTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Color grading LUT texture used in the effect if colorGradingEnabled is set to true

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:110

• `set` **colorGradingTexture**(`value`): `void`

Color grading LUT texture used in the effect if colorGradingEnabled is set to true

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:116

___

### colorGradingWithGreenDepth

• `get` **colorGradingWithGreenDepth**(): `boolean`

Gets whether the color grading effect is using a green depth for the 3d Texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:150

• `set` **colorGradingWithGreenDepth**(`value`): `void`

Sets whether the color grading effect is using a green depth for the 3d Texture.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:156

___

### contrast

• `get` **contrast**(): `number`

Gets the contrast used in the effect.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:251

• `set` **contrast**(`value`): `void`

Sets the contrast used in the effect.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:257

___

### exposure

• `get` **exposure**(): `number`

Gets the Exposure used in the effect.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:191

• `set` **exposure**(`value`): `void`

Sets the Exposure used in the effect.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:197

___

### isEnabled

• `get` **isEnabled**(): `boolean`

Gets whether the image processing is enabled or not.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:392

• `set` **isEnabled**(`value`): `void`

Sets whether the image processing is enabled or not.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:398

___

### skipFinalColorClamp

• `get` **skipFinalColorClamp**(): `boolean`

If apply by post process is set to true, setting this to true will skip the the final color clamp step in the fragment shader
Applies to PBR materials.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:350

• `set` **skipFinalColorClamp**(`value`): `void`

If apply by post process is set to true, setting this to true will skip the the final color clamp step in the fragment shader
Applies to PBR materials.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:357

___

### toneMappingEnabled

• `get` **toneMappingEnabled**(): `boolean`

Gets whether the tone mapping effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:211

• `set` **toneMappingEnabled**(`value`): `void`

Sets whether the tone mapping effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:217

___

### toneMappingType

• `get` **toneMappingType**(): `number`

Gets the type of tone mapping effect.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:231

• `set` **toneMappingType**(`value`): `void`

Sets the type of tone mapping effect used in BabylonJS.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:237

___

### vignetteBlendMode

• `get` **vignetteBlendMode**(): `number`

Gets the vignette blend mode allowing different kind of effect.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:308

• `set` **vignetteBlendMode**(`value`): `void`

Sets the vignette blend mode allowing different kind of effect.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:314

___

### vignetteEnabled

• `get` **vignetteEnabled**(): `boolean`

Gets whether the vignette effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:328

• `set` **vignetteEnabled**(`value`): `void`

Sets whether the vignette effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:334

___

### VIGNETTEMODE\_MULTIPLY

• `Static` `get` **VIGNETTEMODE_MULTIPLY**(): `number`

Used to apply the vignette as a mix with the pixel color.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:608

___

### VIGNETTEMODE\_OPAQUE

• `Static` `get` **VIGNETTEMODE_OPAQUE**(): `number`

Used to apply the vignette as a replacement of the pixel color.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:615

## Methods

### \_updateParameters

▸ `Protected` **_updateParameters**(): `void`

Method called each time the image processing information changes requires to recompile the effect.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:415

___

### bind

▸ **bind**(`effect`, `overrideAspectRatio?`): `void`

Binds the image processing to the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to bind to |
| `overrideAspectRatio?` | `number` | Override the aspect ratio of the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:528

___

### clone

▸ **clone**(): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Clones the current image processing instance.

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

The cloned image processing

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:580

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name.

#### Returns

`string`

"ImageProcessingConfiguration"

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:423

___

### isReady

▸ **isReady**(): `boolean`

Returns true if all the image processing information are ready.

#### Returns

`boolean`

True if ready, otherwise, false

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:518

___

### prepareDefines

▸ **prepareDefines**(`defines`, `forPostProcess?`): `void`

Prepare the list of defines associated to the shader.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `defines` | `IImageProcessingConfigurationDefines` | `undefined` | the list of defines to complete |
| `forPostProcess` | `boolean` | `false` | Define if we are currently in post process mode or not |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:468

___

### serialize

▸ **serialize**(): `any`

Serializes the current image processing instance to a json representation.

#### Returns

`any`

a JSON representation

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:588

___

### Parse

▸ `Static` **Parse**(`source`): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Parses the image processing from a json representation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | the JSON source to parse |

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

The parsed image processing

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:597

___

### PrepareSamplers

▸ `Static` **PrepareSamplers**(`samplersList`, `defines`): `void`

Prepare the list of samplers associated with the Image Processing effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `samplersList` | `string`[] | The list of uniforms used in the effect |
| `defines` | `IImageProcessingConfigurationDefines` | the list of defines currently in use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:457

___

### PrepareUniforms

▸ `Static` **PrepareUniforms**(`uniforms`, `defines`): `void`

Prepare the list of uniforms associated with the Image Processing effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniforms` | `string`[] | The list of uniforms used in the effect |
| `defines` | `IImageProcessingConfigurationDefines` | the list of defines currently in use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/imageProcessingConfiguration.ts:432

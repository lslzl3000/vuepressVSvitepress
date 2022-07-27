[@dev/core](../README.md) / [Exports](../modules.md) / ColorCurves

# Class: ColorCurves

The color grading curves provide additional color adjustment that is applied after any color grading transform (3D LUT).
They allow basic adjustment of saturation and small exposure adjustments, along with color filter tinting to provide white balance adjustment or more stylistic effects.
These are similar to controls found in many professional imaging or colorist software. The global controls are applied to the entire image. For advanced tuning, extra controls are provided to adjust the shadow, midtone and highlight areas of the image;
corresponding to low luminance, medium luminance, and high luminance areas respectively.

## Table of contents

### Constructors

- [constructor](ColorCurves.md#constructor)

### Properties

- [\_dirty](ColorCurves.md#_dirty)
- [\_globalCurve](ColorCurves.md#_globalcurve)
- [\_globalDensity](ColorCurves.md#_globaldensity)
- [\_globalExposure](ColorCurves.md#_globalexposure)
- [\_globalHue](ColorCurves.md#_globalhue)
- [\_globalSaturation](ColorCurves.md#_globalsaturation)
- [\_highlightsCurve](ColorCurves.md#_highlightscurve)
- [\_highlightsDensity](ColorCurves.md#_highlightsdensity)
- [\_highlightsExposure](ColorCurves.md#_highlightsexposure)
- [\_highlightsHue](ColorCurves.md#_highlightshue)
- [\_highlightsSaturation](ColorCurves.md#_highlightssaturation)
- [\_midtonesCurve](ColorCurves.md#_midtonescurve)
- [\_midtonesDensity](ColorCurves.md#_midtonesdensity)
- [\_midtonesExposure](ColorCurves.md#_midtonesexposure)
- [\_midtonesHue](ColorCurves.md#_midtoneshue)
- [\_midtonesSaturation](ColorCurves.md#_midtonessaturation)
- [\_negativeCurve](ColorCurves.md#_negativecurve)
- [\_positiveCurve](ColorCurves.md#_positivecurve)
- [\_shadowsCurve](ColorCurves.md#_shadowscurve)
- [\_shadowsDensity](ColorCurves.md#_shadowsdensity)
- [\_shadowsExposure](ColorCurves.md#_shadowsexposure)
- [\_shadowsHue](ColorCurves.md#_shadowshue)
- [\_shadowsSaturation](ColorCurves.md#_shadowssaturation)
- [\_tempColor](ColorCurves.md#_tempcolor)

### Accessors

- [globalDensity](ColorCurves.md#globaldensity)
- [globalExposure](ColorCurves.md#globalexposure)
- [globalHue](ColorCurves.md#globalhue)
- [globalSaturation](ColorCurves.md#globalsaturation)
- [highlightsDensity](ColorCurves.md#highlightsdensity)
- [highlightsExposure](ColorCurves.md#highlightsexposure)
- [highlightsHue](ColorCurves.md#highlightshue)
- [highlightsSaturation](ColorCurves.md#highlightssaturation)
- [midtonesDensity](ColorCurves.md#midtonesdensity)
- [midtonesExposure](ColorCurves.md#midtonesexposure)
- [midtonesHue](ColorCurves.md#midtoneshue)
- [midtonesSaturation](ColorCurves.md#midtonessaturation)
- [shadowsDensity](ColorCurves.md#shadowsdensity)
- [shadowsExposure](ColorCurves.md#shadowsexposure)
- [shadowsHue](ColorCurves.md#shadowshue)
- [shadowsSaturation](ColorCurves.md#shadowssaturation)

### Methods

- [\_getColorGradingDataToRef](ColorCurves.md#_getcolorgradingdatatoref)
- [clone](ColorCurves.md#clone)
- [getClassName](ColorCurves.md#getclassname)
- [serialize](ColorCurves.md#serialize)
- [Bind](ColorCurves.md#bind)
- [Parse](ColorCurves.md#parse)
- [PrepareUniforms](ColorCurves.md#prepareuniforms)
- [\_ApplyColorGradingSliderNonlinear](ColorCurves.md#_applycolorgradingslidernonlinear)
- [\_Clamp](ColorCurves.md#_clamp)
- [\_FromHSBToRef](ColorCurves.md#_fromhsbtoref)

## Constructors

### constructor

• **new ColorCurves**()

## Properties

### \_dirty

• `Private` **\_dirty**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:12

___

### \_globalCurve

• `Private` **\_globalCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:16

___

### \_globalDensity

• `Private` **\_globalDensity**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:28

___

### \_globalExposure

• `Private` **\_globalExposure**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:34

___

### \_globalHue

• `Private` **\_globalHue**: `number` = `30`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:25

___

### \_globalSaturation

• `Private` **\_globalSaturation**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:31

___

### \_highlightsCurve

• `Private` **\_highlightsCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:17

___

### \_highlightsDensity

• `Private` **\_highlightsDensity**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:104

___

### \_highlightsExposure

• `Private` **\_highlightsExposure**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:110

___

### \_highlightsHue

• `Private` **\_highlightsHue**: `number` = `30`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:101

___

### \_highlightsSaturation

• `Private` **\_highlightsSaturation**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:107

___

### \_midtonesCurve

• `Private` **\_midtonesCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:18

___

### \_midtonesDensity

• `Private` **\_midtonesDensity**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:179

___

### \_midtonesExposure

• `Private` **\_midtonesExposure**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:185

___

### \_midtonesHue

• `Private` **\_midtonesHue**: `number` = `30`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:176

___

### \_midtonesSaturation

• `Private` **\_midtonesSaturation**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:182

___

### \_negativeCurve

• `Private` **\_negativeCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:22

___

### \_positiveCurve

• `Private` **\_positiveCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:21

___

### \_shadowsCurve

• `Private` **\_shadowsCurve**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:19

___

### \_shadowsDensity

• `Private` **\_shadowsDensity**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:251

___

### \_shadowsExposure

• `Private` **\_shadowsExposure**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:253

___

### \_shadowsHue

• `Private` **\_shadowsHue**: `number` = `30`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:250

___

### \_shadowsSaturation

• `Private` **\_shadowsSaturation**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:252

___

### \_tempColor

• `Private` **\_tempColor**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:14

## Accessors

### globalDensity

• `get` **globalDensity**(): `number`

Gets the global Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:56

• `set` **globalDensity**(`value`): `void`

Sets the global Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:64

___

### globalExposure

• `get` **globalExposure**(): `number`

Gets the global Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:88

• `set` **globalExposure**(`value`): `void`

Sets the global Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:95

___

### globalHue

• `get` **globalHue**(): `number`

Gets the global Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:40

• `set` **globalHue**(`value`): `void`

Sets the global Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:47

___

### globalSaturation

• `get` **globalSaturation**(): `number`

Gets the global Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:72

• `set` **globalSaturation**(`value`): `void`

Sets the global Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:79

___

### highlightsDensity

• `get` **highlightsDensity**(): `number`

Gets the highlights Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:132

• `set` **highlightsDensity**(`value`): `void`

Sets the highlights Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:140

___

### highlightsExposure

• `get` **highlightsExposure**(): `number`

Gets the highlights Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:163

• `set` **highlightsExposure**(`value`): `void`

Sets the highlights Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:170

___

### highlightsHue

• `get` **highlightsHue**(): `number`

Gets the highlights Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:116

• `set` **highlightsHue**(`value`): `void`

Sets the highlights Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:123

___

### highlightsSaturation

• `get` **highlightsSaturation**(): `number`

Gets the highlights Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:148

• `set` **highlightsSaturation**(`value`): `void`

Sets the highlights Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:155

___

### midtonesDensity

• `get` **midtonesDensity**(): `number`

Gets the midtones Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:207

• `set` **midtonesDensity**(`value`): `void`

Sets the midtones Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:215

___

### midtonesExposure

• `get` **midtonesExposure**(): `number`

Gets the midtones Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:238

• `set` **midtonesExposure**(`value`): `void`

Sets the midtones Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:245

___

### midtonesHue

• `get` **midtonesHue**(): `number`

Gets the midtones Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:191

• `set` **midtonesHue**(`value`): `void`

Sets the midtones Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:198

___

### midtonesSaturation

• `get` **midtonesSaturation**(): `number`

Gets the midtones Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:223

• `set` **midtonesSaturation**(`value`): `void`

Sets the midtones Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:230

___

### shadowsDensity

• `get` **shadowsDensity**(): `number`

Gets the shadows Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:275

• `set` **shadowsDensity**(`value`): `void`

Sets the shadows Density value.
The density value is in range [-100,+100] where 0 means the color filter has no effect and +100 means the color filter has maximum effect.
Values less than zero provide a filter of opposite hue.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:283

___

### shadowsExposure

• `get` **shadowsExposure**(): `number`

Gets the shadows Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:306

• `set` **shadowsExposure**(`value`): `void`

Sets the shadows Exposure value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase exposure and negative values decrease exposure.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:313

___

### shadowsHue

• `get` **shadowsHue**(): `number`

Gets the shadows Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:259

• `set` **shadowsHue**(`value`): `void`

Sets the shadows Hue value.
The hue value is a standard HSB hue in the range [0,360] where 0=red, 120=green and 240=blue. The default value is 30 degrees (orange).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:266

___

### shadowsSaturation

• `get` **shadowsSaturation**(): `number`

Gets the shadows Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:291

• `set` **shadowsSaturation**(`value`): `void`

Sets the shadows Saturation value.
This is an adjustment value in the range [-100,+100], where the default value of 0.0 makes no adjustment, positive values increase saturation and negative values decrease saturation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:298

## Methods

### \_getColorGradingDataToRef

▸ `Private` **_getColorGradingDataToRef**(`hue`, `density`, `saturation`, `exposure`, `result`): `void`

Returns color grading data based on a hue, density, saturation and exposure value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hue` | `number` |  |
| `density` | `number` |  |
| `saturation` | `number` | The saturation. |
| `exposure` | `number` | The exposure. |
| `result` | [`Color4`](Color4.md) | The result data container. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:411

___

### clone

▸ **clone**(): [`ColorCurves`](ColorCurves.md)

Clones the current color curve instance.

#### Returns

[`ColorCurves`](ColorCurves.md)

The cloned curves

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:540

___

### getClassName

▸ **getClassName**(): `string`

Returns the class name

#### Returns

`string`

The class name

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:322

___

### serialize

▸ **serialize**(): `any`

Serializes the current color curve instance to a json representation.

#### Returns

`any`

a JSON representation

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:548

___

### Bind

▸ `Static` **Bind**(`colorCurves`, `effect`, `positiveUniform?`, `neutralUniform?`, `negativeUniform?`): `void`

Binds the color curves to the shader.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `colorCurves` | [`ColorCurves`](ColorCurves.md) | `undefined` | The color curve to bind |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect to bind to |
| `positiveUniform` | `string` | `"vCameraColorCurvePositive"` | The positive uniform shader parameter |
| `neutralUniform` | `string` | `"vCameraColorCurveNeutral"` | The neutral uniform shader parameter |
| `negativeUniform` | `string` | `"vCameraColorCurveNegative"` | The negative uniform shader parameter |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:334

___

### Parse

▸ `Static` **Parse**(`source`): [`ColorCurves`](ColorCurves.md)

Parses the color curve from a json representation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | the JSON source to parse |

#### Returns

[`ColorCurves`](ColorCurves.md)

The parsed curves

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:557

___

### PrepareUniforms

▸ `Static` **PrepareUniforms**(`uniformsList`): `void`

Prepare the list of uniforms associated with the ColorCurves effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformsList` | `string`[] | The list of uniforms used in the effect |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:399

___

### \_ApplyColorGradingSliderNonlinear

▸ `Static` `Private` **_ApplyColorGradingSliderNonlinear**(`value`): `number`

Takes an input slider value and returns an adjusted value that provides extra control near the centre.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | The input slider value in range [-100,100]. |

#### Returns

`number`

Adjusted value.

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:444

___

### \_Clamp

▸ `Static` `Private` **_Clamp**(`value`, `min`, `max`): `number`

Returns a value clamped between min and max

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | The value to clamp |
| `min` | `number` | The minimum of value |
| `max` | `number` | The maximum of value |

#### Returns

`number`

The clamped value.

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:532

___

### \_FromHSBToRef

▸ `Static` `Private` **_FromHSBToRef**(`hue`, `saturation`, `brightness`, `result`): `void`

Returns an RGBA Color4 based on Hue, Saturation and Brightness (also referred to as value, HSV).

**`Result`**

An RGBA color represented as Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hue` | `number` | The hue (H) input. |
| `saturation` | `number` | The saturation (S) input. |
| `brightness` | `number` | The brightness (B) input. |
| `result` | [`Color4`](Color4.md) |  |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/colorCurves.ts:467

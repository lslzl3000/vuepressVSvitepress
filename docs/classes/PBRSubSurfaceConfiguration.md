[@dev/core](../README.md) / [Exports](../modules.md) / PBRSubSurfaceConfiguration

# Class: PBRSubSurfaceConfiguration

Plugin that implements the sub surface component of the PBR material

## Hierarchy

- [`MaterialPluginBase`](MaterialPluginBase.md)

  ↳ **`PBRSubSurfaceConfiguration`**

## Table of contents

### Constructors

- [constructor](PBRSubSurfaceConfiguration.md#constructor)

### Properties

- [\_internalMarkScenePrePassDirty](PBRSubSurfaceConfiguration.md#_internalmarksceneprepassdirty)
- [\_invertRefractionY](PBRSubSurfaceConfiguration.md#_invertrefractiony)
- [\_isRefractionEnabled](PBRSubSurfaceConfiguration.md#_isrefractionenabled)
- [\_isScatteringEnabled](PBRSubSurfaceConfiguration.md#_isscatteringenabled)
- [\_isTranslucencyEnabled](PBRSubSurfaceConfiguration.md#_istranslucencyenabled)
- [\_material](PBRSubSurfaceConfiguration.md#_material)
- [\_pluginDefineNames](PBRSubSurfaceConfiguration.md#_plugindefinenames)
- [\_pluginManager](PBRSubSurfaceConfiguration.md#_pluginmanager)
- [\_refractionIntensityTexture](PBRSubSurfaceConfiguration.md#_refractionintensitytexture)
- [\_refractionTexture](PBRSubSurfaceConfiguration.md#_refractiontexture)
- [\_scatteringDiffusionProfileIndex](PBRSubSurfaceConfiguration.md#_scatteringdiffusionprofileindex)
- [\_scene](PBRSubSurfaceConfiguration.md#_scene)
- [\_thicknessTexture](PBRSubSurfaceConfiguration.md#_thicknesstexture)
- [\_translucencyIntensityTexture](PBRSubSurfaceConfiguration.md#_translucencyintensitytexture)
- [\_useGltfStyleTextures](PBRSubSurfaceConfiguration.md#_usegltfstyletextures)
- [\_useMaskFromThicknessTexture](PBRSubSurfaceConfiguration.md#_usemaskfromthicknesstexture)
- [\_volumeIndexOfRefraction](PBRSubSurfaceConfiguration.md#_volumeindexofrefraction)
- [diffusionDistance](PBRSubSurfaceConfiguration.md#diffusiondistance)
- [indexOfRefraction](PBRSubSurfaceConfiguration.md#indexofrefraction)
- [invertRefractionY](PBRSubSurfaceConfiguration.md#invertrefractiony)
- [isRefractionEnabled](PBRSubSurfaceConfiguration.md#isrefractionenabled)
- [isScatteringEnabled](PBRSubSurfaceConfiguration.md#isscatteringenabled)
- [isTranslucencyEnabled](PBRSubSurfaceConfiguration.md#istranslucencyenabled)
- [linkRefractionWithTransparency](PBRSubSurfaceConfiguration.md#linkrefractionwithtransparency)
- [markAllDefinesAsDirty](PBRSubSurfaceConfiguration.md#markalldefinesasdirty)
- [maximumThickness](PBRSubSurfaceConfiguration.md#maximumthickness)
- [minimumThickness](PBRSubSurfaceConfiguration.md#minimumthickness)
- [name](PBRSubSurfaceConfiguration.md#name)
- [priority](PBRSubSurfaceConfiguration.md#priority)
- [refractionIntensity](PBRSubSurfaceConfiguration.md#refractionintensity)
- [refractionIntensityTexture](PBRSubSurfaceConfiguration.md#refractionintensitytexture)
- [refractionTexture](PBRSubSurfaceConfiguration.md#refractiontexture)
- [registerForExtraEvents](PBRSubSurfaceConfiguration.md#registerforextraevents)
- [thicknessTexture](PBRSubSurfaceConfiguration.md#thicknesstexture)
- [tintColor](PBRSubSurfaceConfiguration.md#tintcolor)
- [tintColorAtDistance](PBRSubSurfaceConfiguration.md#tintcoloratdistance)
- [translucencyIntensity](PBRSubSurfaceConfiguration.md#translucencyintensity)
- [translucencyIntensityTexture](PBRSubSurfaceConfiguration.md#translucencyintensitytexture)
- [useAlbedoToTintRefraction](PBRSubSurfaceConfiguration.md#usealbedototintrefraction)
- [useAlbedoToTintTranslucency](PBRSubSurfaceConfiguration.md#usealbedototinttranslucency)
- [useGltfStyleTextures](PBRSubSurfaceConfiguration.md#usegltfstyletextures)
- [useMaskFromThicknessTexture](PBRSubSurfaceConfiguration.md#usemaskfromthicknesstexture)
- [useThicknessAsDepth](PBRSubSurfaceConfiguration.md#usethicknessasdepth)

### Accessors

- [disableAlphaBlending](PBRSubSurfaceConfiguration.md#disablealphablending)
- [scatteringDiffusionProfile](PBRSubSurfaceConfiguration.md#scatteringdiffusionprofile)
- [volumeIndexOfRefraction](PBRSubSurfaceConfiguration.md#volumeindexofrefraction)

### Methods

- [\_enable](PBRSubSurfaceConfiguration.md#_enable)
- [\_getRefractionTexture](PBRSubSurfaceConfiguration.md#_getrefractiontexture)
- [addFallbacks](PBRSubSurfaceConfiguration.md#addfallbacks)
- [bindForSubMesh](PBRSubSurfaceConfiguration.md#bindforsubmesh)
- [collectDefines](PBRSubSurfaceConfiguration.md#collectdefines)
- [copyTo](PBRSubSurfaceConfiguration.md#copyto)
- [dispose](PBRSubSurfaceConfiguration.md#dispose)
- [fillRenderTargetTextures](PBRSubSurfaceConfiguration.md#fillrendertargettextures)
- [getActiveTextures](PBRSubSurfaceConfiguration.md#getactivetextures)
- [getAnimatables](PBRSubSurfaceConfiguration.md#getanimatables)
- [getAttributes](PBRSubSurfaceConfiguration.md#getattributes)
- [getClassName](PBRSubSurfaceConfiguration.md#getclassname)
- [getCustomCode](PBRSubSurfaceConfiguration.md#getcustomcode)
- [getSamplers](PBRSubSurfaceConfiguration.md#getsamplers)
- [getUniformBuffersNames](PBRSubSurfaceConfiguration.md#getuniformbuffersnames)
- [getUniforms](PBRSubSurfaceConfiguration.md#getuniforms)
- [hardBindForSubMesh](PBRSubSurfaceConfiguration.md#hardbindforsubmesh)
- [hasRenderTargetTextures](PBRSubSurfaceConfiguration.md#hasrendertargettextures)
- [hasTexture](PBRSubSurfaceConfiguration.md#hastexture)
- [isReadyForSubMesh](PBRSubSurfaceConfiguration.md#isreadyforsubmesh)
- [parse](PBRSubSurfaceConfiguration.md#parse)
- [prepareDefines](PBRSubSurfaceConfiguration.md#preparedefines)
- [prepareDefinesBeforeAttributes](PBRSubSurfaceConfiguration.md#preparedefinesbeforeattributes)
- [serialize](PBRSubSurfaceConfiguration.md#serialize)

## Constructors

### constructor

• **new PBRSubSurfaceConfiguration**(`material`, `addToPluginList?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `material` | [`PBRBaseMaterial`](PBRBaseMaterial.md) | `undefined` |
| `addToPluginList` | `boolean` | `true` |

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[constructor](MaterialPluginBase.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:319

## Properties

### \_internalMarkScenePrePassDirty

• `Private` **\_internalMarkScenePrePassDirty**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:306

___

### \_invertRefractionY

• `Private` **\_invertRefractionY**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:205

___

### \_isRefractionEnabled

• `Private` **\_isRefractionEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:67

___

### \_isScatteringEnabled

• `Private` **\_isScatteringEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:83

___

### \_isTranslucencyEnabled

• `Private` **\_isTranslucencyEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:75

___

### \_material

• `Protected` **\_material**: [`PBRBaseMaterial`](PBRBaseMaterial.md)

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[_material](MaterialPluginBase.md#_material)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:65

___

### \_pluginDefineNames

• `Protected` `Optional` **\_pluginDefineNames**: `Object`

#### Index signature

▪ [name: `string`]: `any`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_pluginDefineNames](MaterialPluginBase.md#_plugindefinenames)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:44

___

### \_pluginManager

• `Protected` **\_pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_pluginManager](MaterialPluginBase.md#_pluginmanager)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:43

___

### \_refractionIntensityTexture

• `Private` **\_refractionIntensityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:274

___

### \_refractionTexture

• `Private` **\_refractionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:158

___

### \_scatteringDiffusionProfileIndex

• `Private` **\_scatteringDiffusionProfileIndex**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:92

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:292

___

### \_thicknessTexture

• `Private` **\_thicknessTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:146

___

### \_translucencyIntensityTexture

• `Private` **\_translucencyIntensityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:283

___

### \_useGltfStyleTextures

• `Private` **\_useGltfStyleTextures**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:293

___

### \_useMaskFromThicknessTexture

• `Private` **\_useMaskFromThicknessTexture**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:263

___

### \_volumeIndexOfRefraction

• `Private` **\_volumeIndexOfRefraction**: `number` = `-1.0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:181

___

### diffusionDistance

• **diffusionDistance**: [`Color3`](Color3.md)

Defines how far each channel transmit through the media.
It is defined as a color to simplify it selection.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:261

___

### indexOfRefraction

• **indexOfRefraction**: `number` = `1.5`

Index of refraction of the material base layer.
https://en.wikipedia.org/wiki/List_of_refractive_indices

This does not only impact refraction but also the Base F0 of Dielectric Materials.

From dielectric fresnel rules: F0 = square((iorT - iorI) / (iorT + iorI))

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:178

___

### invertRefractionY

• **invertRefractionY**: `boolean` = `false`

Controls if refraction needs to be inverted on Y. This could be useful for procedural texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:211

___

### isRefractionEnabled

• **isRefractionEnabled**: `boolean` = `false`

Defines if the refraction is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:73

___

### isScatteringEnabled

• **isScatteringEnabled**: `boolean` = `false`

Defines if the sub surface scattering is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:89

___

### isTranslucencyEnabled

• **isTranslucencyEnabled**: `boolean` = `false`

Defines if the translucency is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:81

___

### linkRefractionWithTransparency

• **linkRefractionWithTransparency**: `boolean` = `false`

This parameters will make the material used its opacity to control how much it is refracting against not.
Materials half opaque for instance using refraction could benefit from this control.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:221

___

### markAllDefinesAsDirty

• `Readonly` **markAllDefinesAsDirty**: () => `void`

#### Type declaration

▸ (): `void`

Helper function to mark defines as being dirty.

##### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[markAllDefinesAsDirty](MaterialPluginBase.md#markalldefinesasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:55

___

### maximumThickness

• **maximumThickness**: `number` = `1`

Defines the maximum thickness stored in the thickness map.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:234

___

### minimumThickness

• **minimumThickness**: `number` = `0`

Defines the minimum thickness stored in the thickness map.
If no thickness map is defined, this value will be used to simulate thickness.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:228

___

### name

• **name**: `string`

Defines the name of the plugin

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[name](MaterialPluginBase.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:28

___

### priority

• **priority**: `number` = `500`

Defines the priority of the plugin. Lower numbers run first.

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[priority](MaterialPluginBase.md#priority)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:34

___

### refractionIntensity

• **refractionIntensity**: `number` = `1`

Defines the refraction intensity of the material.
The refraction when enabled replaces the Diffuse part of the material.
The intensity helps transitioning between diffuse and refraction.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:124

___

### refractionIntensityTexture

• **refractionIntensityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the intensity of the refraction. If provided, it takes precedence over thicknessTexture + useMaskFromThicknessTexture
* the green (red if useGltfStyleTextures = true) channel is the refraction intensity.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:281

___

### refractionTexture

• **refractionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Defines the texture to use for refraction.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:164

___

### registerForExtraEvents

• **registerForExtraEvents**: `boolean` = `false`

Indicates that this plugin should be notified for the extra events (HasRenderTargetTextures / FillRenderTargetTextures / HardBindForSubMesh)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[registerForExtraEvents](MaterialPluginBase.md#registerforextraevents)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:40

___

### thicknessTexture

• **thicknessTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the average thickness of a mesh in a texture (The texture is holding the values linearly).
The red (or green if useGltfStyleTextures=true) channel of the texture should contain the thickness remapped between 0 and 1.
0 would mean minimumThickness
1 would mean maximumThickness
The other channels might be use as a mask to vary the different effects intensity.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:156

___

### tintColor

• **tintColor**: [`Color3`](Color3.md)

Defines the volume tint of the material.
This is used for both translucency and scattering.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:247

___

### tintColorAtDistance

• **tintColorAtDistance**: `number` = `1`

Defines the distance at which the tint color should be found in the media.
This is used for refraction only.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:254

___

### translucencyIntensity

• **translucencyIntensity**: `number` = `1`

Defines the translucency intensity of the material.
When translucency has been enabled, this defines how much of the "translucency"
is added to the diffuse part of the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:132

___

### translucencyIntensityTexture

• **translucencyIntensityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the intensity of the translucency. If provided, it takes precedence over thicknessTexture + useMaskFromThicknessTexture
* the blue channel is the translucency intensity.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:290

___

### useAlbedoToTintRefraction

• **useAlbedoToTintRefraction**: `boolean` = `false`

When enabled, transparent surfaces will be tinted with the albedo colour (independent of thickness)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:138

___

### useAlbedoToTintTranslucency

• **useAlbedoToTintTranslucency**: `boolean` = `false`

When enabled, translucent surfaces will be tinted with the albedo colour (independent of thickness)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:144

___

### useGltfStyleTextures

• **useGltfStyleTextures**: `boolean` = `false`

Use channels layout used by glTF:
* thicknessTexture: the green (instead of red) channel is the thickness
* thicknessTexture/refractionIntensityTexture: the red (instead of green) channel is the refraction intensity
* thicknessTexture/translucencyIntensityTexture: no change, use the blue channel for the translucency intensity

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:302

___

### useMaskFromThicknessTexture

• **useMaskFromThicknessTexture**: `boolean` = `false`

Stores the intensity of the different subsurface effects in the thickness texture.
Note that if refractionIntensityTexture and/or translucencyIntensityTexture is provided it takes precedence over thicknessTexture + useMaskFromThicknessTexture
* the green (red if useGltfStyleTextures = true) channel is the refraction intensity.
* the blue channel is the translucency intensity.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:272

___

### useThicknessAsDepth

• **useThicknessAsDepth**: `boolean` = `false`

Defines that the thickness should be used as a measure of the depth volume.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:240

## Accessors

### disableAlphaBlending

• `get` **disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:592

___

### scatteringDiffusionProfile

• `get` **scatteringDiffusionProfile**(): [`Nullable`](../modules.md#nullable)[`Color3`](Color3.md)

Diffusion profile for subsurface scattering.
Useful for better scattering in the skins or foliages.

#### Returns

[`Nullable`](../modules.md#nullable)[`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:98

• `set` **scatteringDiffusionProfile**(`c`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `c` | [`Nullable`](../modules.md#nullable)[`Color3`](Color3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:106

___

### volumeIndexOfRefraction

• `get` **volumeIndexOfRefraction**(): `number`

Index of refraction of the material's volume.
https://en.wikipedia.org/wiki/List_of_refractive_indices

This ONLY impacts refraction. If not provided or given a non-valid value,
the volume will use the same IOR as the surface.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:190

• `set` **volumeIndexOfRefraction**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:197

## Methods

### \_enable

▸ `Protected` **_enable**(`enable`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enable` | `boolean` |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_enable](MaterialPluginBase.md#_enable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:46

___

### \_getRefractionTexture

▸ `Private` **_getRefractionTexture**(`scene`): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Returns the texture used for refraction or null if none is used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

- Refraction texture if present.  If no refraction texture and refraction
is linked with transparency, returns environment texture.  Otherwise, returns null.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:577

___

### addFallbacks

▸ **addFallbacks**(`defines`, `fallbacks`, `currentRank`): `number`

Add fallbacks to the effect fallbacks list.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSubSurfaceDefines` | defines the Base texture to use. |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current fallback list. |
| `currentRank` | `number` | defines the current fallback rank. |

#### Returns

`number`

the new fallback rank.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[addFallbacks](MaterialPluginBase.md#addfallbacks)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:662

___

### bindForSubMesh

▸ **bindForSubMesh**(`uniformBuffer`, `scene`, `engine`, `subMesh`): `void`

Binds the material data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformBuffer` | [`UniformBuffer`](UniformBuffer.md) | defines the Uniform buffer to fill in. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |
| `engine` | [`Engine`](Engine.md) | the engine this scene belongs to. |
| `subMesh` | [`SubMesh`](SubMesh.md) | the submesh to bind data for |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[bindForSubMesh](MaterialPluginBase.md#bindforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:473

___

### collectDefines

▸ **collectDefines**(`defines`): `void`

Collects all defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `Object` | The object to append to. |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[collectDefines](MaterialPluginBase.md#collectdefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:154

___

### copyTo

▸ **copyTo**(`plugin`): `void`

Makes a duplicate of the current configuration into another one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plugin` | [`MaterialPluginBase`](MaterialPluginBase.md) | define the config where to copy the info |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[copyTo](MaterialPluginBase.md#copyto)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:274

___

### dispose

▸ **dispose**(`forceDisposeTextures?`): `void`

Disposes the resources of the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeTextures?` | `boolean` | Forces the disposal of all textures. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[dispose](MaterialPluginBase.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:646

___

### fillRenderTargetTextures

▸ **fillRenderTargetTextures**(`renderTargets`): `void`

Fills the list of render target textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderTargets` | [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) | the list of render targets to update |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[fillRenderTargetTextures](MaterialPluginBase.md#fillrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:600

___

### getActiveTextures

▸ **getActiveTextures**(`activeTextures`): `void`

Returns an array of the actively used textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeTextures` | [`BaseTexture`](BaseTexture.md)[] | Array of BaseTextures |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[getActiveTextures](MaterialPluginBase.md#getactivetextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:626

___

### getAnimatables

▸ **getAnimatables**(`animatables`): `void`

Returns the animatable textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `animatables` | [`IAnimatable`](../interfaces/IAnimatable.md)[] | Array of animatable textures. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[getAnimatables](MaterialPluginBase.md#getanimatables)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:636

___

### getAttributes

▸ **getAttributes**(`attributes`, `scene`, `mesh`): `void`

Gets the attributes used by the plugin.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attributes` | `string`[] | list that the attribute names should be added to. |
| `scene` | [`Scene`](Scene.md) | the scene that the material belongs to. |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh being rendered. |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[getAttributes](MaterialPluginBase.md#getattributes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:253

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name useful for serialization or dynamic coding.

#### Returns

`string`

The class name.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[getClassName](MaterialPluginBase.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:658

___

### getCustomCode

▸ **getCustomCode**(`shaderType`): [`Nullable`](../modules.md#nullable){ `[pointName: string]`: `string`;  }

Returns a list of custom shader code fragments to customize the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shaderType` | `string` | "vertex" or "fragment" |

#### Returns

[`Nullable`](../modules.md#nullable){ `[pointName: string]`: `string`;  }

null if no code to be added, or a list of pointName => code.
Note that `pointName` can also be a regular expression if it starts with a `!`.
In that case, the string found by the regular expression (if any) will be
replaced by the code provided.

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[getCustomCode](MaterialPluginBase.md#getcustomcode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:146

___

### getSamplers

▸ **getSamplers**(`samplers`): `void`

Gets the samplers used by the plugin.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `samplers` | `string`[] | list that the sampler names should be added to. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[getSamplers](MaterialPluginBase.md#getsamplers)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:672

___

### getUniformBuffersNames

▸ **getUniformBuffersNames**(`ubos`): `void`

Gets the uniform buffers names added by the plugin.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ubos` | `string`[] | list that the ubo names should be added to. |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[getUniformBuffersNames](MaterialPluginBase.md#getuniformbuffersnames)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:260

___

### getUniforms

▸ **getUniforms**(): `Object`

Gets the description of the uniforms to add to the ubo (if engine supports ubos) or to inject directly in the vertex/fragment shaders (if engine does not support ubos)

#### Returns

`Object`

the description of the uniforms

| Name | Type |
| :------ | :------ |
| `fragment?` | `string` |
| `ubo?` | { `name`: `string` ; `size`: `number` ; `type`: `string`  }[] |
| `vertex?` | `string` |

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[getUniforms](MaterialPluginBase.md#getuniforms)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:676

___

### hardBindForSubMesh

▸ **hardBindForSubMesh**(`uniformBuffer`, `scene`, `engine`, `subMesh`): `void`

Binds the material data (this function is called even if mustRebind() returns false)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformBuffer` | [`UniformBuffer`](UniformBuffer.md) | defines the Uniform buffer to fill in. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |
| `engine` | [`Engine`](Engine.md) | defines the engine the material belongs to. |
| `subMesh` | [`SubMesh`](SubMesh.md) | the submesh to bind data for |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[hardBindForSubMesh](MaterialPluginBase.md#hardbindforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:461

___

### hasRenderTargetTextures

▸ **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

true if this uses a render target otherwise false.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[hasRenderTargetTextures](MaterialPluginBase.md#hasrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:618

___

### hasTexture

▸ **hasTexture**(`texture`): `boolean`

Checks to see if a texture is used in the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | Base texture to use. |

#### Returns

`boolean`

- Boolean specifying if a texture is used in the material.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[hasTexture](MaterialPluginBase.md#hastexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:606

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`defines`, `scene`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSubSurfaceDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[isReadyForSubMesh](MaterialPluginBase.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:329

___

### parse

▸ **parse**(`source`, `scene`, `rootUrl`): `void`

Parses a anisotropy Configuration from a serialized object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Serialized object. |
| `scene` | [`Scene`](Scene.md) | Defines the scene we are parsing for |
| `rootUrl` | `string` | Defines the rootUrl to load from |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[parse](MaterialPluginBase.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:292

___

### prepareDefines

▸ **prepareDefines**(`defines`, `scene`, `mesh`): `void`

Sets the defines for the next rendering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh being rendered |

#### Returns

`void`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[prepareDefines](MaterialPluginBase.md#preparedefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:187

___

### prepareDefinesBeforeAttributes

▸ **prepareDefinesBeforeAttributes**(`defines`, `scene`): `void`

Sets the defines for the next rendering. Called before MaterialHelper.PrepareDefinesForAttributes is called.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSubSurfaceDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[prepareDefinesBeforeAttributes](MaterialPluginBase.md#preparedefinesbeforeattributes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrSubSurfaceConfiguration.ts:354

___

### serialize

▸ **serialize**(): `any`

Serializes this clear coat configuration.

#### Returns

`any`

- An object with the serialized config.

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[serialize](MaterialPluginBase.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:282

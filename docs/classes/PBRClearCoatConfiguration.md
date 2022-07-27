[@dev/core](../README.md) / [Exports](../modules.md) / PBRClearCoatConfiguration

# Class: PBRClearCoatConfiguration

Plugin that implements the clear coat component of the PBR material

## Hierarchy

- [`MaterialPluginBase`](MaterialPluginBase.md)

  ↳ **`PBRClearCoatConfiguration`**

## Table of contents

### Constructors

- [constructor](PBRClearCoatConfiguration.md#constructor)

### Properties

- [\_bumpTexture](PBRClearCoatConfiguration.md#_bumptexture)
- [\_indexOfRefraction](PBRClearCoatConfiguration.md#_indexofrefraction)
- [\_isEnabled](PBRClearCoatConfiguration.md#_isenabled)
- [\_isTintEnabled](PBRClearCoatConfiguration.md#_istintenabled)
- [\_material](PBRClearCoatConfiguration.md#_material)
- [\_pluginDefineNames](PBRClearCoatConfiguration.md#_plugindefinenames)
- [\_pluginManager](PBRClearCoatConfiguration.md#_pluginmanager)
- [\_remapF0OnInterfaceChange](PBRClearCoatConfiguration.md#_remapf0oninterfacechange)
- [\_texture](PBRClearCoatConfiguration.md#_texture)
- [\_textureRoughness](PBRClearCoatConfiguration.md#_textureroughness)
- [\_tintTexture](PBRClearCoatConfiguration.md#_tinttexture)
- [\_useRoughnessFromMainTexture](PBRClearCoatConfiguration.md#_useroughnessfrommaintexture)
- [bumpTexture](PBRClearCoatConfiguration.md#bumptexture)
- [indexOfRefraction](PBRClearCoatConfiguration.md#indexofrefraction)
- [intensity](PBRClearCoatConfiguration.md#intensity)
- [isEnabled](PBRClearCoatConfiguration.md#isenabled)
- [isTintEnabled](PBRClearCoatConfiguration.md#istintenabled)
- [markAllDefinesAsDirty](PBRClearCoatConfiguration.md#markalldefinesasdirty)
- [name](PBRClearCoatConfiguration.md#name)
- [priority](PBRClearCoatConfiguration.md#priority)
- [registerForExtraEvents](PBRClearCoatConfiguration.md#registerforextraevents)
- [remapF0OnInterfaceChange](PBRClearCoatConfiguration.md#remapf0oninterfacechange)
- [roughness](PBRClearCoatConfiguration.md#roughness)
- [texture](PBRClearCoatConfiguration.md#texture)
- [textureRoughness](PBRClearCoatConfiguration.md#textureroughness)
- [tintColor](PBRClearCoatConfiguration.md#tintcolor)
- [tintColorAtDistance](PBRClearCoatConfiguration.md#tintcoloratdistance)
- [tintTexture](PBRClearCoatConfiguration.md#tinttexture)
- [tintThickness](PBRClearCoatConfiguration.md#tintthickness)
- [useRoughnessFromMainTexture](PBRClearCoatConfiguration.md#useroughnessfrommaintexture)

### Methods

- [\_enable](PBRClearCoatConfiguration.md#_enable)
- [addFallbacks](PBRClearCoatConfiguration.md#addfallbacks)
- [bindForSubMesh](PBRClearCoatConfiguration.md#bindforsubmesh)
- [collectDefines](PBRClearCoatConfiguration.md#collectdefines)
- [copyTo](PBRClearCoatConfiguration.md#copyto)
- [dispose](PBRClearCoatConfiguration.md#dispose)
- [fillRenderTargetTextures](PBRClearCoatConfiguration.md#fillrendertargettextures)
- [getActiveTextures](PBRClearCoatConfiguration.md#getactivetextures)
- [getAnimatables](PBRClearCoatConfiguration.md#getanimatables)
- [getAttributes](PBRClearCoatConfiguration.md#getattributes)
- [getClassName](PBRClearCoatConfiguration.md#getclassname)
- [getCustomCode](PBRClearCoatConfiguration.md#getcustomcode)
- [getSamplers](PBRClearCoatConfiguration.md#getsamplers)
- [getUniformBuffersNames](PBRClearCoatConfiguration.md#getuniformbuffersnames)
- [getUniforms](PBRClearCoatConfiguration.md#getuniforms)
- [hardBindForSubMesh](PBRClearCoatConfiguration.md#hardbindforsubmesh)
- [hasRenderTargetTextures](PBRClearCoatConfiguration.md#hasrendertargettextures)
- [hasTexture](PBRClearCoatConfiguration.md#hastexture)
- [isReadyForSubMesh](PBRClearCoatConfiguration.md#isreadyforsubmesh)
- [parse](PBRClearCoatConfiguration.md#parse)
- [prepareDefines](PBRClearCoatConfiguration.md#preparedefines)
- [prepareDefinesBeforeAttributes](PBRClearCoatConfiguration.md#preparedefinesbeforeattributes)
- [serialize](PBRClearCoatConfiguration.md#serialize)

## Constructors

### constructor

• **new PBRClearCoatConfiguration**(`material`, `addToPluginList?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `material` | [`PBRBaseMaterial`](PBRBaseMaterial.md) | `undefined` |
| `addToPluginList` | `boolean` | `true` |

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[constructor](MaterialPluginBase.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:179

## Properties

### \_bumpTexture

• `Private` **\_bumpTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:122

___

### \_indexOfRefraction

• `Private` **\_indexOfRefraction**: `number` = `PBRClearCoatConfiguration._DefaultIndexOfRefraction`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:75

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:55

___

### \_isTintEnabled

• `Private` **\_isTintEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:130

___

### \_material

• `Protected` **\_material**: [`PBRBaseMaterial`](PBRBaseMaterial.md)

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[_material](MaterialPluginBase.md#_material)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:46

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

### \_remapF0OnInterfaceChange

• `Private` **\_remapF0OnInterfaceChange**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:114

___

### \_texture

• `Private` **\_texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:86

___

### \_textureRoughness

• `Private` **\_textureRoughness**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:105

___

### \_tintTexture

• `Private` **\_tintTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:160

___

### \_useRoughnessFromMainTexture

• `Private` **\_useRoughnessFromMainTexture**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:96

___

### bumpTexture

• **bumpTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Define the clear coat specific bump texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:128

___

### indexOfRefraction

• **indexOfRefraction**: `number` = `PBRClearCoatConfiguration._DefaultIndexOfRefraction`

Defines the index of refraction of the clear coat.
This defaults to 1.5 corresponding to a 0.04 f0 or a 4% reflectance at normal incidence
The default fits with a polyurethane material.
Changing the default value is more performance intensive.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:84

___

### intensity

• **intensity**: `number` = `1`

Defines the clear coat layer strength (between 0 and 1) it defaults to 1.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:67

___

### isEnabled

• **isEnabled**: `boolean` = `false`

Defines if the clear coat is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:61

___

### isTintEnabled

• **isTintEnabled**: `boolean` = `false`

Defines if the clear coat tint is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:136

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

### registerForExtraEvents

• **registerForExtraEvents**: `boolean` = `false`

Indicates that this plugin should be notified for the extra events (HasRenderTargetTextures / FillRenderTargetTextures / HardBindForSubMesh)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[registerForExtraEvents](MaterialPluginBase.md#registerforextraevents)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:40

___

### remapF0OnInterfaceChange

• **remapF0OnInterfaceChange**: `boolean` = `true`

Defines if the F0 value should be remapped to account for the interface change in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:120

___

### roughness

• **roughness**: `number` = `0`

Defines the clear coat layer roughness.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:73

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the clear coat values in a texture (red channel is intensity and green channel is roughness)
If useRoughnessFromMainTexture is false, the green channel of texture is not used and the green channel of textureRoughness is used instead
if textureRoughness is not empty, else no texture roughness is used

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:94

___

### textureRoughness

• **textureRoughness**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the clear coat roughness in a texture (green channel)
Not used if useRoughnessFromMainTexture is true

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:112

___

### tintColor

• **tintColor**: [`Color3`](Color3.md)

Defines the clear coat tint of the material.
This is only use if tint is enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:143

___

### tintColorAtDistance

• **tintColorAtDistance**: `number` = `1`

Defines the distance at which the tint color should be found in the
clear coat media.
This is only use if tint is enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:151

___

### tintTexture

• **tintTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the clear tint values in a texture.
rgb is tint
a is a thickness factor

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:168

___

### tintThickness

• **tintThickness**: `number` = `1`

Defines the clear coat layer thickness.
This is only use if tint is enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:158

___

### useRoughnessFromMainTexture

• **useRoughnessFromMainTexture**: `boolean` = `true`

Indicates that the green channel of the texture property will be used for roughness (default: true)
If false, the green channel from textureRoughness is used for roughness

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:103

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

### addFallbacks

▸ **addFallbacks**(`defines`, `fallbacks`, `currentRank`): `number`

Add fallbacks to the effect fallbacks list.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialClearCoatDefines` | defines the Base texture to use. |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current fallback list. |
| `currentRank` | `number` | defines the current fallback rank. |

#### Returns

`number`

the new fallback rank.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[addFallbacks](MaterialPluginBase.md#addfallbacks)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:435

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:279

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:422

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

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[fillRenderTargetTextures](MaterialPluginBase.md#fillrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:212

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:386

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:404

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:431

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:448

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:452

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

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[hardBindForSubMesh](MaterialPluginBase.md#hardbindforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:118

___

### hasRenderTargetTextures

▸ **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

true if this uses a render target otherwise false.

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[hasRenderTargetTextures](MaterialPluginBase.md#hasrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:203

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:366

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`defines`, `scene`, `engine`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialClearCoatDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |
| `engine` | [`Engine`](Engine.md) | the engine this scene belongs to. |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[isReadyForSubMesh](MaterialPluginBase.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:185

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
| `defines` | `MaterialClearCoatDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[prepareDefinesBeforeAttributes](MaterialPluginBase.md#preparedefinesbeforeattributes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrClearCoatConfiguration.ts:223

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

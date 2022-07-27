[@dev/core](../README.md) / [Exports](../modules.md) / PBRSheenConfiguration

# Class: PBRSheenConfiguration

Plugin that implements the sheen component of the PBR material.

## Hierarchy

- [`MaterialPluginBase`](MaterialPluginBase.md)

  ↳ **`PBRSheenConfiguration`**

## Table of contents

### Constructors

- [constructor](PBRSheenConfiguration.md#constructor)

### Properties

- [\_albedoScaling](PBRSheenConfiguration.md#_albedoscaling)
- [\_isEnabled](PBRSheenConfiguration.md#_isenabled)
- [\_linkSheenWithAlbedo](PBRSheenConfiguration.md#_linksheenwithalbedo)
- [\_material](PBRSheenConfiguration.md#_material)
- [\_pluginDefineNames](PBRSheenConfiguration.md#_plugindefinenames)
- [\_pluginManager](PBRSheenConfiguration.md#_pluginmanager)
- [\_roughness](PBRSheenConfiguration.md#_roughness)
- [\_texture](PBRSheenConfiguration.md#_texture)
- [\_textureRoughness](PBRSheenConfiguration.md#_textureroughness)
- [\_useRoughnessFromMainTexture](PBRSheenConfiguration.md#_useroughnessfrommaintexture)
- [albedoScaling](PBRSheenConfiguration.md#albedoscaling)
- [color](PBRSheenConfiguration.md#color)
- [intensity](PBRSheenConfiguration.md#intensity)
- [isEnabled](PBRSheenConfiguration.md#isenabled)
- [linkSheenWithAlbedo](PBRSheenConfiguration.md#linksheenwithalbedo)
- [markAllDefinesAsDirty](PBRSheenConfiguration.md#markalldefinesasdirty)
- [name](PBRSheenConfiguration.md#name)
- [priority](PBRSheenConfiguration.md#priority)
- [registerForExtraEvents](PBRSheenConfiguration.md#registerforextraevents)
- [roughness](PBRSheenConfiguration.md#roughness)
- [texture](PBRSheenConfiguration.md#texture)
- [textureRoughness](PBRSheenConfiguration.md#textureroughness)
- [useRoughnessFromMainTexture](PBRSheenConfiguration.md#useroughnessfrommaintexture)

### Methods

- [\_enable](PBRSheenConfiguration.md#_enable)
- [addFallbacks](PBRSheenConfiguration.md#addfallbacks)
- [bindForSubMesh](PBRSheenConfiguration.md#bindforsubmesh)
- [collectDefines](PBRSheenConfiguration.md#collectdefines)
- [copyTo](PBRSheenConfiguration.md#copyto)
- [dispose](PBRSheenConfiguration.md#dispose)
- [fillRenderTargetTextures](PBRSheenConfiguration.md#fillrendertargettextures)
- [getActiveTextures](PBRSheenConfiguration.md#getactivetextures)
- [getAnimatables](PBRSheenConfiguration.md#getanimatables)
- [getAttributes](PBRSheenConfiguration.md#getattributes)
- [getClassName](PBRSheenConfiguration.md#getclassname)
- [getCustomCode](PBRSheenConfiguration.md#getcustomcode)
- [getSamplers](PBRSheenConfiguration.md#getsamplers)
- [getUniformBuffersNames](PBRSheenConfiguration.md#getuniformbuffersnames)
- [getUniforms](PBRSheenConfiguration.md#getuniforms)
- [hardBindForSubMesh](PBRSheenConfiguration.md#hardbindforsubmesh)
- [hasRenderTargetTextures](PBRSheenConfiguration.md#hasrendertargettextures)
- [hasTexture](PBRSheenConfiguration.md#hastexture)
- [isReadyForSubMesh](PBRSheenConfiguration.md#isreadyforsubmesh)
- [parse](PBRSheenConfiguration.md#parse)
- [prepareDefines](PBRSheenConfiguration.md#preparedefines)
- [prepareDefinesBeforeAttributes](PBRSheenConfiguration.md#preparedefinesbeforeattributes)
- [serialize](PBRSheenConfiguration.md#serialize)

## Constructors

### constructor

• **new PBRSheenConfiguration**(`material`, `addToPluginList?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `material` | [`PBRBaseMaterial`](PBRBaseMaterial.md) | `undefined` |
| `addToPluginList` | `boolean` | `true` |

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[constructor](MaterialPluginBase.md#constructor)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:127

## Properties

### \_albedoScaling

• `Private` **\_albedoScaling**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:108

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:41

___

### \_linkSheenWithAlbedo

• `Private` **\_linkSheenWithAlbedo**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:49

___

### \_material

• `Protected` **\_material**: [`Material`](Material.md)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_material](MaterialPluginBase.md#_material)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:42

___

### \_pluginDefineNames

• `Protected` `Optional` **\_pluginDefineNames**: `Object`

#### Index signature

▪ [name: `string`]: `any`

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_pluginDefineNames](MaterialPluginBase.md#_plugindefinenames)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:44

___

### \_pluginManager

• `Protected` **\_pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[_pluginManager](MaterialPluginBase.md#_pluginmanager)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:43

___

### \_roughness

• `Private` **\_roughness**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:89

___

### \_texture

• `Private` **\_texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:69

___

### \_textureRoughness

• `Private` **\_textureRoughness**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:99

___

### \_useRoughnessFromMainTexture

• `Private` **\_useRoughnessFromMainTexture**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:80

___

### albedoScaling

• **albedoScaling**: `boolean` = `false`

If true, the sheen effect is layered above the base BRDF with the albedo-scaling technique.
It allows the strength of the sheen effect to not depend on the base color of the material,
making it easier to setup and tweak the effect

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:116

___

### color

• **color**: [`Color3`](Color3.md)

Defines the sheen color.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:67

___

### intensity

• **intensity**: `number` = `1`

Defines the sheen intensity.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:61

___

### isEnabled

• **isEnabled**: `boolean` = `false`

Defines if the material uses sheen.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:47

___

### linkSheenWithAlbedo

• **linkSheenWithAlbedo**: `boolean` = `false`

Defines if the sheen is linked to the sheen color.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:55

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

packages/dev/core/src/Materials/materialPluginBase.ts:55

___

### name

• **name**: `string`

Defines the name of the plugin

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[name](MaterialPluginBase.md#name)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:28

___

### priority

• **priority**: `number` = `500`

Defines the priority of the plugin. Lower numbers run first.

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[priority](MaterialPluginBase.md#priority)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:34

___

### registerForExtraEvents

• **registerForExtraEvents**: `boolean` = `false`

Indicates that this plugin should be notified for the extra events (HasRenderTargetTextures / FillRenderTargetTextures / HardBindForSubMesh)

#### Inherited from

[MaterialPluginBase](MaterialPluginBase.md).[registerForExtraEvents](MaterialPluginBase.md#registerforextraevents)

#### Defined in

packages/dev/core/src/Materials/materialPluginBase.ts:40

___

### roughness

• **roughness**: [`Nullable`](../modules.md#nullable)`number` = `null`

Defines the sheen roughness.
It is not taken into account if linkSheenWithAlbedo is true.
To stay backward compatible, material roughness is used instead if sheen roughness = null

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:97

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the sheen tint values in a texture.
rgb is tint
a is a intensity or roughness if the roughness property has been defined and useRoughnessFromTexture is true (in that case, textureRoughness won't be used)
If the roughness property has been defined and useRoughnessFromTexture is false then the alpha channel is not used to modulate roughness

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:78

___

### textureRoughness

• **textureRoughness**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the sheen roughness in a texture.
alpha channel is the roughness. This texture won't be used if the texture property is not empty and useRoughnessFromTexture is true

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:106

___

### useRoughnessFromMainTexture

• **useRoughnessFromMainTexture**: `boolean` = `true`

Indicates that the alpha channel of the texture property will be used for roughness.
Has no effect if the roughness (and texture!) property is not defined

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:87

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

packages/dev/core/src/Materials/materialPluginBase.ts:46

___

### addFallbacks

▸ **addFallbacks**(`defines`, `fallbacks`, `currentRank`): `number`

Add fallbacks to the effect fallbacks list.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSheenDefines` | defines the Base texture to use. |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current fallback list. |
| `currentRank` | `number` | defines the current fallback rank. |

#### Returns

`number`

the new fallback rank.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[addFallbacks](MaterialPluginBase.md#addfallbacks)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:289

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:195

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

packages/dev/core/src/Materials/materialPluginBase.ts:154

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

packages/dev/core/src/Materials/materialPluginBase.ts:274

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:278

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

packages/dev/core/src/Materials/materialPluginBase.ts:212

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:258

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:268

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

packages/dev/core/src/Materials/materialPluginBase.ts:253

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:285

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

packages/dev/core/src/Materials/materialPluginBase.ts:146

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:296

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

packages/dev/core/src/Materials/materialPluginBase.ts:260

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:300

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

packages/dev/core/src/Materials/materialPluginBase.ts:118

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

packages/dev/core/src/Materials/materialPluginBase.ts:203

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

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:246

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`defines`, `scene`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSheenDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[isReadyForSubMesh](MaterialPluginBase.md#isreadyforsubmesh)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:133

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

packages/dev/core/src/Materials/materialPluginBase.ts:292

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

packages/dev/core/src/Materials/materialPluginBase.ts:187

___

### prepareDefinesBeforeAttributes

▸ **prepareDefinesBeforeAttributes**(`defines`, `scene`): `void`

Sets the defines for the next rendering. Called before MaterialHelper.PrepareDefinesForAttributes is called.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialSheenDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[prepareDefinesBeforeAttributes](MaterialPluginBase.md#preparedefinesbeforeattributes)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSheenConfiguration.ts:157

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

packages/dev/core/src/Materials/materialPluginBase.ts:282

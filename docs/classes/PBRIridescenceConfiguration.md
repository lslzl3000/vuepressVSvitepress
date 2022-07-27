[@dev/core](../README.md) / [Exports](../modules.md) / PBRIridescenceConfiguration

# Class: PBRIridescenceConfiguration

Plugin that implements the iridescence (thin film) component of the PBR material

## Hierarchy

- [`MaterialPluginBase`](MaterialPluginBase.md)

  ↳ **`PBRIridescenceConfiguration`**

## Table of contents

### Constructors

- [constructor](PBRIridescenceConfiguration.md#constructor)

### Properties

- [\_isEnabled](PBRIridescenceConfiguration.md#_isenabled)
- [\_material](PBRIridescenceConfiguration.md#_material)
- [\_pluginDefineNames](PBRIridescenceConfiguration.md#_plugindefinenames)
- [\_pluginManager](PBRIridescenceConfiguration.md#_pluginmanager)
- [\_texture](PBRIridescenceConfiguration.md#_texture)
- [\_thicknessTexture](PBRIridescenceConfiguration.md#_thicknesstexture)
- [indexOfRefraction](PBRIridescenceConfiguration.md#indexofrefraction)
- [intensity](PBRIridescenceConfiguration.md#intensity)
- [isEnabled](PBRIridescenceConfiguration.md#isenabled)
- [markAllDefinesAsDirty](PBRIridescenceConfiguration.md#markalldefinesasdirty)
- [maximumThickness](PBRIridescenceConfiguration.md#maximumthickness)
- [minimumThickness](PBRIridescenceConfiguration.md#minimumthickness)
- [name](PBRIridescenceConfiguration.md#name)
- [priority](PBRIridescenceConfiguration.md#priority)
- [registerForExtraEvents](PBRIridescenceConfiguration.md#registerforextraevents)
- [texture](PBRIridescenceConfiguration.md#texture)
- [thicknessTexture](PBRIridescenceConfiguration.md#thicknesstexture)

### Methods

- [\_enable](PBRIridescenceConfiguration.md#_enable)
- [addFallbacks](PBRIridescenceConfiguration.md#addfallbacks)
- [bindForSubMesh](PBRIridescenceConfiguration.md#bindforsubmesh)
- [collectDefines](PBRIridescenceConfiguration.md#collectdefines)
- [copyTo](PBRIridescenceConfiguration.md#copyto)
- [dispose](PBRIridescenceConfiguration.md#dispose)
- [fillRenderTargetTextures](PBRIridescenceConfiguration.md#fillrendertargettextures)
- [getActiveTextures](PBRIridescenceConfiguration.md#getactivetextures)
- [getAnimatables](PBRIridescenceConfiguration.md#getanimatables)
- [getAttributes](PBRIridescenceConfiguration.md#getattributes)
- [getClassName](PBRIridescenceConfiguration.md#getclassname)
- [getCustomCode](PBRIridescenceConfiguration.md#getcustomcode)
- [getSamplers](PBRIridescenceConfiguration.md#getsamplers)
- [getUniformBuffersNames](PBRIridescenceConfiguration.md#getuniformbuffersnames)
- [getUniforms](PBRIridescenceConfiguration.md#getuniforms)
- [hardBindForSubMesh](PBRIridescenceConfiguration.md#hardbindforsubmesh)
- [hasRenderTargetTextures](PBRIridescenceConfiguration.md#hasrendertargettextures)
- [hasTexture](PBRIridescenceConfiguration.md#hastexture)
- [isReadyForSubMesh](PBRIridescenceConfiguration.md#isreadyforsubmesh)
- [parse](PBRIridescenceConfiguration.md#parse)
- [prepareDefines](PBRIridescenceConfiguration.md#preparedefines)
- [prepareDefinesBeforeAttributes](PBRIridescenceConfiguration.md#preparedefinesbeforeattributes)
- [serialize](PBRIridescenceConfiguration.md#serialize)

## Constructors

### constructor

• **new PBRIridescenceConfiguration**(`material`, `addToPluginList?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `material` | [`PBRBaseMaterial`](PBRBaseMaterial.md) | `undefined` |
| `addToPluginList` | `boolean` | `true` |

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[constructor](MaterialPluginBase.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:115

## Properties

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:58

___

### \_material

• `Protected` **\_material**: [`PBRBaseMaterial`](PBRBaseMaterial.md)

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[_material](MaterialPluginBase.md#_material)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:35

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

### \_texture

• `Private` **\_texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:90

___

### \_thicknessTexture

• `Private` **\_thicknessTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:98

___

### indexOfRefraction

• **indexOfRefraction**: `number` = `PBRIridescenceConfiguration._DefaultIndexOfRefraction`

Defines the maximum thickness of the thin-film layer given in nanometers (nm).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:88

___

### intensity

• **intensity**: `number` = `1`

Defines the iridescence layer strength (between 0 and 1) it defaults to 1.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:70

___

### isEnabled

• **isEnabled**: `boolean` = `false`

Defines if the iridescence is enabled in the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:64

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

• **maximumThickness**: `number` = `PBRIridescenceConfiguration._DefaultMaximumThickness`

Defines the maximum thickness of the thin-film layer given in nanometers (nm). This will be the thickness used if not thickness texture has been set.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:82

___

### minimumThickness

• **minimumThickness**: `number` = `PBRIridescenceConfiguration._DefaultMinimumThickness`

Defines the minimum thickness of the thin-film layer given in nanometers (nm).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:76

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

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the iridescence intensity in a texture (red channel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:96

___

### thicknessTexture

• **thicknessTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Stores the iridescence thickness in a texture (green channel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:104

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
| `defines` | `MaterialIridescenceDefines` | defines the Base texture to use. |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current fallback list. |
| `currentRank` | `number` | defines the current fallback rank. |

#### Returns

`number`

the new fallback rank.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[addFallbacks](MaterialPluginBase.md#addfallbacks)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:264

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:174

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:253

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:233

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:243

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:260

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:271

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:275

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:221

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`defines`, `scene`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `MaterialIridescenceDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[isReadyForSubMesh](MaterialPluginBase.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:121

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
| `defines` | `MaterialIridescenceDefines` | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |

#### Returns

`void`

#### Overrides

[MaterialPluginBase](MaterialPluginBase.md).[prepareDefinesBeforeAttributes](MaterialPluginBase.md#preparedefinesbeforeattributes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrIridescenceConfiguration.ts:145

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

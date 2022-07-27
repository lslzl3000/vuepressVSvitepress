[@dev/core](../README.md) / [Exports](../modules.md) / MaterialPluginBase

# Class: MaterialPluginBase

Base class for material plugins.

**`Since`**

5.0

## Hierarchy

- **`MaterialPluginBase`**

  ↳ [`PBRAnisotropicConfiguration`](PBRAnisotropicConfiguration.md)

  ↳ [`PBRClearCoatConfiguration`](PBRClearCoatConfiguration.md)

  ↳ [`PBRIridescenceConfiguration`](PBRIridescenceConfiguration.md)

  ↳ [`PBRSheenConfiguration`](PBRSheenConfiguration.md)

  ↳ [`PBRSubSurfaceConfiguration`](PBRSubSurfaceConfiguration.md)

  ↳ [`DetailMapConfiguration`](DetailMapConfiguration.md)

## Table of contents

### Constructors

- [constructor](MaterialPluginBase.md#constructor)

### Properties

- [\_material](MaterialPluginBase.md#_material)
- [\_pluginDefineNames](MaterialPluginBase.md#_plugindefinenames)
- [\_pluginManager](MaterialPluginBase.md#_pluginmanager)
- [markAllDefinesAsDirty](MaterialPluginBase.md#markalldefinesasdirty)
- [name](MaterialPluginBase.md#name)
- [priority](MaterialPluginBase.md#priority)
- [registerForExtraEvents](MaterialPluginBase.md#registerforextraevents)

### Methods

- [\_enable](MaterialPluginBase.md#_enable)
- [addFallbacks](MaterialPluginBase.md#addfallbacks)
- [bindForSubMesh](MaterialPluginBase.md#bindforsubmesh)
- [collectDefines](MaterialPluginBase.md#collectdefines)
- [copyTo](MaterialPluginBase.md#copyto)
- [dispose](MaterialPluginBase.md#dispose)
- [fillRenderTargetTextures](MaterialPluginBase.md#fillrendertargettextures)
- [getActiveTextures](MaterialPluginBase.md#getactivetextures)
- [getAnimatables](MaterialPluginBase.md#getanimatables)
- [getAttributes](MaterialPluginBase.md#getattributes)
- [getClassName](MaterialPluginBase.md#getclassname)
- [getCustomCode](MaterialPluginBase.md#getcustomcode)
- [getSamplers](MaterialPluginBase.md#getsamplers)
- [getUniformBuffersNames](MaterialPluginBase.md#getuniformbuffersnames)
- [getUniforms](MaterialPluginBase.md#getuniforms)
- [hardBindForSubMesh](MaterialPluginBase.md#hardbindforsubmesh)
- [hasRenderTargetTextures](MaterialPluginBase.md#hasrendertargettextures)
- [hasTexture](MaterialPluginBase.md#hastexture)
- [isReadyForSubMesh](MaterialPluginBase.md#isreadyforsubmesh)
- [parse](MaterialPluginBase.md#parse)
- [prepareDefines](MaterialPluginBase.md#preparedefines)
- [prepareDefinesBeforeAttributes](MaterialPluginBase.md#preparedefinesbeforeattributes)
- [serialize](MaterialPluginBase.md#serialize)

## Constructors

### constructor

• **new MaterialPluginBase**(`material`, `name`, `priority`, `defines?`, `addToPluginList?`, `enable?`)

Creates a new material plugin

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `material` | [`Material`](Material.md) | `undefined` | parent material of the plugin |
| `name` | `string` | `undefined` | name of the plugin |
| `priority` | `number` | `undefined` | priority of the plugin |
| `defines?` | `Object` | `undefined` | list of defines used by the plugin. The value of the property is the default value for this property |
| `addToPluginList` | `boolean` | `true` | true to add the plugin to the list of plugins managed by the material plugin manager of the material (default: true) |
| `enable` | `boolean` | `false` | true to enable the plugin (it is handy if the plugin does not handle properties to switch its current activation) |

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:66

## Properties

### \_material

• `Protected` **\_material**: [`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:42

___

### \_pluginDefineNames

• `Protected` `Optional` **\_pluginDefineNames**: `Object`

#### Index signature

▪ [name: `string`]: `any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:44

___

### \_pluginManager

• `Protected` **\_pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:43

___

### markAllDefinesAsDirty

• `Readonly` **markAllDefinesAsDirty**: () => `void`

#### Type declaration

▸ (): `void`

Helper function to mark defines as being dirty.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:55

___

### name

• **name**: `string`

Defines the name of the plugin

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:28

___

### priority

• **priority**: `number` = `500`

Defines the priority of the plugin. Lower numbers run first.

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:34

___

### registerForExtraEvents

• **registerForExtraEvents**: `boolean` = `false`

Indicates that this plugin should be notified for the extra events (HasRenderTargetTextures / FillRenderTargetTextures / HardBindForSubMesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:40

## Methods

### \_enable

▸ `Protected` **_enable**(`enable`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enable` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:46

___

### addFallbacks

▸ **addFallbacks**(`defines`, `fallbacks`, `currentRank`): `number`

Add fallbacks to the effect fallbacks list.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) | defines the Base texture to use. |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current fallback list. |
| `currentRank` | `number` | defines the current fallback rank. |

#### Returns

`number`

the new fallback rank.

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:235

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:128

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:135

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:219

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:226

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:253

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name useful for serialization or dynamic coding.

#### Returns

`string`

The class name.

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:93

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:244

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:266

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:118

___

### hasRenderTargetTextures

▸ **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

true if this uses a render target otherwise false.

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:195

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`defines`, `scene`, `engine`, `subMesh`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene the material belongs to. |
| `engine` | [`Engine`](Engine.md) | the engine this scene belongs to. |
| `subMesh` | [`SubMesh`](SubMesh.md) | the submesh to check for readiness |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:106

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:187

___

### prepareDefinesBeforeAttributes

▸ **prepareDefinesBeforeAttributes**(`defines`, `scene`, `mesh`): `void`

Sets the defines for the next rendering. Called before MaterialHelper.PrepareDefinesForAttributes is called.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) | the list of "defines" to update. |
| `scene` | [`Scene`](Scene.md) | defines the scene to the material belongs to. |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh being rendered |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:178

___

### serialize

▸ **serialize**(): `any`

Serializes this clear coat configuration.

#### Returns

`any`

- An object with the serialized config.

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginBase.ts:282

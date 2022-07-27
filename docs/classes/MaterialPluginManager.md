[@dev/core](../README.md) / [Exports](../modules.md) / MaterialPluginManager

# Class: MaterialPluginManager

Class that manages the plugins of a material

**`Since`**

5.0

## Table of contents

### Constructors

- [constructor](MaterialPluginManager.md#constructor)

### Properties

- [\_activePlugins](MaterialPluginManager.md#_activeplugins)
- [\_activePluginsForExtraEvents](MaterialPluginManager.md#_activepluginsforextraevents)
- [\_codeInjectionPoints](MaterialPluginManager.md#_codeinjectionpoints)
- [\_defineNamesFromPlugins](MaterialPluginManager.md#_definenamesfromplugins)
- [\_engine](MaterialPluginManager.md#_engine)
- [\_fragmentDeclaration](MaterialPluginManager.md#_fragmentdeclaration)
- [\_material](MaterialPluginManager.md#_material)
- [\_plugins](MaterialPluginManager.md#_plugins)
- [\_samplerList](MaterialPluginManager.md#_samplerlist)
- [\_scene](MaterialPluginManager.md#_scene)
- [\_uboDeclaration](MaterialPluginManager.md#_ubodeclaration)
- [\_uboList](MaterialPluginManager.md#_ubolist)
- [\_uniformList](MaterialPluginManager.md#_uniformlist)
- [\_vertexDeclaration](MaterialPluginManager.md#_vertexdeclaration)
- [\_MaterialPluginClassToMainDefine](MaterialPluginManager.md#_materialpluginclasstomaindefine)
- [\_MaterialPluginCounter](MaterialPluginManager.md#_materialplugincounter)

### Methods

- [\_collectPointNames](MaterialPluginManager.md#_collectpointnames)
- [\_handlePluginEvent](MaterialPluginManager.md#_handlepluginevent)
- [\_handlePluginEventBindForSubMesh](MaterialPluginManager.md#_handleplugineventbindforsubmesh)
- [\_handlePluginEventFillRenderTargetTextures](MaterialPluginManager.md#_handleplugineventfillrendertargettextures)
- [\_handlePluginEventHardBindForSubMesh](MaterialPluginManager.md#_handleplugineventhardbindforsubmesh)
- [\_handlePluginEventHasRenderTargetTextures](MaterialPluginManager.md#_handleplugineventhasrendertargettextures)
- [\_handlePluginEventIsReadyForSubMesh](MaterialPluginManager.md#_handleplugineventisreadyforsubmesh)
- [\_handlePluginEventPrepareDefines](MaterialPluginManager.md#_handleplugineventpreparedefines)
- [\_handlePluginEventPrepareDefinesBeforeAttributes](MaterialPluginManager.md#_handleplugineventpreparedefinesbeforeattributes)
- [\_injectCustomCode](MaterialPluginManager.md#_injectcustomcode)
- [getPlugin](MaterialPluginManager.md#getplugin)

## Constructors

### constructor

• **new MaterialPluginManager**(`material`)

Creates a new instance of the plugin manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `material` | [`Material`](Material.md) | material that this manager will manage the plugins for |

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:62

## Properties

### \_activePlugins

• `Protected` **\_activePlugins**: [`MaterialPluginBase`](MaterialPluginBase.md)[] = `[]`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:47

___

### \_activePluginsForExtraEvents

• `Protected` **\_activePluginsForExtraEvents**: [`MaterialPluginBase`](MaterialPluginBase.md)[] = `[]`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:48

___

### \_codeInjectionPoints

• `Protected` **\_codeInjectionPoints**: `Object`

#### Index signature

▪ [shaderType: `string`]: { `[codeName: string]`: `boolean`;  }

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:49

___

### \_defineNamesFromPlugins

• `Protected` `Optional` **\_defineNamesFromPlugins**: `Object`

#### Index signature

▪ [name: `string`]: { `default`: `any` ; `type`: `string`  }

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:50

___

### \_engine

• `Protected` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:45

___

### \_fragmentDeclaration

• `Protected` **\_fragmentDeclaration**: `string`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:53

___

### \_material

• `Protected` **\_material**: [`Material`](Material.md)

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:43

___

### \_plugins

• `Protected` **\_plugins**: [`MaterialPluginBase`](MaterialPluginBase.md)[] = `[]`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:46

___

### \_samplerList

• `Protected` **\_samplerList**: `string`[]

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:55

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:44

___

### \_uboDeclaration

• `Protected` **\_uboDeclaration**: `string`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:51

___

### \_uboList

• `Protected` **\_uboList**: `string`[]

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:56

___

### \_uniformList

• `Protected` **\_uniformList**: `string`[]

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:54

___

### \_vertexDeclaration

• `Protected` **\_vertexDeclaration**: `string`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:52

___

### \_MaterialPluginClassToMainDefine

▪ `Static` `Private` **\_MaterialPluginClassToMainDefine**: `Object` = `{}`

Map a plugin class name to a #define name (used in the vertex/fragment shaders as a marker of the plugin usage)

#### Index signature

▪ [name: `string`]: `string`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:40

___

### \_MaterialPluginCounter

▪ `Static` `Private` **\_MaterialPluginCounter**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:41

## Methods

### \_collectPointNames

▸ `Protected` **_collectPointNames**(`shaderType`, `customCode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `shaderType` | `string` |
| `customCode` | `undefined` \| [`Nullable`](../modules.md#nullable){ `[pointName: string]`: `string`;  } |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:304

___

### \_handlePluginEvent

▸ `Protected` **_handlePluginEvent**(`id`, `info`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `number` |
| `info` | `MaterialPluginDisposed` \| `MaterialPluginHasTexture` \| `MaterialPluginGetDefineNames` \| `MaterialPluginPrepareEffect` \| `MaterialPluginPrepareUniformBuffer` \| `MaterialPluginGetAnimatables` \| `MaterialPluginGetActiveTextures` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:197

___

### \_handlePluginEventBindForSubMesh

▸ `Protected` **_handlePluginEventBindForSubMesh**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginBindForSubMesh` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:174

___

### \_handlePluginEventFillRenderTargetTextures

▸ `Protected` **_handlePluginEventFillRenderTargetTextures**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginFillRenderTargetTextures` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:191

___

### \_handlePluginEventHardBindForSubMesh

▸ `Protected` **_handlePluginEventHardBindForSubMesh**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginHardBindForSubMesh` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:168

___

### \_handlePluginEventHasRenderTargetTextures

▸ `Protected` **_handlePluginEventHasRenderTargetTextures**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginHasRenderTargetTextures` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:180

___

### \_handlePluginEventIsReadyForSubMesh

▸ `Protected` **_handlePluginEventIsReadyForSubMesh**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginIsReadyForSubMesh` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:148

___

### \_handlePluginEventPrepareDefines

▸ `Protected` **_handlePluginEventPrepareDefines**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginPrepareDefines` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:162

___

### \_handlePluginEventPrepareDefinesBeforeAttributes

▸ `Protected` **_handlePluginEventPrepareDefinesBeforeAttributes**(`eventData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventData` | `MaterialPluginPrepareDefines` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:156

___

### \_injectCustomCode

▸ `Protected` **_injectCustomCode**(`existingCallback?`): `ShaderCustomProcessingFunction`

#### Parameters

| Name | Type |
| :------ | :------ |
| `existingCallback?` | (`shaderType`: `string`, `code`: `string`) => `string` |

#### Returns

`ShaderCustomProcessingFunction`

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:316

___

### getPlugin

▸ **getPlugin**(`name`): [`Nullable`](../modules.md#nullable)[`MaterialPluginBase`](MaterialPluginBase.md)

Gets a plugin from the list of plugins managed by this manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | name of the plugin |

#### Returns

[`Nullable`](../modules.md#nullable)[`MaterialPluginBase`](MaterialPluginBase.md)

the plugin if found, else null

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:139

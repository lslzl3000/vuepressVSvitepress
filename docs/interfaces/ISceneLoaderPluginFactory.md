[@dev/core](../README.md) / [Exports](../modules.md) / ISceneLoaderPluginFactory

# Interface: ISceneLoaderPluginFactory

Interface used by SceneLoader plugin factory

## Table of contents

### Properties

- [name](ISceneLoaderPluginFactory.md#name)

### Methods

- [canDirectLoad](ISceneLoaderPluginFactory.md#candirectload)
- [createPlugin](ISceneLoaderPluginFactory.md#createplugin)

## Properties

### name

• **name**: `string`

Defines the name of the factory

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:116

## Methods

### canDirectLoad

▸ `Optional` **canDirectLoad**(`data`): `boolean`

The callback that returns true if the data can be directly loaded.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | string containing the file data |

#### Returns

`boolean`

if the data can be loaded directly

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:129

___

### createPlugin

▸ **createPlugin**(): [`ISceneLoaderPlugin`](ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](ISceneLoaderPluginAsync.md)

Function called to create a new plugin

#### Returns

[`ISceneLoaderPlugin`](ISceneLoaderPlugin.md) \| [`ISceneLoaderPluginAsync`](ISceneLoaderPluginAsync.md)

the new plugin

#### Defined in

https://github.com/babylon.js/core/src/Loading/sceneLoader.ts:122

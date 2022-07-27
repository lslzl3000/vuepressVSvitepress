[@dev/core](../README.md) / [Exports](../modules.md) / SceneLoaderFlags

# Class: SceneLoaderFlags

Class used to represent data loading progression

## Table of contents

### Constructors

- [constructor](SceneLoaderFlags.md#constructor)

### Properties

- [\_CleanBoneMatrixWeights](SceneLoaderFlags.md#_cleanbonematrixweights)
- [\_ForceFullSceneLoadingForIncremental](SceneLoaderFlags.md#_forcefullsceneloadingforincremental)
- [\_LoggingLevel](SceneLoaderFlags.md#_logginglevel)
- [\_ShowLoadingScreen](SceneLoaderFlags.md#_showloadingscreen)

### Accessors

- [CleanBoneMatrixWeights](SceneLoaderFlags.md#cleanbonematrixweights)
- [ForceFullSceneLoadingForIncremental](SceneLoaderFlags.md#forcefullsceneloadingforincremental)
- [ShowLoadingScreen](SceneLoaderFlags.md#showloadingscreen)
- [loggingLevel](SceneLoaderFlags.md#logginglevel)

## Constructors

### constructor

• **new SceneLoaderFlags**()

## Properties

### \_CleanBoneMatrixWeights

▪ `Static` `Private` **\_CleanBoneMatrixWeights**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:10

___

### \_ForceFullSceneLoadingForIncremental

▪ `Static` `Private` **\_ForceFullSceneLoadingForIncremental**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:8

___

### \_LoggingLevel

▪ `Static` `Private` **\_LoggingLevel**: `number` = `Constants.SCENELOADER_NO_LOGGING`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:11

___

### \_ShowLoadingScreen

▪ `Static` `Private` **\_ShowLoadingScreen**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:9

## Accessors

### CleanBoneMatrixWeights

• `Static` `get` **CleanBoneMatrixWeights**(): `boolean`

Gets or set a boolean indicating if matrix weights must be cleaned upon loading

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:52

• `Static` `set` **CleanBoneMatrixWeights**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:56

___

### ForceFullSceneLoadingForIncremental

• `Static` `get` **ForceFullSceneLoadingForIncremental**(): `boolean`

Gets or sets a boolean indicating if entire scene must be loaded even if scene contains incremental data

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:16

• `Static` `set` **ForceFullSceneLoadingForIncremental**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:20

___

### ShowLoadingScreen

• `Static` `get` **ShowLoadingScreen**(): `boolean`

Gets or sets a boolean indicating if loading screen must be displayed while loading a scene

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:27

• `Static` `set` **ShowLoadingScreen**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:31

___

### loggingLevel

• `Static` `get` **loggingLevel**(): `number`

Defines the current logging level (while loading the scene)

**`Ignorenaming`**

#### Returns

`number`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:40

• `Static` `set` **loggingLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Loading/sceneLoaderFlags.ts:45

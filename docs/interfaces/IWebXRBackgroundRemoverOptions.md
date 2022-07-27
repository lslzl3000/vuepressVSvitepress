[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRBackgroundRemoverOptions

# Interface: IWebXRBackgroundRemoverOptions

Options interface for the background remover plugin

## Table of contents

### Properties

- [backgroundMeshes](IWebXRBackgroundRemoverOptions.md#backgroundmeshes)
- [environmentHelperRemovalFlags](IWebXRBackgroundRemoverOptions.md#environmenthelperremovalflags)
- [ignoreEnvironmentHelper](IWebXRBackgroundRemoverOptions.md#ignoreenvironmenthelper)

## Properties

### backgroundMeshes

• `Optional` **backgroundMeshes**: [`AbstractMesh`](../classes/AbstractMesh.md)[]

Further background meshes to disable when entering AR

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:14

___

### environmentHelperRemovalFlags

• `Optional` **environmentHelperRemovalFlags**: `Object`

flags to configure the removal of the environment helper.
If not set, the entire background will be removed. If set, flags should be set as well.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `ground?` | `boolean` | Should the ground be removed (default false) |
| `skyBox?` | `boolean` | Should the skybox be removed (default false) |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:19

___

### ignoreEnvironmentHelper

• `Optional` **ignoreEnvironmentHelper**: `boolean`

don't disable the environment helper

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:32

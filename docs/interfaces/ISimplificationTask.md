[@dev/core](../README.md) / [Exports](../modules.md) / ISimplificationTask

# Interface: ISimplificationTask

Interface used to define a simplification task

## Table of contents

### Properties

- [mesh](ISimplificationTask.md#mesh)
- [parallelProcessing](ISimplificationTask.md#parallelprocessing)
- [settings](ISimplificationTask.md#settings)
- [simplificationType](ISimplificationTask.md#simplificationtype)
- [successCallback](ISimplificationTask.md#successcallback)

## Properties

### mesh

• **mesh**: [`Mesh`](../classes/Mesh.md)

Mesh to simplify

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:79

___

### parallelProcessing

• **parallelProcessing**: `boolean`

Defines if parallel processing can be used

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:87

___

### settings

• **settings**: [`ISimplificationSettings`](ISimplificationSettings.md)[]

Array of settings

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:71

___

### simplificationType

• **simplificationType**: [`QUADRATIC`](../enums/SimplificationType.md#quadratic)

Simplification type

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:75

___

### successCallback

• `Optional` **successCallback**: () => `void`

#### Type declaration

▸ (): `void`

Callback called on success

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:83

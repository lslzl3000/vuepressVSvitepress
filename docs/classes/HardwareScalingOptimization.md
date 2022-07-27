[@dev/core](../README.md) / [Exports](../modules.md) / HardwareScalingOptimization

# Class: HardwareScalingOptimization

Defines an optimization used to increase or decrease the rendering resolution

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- [`SceneOptimization`](SceneOptimization.md)

  ↳ **`HardwareScalingOptimization`**

## Table of contents

### Constructors

- [constructor](HardwareScalingOptimization.md#constructor)

### Properties

- [\_currentScale](HardwareScalingOptimization.md#_currentscale)
- [\_directionOffset](HardwareScalingOptimization.md#_directionoffset)
- [maximumScale](HardwareScalingOptimization.md#maximumscale)
- [priority](HardwareScalingOptimization.md#priority)
- [step](HardwareScalingOptimization.md#step)

### Methods

- [apply](HardwareScalingOptimization.md#apply)
- [getDescription](HardwareScalingOptimization.md#getdescription)

## Constructors

### constructor

• **new HardwareScalingOptimization**(`priority?`, `maximumScale?`, `step?`)

Creates the HardwareScalingOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |
| `maximumScale` | `number` | `2` | defines the maximum scale to use (2 by default) |
| `step` | `number` | `0.25` | defines the step to use between two passes (0.5 by default) |

#### Overrides

[SceneOptimization](SceneOptimization.md).[constructor](SceneOptimization.md#constructor)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:131

## Properties

### \_currentScale

• `Private` **\_currentScale**: `number` = `-1`

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:114

___

### \_directionOffset

• `Private` **\_directionOffset**: `number` = `1`

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:115

___

### maximumScale

• **maximumScale**: `number` = `2`

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:139

___

### priority

• **priority**: `number` = `0`

#### Inherited from

[SceneOptimization](SceneOptimization.md).[priority](SceneOptimization.md#priority)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:135

___

### step

• **step**: `number` = `0.25`

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:143

## Methods

### apply

▸ **apply**(`scene`, `optimizer`): `boolean`

This function will be called by the SceneOptimizer when its priority is reached in order to apply the change required by the current optimization

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the current scene where to apply this optimization |
| `optimizer` | [`SceneOptimizer`](SceneOptimizer.md) | defines the current optimizer |

#### Returns

`boolean`

true if everything that can be done was applied

#### Overrides

[SceneOptimization](SceneOptimization.md).[apply](SceneOptimization.md#apply)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:154

___

### getDescription

▸ **getDescription**(): `string`

Gets a string describing the action executed by the current optimization

#### Returns

`string`

description string

#### Overrides

[SceneOptimization](SceneOptimization.md).[getDescription](SceneOptimization.md#getdescription)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:121

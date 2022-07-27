[@dev/core](../README.md) / [Exports](../modules.md) / SceneOptimizerOptions

# Class: SceneOptimizerOptions

Defines a list of options used by SceneOptimizer

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Table of contents

### Constructors

- [constructor](SceneOptimizerOptions.md#constructor)

### Properties

- [optimizations](SceneOptimizerOptions.md#optimizations)
- [targetFrameRate](SceneOptimizerOptions.md#targetframerate)
- [trackerDuration](SceneOptimizerOptions.md#trackerduration)

### Methods

- [addCustomOptimization](SceneOptimizerOptions.md#addcustomoptimization)
- [addOptimization](SceneOptimizerOptions.md#addoptimization)
- [HighDegradationAllowed](SceneOptimizerOptions.md#highdegradationallowed)
- [LowDegradationAllowed](SceneOptimizerOptions.md#lowdegradationallowed)
- [ModerateDegradationAllowed](SceneOptimizerOptions.md#moderatedegradationallowed)

## Constructors

### constructor

• **new SceneOptimizerOptions**(`targetFrameRate?`, `trackerDuration?`)

Creates a new list of options used by SceneOptimizer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `targetFrameRate` | `number` | `60` | defines the target frame rate to reach (60 by default) |
| `trackerDuration` | `number` | `2000` | defines the interval between two checks (2000ms by default) |

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:476

## Properties

### optimizations

• **optimizations**: [`SceneOptimization`](SceneOptimization.md)[]

Gets the list of optimizations to apply

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:469

___

### targetFrameRate

• **targetFrameRate**: `number` = `60`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:480

___

### trackerDuration

• **trackerDuration**: `number` = `2000`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:484

## Methods

### addCustomOptimization

▸ **addCustomOptimization**(`onApply`, `onGetDescription`, `priority?`): [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

Add a new custom optimization

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `onApply` | (`scene`: [`Scene`](Scene.md), `optimizer`: [`SceneOptimizer`](SceneOptimizer.md)) => `boolean` | `undefined` | defines the callback called to apply the custom optimization (true if everything that can be done was applied) |
| `onGetDescription` | () => `string` | `undefined` | defines the callback called to get the description attached with the optimization. |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |

#### Returns

[`SceneOptimizerOptions`](SceneOptimizerOptions.md)

the current SceneOptimizerOptions

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:504

___

### addOptimization

▸ **addOptimization**(`optimization`): [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

Add a new optimization

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `optimization` | [`SceneOptimization`](SceneOptimization.md) | defines the SceneOptimization to add to the list of active optimizations |

#### Returns

[`SceneOptimizerOptions`](SceneOptimizerOptions.md)

the current SceneOptimizerOptions

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:492

___

### HighDegradationAllowed

▸ `Static` **HighDegradationAllowed**(`targetFrameRate?`): [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

Creates a list of pre-defined optimizations aimed to have a big impact on the scene visual

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `targetFrameRate?` | `number` | defines the target frame rate (60 by default) |

#### Returns

[`SceneOptimizerOptions`](SceneOptimizerOptions.md)

a SceneOptimizerOptions object

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:576

___

### LowDegradationAllowed

▸ `Static` **LowDegradationAllowed**(`targetFrameRate?`): [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

Creates a list of pre-defined optimizations aimed to reduce the visual impact on the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `targetFrameRate?` | `number` | defines the target frame rate (60 by default) |

#### Returns

[`SceneOptimizerOptions`](SceneOptimizerOptions.md)

a SceneOptimizerOptions object

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:518

___

### ModerateDegradationAllowed

▸ `Static` **ModerateDegradationAllowed**(`targetFrameRate?`): [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

Creates a list of pre-defined optimizations aimed to have a moderate impact on the scene visual

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `targetFrameRate?` | `number` | defines the target frame rate (60 by default) |

#### Returns

[`SceneOptimizerOptions`](SceneOptimizerOptions.md)

a SceneOptimizerOptions object

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:543

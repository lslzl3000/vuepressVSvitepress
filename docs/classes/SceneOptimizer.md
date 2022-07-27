[@dev/core](../README.md) / [Exports](../modules.md) / SceneOptimizer

# Class: SceneOptimizer

Class used to run optimizations in order to reach a target frame rate

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](SceneOptimizer.md#constructor)

### Properties

- [\_currentFrameRate](SceneOptimizer.md#_currentframerate)
- [\_currentPriorityLevel](SceneOptimizer.md#_currentprioritylevel)
- [\_improvementMode](SceneOptimizer.md#_improvementmode)
- [\_isRunning](SceneOptimizer.md#_isrunning)
- [\_options](SceneOptimizer.md#_options)
- [\_scene](SceneOptimizer.md#_scene)
- [\_sceneDisposeObserver](SceneOptimizer.md#_scenedisposeobserver)
- [\_targetFrameRate](SceneOptimizer.md#_targetframerate)
- [\_trackerDuration](SceneOptimizer.md#_trackerduration)
- [onFailureObservable](SceneOptimizer.md#onfailureobservable)
- [onNewOptimizationAppliedObservable](SceneOptimizer.md#onnewoptimizationappliedobservable)
- [onSuccessObservable](SceneOptimizer.md#onsuccessobservable)

### Accessors

- [currentFrameRate](SceneOptimizer.md#currentframerate)
- [currentPriorityLevel](SceneOptimizer.md#currentprioritylevel)
- [isInImprovementMode](SceneOptimizer.md#isinimprovementmode)
- [optimizations](SceneOptimizer.md#optimizations)
- [targetFrameRate](SceneOptimizer.md#targetframerate)
- [trackerDuration](SceneOptimizer.md#trackerduration)

### Methods

- [\_checkCurrentState](SceneOptimizer.md#_checkcurrentstate)
- [dispose](SceneOptimizer.md#dispose)
- [reset](SceneOptimizer.md#reset)
- [start](SceneOptimizer.md#start)
- [stop](SceneOptimizer.md#stop)
- [OptimizeAsync](SceneOptimizer.md#optimizeasync)

## Constructors

### constructor

• **new SceneOptimizer**(`scene`, `options?`, `autoGeneratePriorities?`, `improvementMode?`)

Creates a new SceneOptimizer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the scene to work on |
| `options?` | [`SceneOptimizerOptions`](SceneOptimizerOptions.md) | `undefined` | defines the options to use with the SceneOptimizer |
| `autoGeneratePriorities` | `boolean` | `true` | defines if priorities must be generated and not read from SceneOptimization property (true by default) |
| `improvementMode` | `boolean` | `false` | defines if the scene optimizer must run the maximum optimization while staying over a target frame instead of trying to reach the target framerate (false by default) |

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:700

## Properties

### \_currentFrameRate

• `Private` **\_currentFrameRate**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:616

___

### \_currentPriorityLevel

• `Private` **\_currentPriorityLevel**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:613

___

### \_improvementMode

• `Private` **\_improvementMode**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:618

___

### \_isRunning

• `Private` **\_isRunning**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:610

___

### \_options

• `Private` **\_options**: [`SceneOptimizerOptions`](SceneOptimizerOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:611

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:612

___

### \_sceneDisposeObserver

• `Private` **\_sceneDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:617

___

### \_targetFrameRate

• `Private` **\_targetFrameRate**: `number` = `60`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:614

___

### \_trackerDuration

• `Private` **\_trackerDuration**: `number` = `2000`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:615

___

### onFailureObservable

• **onFailureObservable**: [`Observable`](Observable.md)[`SceneOptimizer`](SceneOptimizer.md)

Defines an observable called when the optimizer is not able to reach the target frame rate

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:631

___

### onNewOptimizationAppliedObservable

• **onNewOptimizationAppliedObservable**: [`Observable`](Observable.md)[`SceneOptimization`](SceneOptimization.md)

Defines an observable called when the optimizer enables an optimization

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:627

___

### onSuccessObservable

• **onSuccessObservable**: [`Observable`](Observable.md)[`SceneOptimizer`](SceneOptimizer.md)

Defines an observable called when the optimizer reaches the target frame rate

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:623

## Accessors

### currentFrameRate

• `get` **currentFrameRate**(): `number`

Gets the current frame rate checked by the SceneOptimizer

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:654

___

### currentPriorityLevel

• `get` **currentPriorityLevel**(): `number`

Gets the current priority level (0 at start)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:647

___

### isInImprovementMode

• `get` **isInImprovementMode**(): `boolean`

Gets or sets a boolean indicating if the optimizer is in improvement mode

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:636

• `set` **isInImprovementMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:640

___

### optimizations

• `get` **optimizations**(): [`SceneOptimization`](SceneOptimization.md)[]

Gets the list of active optimizations

#### Returns

[`SceneOptimization`](SceneOptimization.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:689

___

### targetFrameRate

• `get` **targetFrameRate**(): `number`

Gets or sets the current target frame rate (60 by default)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:661

• `set` **targetFrameRate**(`value`): `void`

Gets or sets the current target frame rate (60 by default)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:668

___

### trackerDuration

• `get` **trackerDuration**(): `number`

Gets or sets the current interval between two checks (every 2000ms by default)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:675

• `set` **trackerDuration**(`value`): `void`

Gets or sets the current interval between two checks (every 2000ms by default)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:682

## Methods

### \_checkCurrentState

▸ `Private` **_checkCurrentState**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:763

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:816

___

### reset

▸ **reset**(): `void`

Reset the optimizer to initial step (current priority level = 0)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:740

___

### start

▸ **start**(): `void`

Start the optimizer. By default it will try to reach a specific framerate
but if the optimizer is set with improvementMode === true then it will run all optimization while frame rate is above the target frame rate

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:748

___

### stop

▸ **stop**(): `void`

Stops the current optimizer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:733

___

### OptimizeAsync

▸ `Static` **OptimizeAsync**(`scene`, `options?`, `onSuccess?`, `onFailure?`): [`SceneOptimizer`](SceneOptimizer.md)

Helper function to create a SceneOptimizer with one single line of code

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the scene to work on |
| `options?` | [`SceneOptimizerOptions`](SceneOptimizerOptions.md) | defines the options to use with the SceneOptimizer |
| `onSuccess?` | () => `void` | defines a callback to call on success |
| `onFailure?` | () => `void` | defines a callback to call on failure |

#### Returns

[`SceneOptimizer`](SceneOptimizer.md)

the new SceneOptimizer object

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:834

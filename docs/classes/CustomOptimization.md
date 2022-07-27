[@dev/core](../README.md) / [Exports](../modules.md) / CustomOptimization

# Class: CustomOptimization

Defines an optimization based on user defined callback.

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- [`SceneOptimization`](SceneOptimization.md)

  ↳ **`CustomOptimization`**

## Table of contents

### Constructors

- [constructor](CustomOptimization.md#constructor)

### Properties

- [onApply](CustomOptimization.md#onapply)
- [onGetDescription](CustomOptimization.md#ongetdescription)
- [priority](CustomOptimization.md#priority)

### Methods

- [apply](CustomOptimization.md#apply)
- [getDescription](CustomOptimization.md#getdescription)

## Constructors

### constructor

• **new CustomOptimization**(`priority?`)

Creates the SceneOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |

#### Inherited from

[SceneOptimization](SceneOptimization.md).[constructor](SceneOptimization.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:37

## Properties

### onApply

• **onApply**: (`scene`: [`Scene`](Scene.md), `optimizer`: [`SceneOptimizer`](SceneOptimizer.md)) => `boolean`

#### Type declaration

▸ (`scene`, `optimizer`): `boolean`

Callback called to apply the custom optimization.

##### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `optimizer` | [`SceneOptimizer`](SceneOptimizer.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:253

___

### onGetDescription

• **onGetDescription**: () => `string`

#### Type declaration

▸ (): `string`

Callback called to get custom description

##### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:258

___

### priority

• **priority**: `number` = `0`

#### Inherited from

[SceneOptimization](SceneOptimization.md).[priority](SceneOptimization.md#priority)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:41

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

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:278

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

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:264

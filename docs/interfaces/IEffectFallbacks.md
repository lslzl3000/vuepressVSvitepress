[@dev/core](../README.md) / [Exports](../modules.md) / IEffectFallbacks

# Interface: IEffectFallbacks

Interface used to define common properties for effect fallbacks

## Implemented by

- [`EffectFallbacks`](../classes/EffectFallbacks.md)

## Table of contents

### Properties

- [hasMoreFallbacks](IEffectFallbacks.md#hasmorefallbacks)

### Methods

- [reduce](IEffectFallbacks.md#reduce)
- [unBindMesh](IEffectFallbacks.md#unbindmesh)

## Properties

### hasMoreFallbacks

• **hasMoreFallbacks**: `boolean`

Checks to see if more fallbacks are still available.

#### Defined in

https://github.com/babylon.js/core/src/Materials/iEffectFallbacks.ts:23

## Methods

### reduce

▸ **reduce**(`currentDefines`, `effect`): `string`

Removes the defines that should be removed when falling back.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentDefines` | `string` | defines the current define statements for the shader. |
| `effect` | [`Effect`](../classes/Effect.md) | defines the current effect we try to compile |

#### Returns

`string`

The resulting defines with defines of the current rank removed.

#### Defined in

https://github.com/babylon.js/core/src/Materials/iEffectFallbacks.ts:13

___

### unBindMesh

▸ **unBindMesh**(): `void`

Removes the fallback from the bound mesh.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/iEffectFallbacks.ts:18

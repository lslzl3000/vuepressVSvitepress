[@dev/core](../README.md) / [Exports](../modules.md) / IBakedVertexAnimationManager

# Interface: IBakedVertexAnimationManager

Interface for baked vertex animation texture, see BakedVertexAnimationManager

**`Since`**

5.0

## Implemented by

- [`BakedVertexAnimationManager`](../classes/BakedVertexAnimationManager.md)

## Table of contents

### Properties

- [animationParameters](IBakedVertexAnimationManager.md#animationparameters)
- [isEnabled](IBakedVertexAnimationManager.md#isenabled)
- [texture](IBakedVertexAnimationManager.md#texture)
- [time](IBakedVertexAnimationManager.md#time)

### Methods

- [bind](IBakedVertexAnimationManager.md#bind)
- [dispose](IBakedVertexAnimationManager.md#dispose)
- [getClassName](IBakedVertexAnimationManager.md#getclassname)
- [setAnimationParameters](IBakedVertexAnimationManager.md#setanimationparameters)

## Properties

### animationParameters

• **animationParameters**: [`Vector4`](../classes/Vector4.md)

The animation parameters for the mesh. See setAnimationParameters()

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:27

___

### isEnabled

• **isEnabled**: `boolean`

Gets or sets a boolean indicating if the edgesRenderer is active

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:22

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](../classes/BaseTexture.md)

The vertex animation texture

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:17

___

### time

• **time**: `number`

The time counter, to pick the correct animation frame.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:32

## Methods

### bind

▸ **bind**(`effect`, `useInstances`): `void`

Binds to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](../classes/Effect.md) | The effect to bind to. |
| `useInstances` | `boolean` | True when it's an instance. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:39

___

### dispose

▸ **dispose**(`forceDisposeTextures?`): `void`

Disposes the resources of the manager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeTextures?` | `boolean` | Forces the disposal of all textures. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:54

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name useful for serialization or dynamic coding.

#### Returns

`string`

"BakedVertexAnimationManager"

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:60

___

### setAnimationParameters

▸ **setAnimationParameters**(`startFrame`, `endFrame`, `offset`, `speedFramesPerSecond`): `void`

Sets animation parameters.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startFrame` | `number` | The first frame of the animation. |
| `endFrame` | `number` | The last frame of the animation. |
| `offset` | `number` | The offset when starting the animation. |
| `speedFramesPerSecond` | `number` | The frame rate. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:48

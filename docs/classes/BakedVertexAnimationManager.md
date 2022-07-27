[@dev/core](../README.md) / [Exports](../modules.md) / BakedVertexAnimationManager

# Class: BakedVertexAnimationManager

This class is used to animate meshes using a baked vertex animation texture

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/baked_texture_animations

**`Since`**

5.0

## Implements

- [`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

## Table of contents

### Constructors

- [constructor](BakedVertexAnimationManager.md#constructor)

### Properties

- [\_isEnabled](BakedVertexAnimationManager.md#_isenabled)
- [\_scene](BakedVertexAnimationManager.md#_scene)
- [\_texture](BakedVertexAnimationManager.md#_texture)
- [animationParameters](BakedVertexAnimationManager.md#animationparameters)
- [isEnabled](BakedVertexAnimationManager.md#isenabled)
- [texture](BakedVertexAnimationManager.md#texture)
- [time](BakedVertexAnimationManager.md#time)

### Methods

- [bind](BakedVertexAnimationManager.md#bind)
- [clone](BakedVertexAnimationManager.md#clone)
- [copyTo](BakedVertexAnimationManager.md#copyto)
- [dispose](BakedVertexAnimationManager.md#dispose)
- [getClassName](BakedVertexAnimationManager.md#getclassname)
- [parse](BakedVertexAnimationManager.md#parse)
- [serialize](BakedVertexAnimationManager.md#serialize)
- [setAnimationParameters](BakedVertexAnimationManager.md#setanimationparameters)

## Constructors

### constructor

• **new BakedVertexAnimationManager**(`scene?`)

Creates a new BakedVertexAnimationManager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:103

## Properties

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:79

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:69

___

### \_texture

• `Private` **\_texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:71

___

### animationParameters

• **animationParameters**: [`Vector4`](Vector4.md)

The animation parameters for the mesh. See setAnimationParameters()

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[animationParameters](../interfaces/IBakedVertexAnimationManager.md#animationparameters)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:91

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Enable or disable the vertex animation manager

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[isEnabled](../interfaces/IBakedVertexAnimationManager.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:85

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The vertex animation texture

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[texture](../interfaces/IBakedVertexAnimationManager.md#texture)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:77

___

### time

• **time**: `number` = `0`

The time counter, to pick the correct animation frame.

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[time](../interfaces/IBakedVertexAnimationManager.md#time)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:97

## Methods

### bind

▸ **bind**(`effect`, `useInstances?`): `void`

Binds to the effect.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect to bind to. |
| `useInstances` | `boolean` | `false` | True when it's an instance. |

#### Returns

`void`

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[bind](../interfaces/IBakedVertexAnimationManager.md#bind)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:126

___

### clone

▸ **clone**(): [`BakedVertexAnimationManager`](BakedVertexAnimationManager.md)

Clone the current manager

#### Returns

[`BakedVertexAnimationManager`](BakedVertexAnimationManager.md)

a new BakedVertexAnimationManager

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:146

___

### copyTo

▸ **copyTo**(`vatMap`): `void`

Makes a duplicate of the current instance into another one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vatMap` | [`BakedVertexAnimationManager`](BakedVertexAnimationManager.md) | define the instance where to copy the info |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:185

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

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[dispose](../interfaces/IBakedVertexAnimationManager.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:167

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name useful for serialization or dynamic coding.

#### Returns

`string`

"BakedVertexAnimationManager"

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[getClassName](../interfaces/IBakedVertexAnimationManager.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:177

___

### parse

▸ **parse**(`source`, `scene`, `rootUrl`): `void`

Parses a vertex animation setting from a serialized object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Serialized object. |
| `scene` | [`Scene`](Scene.md) | Defines the scene we are parsing for |
| `rootUrl` | `string` | Defines the rootUrl to load from |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:203

___

### serialize

▸ **serialize**(): `any`

Serializes this vertex animation instance

#### Returns

`any`

- An object with the serialized instance.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:193

___

### setAnimationParameters

▸ **setAnimationParameters**(`startFrame`, `endFrame`, `offset?`, `speedFramesPerSecond?`): `void`

Sets animation parameters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `startFrame` | `number` | `undefined` | The first frame of the animation. |
| `endFrame` | `number` | `undefined` | The last frame of the animation. |
| `offset` | `number` | `0` | The offset when starting the animation. |
| `speedFramesPerSecond` | `number` | `30` | The frame rate. |

#### Returns

`void`

#### Implementation of

[IBakedVertexAnimationManager](../interfaces/IBakedVertexAnimationManager.md).[setAnimationParameters](../interfaces/IBakedVertexAnimationManager.md#setanimationparameters)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/bakedVertexAnimationManager.ts:159

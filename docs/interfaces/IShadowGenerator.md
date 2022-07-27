[@dev/core](../README.md) / [Exports](../modules.md) / IShadowGenerator

# Interface: IShadowGenerator

Interface to implement to create a shadow generator compatible with BJS.

## Implemented by

- [`ShadowGenerator`](../classes/ShadowGenerator.md)

## Table of contents

### Properties

- [id](IShadowGenerator.md#id)

### Methods

- [bindShadowLight](IShadowGenerator.md#bindshadowlight)
- [dispose](IShadowGenerator.md#dispose)
- [forceCompilation](IShadowGenerator.md#forcecompilation)
- [forceCompilationAsync](IShadowGenerator.md#forcecompilationasync)
- [getShadowMap](IShadowGenerator.md#getshadowmap)
- [getTransformMatrix](IShadowGenerator.md#gettransformmatrix)
- [isReady](IShadowGenerator.md#isready)
- [prepareDefines](IShadowGenerator.md#preparedefines)
- [recreateShadowMap](IShadowGenerator.md#recreateshadowmap)
- [serialize](IShadowGenerator.md#serialize)

## Properties

### id

• **id**: `string`

Gets or set the id of the shadow generator. It will be the one from the light if not defined

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:69

## Methods

### bindShadowLight

▸ **bindShadowLight**(`lightIndex`, `effect`): `void`

Binds the shadow related information inside of an effect (information like near, far, darkness...
defined in the generator but impacting the effect).
It implies the uniforms available on the materials are the standard BJS ones.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `lightIndex` | `string` | Index of the light in the enabled light list of the material owning the effect |
| `effect` | [`Effect`](../classes/Effect.md) | The effect we are binding the information for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:98

___

### dispose

▸ **dispose**(): `void`

Disposes the Shadow map and related Textures and effects.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:135

___

### forceCompilation

▸ **forceCompilation**(`onCompiled?`, `options?`): `void`

Forces all the attached effect to compile to enable rendering only once ready vs. lazily compiling effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onCompiled?` | (`generator`: [`IShadowGenerator`](IShadowGenerator.md)) => `void` | Callback triggered at the and of the effects compilation |
| `options?` | `Partial`{ `useInstances`: `boolean`  } | Sets of optional options forcing the compilation with different modes |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:117

___

### forceCompilationAsync

▸ **forceCompilationAsync**(`options?`): `Promise``void`

Forces all the attached effect to compile to enable rendering only once ready vs. lazily compiling effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Partial`{ `useInstances`: `boolean`  } | Sets of optional options forcing the compilation with different modes |

#### Returns

`Promise``void`

A promise that resolves when the compilation completes

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:124

___

### getShadowMap

▸ **getShadowMap**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](../classes/RenderTargetTexture.md)

Gets the main RTT containing the shadow map (usually storing depth from the light point of view).

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](../classes/RenderTargetTexture.md)

The render target texture if present otherwise, null

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:74

___

### getTransformMatrix

▸ **getTransformMatrix**(): [`Matrix`](../classes/Matrix.md)

Gets the transformation matrix used to project the meshes into the map from the light point of view.
(eq to shadow projection matrix * light transform matrix)

#### Returns

[`Matrix`](../classes/Matrix.md)

The transform matrix used to create the shadow map

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:104

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`, `isTransparent`): `boolean`

Determine whether the shadow generator is ready or not (mainly all effects and related post processes needs to be ready).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](../classes/SubMesh.md) | The submesh we want to render in the shadow map |
| `useInstances` | `boolean` | Defines whether will draw in the map using instances |
| `isTransparent` | `boolean` | Indicates that isReady is called for a transparent subMesh |

#### Returns

`boolean`

true if ready otherwise, false

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:83

___

### prepareDefines

▸ **prepareDefines**(`defines`, `lightIndex`): `void`

Prepare all the defines in a material relying on a shadow map at the specified light index.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | [`MaterialDefines`](../classes/MaterialDefines.md) | Defines of the material we want to update |
| `lightIndex` | `number` | Index of the light in the enabled light list of the material |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:90

___

### recreateShadowMap

▸ **recreateShadowMap**(): `void`

Recreates the shadow map dependencies like RTT and post processes. This can be used during the switch between
Cube and 2D textures for instance.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:110

___

### serialize

▸ **serialize**(): `any`

Serializes the shadow generator setup to a json object.

#### Returns

`any`

The serialized JSON object

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:130

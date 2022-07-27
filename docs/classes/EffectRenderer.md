[@dev/core](../README.md) / [Exports](../modules.md) / EffectRenderer

# Class: EffectRenderer

Helper class to render one or more effects.
You can access the previous rendering in your shader by declaring a sampler named textureSampler

## Table of contents

### Constructors

- [constructor](EffectRenderer.md#constructor)

### Properties

- [\_fullscreenViewport](EffectRenderer.md#_fullscreenviewport)
- [\_indexBuffer](EffectRenderer.md#_indexbuffer)
- [\_onContextRestoredObserver](EffectRenderer.md#_oncontextrestoredobserver)
- [\_vertexBuffers](EffectRenderer.md#_vertexbuffers)
- [\_DefaultOptions](EffectRenderer.md#_defaultoptions)

### Methods

- [\_isRenderTargetTexture](EffectRenderer.md#_isrendertargettexture)
- [applyEffectWrapper](EffectRenderer.md#applyeffectwrapper)
- [bindBuffers](EffectRenderer.md#bindbuffers)
- [dispose](EffectRenderer.md#dispose)
- [draw](EffectRenderer.md#draw)
- [render](EffectRenderer.md#render)
- [restoreStates](EffectRenderer.md#restorestates)
- [setViewport](EffectRenderer.md#setviewport)

## Constructors

### constructor

• **new EffectRenderer**(`_engine`, `options?`)

Creates an effect renderer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `_engine` | [`ThinEngine`](ThinEngine.md) | `undefined` | the engine to use for rendering |
| `options` | [`IEffectRendererOptions`](../interfaces/IEffectRendererOptions.md) | `EffectRenderer._DefaultOptions` | defines the options of the effect renderer |

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:53

## Properties

### \_fullscreenViewport

• `Private` **\_fullscreenViewport**: [`Viewport`](Viewport.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:45

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:43

___

### \_onContextRestoredObserver

• `Private` **\_onContextRestoredObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:46

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object`

#### Index signature

▪ [key: `string`]: [`VertexBuffer`](VertexBuffer.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:42

___

### \_DefaultOptions

▪ `Static` `Private` **\_DefaultOptions**: [`IEffectRendererOptions`](../interfaces/IEffectRendererOptions.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:37

## Methods

### \_isRenderTargetTexture

▸ `Private` **_isRenderTargetTexture**(`texture`): texture is IRenderTargetTexture

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`RenderTargetWrapper`](RenderTargetWrapper.md) \| [`IRenderTargetTexture`](../interfaces/IRenderTargetTexture.md) |

#### Returns

texture is IRenderTargetTexture

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:119

___

### applyEffectWrapper

▸ **applyEffectWrapper**(`effectWrapper`): `void`

Sets the current effect wrapper to use during draw.
The effect needs to be ready before calling this api.
This also sets the default full screen position attribute.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effectWrapper` | [`EffectWrapper`](EffectWrapper.md) | Defines the effect to draw with |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:96

___

### bindBuffers

▸ **bindBuffers**(`effect`): `void`

Binds the embedded attributes buffer to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | Defines the effect to bind the attributes for |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:86

___

### dispose

▸ **dispose**(): `void`

Disposes of the effect renderer

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:157

___

### draw

▸ **draw**(): `void`

Draws a full screen quad.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:115

___

### render

▸ **render**(`effectWrapper`, `outputTexture?`): `void`

renders one or more effects to a specified texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `effectWrapper` | [`EffectWrapper`](EffectWrapper.md) | `undefined` | the effect to renderer |
| `outputTexture` | [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) \| [`IRenderTargetTexture`](../interfaces/IRenderTargetTexture.md) | `null` | texture to draw to, if null it will render to the screen. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:128

___

### restoreStates

▸ **restoreStates**(): `void`

Restores engine states

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:107

___

### setViewport

▸ **setViewport**(`viewport?`): `void`

Sets the current viewport in normalized coordinates 0-1

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewport` | [`Viewport`](Viewport.md) | Defines the viewport to set (defaults to 0 0 1 1) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:78

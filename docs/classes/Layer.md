[@dev/core](../README.md) / [Exports](../modules.md) / Layer

# Class: Layer

This represents a full screen 2d layer.
This can be useful to display a picture in the  background of your scene for instance.

**`See`**

https://www.babylonjs-playground.com/#08A2BS#1

## Table of contents

### Constructors

- [constructor](Layer.md#constructor)

### Properties

- [\_drawWrapper](Layer.md#_drawwrapper)
- [\_indexBuffer](Layer.md#_indexbuffer)
- [\_onAfterRenderObserver](Layer.md#_onafterrenderobserver)
- [\_onBeforeRenderObserver](Layer.md#_onbeforerenderobserver)
- [\_onDisposeObserver](Layer.md#_ondisposeobserver)
- [\_previousDefines](Layer.md#_previousdefines)
- [\_scene](Layer.md#_scene)
- [\_vertexBuffers](Layer.md#_vertexbuffers)
- [alphaBlendingMode](Layer.md#alphablendingmode)
- [alphaTest](Layer.md#alphatest)
- [color](Layer.md#color)
- [isBackground](Layer.md#isbackground)
- [isEnabled](Layer.md#isenabled)
- [layerMask](Layer.md#layermask)
- [name](Layer.md#name)
- [offset](Layer.md#offset)
- [onAfterRenderObservable](Layer.md#onafterrenderobservable)
- [onBeforeRenderObservable](Layer.md#onbeforerenderobservable)
- [onDisposeObservable](Layer.md#ondisposeobservable)
- [renderOnlyInRenderTargetTextures](Layer.md#renderonlyinrendertargettextures)
- [renderTargetTextures](Layer.md#rendertargettextures)
- [scale](Layer.md#scale)
- [texture](Layer.md#texture)

### Accessors

- [onAfterRender](Layer.md#onafterrender)
- [onBeforeRender](Layer.md#onbeforerender)
- [onDispose](Layer.md#ondispose)

### Methods

- [\_createIndexBuffer](Layer.md#_createindexbuffer)
- [dispose](Layer.md#dispose)
- [render](Layer.md#render)

## Constructors

### constructor

• **new Layer**(`name`, `imgUrl`, `scene`, `isBackground?`, `color?`)

Instantiates a new layer.
This represents a full screen 2d layer.
This can be useful to display a picture in the  background of your scene for instance.

**`See`**

https://www.babylonjs-playground.com/#08A2BS#1

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the layer in the scene |
| `imgUrl` | [`Nullable`](../modules.md#nullable)`string` | Define the url of the texture to display in the layer |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | Define the scene the layer belongs to |
| `isBackground?` | `boolean` | Defines whether the layer is displayed in front or behind the scene |
| `color?` | [`Color4`](Color4.md) | Defines a color for the layer |

#### Defined in

packages/dev/core/src/Layers/layer.ts:154

## Properties

### \_drawWrapper

• `Private` **\_drawWrapper**: `DrawWrapper`

#### Defined in

packages/dev/core/src/Layers/layer.ts:89

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:88

___

### \_onAfterRenderObserver

• `Private` **\_onAfterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Layer`](Layer.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:131

___

### \_onBeforeRenderObserver

• `Private` **\_onBeforeRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Layer`](Layer.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:114

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Layer`](Layer.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:97

___

### \_previousDefines

• `Private` **\_previousDefines**: `string`

#### Defined in

packages/dev/core/src/Layers/layer.ts:90

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:86

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

packages/dev/core/src/Layers/layer.ts:87

___

### alphaBlendingMode

• **alphaBlendingMode**: `number` = `Constants.ALPHA_COMBINE`

Define the alpha blending mode used in the layer in case the texture or color has an alpha.

#### Defined in

packages/dev/core/src/Layers/layer.ts:56

___

### alphaTest

• **alphaTest**: `boolean`

Define if the layer should alpha test or alpha blend with the rest of the scene.
Alpha test will not mix with the background color in case of transparency.
It will either use the texture color or the background depending on the alpha value of the current pixel.

#### Defined in

packages/dev/core/src/Layers/layer.ts:63

___

### color

• **color**: [`Color4`](Color4.md)

Define the color of the layer (instead of texture).

#### Defined in

packages/dev/core/src/Layers/layer.ts:41

___

### isBackground

• **isBackground**: `boolean`

Is the layer in background or foreground.

#### Defined in

packages/dev/core/src/Layers/layer.ts:36

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Define if the layer is enabled (ie. should be displayed). Default: true

#### Defined in

packages/dev/core/src/Layers/layer.ts:84

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Define a mask to restrict the layer to only some of the scene cameras.

#### Defined in

packages/dev/core/src/Layers/layer.ts:68

___

### name

• **name**: `string`

#### Defined in

packages/dev/core/src/Layers/layer.ts:158

___

### offset

• **offset**: [`Vector2`](Vector2.md)

Define an offset for the layer in order to shift the texture.

#### Defined in

packages/dev/core/src/Layers/layer.ts:51

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Layer`](Layer.md)

An event triggered after rendering the scene

#### Defined in

packages/dev/core/src/Layers/layer.ts:129

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Layer`](Layer.md)

An event triggered before rendering the scene

#### Defined in

packages/dev/core/src/Layers/layer.ts:112

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Layer`](Layer.md)

An event triggered when the layer is disposed.

#### Defined in

packages/dev/core/src/Layers/layer.ts:95

___

### renderOnlyInRenderTargetTextures

• **renderOnlyInRenderTargetTextures**: `boolean` = `false`

Define if the layer is only used in renderTarget or if it also
renders in the main frame buffer of the canvas.

#### Defined in

packages/dev/core/src/Layers/layer.ts:79

___

### renderTargetTextures

• **renderTargetTextures**: [`RenderTargetTexture`](RenderTargetTexture.md)[] = `[]`

Define the list of render target the layer is visible into.

#### Defined in

packages/dev/core/src/Layers/layer.ts:73

___

### scale

• **scale**: [`Vector2`](Vector2.md)

Define the scale of the layer in order to zoom in out of the texture.

#### Defined in

packages/dev/core/src/Layers/layer.ts:46

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define the texture the layer should display.

#### Defined in

packages/dev/core/src/Layers/layer.ts:31

## Accessors

### onAfterRender

• `set` **onAfterRender**(`callback`): `void`

Back compatibility with callback before the onAfterRenderObservable existed.
The set callback will be triggered just after rendering the layer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:136

___

### onBeforeRender

• `set` **onBeforeRender**(`callback`): `void`

Back compatibility with callback before the onBeforeRenderObservable existed.
The set callback will be triggered just before rendering the layer.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:119

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Back compatibility with callback before the onDisposeObservable existed.
The set callback will be triggered when the layer has been disposed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:102

## Methods

### \_createIndexBuffer

▸ `Private` **_createIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:193

___

### dispose

▸ **dispose**(): `void`

Disposes and releases the associated resources.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:286

___

### render

▸ **render**(): `void`

Renders the layer in the scene.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/layer.ts:223

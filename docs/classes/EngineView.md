[@dev/core](../README.md) / [Exports](../modules.md) / EngineView

# Class: EngineView

Class used to define an additional view for the engine

**`See`**

https://doc.babylonjs.com/divingDeeper/scene/multiCanvas

## Table of contents

### Constructors

- [constructor](EngineView.md#constructor)

### Properties

- [camera](EngineView.md#camera)
- [clearBeforeCopy](EngineView.md#clearbeforecopy)
- [customResize](EngineView.md#customresize)
- [enabled](EngineView.md#enabled)
- [target](EngineView.md#target)

## Constructors

### constructor

• **new EngineView**()

## Properties

### camera

• `Optional` **camera**: [`Camera`](Camera.md)

Defines an optional camera used to render the view (will use active camera else)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.views.ts:14

___

### clearBeforeCopy

• `Optional` **clearBeforeCopy**: `boolean`

Indicates if the destination view canvas should be cleared before copying the parent canvas. Can help if the scene clear color has alpha  1

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.views.ts:16

___

### customResize

• `Optional` **customResize**: (`canvas`: `HTMLCanvasElement`) => `void`

#### Type declaration

▸ (`canvas`): `void`

Defines a custom function to handle canvas size changes. (the canvas to render into is provided to the callback)

##### Parameters

| Name | Type |
| :------ | :------ |
| `canvas` | `HTMLCanvasElement` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.views.ts:20

___

### enabled

• **enabled**: `boolean`

Indicates if the view is enabled (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.views.ts:18

___

### target

• **target**: `HTMLCanvasElement`

Defines the canvas where to render the view

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.views.ts:12

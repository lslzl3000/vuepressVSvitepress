[@dev/core](../README.md) / [Exports](../modules.md) / IEffectLayerOptions

# Interface: IEffectLayerOptions

Effect layer options. This helps customizing the behaviour
of the effect layer.

## Table of contents

### Properties

- [alphaBlendingMode](IEffectLayerOptions.md#alphablendingmode)
- [camera](IEffectLayerOptions.md#camera)
- [mainTextureFixedSize](IEffectLayerOptions.md#maintexturefixedsize)
- [mainTextureRatio](IEffectLayerOptions.md#maintextureratio)
- [renderingGroupId](IEffectLayerOptions.md#renderinggroupid)

## Properties

### alphaBlendingMode

• **alphaBlendingMode**: `number`

Alpha blending mode used to apply the blur. Default depends of the implementation.

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:51

___

### camera

• **camera**: [`Nullable`](../modules.md#nullable)[`Camera`](../classes/Camera.md)

The camera attached to the layer.

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:56

___

### mainTextureFixedSize

• `Optional` **mainTextureFixedSize**: `number`

Enforces a fixed size texture to ensure effect stability across devices.

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:46

___

### mainTextureRatio

• **mainTextureRatio**: `number`

Multiplication factor apply to the canvas size to compute the render target size
used to generated the objects (the smaller the faster).

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:41

___

### renderingGroupId

• **renderingGroupId**: `number`

The rendering group to draw the layer in.

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:61

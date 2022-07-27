[@dev/core](../README.md) / [Exports](../modules.md) / IHighlightLayerOptions

# Interface: IHighlightLayerOptions

Highlight layer options. This helps customizing the behaviour
of the highlight layer.

## Table of contents

### Properties

- [alphaBlendingMode](IHighlightLayerOptions.md#alphablendingmode)
- [blurHorizontalSize](IHighlightLayerOptions.md#blurhorizontalsize)
- [blurTextureSizeRatio](IHighlightLayerOptions.md#blurtexturesizeratio)
- [blurVerticalSize](IHighlightLayerOptions.md#blurverticalsize)
- [camera](IHighlightLayerOptions.md#camera)
- [isStroke](IHighlightLayerOptions.md#isstroke)
- [mainTextureFixedSize](IHighlightLayerOptions.md#maintexturefixedsize)
- [mainTextureRatio](IHighlightLayerOptions.md#maintextureratio)
- [renderingGroupId](IHighlightLayerOptions.md#renderinggroupid)

## Properties

### alphaBlendingMode

• **alphaBlendingMode**: `number`

Alpha blending mode used to apply the blur. Default is combine.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:115

___

### blurHorizontalSize

• **blurHorizontalSize**: `number`

How big in texel of the blur texture is the horizontal blur.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:110

___

### blurTextureSizeRatio

• **blurTextureSizeRatio**: `number`

Multiplication factor apply to the main texture size in the first step of the blur to reduce the size
of the picture to blur (the smaller the faster).

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:100

___

### blurVerticalSize

• **blurVerticalSize**: `number`

How big in texel of the blur texture is the vertical blur.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:105

___

### camera

• **camera**: [`Nullable`](../modules.md#nullable)[`Camera`](../classes/Camera.md)

The camera attached to the layer.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:120

___

### isStroke

• `Optional` **isStroke**: `boolean`

Should we display highlight as a solid stroke?

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:125

___

### mainTextureFixedSize

• `Optional` **mainTextureFixedSize**: `number`

Enforces a fixed size texture to ensure resize independent blur.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:94

___

### mainTextureRatio

• **mainTextureRatio**: `number`

Multiplication factor apply to the canvas size to compute the render target size
used to generated the glowing objects (the smaller the faster).

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:89

___

### renderingGroupId

• **renderingGroupId**: `number`

The rendering group to draw the layer in.

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:130

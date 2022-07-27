[@dev/core](../README.md) / [Exports](../modules.md) / IGlowLayerOptions

# Interface: IGlowLayerOptions

Glow layer options. This helps customizing the behaviour
of the glow layer.

## Table of contents

### Properties

- [alphaBlendingMode](IGlowLayerOptions.md#alphablendingmode)
- [blurKernelSize](IGlowLayerOptions.md#blurkernelsize)
- [camera](IGlowLayerOptions.md#camera)
- [ldrMerge](IGlowLayerOptions.md#ldrmerge)
- [mainTextureFixedSize](IGlowLayerOptions.md#maintexturefixedsize)
- [mainTextureRatio](IGlowLayerOptions.md#maintextureratio)
- [mainTextureSamples](IGlowLayerOptions.md#maintexturesamples)
- [renderingGroupId](IGlowLayerOptions.md#renderinggroupid)

## Properties

### alphaBlendingMode

• `Optional` **alphaBlendingMode**: `number`

Defines the blend mode used by the merge

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:94

___

### blurKernelSize

• **blurKernelSize**: `number`

How big is the kernel of the blur texture.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:69

___

### camera

• **camera**: [`Nullable`](../modules.md#nullable)[`Camera`](../classes/Camera.md)

The camera attached to the layer.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:74

___

### ldrMerge

• `Optional` **ldrMerge**: `boolean`

Forces the merge step to be done in ldr (clamp values > 1)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:89

___

### mainTextureFixedSize

• `Optional` **mainTextureFixedSize**: `number`

Enforces a fixed size texture to ensure resize independent blur.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:64

___

### mainTextureRatio

• **mainTextureRatio**: `number`

Multiplication factor apply to the canvas size to compute the render target size
used to generated the glowing objects (the smaller the faster).

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:59

___

### mainTextureSamples

• `Optional` **mainTextureSamples**: `number`

Enable MSAA by choosing the number of samples.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:79

___

### renderingGroupId

• **renderingGroupId**: `number`

The rendering group to draw the layer in.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:84

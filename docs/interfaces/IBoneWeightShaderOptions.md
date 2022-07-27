[@dev/core](../README.md) / [Exports](../modules.md) / IBoneWeightShaderOptions

# Interface: IBoneWeightShaderOptions

Defines the constructor options for the BoneWeight Shader.

## Table of contents

### Properties

- [colorBase](IBoneWeightShaderOptions.md#colorbase)
- [colorFull](IBoneWeightShaderOptions.md#colorfull)
- [colorHalf](IBoneWeightShaderOptions.md#colorhalf)
- [colorQuarter](IBoneWeightShaderOptions.md#colorquarter)
- [colorZero](IBoneWeightShaderOptions.md#colorzero)
- [skeleton](IBoneWeightShaderOptions.md#skeleton)
- [targetBoneIndex](IBoneWeightShaderOptions.md#targetboneindex)

## Properties

### colorBase

• `Optional` **colorBase**: [`Color3`](../classes/Color3.md)

Colors for Uninfluenced bones

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:64

___

### colorFull

• `Optional` **colorFull**: [`Color3`](../classes/Color3.md)

Color for 0.75-1 Weight Influence

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:76

___

### colorHalf

• `Optional` **colorHalf**: [`Color3`](../classes/Color3.md)

Color for 0.5-0.75 Weight Influence

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:73

___

### colorQuarter

• `Optional` **colorQuarter**: [`Color3`](../classes/Color3.md)

Color for 0.25-0.5 Weight Influence

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:70

___

### colorZero

• `Optional` **colorZero**: [`Color3`](../classes/Color3.md)

Colors for 0.0-0.25 Weight bones

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:67

___

### skeleton

• **skeleton**: [`Skeleton`](../classes/Skeleton.md)

Skeleton to Map

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:61

___

### targetBoneIndex

• `Optional` **targetBoneIndex**: `number`

Color for Zero Weight Influence

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:79

[@dev/core](../README.md) / [Exports](../modules.md) / ISkeletonMapShaderOptions

# Interface: ISkeletonMapShaderOptions

Defines the constructor options for the SkeletonMap Shader.

## Table of contents

### Properties

- [colorMap](ISkeletonMapShaderOptions.md#colormap)
- [skeleton](ISkeletonMapShaderOptions.md#skeleton)

## Properties

### colorMap

• `Optional` **colorMap**: [`ISkeletonMapShaderColorMapKnot`](ISkeletonMapShaderColorMapKnot.md)[]

Array of ColorMapKnots that make the gradient must be ordered with knot[i].location  knot[i+1].location

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:99

___

### skeleton

• **skeleton**: [`Skeleton`](../classes/Skeleton.md)

Skeleton to Map

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:97

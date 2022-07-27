[@dev/core](../README.md) / [Exports](../modules.md) / ISkeletonViewerDisplayOptions

# Interface: ISkeletonViewerDisplayOptions

Defines how to display the various bone meshes for the viewer.

## Table of contents

### Properties

- [localAxesSize](ISkeletonViewerDisplayOptions.md#localaxessize)
- [midStep](ISkeletonViewerDisplayOptions.md#midstep)
- [midStepFactor](ISkeletonViewerDisplayOptions.md#midstepfactor)
- [showLocalAxes](ISkeletonViewerDisplayOptions.md#showlocalaxes)
- [sphereBaseSize](ISkeletonViewerDisplayOptions.md#spherebasesize)
- [sphereFactor](ISkeletonViewerDisplayOptions.md#spherefactor)
- [sphereScaleUnit](ISkeletonViewerDisplayOptions.md#spherescaleunit)
- [spurFollowsChild](ISkeletonViewerDisplayOptions.md#spurfollowschild)

## Properties

### localAxesSize

• `Optional` **localAxesSize**: `number`

Length of each local axis

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:53

___

### midStep

• `Optional` **midStep**: `number`

How far down to start tapering the bone spurs

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:32

___

### midStepFactor

• `Optional` **midStepFactor**: `number`

How big is the midStep?

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:35

___

### showLocalAxes

• `Optional` **showLocalAxes**: `boolean`

Whether to show local axes or not

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:50

___

### sphereBaseSize

• `Optional` **sphereBaseSize**: `number`

Base for the Sphere Size

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:38

___

### sphereFactor

• `Optional` **sphereFactor**: `number`

Ratio for the Sphere Size

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:44

___

### sphereScaleUnit

• `Optional` **sphereScaleUnit**: `number`

The ratio of the sphere to the longest bone in units

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:41

___

### spurFollowsChild

• `Optional` **spurFollowsChild**: `boolean`

Whether a spur should attach its far end to the child bone position

#### Defined in

https://github.com/babylon.js/core/src/Debug/ISkeletonViewer.ts:47

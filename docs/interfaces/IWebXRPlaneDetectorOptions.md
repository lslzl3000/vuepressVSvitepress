[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRPlaneDetectorOptions

# Interface: IWebXRPlaneDetectorOptions

Options used in the plane detector module

## Table of contents

### Properties

- [doNotRemovePlanesOnSessionEnded](IWebXRPlaneDetectorOptions.md#donotremoveplanesonsessionended)
- [preferredDetectorOptions](IWebXRPlaneDetectorOptions.md#preferreddetectoroptions)
- [worldParentNode](IWebXRPlaneDetectorOptions.md#worldparentnode)

## Properties

### doNotRemovePlanesOnSessionEnded

• `Optional` **doNotRemovePlanesOnSessionEnded**: `boolean`

If set to true a reference of the created planes will be kept until the next session starts
If not defined, planes will be removed from the array when the feature is detached or the session ended.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:22

___

### preferredDetectorOptions

• `Optional` **preferredDetectorOptions**: `XRGeometryDetectorOptions`

Preferred detector configuration, not all preferred options will be supported by all platforms.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:26

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

The node to use to transform the local results to world coordinates

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:17

[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRAnchorSystemOptions

# Interface: IWebXRAnchorSystemOptions

Configuration options of the anchor system

## Table of contents

### Properties

- [doNotRemoveAnchorsOnSessionEnded](IWebXRAnchorSystemOptions.md#donotremoveanchorsonsessionended)
- [worldParentNode](IWebXRAnchorSystemOptions.md#worldparentnode)

## Properties

### doNotRemoveAnchorsOnSessionEnded

• `Optional` **doNotRemoveAnchorsOnSessionEnded**: `boolean`

If set to true a reference of the created anchors will be kept until the next session starts
If not defined, anchors will be removed from the array when the feature is detached or the session ended.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:23

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

a node that will be used to convert local to world coordinates

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:17

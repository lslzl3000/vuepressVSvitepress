[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRLegacyHitTestOptions

# Interface: IWebXRLegacyHitTestOptions

Options used for hit testing

## Hierarchy

- **`IWebXRLegacyHitTestOptions`**

  ↳ [`IWebXRHitTestOptions`](IWebXRHitTestOptions.md)

## Table of contents

### Properties

- [testOnPointerDownOnly](IWebXRLegacyHitTestOptions.md#testonpointerdownonly)
- [worldParentNode](IWebXRLegacyHitTestOptions.md#worldparentnode)

## Properties

### testOnPointerDownOnly

• `Optional` **testOnPointerDownOnly**: `boolean`

Only test when user interacted with the scene. Default - hit test every frame

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:29

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

The node to use to transform the local results to world coordinates

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:33

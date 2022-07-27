[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRLegacyHitResult

# Interface: IWebXRLegacyHitResult

Interface defining the babylon result of raycasting/hit-test

## Hierarchy

- **`IWebXRLegacyHitResult`**

  ↳ [`IWebXRHitResult`](IWebXRHitResult.md)

## Table of contents

### Properties

- [transformationMatrix](IWebXRLegacyHitResult.md#transformationmatrix)
- [xrHitResult](IWebXRLegacyHitResult.md#xrhitresult)

## Properties

### transformationMatrix

• **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

Transformation matrix that can be applied to a node that will put it in the hit point location

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:43

___

### xrHitResult

• **xrHitResult**: `XRHitResult` \| `XRHitTestResult`

The native hit test result

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:47

[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRHitResult

# Interface: IWebXRHitResult

Interface defining the babylon result of hit-test

## Hierarchy

- [`IWebXRLegacyHitResult`](IWebXRLegacyHitResult.md)

  ↳ **`IWebXRHitResult`**

## Table of contents

### Properties

- [inputSource](IWebXRHitResult.md#inputsource)
- [isTransient](IWebXRHitResult.md#istransient)
- [position](IWebXRHitResult.md#position)
- [rotationQuaternion](IWebXRHitResult.md#rotationquaternion)
- [transformationMatrix](IWebXRHitResult.md#transformationmatrix)
- [xrHitResult](IWebXRHitResult.md#xrhitresult)

## Properties

### inputSource

• `Optional` **inputSource**: `XRInputSource`

The input source that generated this hit test (if transient)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:53

___

### isTransient

• `Optional` **isTransient**: `boolean`

Is this a transient hit test

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:57

___

### position

• **position**: [`Vector3`](../classes/Vector3.md)

Position of the hit test result

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:61

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](../classes/Quaternion.md)

Rotation of the hit test result

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:65

___

### transformationMatrix

• **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

Transformation matrix that can be applied to a node that will put it in the hit point location

#### Inherited from

[IWebXRLegacyHitResult](IWebXRLegacyHitResult.md).[transformationMatrix](IWebXRLegacyHitResult.md#transformationmatrix)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:43

___

### xrHitResult

• **xrHitResult**: `XRHitTestResult`

The native hit test result

#### Overrides

[IWebXRLegacyHitResult](IWebXRLegacyHitResult.md).[xrHitResult](IWebXRLegacyHitResult.md#xrhitresult)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:70

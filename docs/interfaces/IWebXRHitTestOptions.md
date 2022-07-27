[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRHitTestOptions

# Interface: IWebXRHitTestOptions

Options used for hit testing (version 2)

## Hierarchy

- [`IWebXRLegacyHitTestOptions`](IWebXRLegacyHitTestOptions.md)

  ↳ **`IWebXRHitTestOptions`**

## Table of contents

### Properties

- [disablePermanentHitTest](IWebXRHitTestOptions.md#disablepermanenthittest)
- [enableTransientHitTest](IWebXRHitTestOptions.md#enabletransienthittest)
- [entityTypes](IWebXRHitTestOptions.md#entitytypes)
- [offsetRay](IWebXRHitTestOptions.md#offsetray)
- [testOnPointerDownOnly](IWebXRHitTestOptions.md#testonpointerdownonly)
- [transientHitTestProfile](IWebXRHitTestOptions.md#transienthittestprofile)
- [transientOffsetRay](IWebXRHitTestOptions.md#transientoffsetray)
- [useReferenceSpace](IWebXRHitTestOptions.md#usereferencespace)
- [worldParentNode](IWebXRHitTestOptions.md#worldparentnode)

## Properties

### disablePermanentHitTest

• `Optional` **disablePermanentHitTest**: `boolean`

Do not create a permanent hit test. Will usually be used when only
transient inputs are needed.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:18

___

### enableTransientHitTest

• `Optional` **enableTransientHitTest**: `boolean`

Enable transient (for example touch-based) hit test inspections

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:22

___

### entityTypes

• `Optional` **entityTypes**: `XRHitTestTrackableType`[]

Override the default entity type(s) of the hit-test result

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:43

___

### offsetRay

• `Optional` **offsetRay**: [`Vector3`](../classes/Vector3.md)

Offset ray for the permanent hit test

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:30

___

### testOnPointerDownOnly

• `Optional` **testOnPointerDownOnly**: `boolean`

Only test when user interacted with the scene. Default - hit test every frame

#### Inherited from

[IWebXRLegacyHitTestOptions](IWebXRLegacyHitTestOptions.md).[testOnPointerDownOnly](IWebXRLegacyHitTestOptions.md#testonpointerdownonly)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:29

___

### transientHitTestProfile

• `Optional` **transientHitTestProfile**: `string`

Override the default transient hit test profile (generic-touchscreen).

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:26

___

### transientOffsetRay

• `Optional` **transientOffsetRay**: [`Vector3`](../classes/Vector3.md)

Offset ray for the transient hit test

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:34

___

### useReferenceSpace

• `Optional` **useReferenceSpace**: `boolean`

Instead of using viewer space for hit tests, use the reference space defined in the session manager

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:38

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

The node to use to transform the local results to world coordinates

#### Inherited from

[IWebXRLegacyHitTestOptions](IWebXRLegacyHitTestOptions.md).[worldParentNode](IWebXRLegacyHitTestOptions.md#worldparentnode)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:33

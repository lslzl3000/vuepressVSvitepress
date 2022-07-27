[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRMotionControllerComponentChanges

# Interface: IWebXRMotionControllerComponentChanges

Represents changes in the component between current frame and last values recorded

## Table of contents

### Properties

- [axes](IWebXRMotionControllerComponentChanges.md#axes)
- [pressed](IWebXRMotionControllerComponentChanges.md#pressed)
- [touched](IWebXRMotionControllerComponentChanges.md#touched)
- [value](IWebXRMotionControllerComponentChanges.md#value)

## Properties

### axes

• `Optional` **axes**: [`IWebXRMotionControllerComponentChangesValues`](IWebXRMotionControllerComponentChangesValues.md)[`IWebXRMotionControllerAxesValue`](IWebXRMotionControllerAxesValue.md)

will be populated with previous and current values if axes changed

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:40

___

### pressed

• `Optional` **pressed**: [`IWebXRMotionControllerComponentChangesValues`](IWebXRMotionControllerComponentChangesValues.md)`boolean`

will be populated with previous and current values if pressed changed

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:44

___

### touched

• `Optional` **touched**: [`IWebXRMotionControllerComponentChangesValues`](IWebXRMotionControllerComponentChangesValues.md)`boolean`

will be populated with previous and current values if touched changed

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:48

___

### value

• `Optional` **value**: [`IWebXRMotionControllerComponentChangesValues`](IWebXRMotionControllerComponentChangesValues.md)`number`

will be populated with previous and current values if value changed

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:52

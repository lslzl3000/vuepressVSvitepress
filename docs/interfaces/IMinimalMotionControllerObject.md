[@dev/core](../README.md) / [Exports](../modules.md) / IMinimalMotionControllerObject

# Interface: IMinimalMotionControllerObject

The elements needed for change-detection of the gamepad objects in motion controllers

## Table of contents

### Properties

- [axes](IMinimalMotionControllerObject.md#axes)
- [buttons](IMinimalMotionControllerObject.md#buttons)
- [hapticActuators](IMinimalMotionControllerObject.md#hapticactuators)

## Properties

### axes

• **axes**: `number`[]

Available axes of this controller

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:199

___

### buttons

• **buttons**: { `pressed`: `boolean` ; `touched`: `boolean` ; `value`: `number`  }[]

An array of available buttons

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:203

___

### hapticActuators

• `Optional` **hapticActuators**: { `pulse`: (`value`: `number`, `duration`: `number`) => `Promise``boolean`  }[]

EXPERIMENTAL haptic support.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:221

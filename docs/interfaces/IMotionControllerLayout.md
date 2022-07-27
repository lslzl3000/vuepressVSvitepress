[@dev/core](../README.md) / [Exports](../modules.md) / IMotionControllerLayout

# Interface: IMotionControllerLayout

The schema of motion controller layout.
No object will be initialized using this interface
This is used just to define the profile.

## Table of contents

### Properties

- [assetPath](IMotionControllerLayout.md#assetpath)
- [components](IMotionControllerLayout.md#components)
- [gamepadMapping](IMotionControllerLayout.md#gamepadmapping)
- [rootNodeName](IMotionControllerLayout.md#rootnodename)
- [selectComponentId](IMotionControllerLayout.md#selectcomponentid)

## Properties

### assetPath

• **assetPath**: `string`

Path to load the assets. Usually relative to the base path

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:35

___

### components

• **components**: `Object`

Available components (unsorted)

#### Index signature

▪ [componentId: `string`]: { `gamepadIndices`: { `button?`: `number` ; `xAxis?`: `number` ; `yAxis?`: `number`  } ; `rootNodeName`: `string` ; `touchPointNodeName?`: `string` ; `type`: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) ; `visualResponses`: { `[stateKey: string]`: { `componentProperty`: ``"xAxis"`` \| ``"yAxis"`` \| ``"button"`` \| ``"state"`` ; `maxNodeName?`: `string` ; `minNodeName?`: `string` ; `states`: [`MotionControllerComponentStateType`](../modules.md#motioncontrollercomponentstatetype)[] ; `valueNodeName?`: `string` ; `valueNodeProperty`: ``"transform"`` \| ``"visibility"``  };  }  }

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:39

___

### gamepadMapping

• **gamepadMapping**: ``""`` \| ``"xr-standard"``

Is it xr standard mapping or not

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:109

___

### rootNodeName

• **rootNodeName**: `string`

Base root node of this entire model

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:113

___

### selectComponentId

• **selectComponentId**: `string`

Defines the main button component id

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:117

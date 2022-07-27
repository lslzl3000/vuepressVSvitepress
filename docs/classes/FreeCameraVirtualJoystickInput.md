[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraVirtualJoystickInput

# Class: FreeCameraVirtualJoystickInput

Manage the Virtual Joystick inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraVirtualJoystickInput.md#constructor)

### Properties

- [\_leftjoystick](FreeCameraVirtualJoystickInput.md#_leftjoystick)
- [\_rightjoystick](FreeCameraVirtualJoystickInput.md#_rightjoystick)
- [camera](FreeCameraVirtualJoystickInput.md#camera)

### Methods

- [attachControl](FreeCameraVirtualJoystickInput.md#attachcontrol)
- [checkInputs](FreeCameraVirtualJoystickInput.md#checkinputs)
- [detachControl](FreeCameraVirtualJoystickInput.md#detachcontrol)
- [getClassName](FreeCameraVirtualJoystickInput.md#getclassname)
- [getLeftJoystick](FreeCameraVirtualJoystickInput.md#getleftjoystick)
- [getRightJoystick](FreeCameraVirtualJoystickInput.md#getrightjoystick)
- [getSimpleName](FreeCameraVirtualJoystickInput.md#getsimplename)

## Constructors

### constructor

• **new FreeCameraVirtualJoystickInput**()

## Properties

### \_leftjoystick

• `Private` **\_leftjoystick**: [`VirtualJoystick`](VirtualJoystick.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:38

___

### \_rightjoystick

• `Private` **\_rightjoystick**: [`VirtualJoystick`](VirtualJoystick.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:39

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:36

## Methods

### attachControl

▸ **attachControl**(): `void`

Attach the input controls to a specific dom element to get the input from.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:85

___

### checkInputs

▸ **checkInputs**(): `void`

Update the current camera state depending on the inputs that have been used this frame.
This is a dynamically created lambda to avoid the performance penalty of looping for inputs in the render loop.

#### Returns

`void`

#### Implementation of

ICameraInput.checkInputs

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:61

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:101

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getClassName](../interfaces/ICameraInput.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:110

___

### getLeftJoystick

▸ **getLeftJoystick**(): [`VirtualJoystick`](VirtualJoystick.md)

Gets the left stick of the virtual joystick.

#### Returns

[`VirtualJoystick`](VirtualJoystick.md)

The virtual Joystick

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:45

___

### getRightJoystick

▸ **getRightJoystick**(): [`VirtualJoystick`](VirtualJoystick.md)

Gets the right stick of the virtual joystick.

#### Returns

[`VirtualJoystick`](VirtualJoystick.md)

The virtual Joystick

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:53

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getSimpleName](../interfaces/ICameraInput.md#getsimplename)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:118

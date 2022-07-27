[@dev/core](../README.md) / [Exports](../modules.md) / PoseEnabledControllerHelper

# Class: PoseEnabledControllerHelper

Defines the PoseEnabledControllerHelper object that is used initialize a gamepad as the controller type it is specified as (eg. windows mixed reality controller)

## Table of contents

### Constructors

- [constructor](PoseEnabledControllerHelper.md#constructor)

### Methods

- [InitiateController](PoseEnabledControllerHelper.md#initiatecontroller)

## Constructors

### constructor

• **new PoseEnabledControllerHelper**()

## Methods

### InitiateController

▸ `Static` **InitiateController**(`vrGamepad`): [`Gamepad`](Gamepad.md)

Initializes a gamepad as the controller type it is specified as (eg. windows mixed reality controller)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vrGamepad` | `any` | the gamepad to initialized |

#### Returns

[`Gamepad`](Gamepad.md)

a vr controller of the type the gamepad identified as

#### Defined in

packages/dev/core/src/Gamepads/Controllers/poseEnabledController.ts:114

[@dev/core](../README.md) / [Exports](../modules.md) / WebXRDefaultExperience

# Class: WebXRDefaultExperience

Default experience which provides a similar setup to the previous webVRExperience

## Table of contents

### Constructors

- [constructor](WebXRDefaultExperience.md#constructor)

### Properties

- [baseExperience](WebXRDefaultExperience.md#baseexperience)
- [enterExitUI](WebXRDefaultExperience.md#enterexitui)
- [input](WebXRDefaultExperience.md#input)
- [nearInteraction](WebXRDefaultExperience.md#nearinteraction)
- [pointerSelection](WebXRDefaultExperience.md#pointerselection)
- [renderTarget](WebXRDefaultExperience.md#rendertarget)
- [teleportation](WebXRDefaultExperience.md#teleportation)

### Methods

- [dispose](WebXRDefaultExperience.md#dispose)
- [CreateAsync](WebXRDefaultExperience.md#createasync)

## Constructors

### constructor

• `Private` **new WebXRDefaultExperience**()

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:117

## Properties

### baseExperience

• **baseExperience**: [`WebXRExperienceHelper`](WebXRExperienceHelper.md)

Base experience

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:90

___

### enterExitUI

• **enterExitUI**: [`WebXREnterExitUI`](WebXREnterExitUI.md)

Enables ui for entering/exiting xr

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:94

___

### input

• **input**: [`WebXRInput`](WebXRInput.md)

Input experience extension

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:98

___

### nearInteraction

• **nearInteraction**: [`WebXRNearInteraction`](WebXRNearInteraction.md)

Enables near interaction for hands/controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:115

___

### pointerSelection

• **pointerSelection**: [`WebXRControllerPointerSelection`](WebXRControllerPointerSelection.md)

Enables laser pointer and selection

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:102

___

### renderTarget

• **renderTarget**: [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

Default target xr should render to

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:106

___

### teleportation

• **teleportation**: [`WebXRMotionControllerTeleportation`](WebXRMotionControllerTeleportation.md)

Enables teleportation

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:110

## Methods

### dispose

▸ **dispose**(): `void`

Disposes of the experience helper

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:232

___

### CreateAsync

▸ `Static` **CreateAsync**(`scene`, `options?`): `Promise`[`WebXRDefaultExperience`](WebXRDefaultExperience.md)

Creates the default xr experience

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | scene |
| `options` | [`WebXRDefaultExperienceOptions`](WebXRDefaultExperienceOptions.md) | options for basic configuration |

#### Returns

`Promise`[`WebXRDefaultExperience`](WebXRDefaultExperience.md)

resulting WebXRDefaultExperience

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:125

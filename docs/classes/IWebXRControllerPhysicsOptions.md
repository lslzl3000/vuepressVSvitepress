[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRControllerPhysicsOptions

# Class: IWebXRControllerPhysicsOptions

Options for the controller physics feature

## Table of contents

### Constructors

- [constructor](IWebXRControllerPhysicsOptions.md#constructor)

### Properties

- [enableHeadsetImpostor](IWebXRControllerPhysicsOptions.md#enableheadsetimpostor)
- [headsetImpostorParams](IWebXRControllerPhysicsOptions.md#headsetimpostorparams)
- [physicsProperties](IWebXRControllerPhysicsOptions.md#physicsproperties)
- [xrInput](IWebXRControllerPhysicsOptions.md#xrinput)

## Constructors

### constructor

• **new IWebXRControllerPhysicsOptions**()

## Properties

### enableHeadsetImpostor

• `Optional` **enableHeadsetImpostor**: `boolean`

Should the headset get its own impostor

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPhysics.ts:20

___

### headsetImpostorParams

• `Optional` **headsetImpostorParams**: `Object`

Optional parameters for the headset impostor

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `friction?` | `number` | Friction definitions |
| `impostorSize?` | `number` \| { `depth`: `number` ; `height`: `number` ; `width`: `number`  } | the size of the impostor. Defaults to 10cm |
| `impostorType` | `number` | The type of impostor to create. Default is sphere |
| `restitution?` | `number` | Restitution |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPhysics.ts:24

___

### physicsProperties

• `Optional` **physicsProperties**: `Object`

The physics properties of the future impostors

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `friction?` | `number` | Friction definitions |
| `impostorSize?` | `number` \| { `depth`: `number` ; `height`: `number` ; `width`: `number`  } | the size of the impostor. Defaults to 10cm |
| `impostorType?` | `number` | The type of impostor to create. Default is sphere |
| `restitution?` | `number` | Restitution |
| `useControllerMesh?` | `boolean` | If set to true, a mesh impostor will be created when the controller mesh was loaded  Note that this requires a physics engine that supports mesh impostors! |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPhysics.ts:45

___

### xrInput

• **xrInput**: [`WebXRInput`](WebXRInput.md)

the xr input to use with this pointer selection

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPhysics.ts:71

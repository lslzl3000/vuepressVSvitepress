[@dev/core](../README.md) / [Exports](../modules.md) / GamepadSystemSceneComponent

# Class: GamepadSystemSceneComponent

Defines the gamepad scene component responsible to manage gamepads in a given scene

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](GamepadSystemSceneComponent.md#constructor)

### Properties

- [name](GamepadSystemSceneComponent.md#name)
- [scene](GamepadSystemSceneComponent.md#scene)

### Methods

- [\_beforeCameraUpdate](GamepadSystemSceneComponent.md#_beforecameraupdate)
- [dispose](GamepadSystemSceneComponent.md#dispose)
- [rebuild](GamepadSystemSceneComponent.md#rebuild)
- [register](GamepadSystemSceneComponent.md#register)

## Constructors

### constructor

• **new GamepadSystemSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:102

## Properties

### name

• `Readonly` **name**: ``"Gamepad"``

The component name helpfull to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:91

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:96

## Methods

### \_beforeCameraUpdate

▸ `Private` **_beforeCameraUpdate**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:132

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:124

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:117

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:109

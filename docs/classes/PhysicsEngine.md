[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsEngine

# Class: PhysicsEngine

Class used to control physics engine

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Implements

- [`IPhysicsEngine`](../interfaces/IPhysicsEngine.md)

## Table of contents

### Constructors

- [constructor](PhysicsEngine.md#constructor)

### Properties

- [\_impostors](PhysicsEngine.md#_impostors)
- [\_joints](PhysicsEngine.md#_joints)
- [\_subTimeStep](PhysicsEngine.md#_subtimestep)
- [\_uniqueIdCounter](PhysicsEngine.md#_uniqueidcounter)
- [gravity](PhysicsEngine.md#gravity)
- [Epsilon](PhysicsEngine.md#epsilon)

### Methods

- [\_step](PhysicsEngine.md#_step)
- [addImpostor](PhysicsEngine.md#addimpostor)
- [addJoint](PhysicsEngine.md#addjoint)
- [dispose](PhysicsEngine.md#dispose)
- [getImpostorForPhysicsObject](PhysicsEngine.md#getimpostorforphysicsobject)
- [getImpostorWithPhysicsBody](PhysicsEngine.md#getimpostorwithphysicsbody)
- [getImpostors](PhysicsEngine.md#getimpostors)
- [getPhysicsPlugin](PhysicsEngine.md#getphysicsplugin)
- [getPhysicsPluginName](PhysicsEngine.md#getphysicspluginname)
- [getSubTimeStep](PhysicsEngine.md#getsubtimestep)
- [getTimeStep](PhysicsEngine.md#gettimestep)
- [raycast](PhysicsEngine.md#raycast)
- [removeImpostor](PhysicsEngine.md#removeimpostor)
- [removeJoint](PhysicsEngine.md#removejoint)
- [setGravity](PhysicsEngine.md#setgravity)
- [setSubTimeStep](PhysicsEngine.md#setsubtimestep)
- [setTimeStep](PhysicsEngine.md#settimestep)
- [DefaultPluginFactory](PhysicsEngine.md#defaultpluginfactory)

## Constructors

### constructor

• **new PhysicsEngine**(`gravity`, `_physicsPlugin?`)

Creates a new Physics Engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gravity` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | defines the gravity vector used by the simulation |
| `_physicsPlugin` | `IPhysicsEnginePlugin` | defines the plugin to use (CannonJS by default) |

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:42

## Properties

### \_impostors

• `Private` **\_impostors**: [`PhysicsImpostor`](PhysicsImpostor.md)[] = `[]`

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:19

___

### \_joints

• `Private` **\_joints**: [`PhysicsImpostorJoint`](../interfaces/PhysicsImpostorJoint.md)[] = `[]`

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:20

___

### \_subTimeStep

• `Private` **\_subTimeStep**: `number` = `0`

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:21

___

### \_uniqueIdCounter

• `Private` **\_uniqueIdCounter**: `number` = `0`

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:22

___

### gravity

• **gravity**: [`Vector3`](Vector3.md)

Gets the gravity vector used by the simulation

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[gravity](../interfaces/IPhysicsEngine.md#gravity)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:27

___

### Epsilon

▪ `Static` **Epsilon**: `number` = `0.001`

Global value used to control the smallest number supported by the simulation

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:17

## Methods

### \_step

▸ **_step**(`delta`): `void`

Called by the scene. No need to call it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `delta` | `number` | defines the timespan between frames |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[_step](../interfaces/IPhysicsEngine.md#_step)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:182

___

### addImpostor

▸ **addImpostor**(`impostor`): `void`

Adding a new impostor for the impostor tracking.
This will be done by the impostor itself.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | the impostor to add |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[addImpostor](../interfaces/IPhysicsEngine.md#addimpostor)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:120

___

### addJoint

▸ **addJoint**(`mainImpostor`, `connectedImpostor`, `joint`): `void`

Add a joint to the physics engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mainImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | defines the main impostor to which the joint is added. |
| `connectedImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | defines the impostor that is connected to the main impostor using this joint |
| `joint` | [`PhysicsJoint`](PhysicsJoint.md) | defines the joint that will connect both impostors. |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[addJoint](../interfaces/IPhysicsEngine.md#addjoint)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:151

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[dispose](../interfaces/IPhysicsEngine.md#dispose)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:100

___

### getImpostorForPhysicsObject

▸ **getImpostorForPhysicsObject**(`object`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets the impostor for a physics enabled object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `object` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) | defines the object impersonated by the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

the PhysicsImpostor or null if not found

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getImpostorForPhysicsObject](../interfaces/IPhysicsEngine.md#getimpostorforphysicsobject)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:220

___

### getImpostorWithPhysicsBody

▸ **getImpostorWithPhysicsBody**(`body`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets the impostor for a physics body object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `body` | `any` | defines physics body used by the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

the PhysicsImpostor or null if not found

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getImpostorWithPhysicsBody](../interfaces/IPhysicsEngine.md#getimpostorwithphysicsbody)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:235

___

### getImpostors

▸ **getImpostors**(): [`PhysicsImpostor`](PhysicsImpostor.md)[]

Gets the list of physic impostors

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)[]

an array of PhysicsImpostor

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getImpostors](../interfaces/IPhysicsEngine.md#getimpostors)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:211

___

### getPhysicsPlugin

▸ **getPhysicsPlugin**(): `IPhysicsEnginePlugin`

Gets the current plugin used to run the simulation

#### Returns

`IPhysicsEnginePlugin`

current plugin

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getPhysicsPlugin](../interfaces/IPhysicsEngine.md#getphysicsplugin)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:203

___

### getPhysicsPluginName

▸ **getPhysicsPluginName**(): `string`

Gets the name of the current physics plugin

#### Returns

`string`

the name of the plugin

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getPhysicsPluginName](../interfaces/IPhysicsEngine.md#getphysicspluginname)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:111

___

### getSubTimeStep

▸ **getSubTimeStep**(): `number`

Get the sub time step of the physics engine.

#### Returns

`number`

the current sub time step

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getSubTimeStep](../interfaces/IPhysicsEngine.md#getsubtimestep)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:93

___

### getTimeStep

▸ **getTimeStep**(): `number`

Get the time step of the physics engine.

#### Returns

`number`

the current time step

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[getTimeStep](../interfaces/IPhysicsEngine.md#gettimestep)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:75

___

### raycast

▸ **raycast**(`from`, `to`): `PhysicsRaycastResult`

Does a raycast in the physics world

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | [`Vector3`](Vector3.md) | when should the ray start? |
| `to` | [`Vector3`](Vector3.md) | when should the ray end? |

#### Returns

`PhysicsRaycastResult`

PhysicsRaycastResult

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[raycast](../interfaces/IPhysicsEngine.md#raycast)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:251

___

### removeImpostor

▸ **removeImpostor**(`impostor`): `void`

Remove an impostor from the engine.
This impostor and its mesh will not longer be updated by the physics engine.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | the impostor to remove |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[removeImpostor](../interfaces/IPhysicsEngine.md#removeimpostor)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:134

___

### removeJoint

▸ **removeJoint**(`mainImpostor`, `connectedImpostor`, `joint`): `void`

Removes a joint from the simulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mainImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | defines the impostor used with the joint |
| `connectedImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | defines the other impostor connected to the main one by the joint |
| `joint` | [`PhysicsJoint`](PhysicsJoint.md) | defines the joint to remove |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[removeJoint](../interfaces/IPhysicsEngine.md#removejoint)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:168

___

### setGravity

▸ **setGravity**(`gravity`): `void`

Sets the gravity vector used by the simulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gravity` | [`Vector3`](Vector3.md) | defines the gravity vector to use |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[setGravity](../interfaces/IPhysicsEngine.md#setgravity)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:55

___

### setSubTimeStep

▸ **setSubTimeStep**(`subTimeStep?`): `void`

Set the sub time step of the physics engine.
Default is 0 meaning there is no sub steps
To increase physics resolution precision, set a small value (like 1 ms)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `subTimeStep` | `number` | `0` | defines the new sub timestep used for physics resolution. |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[setSubTimeStep](../interfaces/IPhysicsEngine.md#setsubtimestep)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:85

___

### setTimeStep

▸ **setTimeStep**(`newTimeStep?`): `void`

Set the time step of the physics engine.
Default is 1/60.
To slow it down, enter 1/600 for example.
To speed it up, 1/30

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTimeStep` | `number` | defines the new timestep to apply to this world. |

#### Returns

`void`

#### Implementation of

[IPhysicsEngine](../interfaces/IPhysicsEngine.md).[setTimeStep](../interfaces/IPhysicsEngine.md#settimestep)

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:67

___

### DefaultPluginFactory

▸ `Static` **DefaultPluginFactory**(): `IPhysicsEnginePlugin`

Factory used to create the default physics plugin.

#### Returns

`IPhysicsEnginePlugin`

The default physics plugin

#### Defined in

packages/dev/core/src/Physics/physicsEngine.ts:33

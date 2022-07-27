[@dev/core](../README.md) / [Exports](../modules.md) / IPhysicsEngine

# Interface: IPhysicsEngine

Interface used to define a physics engine

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Implemented by

- [`PhysicsEngine`](../classes/PhysicsEngine.md)

## Table of contents

### Properties

- [gravity](IPhysicsEngine.md#gravity)

### Methods

- [\_step](IPhysicsEngine.md#_step)
- [addImpostor](IPhysicsEngine.md#addimpostor)
- [addJoint](IPhysicsEngine.md#addjoint)
- [dispose](IPhysicsEngine.md#dispose)
- [getImpostorForPhysicsObject](IPhysicsEngine.md#getimpostorforphysicsobject)
- [getImpostorWithPhysicsBody](IPhysicsEngine.md#getimpostorwithphysicsbody)
- [getImpostors](IPhysicsEngine.md#getimpostors)
- [getPhysicsPlugin](IPhysicsEngine.md#getphysicsplugin)
- [getPhysicsPluginName](IPhysicsEngine.md#getphysicspluginname)
- [getSubTimeStep](IPhysicsEngine.md#getsubtimestep)
- [getTimeStep](IPhysicsEngine.md#gettimestep)
- [raycast](IPhysicsEngine.md#raycast)
- [removeImpostor](IPhysicsEngine.md#removeimpostor)
- [removeJoint](IPhysicsEngine.md#removejoint)
- [setGravity](IPhysicsEngine.md#setgravity)
- [setSubTimeStep](IPhysicsEngine.md#setsubtimestep)
- [setTimeStep](IPhysicsEngine.md#settimestep)

## Properties

### gravity

• **gravity**: [`Vector3`](../classes/Vector3.md)

Gets the gravity vector used by the simulation

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:78

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

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:194

___

### addImpostor

▸ **addImpostor**(`impostor`): `void`

Adding a new impostor for the impostor tracking.
This will be done by the impostor itself.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | the impostor to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:131

___

### addJoint

▸ **addJoint**(`mainImpostor`, `connectedImpostor`, `joint`): `void`

Add a joint to the physics engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mainImpostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | defines the main impostor to which the joint is added. |
| `connectedImpostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | defines the impostor that is connected to the main impostor using this joint |
| `joint` | [`PhysicsJoint`](../classes/PhysicsJoint.md) | defines the joint that will connect both impostors. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:146

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:118

___

### getImpostorForPhysicsObject

▸ **getImpostorForPhysicsObject**(`object`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](../classes/PhysicsImpostor.md)

Gets the impostor for a physics enabled object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `object` | [`IPhysicsEnabledObject`](IPhysicsEnabledObject.md) | defines the object impersonated by the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](../classes/PhysicsImpostor.md)

the PhysicsImpostor or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:173

___

### getImpostorWithPhysicsBody

▸ **getImpostorWithPhysicsBody**(`body`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](../classes/PhysicsImpostor.md)

Gets the impostor for a physics body object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `body` | `any` | defines physics body used by the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](../classes/PhysicsImpostor.md)

the PhysicsImpostor or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:180

___

### getImpostors

▸ **getImpostors**(): [`PhysicsImpostor`](../classes/PhysicsImpostor.md)[]

Gets the list of physic impostors

#### Returns

[`PhysicsImpostor`](../classes/PhysicsImpostor.md)[]

an array of PhysicsImpostor

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:166

___

### getPhysicsPlugin

▸ **getPhysicsPlugin**(): `IPhysicsEnginePlugin`

Gets the current plugin used to run the simulation

#### Returns

`IPhysicsEnginePlugin`

current plugin

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:160

___

### getPhysicsPluginName

▸ **getPhysicsPluginName**(): `string`

Gets the name of the current physics plugin

#### Returns

`string`

the name of the plugin

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:124

___

### getSubTimeStep

▸ **getSubTimeStep**(): `number`

Get the sub time step of the physics engine.

#### Returns

`number`

the current sub time step

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:113

___

### getTimeStep

▸ **getTimeStep**(): `number`

Get the time step of the physics engine.

#### Returns

`number`

the current time step

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:99

___

### raycast

▸ **raycast**(`from`, `to`): `PhysicsRaycastResult`

Does a raycast in the physics world

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | [`Vector3`](../classes/Vector3.md) | when should the ray start? |
| `to` | [`Vector3`](../classes/Vector3.md) | when should the ray end? |

#### Returns

`PhysicsRaycastResult`

PhysicsRaycastResult

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:188

___

### removeImpostor

▸ **removeImpostor**(`impostor`): `void`

Remove an impostor from the engine.
This impostor and its mesh will not longer be updated by the physics engine.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | the impostor to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:138

___

### removeJoint

▸ **removeJoint**(`mainImpostor`, `connectedImpostor`, `joint`): `void`

Removes a joint from the simulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mainImpostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | defines the impostor used with the joint |
| `connectedImpostor` | [`PhysicsImpostor`](../classes/PhysicsImpostor.md) | defines the other impostor connected to the main one by the joint |
| `joint` | [`PhysicsJoint`](../classes/PhysicsJoint.md) | defines the joint to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:154

___

### setGravity

▸ **setGravity**(`gravity`): `void`

Sets the gravity vector used by the simulation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gravity` | [`Vector3`](../classes/Vector3.md) | defines the gravity vector to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:84

___

### setSubTimeStep

▸ **setSubTimeStep**(`subTimeStep`): `void`

Set the sub time step of the physics engine.
Default is 0 meaning there is no sub steps
To increase physics resolution precision, set a small value (like 1 ms)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subTimeStep` | `number` | defines the new sub timestep used for physics resolution. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:107

___

### setTimeStep

▸ **setTimeStep**(`newTimeStep`): `void`

Set the time step of the physics engine.
Default is 1/60.
To slow it down, enter 1/600 for example.
To speed it up, 1/30

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTimeStep` | `number` | the new timestep to apply to this world. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/IPhysicsEngine.ts:93

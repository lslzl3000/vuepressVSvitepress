[@dev/core](../README.md) / [Exports](../modules.md) / AmmoJSPlugin

# Class: AmmoJSPlugin

AmmoJS Physics plugin

**`See`**

 - https://doc.babylonjs.com/how_to/using_the_physics_engine
 - https://github.com/kripken/ammo.js/

## Implements

- `IPhysicsEnginePlugin`

## Table of contents

### Constructors

- [constructor](AmmoJSPlugin.md#constructor)

### Properties

- [\_collisionConfiguration](AmmoJSPlugin.md#_collisionconfiguration)
- [\_dispatcher](AmmoJSPlugin.md#_dispatcher)
- [\_fixedTimeStep](AmmoJSPlugin.md#_fixedtimestep)
- [\_maxSteps](AmmoJSPlugin.md#_maxsteps)
- [\_overlappingPairCache](AmmoJSPlugin.md#_overlappingpaircache)
- [\_raycastResult](AmmoJSPlugin.md#_raycastresult)
- [\_softBodySolver](AmmoJSPlugin.md#_softbodysolver)
- [\_solver](AmmoJSPlugin.md#_solver)
- [\_timeStep](AmmoJSPlugin.md#_timestep)
- [\_tmpAmmoConcreteContactResultCallback](AmmoJSPlugin.md#_tmpammoconcretecontactresultcallback)
- [\_tmpAmmoQuaternion](AmmoJSPlugin.md#_tmpammoquaternion)
- [\_tmpAmmoTransform](AmmoJSPlugin.md#_tmpammotransform)
- [\_tmpAmmoVectorA](AmmoJSPlugin.md#_tmpammovectora)
- [\_tmpAmmoVectorB](AmmoJSPlugin.md#_tmpammovectorb)
- [\_tmpAmmoVectorC](AmmoJSPlugin.md#_tmpammovectorc)
- [\_tmpAmmoVectorD](AmmoJSPlugin.md#_tmpammovectord)
- [\_tmpAmmoVectorRCA](AmmoJSPlugin.md#_tmpammovectorrca)
- [\_tmpAmmoVectorRCB](AmmoJSPlugin.md#_tmpammovectorrcb)
- [\_tmpContactCallbackResult](AmmoJSPlugin.md#_tmpcontactcallbackresult)
- [\_tmpContactPoint](AmmoJSPlugin.md#_tmpcontactpoint)
- [\_tmpMatrix](AmmoJSPlugin.md#_tmpmatrix)
- [\_tmpQuaternion](AmmoJSPlugin.md#_tmpquaternion)
- [\_tmpVec3](AmmoJSPlugin.md#_tmpvec3)
- [bjsAMMO](AmmoJSPlugin.md#bjsammo)
- [name](AmmoJSPlugin.md#name)
- [onCreateCustomConvexHullImpostor](AmmoJSPlugin.md#oncreatecustomconvexhullimpostor)
- [onCreateCustomMeshImpostor](AmmoJSPlugin.md#oncreatecustommeshimpostor)
- [onCreateCustomShape](AmmoJSPlugin.md#oncreatecustomshape)
- [world](AmmoJSPlugin.md#world)
- [\_DISABLE\_COLLISION\_FLAG](AmmoJSPlugin.md#_disable_collision_flag)
- [\_DISABLE\_DEACTIVATION\_FLAG](AmmoJSPlugin.md#_disable_deactivation_flag)
- [\_KINEMATIC\_FLAG](AmmoJSPlugin.md#_kinematic_flag)

### Methods

- [\_addHullVerts](AmmoJSPlugin.md#_addhullverts)
- [\_addMeshVerts](AmmoJSPlugin.md#_addmeshverts)
- [\_afterSoftStep](AmmoJSPlugin.md#_aftersoftstep)
- [\_createCloth](AmmoJSPlugin.md#_createcloth)
- [\_createCustom](AmmoJSPlugin.md#_createcustom)
- [\_createRope](AmmoJSPlugin.md#_createrope)
- [\_createShape](AmmoJSPlugin.md#_createshape)
- [\_createSoftbody](AmmoJSPlugin.md#_createsoftbody)
- [\_isImpostorInContact](AmmoJSPlugin.md#_isimpostorincontact)
- [\_isImpostorPairInContact](AmmoJSPlugin.md#_isimpostorpairincontact)
- [\_ropeStep](AmmoJSPlugin.md#_ropestep)
- [\_softVertexData](AmmoJSPlugin.md#_softvertexdata)
- [\_softbodyOrClothStep](AmmoJSPlugin.md#_softbodyorclothstep)
- [\_stepSimulation](AmmoJSPlugin.md#_stepsimulation)
- [appendAnchor](AmmoJSPlugin.md#appendanchor)
- [appendHook](AmmoJSPlugin.md#appendhook)
- [applyForce](AmmoJSPlugin.md#applyforce)
- [applyImpulse](AmmoJSPlugin.md#applyimpulse)
- [dispose](AmmoJSPlugin.md#dispose)
- [executeStep](AmmoJSPlugin.md#executestep)
- [generateJoint](AmmoJSPlugin.md#generatejoint)
- [generatePhysicsBody](AmmoJSPlugin.md#generatephysicsbody)
- [getAngularVelocity](AmmoJSPlugin.md#getangularvelocity)
- [getBodyFriction](AmmoJSPlugin.md#getbodyfriction)
- [getBodyMass](AmmoJSPlugin.md#getbodymass)
- [getBodyPositionIterations](AmmoJSPlugin.md#getbodypositioniterations)
- [getBodyPressure](AmmoJSPlugin.md#getbodypressure)
- [getBodyRestitution](AmmoJSPlugin.md#getbodyrestitution)
- [getBodyStiffness](AmmoJSPlugin.md#getbodystiffness)
- [getBodyVelocityIterations](AmmoJSPlugin.md#getbodyvelocityiterations)
- [getBoxSizeToRef](AmmoJSPlugin.md#getboxsizetoref)
- [getLinearVelocity](AmmoJSPlugin.md#getlinearvelocity)
- [getRadius](AmmoJSPlugin.md#getradius)
- [getTimeStep](AmmoJSPlugin.md#gettimestep)
- [isSupported](AmmoJSPlugin.md#issupported)
- [raycast](AmmoJSPlugin.md#raycast)
- [removeJoint](AmmoJSPlugin.md#removejoint)
- [removePhysicsBody](AmmoJSPlugin.md#removephysicsbody)
- [setAngularVelocity](AmmoJSPlugin.md#setangularvelocity)
- [setBodyFriction](AmmoJSPlugin.md#setbodyfriction)
- [setBodyMass](AmmoJSPlugin.md#setbodymass)
- [setBodyPositionIterations](AmmoJSPlugin.md#setbodypositioniterations)
- [setBodyPressure](AmmoJSPlugin.md#setbodypressure)
- [setBodyRestitution](AmmoJSPlugin.md#setbodyrestitution)
- [setBodyStiffness](AmmoJSPlugin.md#setbodystiffness)
- [setBodyVelocityIterations](AmmoJSPlugin.md#setbodyvelocityiterations)
- [setFixedTimeStep](AmmoJSPlugin.md#setfixedtimestep)
- [setGravity](AmmoJSPlugin.md#setgravity)
- [setLimit](AmmoJSPlugin.md#setlimit)
- [setLinearVelocity](AmmoJSPlugin.md#setlinearvelocity)
- [setMaxSteps](AmmoJSPlugin.md#setmaxsteps)
- [setMotor](AmmoJSPlugin.md#setmotor)
- [setPhysicsBodyTransformation](AmmoJSPlugin.md#setphysicsbodytransformation)
- [setTimeStep](AmmoJSPlugin.md#settimestep)
- [setTransformationFromPhysicsBody](AmmoJSPlugin.md#settransformationfromphysicsbody)
- [sleepBody](AmmoJSPlugin.md#sleepbody)
- [syncMeshWithImpostor](AmmoJSPlugin.md#syncmeshwithimpostor)
- [updateDistanceJoint](AmmoJSPlugin.md#updatedistancejoint)
- [wakeUpBody](AmmoJSPlugin.md#wakeupbody)

## Constructors

### constructor

• **new AmmoJSPlugin**(`_useDeltaForWorldStep?`, `ammoInjection?`, `overlappingPairCache?`)

Initializes the ammoJS plugin

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `_useDeltaForWorldStep` | `boolean` | `true` | if the time between frames should be used when calculating physics steps (Default: true) |
| `ammoInjection` | `any` | `Ammo` | can be used to inject your own ammo reference |
| `overlappingPairCache` | `any` | `null` | can be used to specify your own overlapping pair cache |

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:75

## Properties

### \_collisionConfiguration

• `Private` **\_collisionConfiguration**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:49

___

### \_dispatcher

• `Private` **\_dispatcher**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:50

___

### \_fixedTimeStep

• `Private` **\_fixedTimeStep**: `number`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:43

___

### \_maxSteps

• `Private` **\_maxSteps**: `number` = `5`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:44

___

### \_overlappingPairCache

• `Private` **\_overlappingPairCache**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:51

___

### \_raycastResult

• `Private` **\_raycastResult**: `PhysicsRaycastResult`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:61

___

### \_softBodySolver

• `Private` **\_softBodySolver**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:53

___

### \_solver

• `Private` **\_solver**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:52

___

### \_timeStep

• `Private` **\_timeStep**: `number`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:42

___

### \_tmpAmmoConcreteContactResultCallback

• `Private` **\_tmpAmmoConcreteContactResultCallback**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:48

___

### \_tmpAmmoQuaternion

• `Private` **\_tmpAmmoQuaternion**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:47

___

### \_tmpAmmoTransform

• `Private` **\_tmpAmmoTransform**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:46

___

### \_tmpAmmoVectorA

• `Private` **\_tmpAmmoVectorA**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:54

___

### \_tmpAmmoVectorB

• `Private` **\_tmpAmmoVectorB**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:55

___

### \_tmpAmmoVectorC

• `Private` **\_tmpAmmoVectorC**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:56

___

### \_tmpAmmoVectorD

• `Private` **\_tmpAmmoVectorD**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:57

___

### \_tmpAmmoVectorRCA

• `Private` **\_tmpAmmoVectorRCA**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:59

___

### \_tmpAmmoVectorRCB

• `Private` **\_tmpAmmoVectorRCB**: `any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:60

___

### \_tmpContactCallbackResult

• `Private` **\_tmpContactCallbackResult**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:58

___

### \_tmpContactPoint

• `Private` **\_tmpContactPoint**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:62

___

### \_tmpMatrix

• `Private` **\_tmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:350

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:45

___

### \_tmpVec3

• `Private` **\_tmpVec3**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:63

___

### bjsAMMO

• **bjsAMMO**: `any` = `{}`

Reference to the Ammo library

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:32

___

### name

• **name**: `string` = `"AmmoJSPlugin"`

Name of the plugin

#### Implementation of

IPhysicsEnginePlugin.name

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:40

___

### onCreateCustomConvexHullImpostor

• **onCreateCustomConvexHullImpostor**: (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `any`

#### Type declaration

▸ (`impostor`): `any`

The create custom convex hull impostor handler function to support building custom convex hull impostor vertex data

##### Parameters

| Name | Type |
| :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:173

___

### onCreateCustomMeshImpostor

• **onCreateCustomMeshImpostor**: (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `any`

#### Type declaration

▸ (`impostor`): `any`

The create custom mesh impostor handler function to support building custom mesh impostor vertex data

##### Parameters

| Name | Type |
| :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:168

___

### onCreateCustomShape

• **onCreateCustomShape**: (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `any`

#### Type declaration

▸ (`impostor`): `any`

The create custom shape handler function to be called when using BABYLON.PhysicsImposter.CustomImpostor

##### Parameters

| Name | Type |
| :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:163

___

### world

• **world**: `any`

Created ammoJS world which physics bodies are added to

#### Implementation of

IPhysicsEnginePlugin.world

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:36

___

### \_DISABLE\_COLLISION\_FLAG

▪ `Static` `Private` `Readonly` **\_DISABLE\_COLLISION\_FLAG**: ``4``

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:65

___

### \_DISABLE\_DEACTIVATION\_FLAG

▪ `Static` `Private` `Readonly` **\_DISABLE\_DEACTIVATION\_FLAG**: ``4``

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:67

___

### \_KINEMATIC\_FLAG

▪ `Static` `Private` `Readonly` **\_KINEMATIC\_FLAG**: ``2``

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:66

## Methods

### \_addHullVerts

▸ `Private` **_addHullVerts**(`btConvexHullShape`, `topLevelObject`, `object`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `btConvexHullShape` | `any` |
| `topLevelObject` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) |
| `object` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:894

___

### \_addMeshVerts

▸ `Private` **_addMeshVerts**(`btTriangleMesh`, `topLevelObject`, `object`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `btTriangleMesh` | `any` |
| `topLevelObject` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) |
| `object` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:608

___

### \_afterSoftStep

▸ `Private` **_afterSoftStep**(`impostor`): `void`

Update babylon mesh to match physics world object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to match |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:260

___

### \_createCloth

▸ `Private` **_createCloth**(`impostor`): `any`

Create cloth for an impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | to create the softbody for |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:782

___

### \_createCustom

▸ `Private` **_createCustom**(`impostor`): `any`

Create a custom physics impostor shape using the plugin's onCreateCustomShape handler

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | to create the custom physics shape for |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:882

___

### \_createRope

▸ `Private` **_createRope**(`impostor`): `any`

Create rope for an impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | to create the softbody for |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:826

___

### \_createShape

▸ `Private` **_createShape**(`impostor`, `ignoreChildren?`): `any`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | `undefined` |
| `ignoreChildren` | `boolean` | `false` |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:945

___

### \_createSoftbody

▸ `Private` **_createSoftbody**(`impostor`): `any`

Create an impostor's soft body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | to create the softbody for |

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:737

___

### \_isImpostorInContact

▸ `Private` **_isImpostorInContact**(`impostor`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:176

___

### \_isImpostorPairInContact

▸ `Private` **_isImpostorPairInContact**(`impostorA`, `impostorB`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `impostorA` | [`PhysicsImpostor`](PhysicsImpostor.md) |
| `impostorB` | [`PhysicsImpostor`](PhysicsImpostor.md) |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:184

___

### \_ropeStep

▸ `Private` **_ropeStep**(`impostor`): `void`

Update babylon mesh vertices vertices to match physics world softbody or cloth

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to match |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:272

___

### \_softVertexData

▸ `Private` **_softVertexData**(`impostor`): [`VertexData`](VertexData.md)

Initialise the soft body vertices to match its object's (mesh) vertices
Softbody vertices (nodes) are in world space and to match this
The object's position and rotation is set to zero and so its vertices are also then set in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | to create the softbody for |

#### Returns

[`VertexData`](VertexData.md)

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:684

___

### \_softbodyOrClothStep

▸ `Private` **_softbodyOrClothStep**(`impostor`): `void`

Update babylon mesh vertices vertices to match physics world softbody or cloth

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to match |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:300

___

### \_stepSimulation

▸ `Private` **_stepSimulation**(`timeStep?`, `maxSteps?`, `fixedTimeStep?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `timeStep` | `number` | `undefined` |
| `maxSteps` | `number` | `10` |
| `fixedTimeStep` | `number` | `undefined` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:196

___

### appendAnchor

▸ **appendAnchor**(`impostor`, `otherImpostor`, `width`, `height`, `influence?`, `noCollisionBetweenLinkedBodies?`): `void`

Append an anchor to a cloth object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | `undefined` | is the cloth impostor to add anchor to |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | `undefined` | is the rigid impostor to anchor to |
| `width` | `number` | `undefined` | ratio across width from 0 to 1 |
| `height` | `number` | `undefined` | ratio up height from 0 to 1 |
| `influence` | `number` | `1` | the elasticity between cloth impostor and anchor from 0, very stretchy to 1, little stretch |
| `noCollisionBetweenLinkedBodies` | `boolean` | `false` | when true collisions between soft impostor and anchor are ignored; default false |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.appendAnchor

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1433

___

### appendHook

▸ **appendHook**(`impostor`, `otherImpostor`, `length`, `influence?`, `noCollisionBetweenLinkedBodies?`): `void`

Append an hook to a rope object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | `undefined` | is the rope impostor to add hook to |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | `undefined` | is the rigid impostor to hook to |
| `length` | `number` | `undefined` | ratio along the rope from 0 to 1 |
| `influence` | `number` | `1` | the elasticity between soft impostor and anchor from 0, very stretchy to 1, little stretch |
| `noCollisionBetweenLinkedBodies` | `boolean` | `false` | when true collisions between soft impostor and anchor are ignored; default false |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.appendHook

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1457

___

### applyForce

▸ **applyForce**(`impostor`, `force`, `contactPoint`): `void`

Applies a force on the imposter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to apply force |
| `force` | [`Vector3`](Vector3.md) | amount of force to be applied to the imposter |
| `contactPoint` | [`Vector3`](Vector3.md) | the location to apply the force on the imposter |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.applyForce

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:383

___

### applyImpulse

▸ **applyImpulse**(`impostor`, `force`, `contactPoint`): `void`

Applies an impulse on the imposter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to apply impulse to |
| `force` | [`Vector3`](Vector3.md) | amount of force to be applied to the imposter |
| `contactPoint` | [`Vector3`](Vector3.md) | the location to apply the impulse on the imposter |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.applyImpulse

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:357

___

### dispose

▸ **dispose**(): `void`

Disposes of the impostor

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.dispose

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1549

___

### executeStep

▸ **executeStep**(`delta`, `impostors`): `void`

Moves the physics simulation forward delta seconds and updates the given physics imposters
Prior to the step the imposters physics location is set to the position of the babylon meshes
After the step the babylon meshes are set to the position of the physics imposters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `delta` | `number` | amount of time to step forward |
| `impostors` | [`PhysicsImpostor`](PhysicsImpostor.md)[] | array of imposters to update before/after the step |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.executeStep

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:220

___

### generateJoint

▸ **generateJoint**(`impostorJoint`): `void`

Generates a joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostorJoint` | [`PhysicsImpostorJoint`](../interfaces/PhysicsImpostorJoint.md) | the imposter joint to create the joint with |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.generateJoint

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:525

___

### generatePhysicsBody

▸ **generatePhysicsBody**(`impostor`): `void`

Creates a physics body using the plugin

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | the imposter to create the physics body on |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.generatePhysicsBody

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:409

___

### getAngularVelocity

▸ **getAngularVelocity**(`impostor`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

gets the angular velocity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to get angular velocity from |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

angular velocity

#### Implementation of

IPhysicsEnginePlugin.getAngularVelocity

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1226

___

### getBodyFriction

▸ **getBodyFriction**(`impostor`): `number`

Gets friction of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get friction from |

#### Returns

`number`

friction value

#### Implementation of

IPhysicsEnginePlugin.getBodyFriction

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1269

___

### getBodyMass

▸ **getBodyMass**(`impostor`): `number`

Gets the mass of the physics body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to get the mass from |

#### Returns

`number`

mass

#### Implementation of

IPhysicsEnginePlugin.getBodyMass

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1260

___

### getBodyPositionIterations

▸ **getBodyPositionIterations**(`impostor`): `number`

Gets positionIterations of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get position iterations from |

#### Returns

`number`

positionIterations value

#### Implementation of

IPhysicsEnginePlugin.getBodyPositionIterations

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1401

___

### getBodyPressure

▸ **getBodyPressure**(`impostor`): `number`

Gets pressure inside the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get pressure from |

#### Returns

`number`

pressure value

#### Implementation of

IPhysicsEnginePlugin.getBodyPressure

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1311

___

### getBodyRestitution

▸ **getBodyRestitution**(`impostor`): `number`

Gets restitution of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get restitution from |

#### Returns

`number`

restitution value

#### Implementation of

IPhysicsEnginePlugin.getBodyRestitution

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1292

___

### getBodyStiffness

▸ **getBodyStiffness**(`impostor`): `number`

Gets stiffness of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get stiffness from |

#### Returns

`number`

pressure value

#### Implementation of

IPhysicsEnginePlugin.getBodyStiffness

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1344

___

### getBodyVelocityIterations

▸ **getBodyVelocityIterations**(`impostor`): `number`

Gets velocityIterations of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get velocity iterations from |

#### Returns

`number`

velocityIterations value

#### Implementation of

IPhysicsEnginePlugin.getBodyVelocityIterations

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1373

___

### getBoxSizeToRef

▸ **getBoxSizeToRef**(`impostor`, `result`): `void`

Gets the box size of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get box size from |
| `result` | [`Vector3`](Vector3.md) | the resulting box size |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.getBoxSizeToRef

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1539

___

### getLinearVelocity

▸ **getLinearVelocity**(`impostor`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

gets the linear velocity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to get linear velocity from |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

linear velocity

#### Implementation of

IPhysicsEnginePlugin.getLinearVelocity

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1206

___

### getRadius

▸ **getRadius**(`impostor`): `number`

Gets the radius of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to get radius from |

#### Returns

`number`

the radius

#### Implementation of

IPhysicsEnginePlugin.getRadius

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1529

___

### getTimeStep

▸ **getTimeStep**(): `number`

Gets the current timestep (only used if useDeltaForWorldStep is false in the constructor)

#### Returns

`number`

the current timestep in seconds

#### Implementation of

IPhysicsEnginePlugin.getTimeStep

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:156

___

### isSupported

▸ **isSupported**(): `boolean`

If this plugin is supported

#### Returns

`boolean`

true if its supported

#### Implementation of

IPhysicsEnginePlugin.isSupported

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1169

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

IPhysicsEnginePlugin.raycast

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1574

___

### removeJoint

▸ **removeJoint**(`impostorJoint`): `void`

Removes a joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostorJoint` | [`PhysicsImpostorJoint`](../interfaces/PhysicsImpostorJoint.md) | the imposter joint to remove the joint from |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.removeJoint

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:601

___

### removePhysicsBody

▸ **removePhysicsBody**(`impostor`): `void`

Removes the physics body from the imposter and disposes of the body's memory

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to remove the physics body from |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.removePhysicsBody

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:504

___

### setAngularVelocity

▸ **setAngularVelocity**(`impostor`, `velocity`): `void`

Sets the angular velocity of the physics body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to set the velocity on |
| `velocity` | [`Vector3`](Vector3.md) | velocity to set |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setAngularVelocity

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1192

___

### setBodyFriction

▸ **setBodyFriction**(`impostor`, `friction`): `void`

Sets friction of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set friction on |
| `friction` | `number` | friction value |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyFriction

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1278

___

### setBodyMass

▸ **setBodyMass**(`impostor`, `mass`): `void`

Sets the mass of physics body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to set the mass on |
| `mass` | `number` | mass to set |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyMass

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1246

___

### setBodyPositionIterations

▸ **setBodyPositionIterations**(`impostor`, `positionIterations`): `void`

Sets positionIterations of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set position on |
| `positionIterations` | `number` | positionIterations value |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyPositionIterations

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1414

___

### setBodyPressure

▸ **setBodyPressure**(`impostor`, `pressure`): `void`

Sets pressure inside a soft body impostor
Cloth and rope must remain 0 pressure

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set pressure on |
| `pressure` | `number` | pressure value |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyPressure

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1325

___

### setBodyRestitution

▸ **setBodyRestitution**(`impostor`, `restitution`): `void`

Sets restitution of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set resitution on |
| `restitution` | `number` | resitution value |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyRestitution

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1301

___

### setBodyStiffness

▸ **setBodyStiffness**(`impostor`, `stiffness`): `void`

Sets stiffness of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set stiffness on |
| `stiffness` | `number` | stiffness value from 0 to 1 |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyStiffness

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1357

___

### setBodyVelocityIterations

▸ **setBodyVelocityIterations**(`impostor`, `velocityIterations`): `void`

Sets velocityIterations of the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to set velocity iterations on |
| `velocityIterations` | `number` | velocityIterations value |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setBodyVelocityIterations

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1386

___

### setFixedTimeStep

▸ **setFixedTimeStep**(`fixedTimeStep`): `void`

Increment to step forward in the physics engine (If timeStep is set to 1/60 and fixedTimeStep is set to 1/120 the physics engine should run 2 steps per frame) (Default: 1/60)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fixedTimeStep` | `number` | fixedTimeStep to use in seconds |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:140

___

### setGravity

▸ **setGravity**(`gravity`): `void`

Sets the gravity of the physics world (m/(s^2))

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gravity` | [`Vector3`](Vector3.md) | Gravity to set |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setGravity

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:122

___

### setLimit

▸ **setLimit**(): `void`

Sets the motors limit

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setLimit

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1498

___

### setLinearVelocity

▸ **setLinearVelocity**(`impostor`, `velocity`): `void`

Sets the linear velocity of the physics body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter to set the velocity on |
| `velocity` | [`Vector3`](Vector3.md) | velocity to set |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setLinearVelocity

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1178

___

### setMaxSteps

▸ **setMaxSteps**(`maxSteps`): `void`

Sets the maximum number of steps by the physics engine per frame (Default: 5)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxSteps` | `number` | the maximum number of steps by the physics engine per frame |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:148

___

### setMotor

▸ **setMotor**(`joint`, `speed?`, `maxForce?`): `void`

Sets a motor on the joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `joint` | [`IMotorEnabledJoint`](../interfaces/IMotorEnabledJoint.md) | joint to set motor on |
| `speed?` | `number` | speed of the motor |
| `maxForce?` | `number` | maximum force of the motor |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setMotor

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1491

___

### setPhysicsBodyTransformation

▸ **setPhysicsBodyTransformation**(`impostor`, `newPosition`, `newRotation`): `void`

Sets the babylon object's position/rotation from the physics body's position/rotation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter containing the physics body and babylon object |
| `newPosition` | [`Vector3`](Vector3.md) | new position |
| `newRotation` | [`Quaternion`](Quaternion.md) | new rotation |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setPhysicsBodyTransformation

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1133

___

### setTimeStep

▸ **setTimeStep**(`timeStep`): `void`

Amount of time to step forward on each frame (only used if useDeltaForWorldStep is false in the constructor)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `timeStep` | `number` | timestep to use in seconds |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setTimeStep

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:132

___

### setTransformationFromPhysicsBody

▸ **setTransformationFromPhysicsBody**(`impostor`): `void`

Sets the physics body position/rotation from the babylon mesh's position/rotation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | imposter containing the physics body and babylon object |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.setTransformationFromPhysicsBody

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1103

___

### sleepBody

▸ **sleepBody**(`impostor`): `void`

Sleeps the physics body and stops it from being active

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to sleep |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.sleepBody

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1466

___

### syncMeshWithImpostor

▸ **syncMeshWithImpostor**(`mesh`, `impostor`): `void`

Syncs the position and rotation of a mesh with the impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | mesh to sync |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to update the mesh with |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.syncMeshWithImpostor

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1507

___

### updateDistanceJoint

▸ **updateDistanceJoint**(): `void`

Updates the distance parameters of the joint

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.updateDistanceJoint

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1481

___

### wakeUpBody

▸ **wakeUpBody**(`impostor`): `void`

Activates the physics body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | impostor to activate |

#### Returns

`void`

#### Implementation of

IPhysicsEnginePlugin.wakeUpBody

#### Defined in

packages/dev/core/src/Physics/Plugins/ammoJSPlugin.ts:1474

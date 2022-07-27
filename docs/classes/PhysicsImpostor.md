[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsImpostor

# Class: PhysicsImpostor

Represents a physics imposter

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Table of contents

### Constructors

- [constructor](PhysicsImpostor.md#constructor)

### Properties

- [\_bodyUpdateRequired](PhysicsImpostor.md#_bodyupdaterequired)
- [\_deltaPosition](PhysicsImpostor.md#_deltaposition)
- [\_deltaRotation](PhysicsImpostor.md#_deltarotation)
- [\_deltaRotationConjugated](PhysicsImpostor.md#_deltarotationconjugated)
- [\_isDisposed](PhysicsImpostor.md#_isdisposed)
- [\_joints](PhysicsImpostor.md#_joints)
- [\_onAfterPhysicsStepCallbacks](PhysicsImpostor.md#_onafterphysicsstepcallbacks)
- [\_onBeforePhysicsStepCallbacks](PhysicsImpostor.md#_onbeforephysicsstepcallbacks)
- [\_parent](PhysicsImpostor.md#_parent)
- [\_physicsBody](PhysicsImpostor.md#_physicsbody)
- [\_physicsEngine](PhysicsImpostor.md#_physicsengine)
- [\_tmpQuat](PhysicsImpostor.md#_tmpquat)
- [\_tmpQuat2](PhysicsImpostor.md#_tmpquat2)
- [object](PhysicsImpostor.md#object)
- [onCollideEvent](PhysicsImpostor.md#oncollideevent)
- [type](PhysicsImpostor.md#type)
- [uniqueId](PhysicsImpostor.md#uniqueid)
- [BoxImpostor](PhysicsImpostor.md#boximpostor)
- [CapsuleImpostor](PhysicsImpostor.md#capsuleimpostor)
- [ClothImpostor](PhysicsImpostor.md#clothimpostor)
- [ConvexHullImpostor](PhysicsImpostor.md#convexhullimpostor)
- [CustomImpostor](PhysicsImpostor.md#customimpostor)
- [CylinderImpostor](PhysicsImpostor.md#cylinderimpostor)
- [DEFAULT\_OBJECT\_SIZE](PhysicsImpostor.md#default_object_size)
- [HeightmapImpostor](PhysicsImpostor.md#heightmapimpostor)
- [IDENTITY\_QUATERNION](PhysicsImpostor.md#identity_quaternion)
- [MeshImpostor](PhysicsImpostor.md#meshimpostor)
- [NoImpostor](PhysicsImpostor.md#noimpostor)
- [ParticleImpostor](PhysicsImpostor.md#particleimpostor)
- [PlaneImpostor](PhysicsImpostor.md#planeimpostor)
- [RopeImpostor](PhysicsImpostor.md#ropeimpostor)
- [SoftbodyImpostor](PhysicsImpostor.md#softbodyimpostor)
- [SphereImpostor](PhysicsImpostor.md#sphereimpostor)
- [\_TmpQuat](PhysicsImpostor.md#_tmpquat-1)
- [\_TmpVecs](PhysicsImpostor.md#_tmpvecs)

### Accessors

- [friction](PhysicsImpostor.md#friction)
- [isDisposed](PhysicsImpostor.md#isdisposed)
- [mass](PhysicsImpostor.md#mass)
- [parent](PhysicsImpostor.md#parent)
- [physicsBody](PhysicsImpostor.md#physicsbody)
- [positionIterations](PhysicsImpostor.md#positioniterations)
- [pressure](PhysicsImpostor.md#pressure)
- [restitution](PhysicsImpostor.md#restitution)
- [stiffness](PhysicsImpostor.md#stiffness)
- [velocityIterations](PhysicsImpostor.md#velocityiterations)

### Methods

- [\_getPhysicsParent](PhysicsImpostor.md#_getphysicsparent)
- [addAnchor](PhysicsImpostor.md#addanchor)
- [addHook](PhysicsImpostor.md#addhook)
- [addJoint](PhysicsImpostor.md#addjoint)
- [afterStep](PhysicsImpostor.md#afterstep)
- [applyForce](PhysicsImpostor.md#applyforce)
- [applyImpulse](PhysicsImpostor.md#applyimpulse)
- [beforeStep](PhysicsImpostor.md#beforestep)
- [clone](PhysicsImpostor.md#clone)
- [createJoint](PhysicsImpostor.md#createjoint)
- [dispose](PhysicsImpostor.md#dispose)
- [executeNativeFunction](PhysicsImpostor.md#executenativefunction)
- [forceUpdate](PhysicsImpostor.md#forceupdate)
- [getAngularVelocity](PhysicsImpostor.md#getangularvelocity)
- [getBoxSizeToRef](PhysicsImpostor.md#getboxsizetoref)
- [getLinearVelocity](PhysicsImpostor.md#getlinearvelocity)
- [getObjectCenter](PhysicsImpostor.md#getobjectcenter)
- [getObjectExtendSize](PhysicsImpostor.md#getobjectextendsize)
- [getParam](PhysicsImpostor.md#getparam)
- [getParentsRotation](PhysicsImpostor.md#getparentsrotation)
- [getRadius](PhysicsImpostor.md#getradius)
- [isBodyInitRequired](PhysicsImpostor.md#isbodyinitrequired)
- [onCollide](PhysicsImpostor.md#oncollide)
- [registerAfterPhysicsStep](PhysicsImpostor.md#registerafterphysicsstep)
- [registerBeforePhysicsStep](PhysicsImpostor.md#registerbeforephysicsstep)
- [registerOnPhysicsCollide](PhysicsImpostor.md#registeronphysicscollide)
- [resetUpdateFlags](PhysicsImpostor.md#resetupdateflags)
- [setAngularVelocity](PhysicsImpostor.md#setangularvelocity)
- [setDeltaPosition](PhysicsImpostor.md#setdeltaposition)
- [setDeltaRotation](PhysicsImpostor.md#setdeltarotation)
- [setLinearVelocity](PhysicsImpostor.md#setlinearvelocity)
- [setMass](PhysicsImpostor.md#setmass)
- [setParam](PhysicsImpostor.md#setparam)
- [setScalingUpdated](PhysicsImpostor.md#setscalingupdated)
- [sleep](PhysicsImpostor.md#sleep)
- [syncBoneWithImpostor](PhysicsImpostor.md#syncbonewithimpostor)
- [syncImpostorWithBone](PhysicsImpostor.md#syncimpostorwithbone)
- [unregisterAfterPhysicsStep](PhysicsImpostor.md#unregisterafterphysicsstep)
- [unregisterBeforePhysicsStep](PhysicsImpostor.md#unregisterbeforephysicsstep)
- [unregisterOnPhysicsCollide](PhysicsImpostor.md#unregisteronphysicscollide)
- [wakeUp](PhysicsImpostor.md#wakeup)

## Constructors

### constructor

• **new PhysicsImpostor**(`object`, `type`, `_options?`, `_scene?`)

Initializes the physics imposter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `object` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) | The physics-enabled object used as the physics imposter |
| `type` | `number` | The type of the physics imposter. Types are available as static members of this class. |
| `_options` | [`PhysicsImpostorParameters`](../interfaces/PhysicsImpostorParameters.md) | The options for the physics imposter |
| `_scene?` | [`Scene`](Scene.md) | The Babylon scene |

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:439

## Properties

### \_bodyUpdateRequired

• `Private` **\_bodyUpdateRequired**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:222

___

### \_deltaPosition

• `Private` **\_deltaPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:232

___

### \_deltaRotation

• `Private` **\_deltaRotation**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:233

___

### \_deltaRotationConjugated

• `Private` **\_deltaRotationConjugated**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:234

___

### \_isDisposed

• `Private` **\_isDisposed**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:242

___

### \_joints

• `Private` **\_joints**: { `joint`: [`PhysicsJoint`](PhysicsJoint.md) ; `otherImpostor`: [`PhysicsImpostor`](PhysicsImpostor.md)  }[]

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:427

___

### \_onAfterPhysicsStepCallbacks

• `Private` **\_onAfterPhysicsStepCallbacks**: (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void`[]

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:225

___

### \_onBeforePhysicsStepCallbacks

• `Private` **\_onBeforePhysicsStepCallbacks**: (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void`[]

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:224

___

### \_parent

• `Private` **\_parent**: [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:240

___

### \_physicsBody

• `Private` **\_physicsBody**: `any`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:221

___

### \_physicsEngine

• `Private` **\_physicsEngine**: [`Nullable`](../modules.md#nullable)[`IPhysicsEngine`](../interfaces/IPhysicsEngine.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:219

___

### \_tmpQuat

• `Private` **\_tmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:825

___

### \_tmpQuat2

• `Private` **\_tmpQuat2**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:826

___

### object

• **object**: [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:443

___

### onCollideEvent

• **onCollideEvent**: [`Nullable`](../modules.md#nullable)(`collider`: [`PhysicsImpostor`](PhysicsImpostor.md), `collidedWith`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void` = `null`

Legacy collision detection event support

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:904

___

### type

• **type**: `number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:447

___

### uniqueId

• **uniqueId**: `number`

The unique id of the physics imposter
set by the physics engine when adding this impostor to the array

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:415

___

### BoxImpostor

▪ `Static` **BoxImpostor**: `number` = `2`

Box-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1263

___

### CapsuleImpostor

▪ `Static` **CapsuleImpostor**: `number` = `6`

Capsule-Impostor type (Ammo.js plugin only)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1275

___

### ClothImpostor

▪ `Static` **ClothImpostor**: `number` = `102`

Cloth-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1303

___

### ConvexHullImpostor

▪ `Static` **ConvexHullImpostor**: `number` = `10`

ConvexHull-Impostor type (Ammo.js plugin only)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1291

___

### CustomImpostor

▪ `Static` **CustomImpostor**: `number` = `100`

Custom-Imposter type (Ammo.js plugin only)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1295

___

### CylinderImpostor

▪ `Static` **CylinderImpostor**: `number` = `7`

Cylinder-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1279

___

### DEFAULT\_OBJECT\_SIZE

▪ `Static` **DEFAULT\_OBJECT\_SIZE**: [`Vector3`](Vector3.md)

The default object size of the imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:209

___

### HeightmapImpostor

▪ `Static` **HeightmapImpostor**: `number` = `9`

Heightmap-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1287

___

### IDENTITY\_QUATERNION

▪ `Static` **IDENTITY\_QUATERNION**: [`Quaternion`](Quaternion.md)

The identity quaternion of the imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:214

___

### MeshImpostor

▪ `Static` **MeshImpostor**: `number` = `4`

Mesh-imposter type (Only available to objects with vertices data)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1271

___

### NoImpostor

▪ `Static` **NoImpostor**: `number` = `0`

No-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1255

___

### ParticleImpostor

▪ `Static` **ParticleImpostor**: `number` = `8`

Particle-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1283

___

### PlaneImpostor

▪ `Static` **PlaneImpostor**: `number` = `3`

Plane-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1267

___

### RopeImpostor

▪ `Static` **RopeImpostor**: `number` = `101`

Rope-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1299

___

### SoftbodyImpostor

▪ `Static` **SoftbodyImpostor**: `number` = `103`

Softbody-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1307

___

### SphereImpostor

▪ `Static` **SphereImpostor**: `number` = `1`

Sphere-Imposter type

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1259

___

### \_TmpQuat

▪ `Static` `Private` **\_TmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:245

___

### \_TmpVecs

▪ `Static` `Private` **\_TmpVecs**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:244

## Accessors

### friction

• `get` **friction**(): `number`

Gets the coefficient of friction

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:268

• `set` **friction**(`value`): `void`

Sets the coefficient of friction

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:275

___

### isDisposed

• `get` **isDisposed**(): `boolean`

Specifies if the physics imposter is disposed

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:250

___

### mass

• `get` **mass**(): `number`

Gets the mass of the physics imposter

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:257

• `set` **mass**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:261

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Get the parent of the physics imposter

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Physics imposter or null

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:581

• `set` **parent**(`value`): `void`

Sets the parent of the physics imposter

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:588

___

### physicsBody

• `get` **physicsBody**(): `any`

Gets the body that holds this impostor. Either its own, or its parent.

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:573

• `set` **physicsBody**(`physicsBody`): `void`

Set the physics body. Used mainly by the physics engine/plugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `physicsBody` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:595

___

### positionIterations

• `get` **positionIterations**(): `number`

Gets the positionIterations of a soft body; only supported by the AmmoJSPlugin

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:386

• `set` **positionIterations**(`value`): `void`

Sets the positionIterations of a soft body; only supported by the AmmoJSPlugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:400

___

### pressure

• `get` **pressure**(): `number`

Gets the pressure of a soft body; only supported by the AmmoJSPlugin

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:302

• `set` **pressure**(`value`): `void`

Sets the pressure of a soft body; only supported by the AmmoJSPlugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:316

___

### restitution

• `get` **restitution**(): `number`

Gets the coefficient of restitution

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:285

• `set` **restitution**(`value`): `void`

Sets the coefficient of restitution

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:292

___

### stiffness

• `get` **stiffness**(): `number`

Gets the stiffness of a soft body; only supported by the AmmoJSPlugin

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:330

• `set` **stiffness**(`value`): `void`

Sets the stiffness of a soft body; only supported by the AmmoJSPlugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:344

___

### velocityIterations

• `get` **velocityIterations**(): `number`

Gets the velocityIterations of a soft body; only supported by the AmmoJSPlugin

#### Returns

`number`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:358

• `set` **velocityIterations**(`value`): `void`

Sets the velocityIterations of a soft body; only supported by the AmmoJSPlugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:372

## Methods

### \_getPhysicsParent

▸ `Private` **_getPhysicsParent**(): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:532

___

### addAnchor

▸ **addAnchor**(`otherImpostor`, `width`, `height`, `influence`, `noCollisionBetweenLinkedBodies`): [`PhysicsImpostor`](PhysicsImpostor.md)

Add an anchor to a cloth impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | rigid impostor to anchor to |
| `width` | `number` | ratio across width from 0 to 1 |
| `height` | `number` | ratio up height from 0 to 1 |
| `influence` | `number` | the elasticity between cloth impostor and anchor from 0, very stretchy to 1, little stretch |
| `noCollisionBetweenLinkedBodies` | `boolean` | when true collisions between cloth impostor and anchor are ignored; default false |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

impostor the soft imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1005

___

### addHook

▸ **addHook**(`otherImpostor`, `length`, `influence`, `noCollisionBetweenLinkedBodies`): [`PhysicsImpostor`](PhysicsImpostor.md)

Add a hook to a rope impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | rigid impostor to anchor to |
| `length` | `number` | ratio across rope from 0 to 1 |
| `influence` | `number` | the elasticity between rope impostor and anchor from 0, very stretchy to 1, little stretch |
| `noCollisionBetweenLinkedBodies` | `boolean` | when true collisions between soft impostor and anchor are ignored; default false |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

impostor the rope imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1027

___

### addJoint

▸ **addJoint**(`otherImpostor`, `joint`): [`PhysicsImpostor`](PhysicsImpostor.md)

Add a joint to this impostor with a different impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | A physics imposter used to add a joint |
| `joint` | [`PhysicsJoint`](PhysicsJoint.md) | The joint to add |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:983

___

### afterStep

▸ **afterStep**(): `void`

this function is executed by the physics engine

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:879

___

### applyForce

▸ **applyForce**(`force`, `contactPoint`): [`PhysicsImpostor`](PhysicsImpostor.md)

Apply a force

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force` | [`Vector3`](Vector3.md) | The force to apply |
| `contactPoint` | [`Vector3`](Vector3.md) | The contact point for the force |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:942

___

### applyImpulse

▸ **applyImpulse**(`force`, `contactPoint`): [`PhysicsImpostor`](PhysicsImpostor.md)

Apply an impulse

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force` | [`Vector3`](Vector3.md) | The impulse force |
| `contactPoint` | [`Vector3`](Vector3.md) | The contact point for the impulse force |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:955

___

### beforeStep

▸ **beforeStep**(): `void`

this function is executed by the physics engine.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:850

___

### clone

▸ **clone**(`newObject`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Clones the physics imposter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newObject` | [`IPhysicsEnabledObject`](../interfaces/IPhysicsEnabledObject.md) | The physics imposter clones to this physics-enabled object |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

A nullable physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1070

___

### createJoint

▸ **createJoint**(`otherImpostor`, `jointType`, `jointData`): [`PhysicsImpostor`](PhysicsImpostor.md)

A help function to create a joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherImpostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | A physics imposter used to create a joint |
| `jointType` | `number` | The type of joint |
| `jointData` | [`PhysicsJointData`](../interfaces/PhysicsJointData.md) | The data for the joint |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:970

___

### dispose

▸ **dispose**(): `void`

Disposes the physics imposter

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1080

___

### executeNativeFunction

▸ **executeNativeFunction**(`func`): `void`

Execute a function with the physics plugin native code
Provide a function the will have two variables - the world object and the physics body object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`world`: `any`, `physicsBody`: `any`) => `void` | The function to execute with the physics plugin native code |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:728

___

### forceUpdate

▸ **forceUpdate**(): `void`

Force a regeneration of this or the parent's impostor's body.
Use under cautious - This will remove all joints already implemented.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:559

___

### getAngularVelocity

▸ **getAngularVelocity**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the angular velocity

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

angular velocity or null

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:708

___

### getBoxSizeToRef

▸ **getBoxSizeToRef**(`result`): [`PhysicsImpostor`](PhysicsImpostor.md)

Gets the box size of the physics imposter and stores the result in the input parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | Stores the box size |

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1134

___

### getLinearVelocity

▸ **getLinearVelocity**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the linear velocity

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

linear velocity or null

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:690

___

### getObjectCenter

▸ **getObjectCenter**(): [`Vector3`](Vector3.md)

Gets the object center

#### Returns

[`Vector3`](Vector3.md)

The object center

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:645

___

### getObjectExtendSize

▸ **getObjectExtendSize**(): [`Vector3`](Vector3.md)

Gets the object extend size

#### Returns

[`Vector3`](Vector3.md)

the object extend size

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:614

___

### getParam

▸ **getParam**(`paramName`): `any`

Get a specific parameter from the options parameters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `paramName` | `string` | The object parameter name |

#### Returns

`any`

The object parameter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:659

___

### getParentsRotation

▸ **getParentsRotation**(): [`Quaternion`](Quaternion.md)

Get the parent rotation

#### Returns

[`Quaternion`](Quaternion.md)

The parent rotation

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:832

___

### getRadius

▸ **getRadius**(): `number`

Gets the radius of the physics imposter

#### Returns

`number`

Radius of the physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1146

___

### isBodyInitRequired

▸ **isBodyInitRequired**(): `boolean`

Should a new body be generated.

#### Returns

`boolean`

boolean specifying if body initialization is required

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:544

___

### onCollide

▸ **onCollide**(`e`): `void`

event and body object due to cannon's event-based architecture.

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `Object` |
| `e.body` | `any` |
| `e.point` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:912

___

### registerAfterPhysicsStep

▸ **registerAfterPhysicsStep**(`func`): `void`

Register a function that will be executed after the physics step

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void` | The function to execute after physics step |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:760

___

### registerBeforePhysicsStep

▸ **registerBeforePhysicsStep**(`func`): `void`

Register a function that will be executed before the physics world is stepping forward

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void` | The function to execute before the physics world is stepped forward |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:738

___

### registerOnPhysicsCollide

▸ **registerOnPhysicsCollide**(`collideAgainst`, `func`): `void`

register a function that will be executed when this impostor collides against a different body

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `collideAgainst` | [`PhysicsImpostor`](PhysicsImpostor.md) \| [`PhysicsImpostor`](PhysicsImpostor.md)[] | Physics imposter, or array of physics imposters to collide against |
| `func` | (`collider`: [`PhysicsImpostor`](PhysicsImpostor.md), `collidedAgainst`: [`PhysicsImpostor`](PhysicsImpostor.md), `point`: [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)) => `void` | Callback that is executed on collision |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:783

___

### resetUpdateFlags

▸ **resetUpdateFlags**(): `void`

Resets the update flags

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:606

___

### setAngularVelocity

▸ **setAngularVelocity**(`velocity`): `void`

Sets the angular velocity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `velocity` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | The velocity or null |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:716

___

### setDeltaPosition

▸ **setDeltaPosition**(`position`): `void`

Sets the delta position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | The delta position amount |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1113

___

### setDeltaRotation

▸ **setDeltaRotation**(`rotation`): `void`

Sets the delta rotation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rotation` | [`Quaternion`](Quaternion.md) | The delta rotation amount |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1121

___

### setLinearVelocity

▸ **setLinearVelocity**(`velocity`): `void`

Sets the linear velocity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `velocity` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | linear velocity or null |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:698

___

### setMass

▸ **setMass**(`mass`): `void`

Specifically change the body's mass option. Won't recreate the physics body object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mass` | `number` | The mass of the physics imposter |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:677

___

### setParam

▸ **setParam**(`paramName`, `value`): `void`

Sets a specific parameter in the options given to the physics plugin

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `paramName` | `string` | The parameter name |
| `value` | `number` | The value of the parameter |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:668

___

### setScalingUpdated

▸ **setScalingUpdated**(): `void`

Sets the updated scaling

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:551

___

### sleep

▸ **sleep**(): [`PhysicsImpostor`](PhysicsImpostor.md)

Will keep this body still, in a sleep mode.

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

the physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1045

___

### syncBoneWithImpostor

▸ **syncBoneWithImpostor**(`bone`, `boneMesh`, `jointPivot`, `distToJoint?`, `adjustRotation?`): `void`

Sync a bone with this impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bone` | [`Bone`](Bone.md) | The bone to sync to the impostor. |
| `boneMesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh that the bone is influencing. |
| `jointPivot` | [`Vector3`](Vector3.md) | The pivot of the joint / bone in local space. |
| `distToJoint?` | `number` | Optional distance from the impostor to the joint. |
| `adjustRotation?` | [`Quaternion`](Quaternion.md) | Optional quaternion for adjusting the local rotation of the bone. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1158

___

### syncImpostorWithBone

▸ **syncImpostorWithBone**(`bone`, `boneMesh`, `jointPivot`, `distToJoint?`, `adjustRotation?`, `boneAxis?`): `void`

Sync impostor to a bone

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bone` | [`Bone`](Bone.md) | The bone that the impostor will be synced to. |
| `boneMesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh that the bone is influencing. |
| `jointPivot` | [`Vector3`](Vector3.md) | The pivot of the joint / bone in local space. |
| `distToJoint?` | `number` | Optional distance from the impostor to the joint. |
| `adjustRotation?` | [`Quaternion`](Quaternion.md) | Optional quaternion for adjusting the local rotation of the bone. |
| `boneAxis?` | [`Vector3`](Vector3.md) | Optional vector3 axis the bone is aligned with |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1212

___

### unregisterAfterPhysicsStep

▸ **unregisterAfterPhysicsStep**(`func`): `void`

Unregisters a function that will be executed after the physics step

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void` | The function to execute after physics step |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:768

___

### unregisterBeforePhysicsStep

▸ **unregisterBeforePhysicsStep**(`func`): `void`

Unregister a function that will be executed before the physics world is stepping forward

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`impostor`: [`PhysicsImpostor`](PhysicsImpostor.md)) => `void` | The function to execute before the physics world is stepped forward |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:746

___

### unregisterOnPhysicsCollide

▸ **unregisterOnPhysicsCollide**(`collideAgainst`, `func`): `void`

Unregisters the physics imposter on contact

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `collideAgainst` | [`PhysicsImpostor`](PhysicsImpostor.md) \| [`PhysicsImpostor`](PhysicsImpostor.md)[] | The physics object to collide against |
| `func` | (`collider`: [`PhysicsImpostor`](PhysicsImpostor.md), `collidedAgainst`: [`PhysicsImpostor`](PhysicsImpostor.md) \| [`PhysicsImpostor`](PhysicsImpostor.md)[], `point`: [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)) => `void` | Callback to execute on collision |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:796

___

### wakeUp

▸ **wakeUp**(): [`PhysicsImpostor`](PhysicsImpostor.md)

Wake the body up.

#### Returns

[`PhysicsImpostor`](PhysicsImpostor.md)

The physics imposter

#### Defined in

packages/dev/core/src/Physics/physicsImpostor.ts:1057

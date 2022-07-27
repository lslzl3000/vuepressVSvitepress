[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsHelper

# Class: PhysicsHelper

A helper for physics simulations

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine#further-functionality-of-the-impostor-class

## Table of contents

### Constructors

- [constructor](PhysicsHelper.md#constructor)

### Properties

- [\_physicsEngine](PhysicsHelper.md#_physicsengine)
- [\_scene](PhysicsHelper.md#_scene)

### Methods

- [applyRadialExplosionForce](PhysicsHelper.md#applyradialexplosionforce)
- [applyRadialExplosionImpulse](PhysicsHelper.md#applyradialexplosionimpulse)
- [gravitationalField](PhysicsHelper.md#gravitationalfield)
- [updraft](PhysicsHelper.md#updraft)
- [vortex](PhysicsHelper.md#vortex)

## Constructors

### constructor

• **new PhysicsHelper**(`scene`)

Initializes the Physics helper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Babylon.js scene |

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:26

## Properties

### \_physicsEngine

• `Private` **\_physicsEngine**: [`Nullable`](../modules.md#nullable)[`IPhysicsEngine`](../interfaces/IPhysicsEngine.md)

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:20

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:19

## Methods

### applyRadialExplosionForce

▸ **applyRadialExplosionForce**(`origin`, `radiusOrEventOptions`, `strength?`, `falloff?`): [`Nullable`](../modules.md#nullable)`PhysicsRadialExplosionEvent`

Applies a radial explosion force

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | the origin of the explosion |
| `radiusOrEventOptions` | `number` \| [`PhysicsRadialExplosionEventOptions`](PhysicsRadialExplosionEventOptions.md) | the radius or the options of radial explosion |
| `strength?` | `number` | the explosion strength |
| `falloff?` | [`PhysicsRadialImpulseFalloff`](../enums/PhysicsRadialImpulseFalloff.md) | possible options: Constant & Linear. Defaults to Constant |

#### Returns

[`Nullable`](../modules.md#nullable)`PhysicsRadialExplosionEvent`

A physics radial explosion event, or null

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:99

___

### applyRadialExplosionImpulse

▸ **applyRadialExplosionImpulse**(`origin`, `radiusOrEventOptions`, `strength?`, `falloff?`): [`Nullable`](../modules.md#nullable)`PhysicsRadialExplosionEvent`

Applies a radial explosion impulse

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | the origin of the explosion |
| `radiusOrEventOptions` | `number` \| [`PhysicsRadialExplosionEventOptions`](PhysicsRadialExplosionEventOptions.md) | the radius or the options of radial explosion |
| `strength?` | `number` | the explosion strength |
| `falloff?` | [`PhysicsRadialImpulseFalloff`](../enums/PhysicsRadialImpulseFalloff.md) | possible options: Constant & Linear. Defaults to Constant |

#### Returns

[`Nullable`](../modules.md#nullable)`PhysicsRadialExplosionEvent`

A physics radial explosion event, or null

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:44

___

### gravitationalField

▸ **gravitationalField**(`origin`, `radiusOrEventOptions`, `strength?`, `falloff?`): [`Nullable`](../modules.md#nullable)`PhysicsGravitationalFieldEvent`

Creates a gravitational field

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | the origin of the explosion |
| `radiusOrEventOptions` | `number` \| [`PhysicsRadialExplosionEventOptions`](PhysicsRadialExplosionEventOptions.md) | the radius or the options of radial explosion |
| `strength?` | `number` | the explosion strength |
| `falloff?` | [`PhysicsRadialImpulseFalloff`](../enums/PhysicsRadialImpulseFalloff.md) | possible options: Constant & Linear. Defaults to Constant |

#### Returns

[`Nullable`](../modules.md#nullable)`PhysicsGravitationalFieldEvent`

A physics gravitational field event, or null

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:154

___

### updraft

▸ **updraft**(`origin`, `radiusOrEventOptions`, `strength?`, `height?`, `updraftMode?`): [`Nullable`](../modules.md#nullable)`PhysicsUpdraftEvent`

Creates a physics updraft event

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | the origin of the updraft |
| `radiusOrEventOptions` | `number` \| [`PhysicsUpdraftEventOptions`](PhysicsUpdraftEventOptions.md) | the radius or the options of the updraft |
| `strength?` | `number` | the strength of the updraft |
| `height?` | `number` | the height of the updraft |
| `updraftMode?` | [`PhysicsUpdraftMode`](../enums/PhysicsUpdraftMode.md) | possible options: Center & Perpendicular. Defaults to Center |

#### Returns

[`Nullable`](../modules.md#nullable)`PhysicsUpdraftEvent`

A physics updraft event, or null

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:193

___

### vortex

▸ **vortex**(`origin`, `radiusOrEventOptions`, `strength?`, `height?`): [`Nullable`](../modules.md#nullable)`PhysicsVortexEvent`

Creates a physics vortex event

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `origin` | [`Vector3`](Vector3.md) | the of the vortex |
| `radiusOrEventOptions` | `number` \| [`PhysicsVortexEventOptions`](PhysicsVortexEventOptions.md) | the radius or the options of the vortex |
| `strength?` | `number` | the strength of the vortex |
| `height?` | `number` | the height of the vortex |

#### Returns

[`Nullable`](../modules.md#nullable)`PhysicsVortexEvent`

a Physics vortex event, or null
A physics vortex event or null

#### Defined in

packages/dev/core/src/Physics/physicsHelper.ts:233

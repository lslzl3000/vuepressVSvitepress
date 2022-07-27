[@dev/core](../README.md) / [Exports](../modules.md) / Behavior

# Interface: BehaviorT

Interface used to define a behavior

## Type parameters

| Name |
| :------ |
| `T` |

## Implemented by

- [`AttachToBoxBehavior`](../classes/AttachToBoxBehavior.md)
- [`AutoRotationBehavior`](../classes/AutoRotationBehavior.md)
- [`BaseSixDofDragBehavior`](../classes/BaseSixDofDragBehavior.md)
- [`BouncingBehavior`](../classes/BouncingBehavior.md)
- [`FadeInOutBehavior`](../classes/FadeInOutBehavior.md)
- [`FollowBehavior`](../classes/FollowBehavior.md)
- [`FramingBehavior`](../classes/FramingBehavior.md)
- [`HandConstraintBehavior`](../classes/HandConstraintBehavior.md)
- [`MultiPointerScaleBehavior`](../classes/MultiPointerScaleBehavior.md)
- [`PointerDragBehavior`](../classes/PointerDragBehavior.md)
- [`SurfaceMagnetismBehavior`](../classes/SurfaceMagnetismBehavior.md)

## Table of contents

### Properties

- [name](Behavior.md#name)

### Methods

- [attach](Behavior.md#attach)
- [detach](Behavior.md#detach)
- [init](Behavior.md#init)

## Properties

### name

• **name**: `string`

gets or sets behavior's name

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:8

## Methods

### attach

▸ **attach**(`target`): `void`

Called when the behavior is attached to a target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `T` | defines the target where the behavior is attached to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:18

___

### detach

▸ **detach**(): `void`

Called when the behavior is detached from its target

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:22

___

### init

▸ **init**(): `void`

Function called when the behavior needs to be initialized (after attaching it to a target)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/behavior.ts:13

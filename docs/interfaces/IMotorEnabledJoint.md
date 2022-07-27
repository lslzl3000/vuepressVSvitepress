[@dev/core](../README.md) / [Exports](../modules.md) / IMotorEnabledJoint

# Interface: IMotorEnabledJoint

Interface for a motor enabled joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Implemented by

- [`MotorEnabledJoint`](../classes/MotorEnabledJoint.md)

## Table of contents

### Properties

- [physicsJoint](IMotorEnabledJoint.md#physicsjoint)

### Methods

- [setLimit](IMotorEnabledJoint.md#setlimit)
- [setMotor](IMotorEnabledJoint.md#setmotor)

## Properties

### physicsJoint

• **physicsJoint**: `any`

Physics joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:286

## Methods

### setLimit

▸ **setLimit**(`upperLimit`, `lowerLimit?`, `motorIndex?`): `void`

Sets the limit of the motor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `upperLimit` | `number` | The upper limit of the motor |
| `lowerLimit?` | `number` | The lower limit of the motor |
| `motorIndex?` | `number` | The index of the motor |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:300

___

### setMotor

▸ **setMotor**(`force?`, `maxForce?`, `motorIndex?`): `void`

Sets the motor of the motor-enabled joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `number` | The force of the motor |
| `maxForce?` | `number` | The maximum force of the motor |
| `motorIndex?` | `number` | The index of the motor |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:293

[@dev/core](../README.md) / [Exports](../modules.md) / TrajectoryClassifier

# Class: TrajectoryClassifier

Class representing a set of known, named trajectories to which Trajectories can be
added and using which Trajectories can be recognized.

## Table of contents

### Constructors

- [constructor](TrajectoryClassifier.md#constructor)

### Properties

- [\_levenshteinAlphabet](TrajectoryClassifier.md#_levenshteinalphabet)
- [\_maximumAllowableMatchCost](TrajectoryClassifier.md#_maximumallowablematchcost)
- [\_nameToDescribedTrajectory](TrajectoryClassifier.md#_nametodescribedtrajectory)
- [\_vector3Alphabet](TrajectoryClassifier.md#_vector3alphabet)

### Methods

- [addTrajectoryToClassification](TrajectoryClassifier.md#addtrajectorytoclassification)
- [classifyTrajectory](TrajectoryClassifier.md#classifytrajectory)
- [deleteClassification](TrajectoryClassifier.md#deleteclassification)
- [serialize](TrajectoryClassifier.md#serialize)
- [Deserialize](TrajectoryClassifier.md#deserialize)
- [Generate](TrajectoryClassifier.md#generate)

## Constructors

### constructor

• `Private` **new TrajectoryClassifier**()

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:789

## Properties

### \_levenshteinAlphabet

• `Private` **\_levenshteinAlphabet**: `Alphabet``number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:722

___

### \_maximumAllowableMatchCost

• `Private` **\_maximumAllowableMatchCost**: `number` = `4`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:720

___

### \_nameToDescribedTrajectory

• `Private` **\_nameToDescribedTrajectory**: `Map``string`, `TrajectoryClass`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:723

___

### \_vector3Alphabet

• `Private` **\_vector3Alphabet**: `Vector3Alphabet`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:721

## Methods

### addTrajectoryToClassification

▸ **addTrajectoryToClassification**(`trajectory`, `classification`): `void`

Add a new Trajectory to the set with a given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trajectory` | [`Trajectory`](Trajectory.md) | new Trajectory to be added |
| `classification` | `string` | name to which to add the Trajectory |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:798

___

### classifyTrajectory

▸ **classifyTrajectory**(`trajectory`): [`Nullable`](../modules.md#nullable)`string`

Attempt to recognize a Trajectory from among all the classifications
already known to the classifier.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trajectory` | [`Trajectory`](Trajectory.md) | Trajectory to be recognized |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

classification of Trajectory if recognized, null otherwise

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:821

___

### deleteClassification

▸ **deleteClassification**(`classification`): `boolean`

Remove a known named trajectory and all Trajectories associated with it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `classification` | `string` | name to remove |

#### Returns

`boolean`

whether anything was removed

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:811

___

### serialize

▸ **serialize**(): `string`

Serialize to JSON.

#### Returns

`string`

JSON serialization

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:729

___

### Deserialize

▸ `Static` **Deserialize**(`json`): [`TrajectoryClassifier`](TrajectoryClassifier.md)

Deserialize from JSON.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `json` | `string` | JSON serialization |

#### Returns

[`TrajectoryClassifier`](TrajectoryClassifier.md)

deserialized TrajectorySet

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:747

___

### Generate

▸ `Static` **Generate**(): [`TrajectoryClassifier`](TrajectoryClassifier.md)

Initialize a new empty TrajectorySet with auto-generated Alphabets.
VERY naive, need to be generating these things from known
sets. Better version later, probably eliminating this one.

#### Returns

[`TrajectoryClassifier`](TrajectoryClassifier.md)

auto-generated TrajectorySet

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:768

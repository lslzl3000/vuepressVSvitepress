[@dev/core](../README.md) / [Exports](../modules.md) / Trajectory

# Class: Trajectory

A 3D trajectory consisting of an order list of vectors describing a
path of motion through 3D space.

## Table of contents

### Constructors

- [constructor](Trajectory.md#constructor)

### Properties

- [\_points](Trajectory.md#_points)
- [\_segmentLength](Trajectory.md#_segmentlength)
- [\_BestMatch](Trajectory.md#_bestmatch)
- [\_BestScore](Trajectory.md#_bestscore)
- [\_ForwardDir](Trajectory.md#_forwarddir)
- [\_FromToVec](Trajectory.md#_fromtovec)
- [\_InverseFromVec](Trajectory.md#_inversefromvec)
- [\_LookMatrix](Trajectory.md#_lookmatrix)
- [\_Score](Trajectory.md#_score)
- [\_UpDir](Trajectory.md#_updir)

### Methods

- [add](Trajectory.md#add)
- [getLength](Trajectory.md#getlength)
- [resampleAtTargetResolution](Trajectory.md#resampleattargetresolution)
- [serialize](Trajectory.md#serialize)
- [tokenize](Trajectory.md#tokenize)
- [Deserialize](Trajectory.md#deserialize)
- [\_TokenizeSegment](Trajectory.md#_tokenizesegment)
- [\_TransformSegmentDirToRef](Trajectory.md#_transformsegmentdirtoref)

## Constructors

### constructor

• **new Trajectory**(`segmentLength?`)

Create a new empty Trajectory.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `segmentLength` | `number` | `0.01` | radius of discretization for Trajectory points |

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:269

## Properties

### \_points

• `Private` **\_points**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:240

___

### \_segmentLength

• `Private` `Readonly` **\_segmentLength**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:241

___

### \_BestMatch

▪ `Static` `Private` **\_BestMatch**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:376

___

### \_BestScore

▪ `Static` `Private` **\_BestScore**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:378

___

### \_ForwardDir

▪ `Static` `Private` **\_ForwardDir**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:338

___

### \_FromToVec

▪ `Static` `Private` **\_FromToVec**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:341

___

### \_InverseFromVec

▪ `Static` `Private` **\_InverseFromVec**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:339

___

### \_LookMatrix

▪ `Static` `Private` **\_LookMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:342

___

### \_Score

▪ `Static` `Private` **\_Score**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:377

___

### \_UpDir

▪ `Static` `Private` **\_UpDir**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:340

## Methods

### add

▸ **add**(`point`): `void`

Append a new point to the Trajectory.
NOTE: This implementation has many allocations.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | point to append to the Trajectory |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:287

___

### getLength

▸ **getLength**(): `number`

Get the length of the Trajectory.

#### Returns

`number`

length of the Trajectory

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:278

___

### resampleAtTargetResolution

▸ **resampleAtTargetResolution**(`targetResolution`): [`Trajectory`](Trajectory.md)

Create a new Trajectory with a segment length chosen to make it
probable that the new Trajectory will have a specified number of
segments. This operation is imprecise.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `targetResolution` | `number` | number of segments desired |

#### Returns

[`Trajectory`](Trajectory.md)

new Trajectory with approximately the requested number of segments

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:309

___

### serialize

▸ **serialize**(): `string`

Serialize to JSON.

#### Returns

`string`

serialized JSON string

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:247

___

### tokenize

▸ **tokenize**(`tokens`): `number`[]

Convert Trajectory segments into tokenized representation. This
representation is an array of numbers where each nth number is the
index of the token which is most similar to the nth segment of the
Trajectory.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tokens` | `DeepImmutableArray`[`Vector3`](Vector3.md) | list of vectors which serve as discrete tokens |

#### Returns

`number`[]

list of indices of most similar token per segment

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:325

___

### Deserialize

▸ `Static` **Deserialize**(`json`): [`Trajectory`](Trajectory.md)

Deserialize from JSON.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `json` | `string` | serialized JSON string |

#### Returns

[`Trajectory`](Trajectory.md)

deserialized Trajectory

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:256

___

### \_TokenizeSegment

▸ `Static` `Private` **_TokenizeSegment**(`segment`, `tokens`): `number`

Determine which token vector is most similar to the
segment vector.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `segment` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | segment vector |
| `tokens` | `DeepImmutableArray`[`Vector3`](Vector3.md) | token vector list |

#### Returns

`number`

index of the most similar token to the segment

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:387

___

### \_TransformSegmentDirToRef

▸ `Static` `Private` **_TransformSegmentDirToRef**(`priorVec`, `fromVec`, `toVec`, `result`): `boolean`

Transform the rotation (i.e., direction) of a segment to isolate
the relative transformation represented by the segment. This operation
may or may not succeed due to singularities in the equations that define
motion relativity in this context.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `priorVec` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the origin of the prior segment |
| `fromVec` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the origin of the current segment |
| `toVec` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the destination of the current segment |
| `result` | [`Vector3`](Vector3.md) | reference to output variable |

#### Returns

`boolean`

whether or not transformation was successful

#### Defined in

https://github.com/babylon.js/core/src/Misc/trajectoryClassifier.ts:355

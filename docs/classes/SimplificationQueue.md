[@dev/core](../README.md) / [Exports](../modules.md) / SimplificationQueue

# Class: SimplificationQueue

Queue used to order the simplification tasks

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

## Table of contents

### Constructors

- [constructor](SimplificationQueue.md#constructor)

### Properties

- [\_simplificationArray](SimplificationQueue.md#_simplificationarray)
- [running](SimplificationQueue.md#running)

### Methods

- [\_getSimplifier](SimplificationQueue.md#_getsimplifier)
- [addTask](SimplificationQueue.md#addtask)
- [executeNext](SimplificationQueue.md#executenext)
- [runSimplification](SimplificationQueue.md#runsimplification)

## Constructors

### constructor

• **new SimplificationQueue**()

Creates a new queue

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:105

## Properties

### \_simplificationArray

• `Private` **\_simplificationArray**: [`ISimplificationTask`](../interfaces/ISimplificationTask.md)[]

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:95

___

### running

• **running**: `boolean`

Gets a boolean indicating that the process is still running

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:100

## Methods

### \_getSimplifier

▸ `Private` **_getSimplifier**(`task`): [`ISimplifier`](../interfaces/ISimplifier.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `task` | [`ISimplificationTask`](../interfaces/ISimplificationTask.md) |

#### Returns

[`ISimplifier`](../interfaces/ISimplifier.md)

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:186

___

### addTask

▸ **addTask**(`task`): `void`

Adds a new simplification task

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`ISimplificationTask`](../interfaces/ISimplificationTask.md) | defines a task to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:114

___

### executeNext

▸ **executeNext**(): `void`

Execute next task

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:121

___

### runSimplification

▸ **runSimplification**(`task`): `void`

Execute a simplification task

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`ISimplificationTask`](../interfaces/ISimplificationTask.md) | defines the task to run |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/meshSimplification.ts:135

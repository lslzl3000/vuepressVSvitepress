[@dev/core](../README.md) / [Exports](../modules.md) / RecastJSPlugin

# Class: RecastJSPlugin

RecastJS navigation plugin

## Implements

- [`INavigationEnginePlugin`](../interfaces/INavigationEnginePlugin.md)

## Table of contents

### Constructors

- [constructor](RecastJSPlugin.md#constructor)

### Properties

- [\_maximumSubStepCount](RecastJSPlugin.md#_maximumsubstepcount)
- [\_tempVec1](RecastJSPlugin.md#_tempvec1)
- [\_tempVec2](RecastJSPlugin.md#_tempvec2)
- [\_timeStep](RecastJSPlugin.md#_timestep)
- [\_worker](RecastJSPlugin.md#_worker)
- [bjsRECAST](RecastJSPlugin.md#bjsrecast)
- [name](RecastJSPlugin.md#name)
- [navMesh](RecastJSPlugin.md#navmesh)

### Methods

- [addBoxObstacle](RecastJSPlugin.md#addboxobstacle)
- [addCylinderObstacle](RecastJSPlugin.md#addcylinderobstacle)
- [buildFromNavmeshData](RecastJSPlugin.md#buildfromnavmeshdata)
- [computePath](RecastJSPlugin.md#computepath)
- [createCrowd](RecastJSPlugin.md#createcrowd)
- [createDebugNavMesh](RecastJSPlugin.md#createdebugnavmesh)
- [createNavMesh](RecastJSPlugin.md#createnavmesh)
- [dispose](RecastJSPlugin.md#dispose)
- [getClosestPoint](RecastJSPlugin.md#getclosestpoint)
- [getClosestPointToRef](RecastJSPlugin.md#getclosestpointtoref)
- [getDefaultQueryExtent](RecastJSPlugin.md#getdefaultqueryextent)
- [getDefaultQueryExtentToRef](RecastJSPlugin.md#getdefaultqueryextenttoref)
- [getMaximumSubStepCount](RecastJSPlugin.md#getmaximumsubstepcount)
- [getNavmeshData](RecastJSPlugin.md#getnavmeshdata)
- [getRandomPointAround](RecastJSPlugin.md#getrandompointaround)
- [getRandomPointAroundToRef](RecastJSPlugin.md#getrandompointaroundtoref)
- [getTimeStep](RecastJSPlugin.md#gettimestep)
- [isSupported](RecastJSPlugin.md#issupported)
- [moveAlong](RecastJSPlugin.md#movealong)
- [moveAlongToRef](RecastJSPlugin.md#movealongtoref)
- [removeObstacle](RecastJSPlugin.md#removeobstacle)
- [setDefaultQueryExtent](RecastJSPlugin.md#setdefaultqueryextent)
- [setMaximumSubStepCount](RecastJSPlugin.md#setmaximumsubstepcount)
- [setTimeStep](RecastJSPlugin.md#settimestep)
- [setWorkerURL](RecastJSPlugin.md#setworkerurl)

## Constructors

### constructor

• **new RecastJSPlugin**(`recastInjection?`)

Initializes the recastJS plugin

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `recastInjection` | `any` | `Recast` | can be used to inject your own recast reference |

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:47

## Properties

### \_maximumSubStepCount

• `Private` **\_maximumSubStepCount**: `number` = `10`

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:35

___

### \_tempVec1

• `Private` **\_tempVec1**: `any`

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:38

___

### \_tempVec2

• `Private` **\_tempVec2**: `any`

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:39

___

### \_timeStep

• `Private` **\_timeStep**: `number`

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:36

___

### \_worker

• `Private` **\_worker**: [`Nullable`](../modules.md#nullable)`Worker` = `null`

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:41

___

### bjsRECAST

• **bjsRECAST**: `any` = `{}`

Reference to the Recast library

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:23

___

### name

• **name**: `string` = `"RecastJSPlugin"`

plugin name

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[name](../interfaces/INavigationEnginePlugin.md#name)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:28

___

### navMesh

• **navMesh**: `any`

the first navmesh created. We might extend this to support multiple navmeshes

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:33

## Methods

### addBoxObstacle

▸ **addBoxObstacle**(`position`, `extent`, `angle`): [`IObstacle`](../interfaces/IObstacle.md)

Creates an oriented box obstacle and add it to the navigation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `extent` | [`Vector3`](Vector3.md) | box size |
| `angle` | `number` | angle in radians of the box orientation on Y axis |

#### Returns

[`IObstacle`](../interfaces/IObstacle.md)

the obstacle freshly created

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[addBoxObstacle](../interfaces/INavigationEnginePlugin.md#addboxobstacle)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:462

___

### addCylinderObstacle

▸ **addCylinderObstacle**(`position`, `radius`, `height`): [`IObstacle`](../interfaces/IObstacle.md)

Creates a cylinder obstacle and add it to the navigation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `radius` | `number` | cylinder radius |
| `height` | `number` | cylinder height |

#### Returns

[`IObstacle`](../interfaces/IObstacle.md)

the obstacle freshly created

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[addCylinderObstacle](../interfaces/INavigationEnginePlugin.md#addcylinderobstacle)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:448

___

### buildFromNavmeshData

▸ **buildFromNavmeshData**(`data`): `void`

build the navmesh from a previously saved state using getNavmeshData

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Uint8Array` | the Uint8Array returned by getNavmeshData |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[buildFromNavmeshData](../interfaces/INavigationEnginePlugin.md#buildfromnavmeshdata)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:397

___

### computePath

▸ **computePath**(`start`, `end`): [`Vector3`](Vector3.md)[]

Compute a navigation path from start to end. Returns an empty array if no path can be computed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Vector3`](Vector3.md) | world position |
| `end` | [`Vector3`](Vector3.md) | world position |

#### Returns

[`Vector3`](Vector3.md)[]

array containing world position composing the path

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[computePath](../interfaces/INavigationEnginePlugin.md#computepath)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:341

___

### createCrowd

▸ **createCrowd**(`maxAgents`, `maxAgentRadius`, `scene`): [`ICrowd`](../interfaces/ICrowd.md)

Create a new Crowd so you can add agents

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxAgents` | `number` | the maximum agent count in the crowd |
| `maxAgentRadius` | `number` | the maximum radius an agent can have |
| `scene` | [`Scene`](Scene.md) | to attach the crowd to |

#### Returns

[`ICrowd`](../interfaces/ICrowd.md)

the crowd you can add agents to

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[createCrowd](../interfaces/INavigationEnginePlugin.md#createcrowd)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:366

___

### createDebugNavMesh

▸ **createDebugNavMesh**(`scene`): [`Mesh`](Mesh.md)

Create a navigation mesh debug mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | is where the mesh will be added |

#### Returns

[`Mesh`](Mesh.md)

debug display mesh

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[createDebugNavMesh](../interfaces/INavigationEnginePlugin.md#createdebugnavmesh)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:217

___

### createNavMesh

▸ **createNavMesh**(`meshes`, `parameters`, `completion?`): `void`

Creates a navigation mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`Mesh`](Mesh.md)[] | array of all the geometry used to compute the navigation mesh |
| `parameters` | [`INavMeshParameters`](../interfaces/INavMeshParameters.md) | bunch of parameters used to filter geometry |
| `completion?` | (`navmeshData`: `Uint8Array`) => `void` | callback when data is available from the worker. Not used without a worker |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[createNavMesh](../interfaces/INavigationEnginePlugin.md#createnavmesh)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:120

___

### dispose

▸ **dispose**(): `void`

Disposes

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[dispose](../interfaces/INavigationEnginePlugin.md#dispose)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:439

___

### getClosestPoint

▸ **getClosestPoint**(`position`): [`Vector3`](Vector3.md)

Get a navigation mesh constrained position, closest to the parameter position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |

#### Returns

[`Vector3`](Vector3.md)

the closest point to position constrained by the navigation mesh

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getClosestPoint](../interfaces/INavigationEnginePlugin.md#getclosestpoint)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:249

___

### getClosestPointToRef

▸ **getClosestPointToRef**(`position`, `result`): `void`

Get a navigation mesh constrained position, closest to the parameter position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `result` | [`Vector3`](Vector3.md) | output the closest point to position constrained by the navigation mesh |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getClosestPointToRef](../interfaces/INavigationEnginePlugin.md#getclosestpointtoref)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:263

___

### getDefaultQueryExtent

▸ **getDefaultQueryExtent**(): [`Vector3`](Vector3.md)

Get the Bounding box extent specified by setDefaultQueryExtent

#### Returns

[`Vector3`](Vector3.md)

the box extent values

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getDefaultQueryExtent](../interfaces/INavigationEnginePlugin.md#getdefaultqueryextent)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:388

___

### getDefaultQueryExtentToRef

▸ **getDefaultQueryExtentToRef**(`result`): `void`

Get the Bounding box extent result specified by setDefaultQueryExtent

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | output the box extent values |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getDefaultQueryExtentToRef](../interfaces/INavigationEnginePlugin.md#getdefaultqueryextenttoref)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:431

___

### getMaximumSubStepCount

▸ **getMaximumSubStepCount**(): `number`

Get the maximum number of iterations per navigation tick update

#### Returns

`number`

the maximum number of iterations

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getMaximumSubStepCount](../interfaces/INavigationEnginePlugin.md#getmaximumsubstepcount)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:110

___

### getNavmeshData

▸ **getNavmeshData**(): `Uint8Array`

returns the navmesh data that can be used later. The navmesh must be built before retrieving the data

#### Returns

`Uint8Array`

data the Uint8Array that can be saved and reused

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getNavmeshData](../interfaces/INavigationEnginePlugin.md#getnavmeshdata)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:418

___

### getRandomPointAround

▸ **getRandomPointAround**(`position`, `maxRadius`): [`Vector3`](Vector3.md)

Get a navigation mesh constrained position, within a particular radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `maxRadius` | `number` | the maximum distance to the constrained world position |

#### Returns

[`Vector3`](Vector3.md)

the closest point to position constrained by the navigation mesh

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getRandomPointAround](../interfaces/INavigationEnginePlugin.md#getrandompointaround)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:277

___

### getRandomPointAroundToRef

▸ **getRandomPointAroundToRef**(`position`, `maxRadius`, `result`): `void`

Get a navigation mesh constrained position, within a particular radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `maxRadius` | `number` | the maximum distance to the constrained world position |
| `result` | [`Vector3`](Vector3.md) | output the closest point to position constrained by the navigation mesh |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getRandomPointAroundToRef](../interfaces/INavigationEnginePlugin.md#getrandompointaroundtoref)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:292

___

### getTimeStep

▸ **getTimeStep**(): `number`

Get the time step of the navigation tick update.

#### Returns

`number`

the current time step

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[getTimeStep](../interfaces/INavigationEnginePlugin.md#gettimestep)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:91

___

### isSupported

▸ **isSupported**(): `boolean`

If this plugin is supported

#### Returns

`boolean`

true if plugin is supported

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[isSupported](../interfaces/INavigationEnginePlugin.md#issupported)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:484

___

### moveAlong

▸ **moveAlong**(`position`, `destination`): [`Vector3`](Vector3.md)

Compute the final position from a segment made of destination-position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `destination` | [`Vector3`](Vector3.md) | world position |

#### Returns

[`Vector3`](Vector3.md)

the resulting point along the navmesh

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[moveAlong](../interfaces/INavigationEnginePlugin.md#movealong)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:306

___

### moveAlongToRef

▸ **moveAlongToRef**(`position`, `destination`, `result`): `void`

Compute the final position from a segment made of destination-position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | world position |
| `destination` | [`Vector3`](Vector3.md) | world position |
| `result` | [`Vector3`](Vector3.md) | output the resulting point along the navmesh |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[moveAlongToRef](../interfaces/INavigationEnginePlugin.md#movealongtoref)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:324

___

### removeObstacle

▸ **removeObstacle**(`obstacle`): `void`

Removes an obstacle created by addCylinderObstacle or addBoxObstacle

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obstacle` | [`IObstacle`](../interfaces/IObstacle.md) | obstacle to remove from the navigation |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[removeObstacle](../interfaces/INavigationEnginePlugin.md#removeobstacle)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:476

___

### setDefaultQueryExtent

▸ **setDefaultQueryExtent**(`extent`): `void`

Set the Bounding box extent for doing spatial queries (getClosestPoint, getRandomPointAround, ...)
The queries will try to find a solution within those bounds
default is (1,1,1)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extent` | [`Vector3`](Vector3.md) | x,y,z value that define the extent around the queries point of reference |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[setDefaultQueryExtent](../interfaces/INavigationEnginePlugin.md#setdefaultqueryextent)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:377

___

### setMaximumSubStepCount

▸ **setMaximumSubStepCount**(`newStepCount?`): `void`

If delta time in navigation tick update is greater than the time step
a number of sub iterations are done. If more iterations are need to reach deltatime
they will be discarded.
A value of 0 will set to no maximum and update will use as many substeps as needed

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newStepCount` | `number` | `10` | the maximum number of iterations |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[setMaximumSubStepCount](../interfaces/INavigationEnginePlugin.md#setmaximumsubstepcount)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:102

___

### setTimeStep

▸ **setTimeStep**(`newTimeStep?`): `void`

Set the time step of the navigation tick update.
Default is 1/60.
A value of 0 will disable fixed time update

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTimeStep` | `number` | the new timestep to apply to this world. |

#### Returns

`void`

#### Implementation of

[INavigationEnginePlugin](../interfaces/INavigationEnginePlugin.md).[setTimeStep](../interfaces/INavigationEnginePlugin.md#settimestep)

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:83

___

### setWorkerURL

▸ **setWorkerURL**(`workerURL`): `boolean`

Set worker URL to be used when generating a new navmesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workerURL` | `string` | url string |

#### Returns

`boolean`

boolean indicating if worker is created

#### Defined in

packages/dev/core/src/Navigation/Plugins/recastJSPlugin.ts:69

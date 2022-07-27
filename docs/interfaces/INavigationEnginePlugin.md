[@dev/core](../README.md) / [Exports](../modules.md) / INavigationEnginePlugin

# Interface: INavigationEnginePlugin

Navigation plugin interface to add navigation constrained by a navigation mesh

## Implemented by

- [`RecastJSPlugin`](../classes/RecastJSPlugin.md)

## Table of contents

### Properties

- [name](INavigationEnginePlugin.md#name)

### Methods

- [addBoxObstacle](INavigationEnginePlugin.md#addboxobstacle)
- [addCylinderObstacle](INavigationEnginePlugin.md#addcylinderobstacle)
- [buildFromNavmeshData](INavigationEnginePlugin.md#buildfromnavmeshdata)
- [computePath](INavigationEnginePlugin.md#computepath)
- [createCrowd](INavigationEnginePlugin.md#createcrowd)
- [createDebugNavMesh](INavigationEnginePlugin.md#createdebugnavmesh)
- [createNavMesh](INavigationEnginePlugin.md#createnavmesh)
- [dispose](INavigationEnginePlugin.md#dispose)
- [getClosestPoint](INavigationEnginePlugin.md#getclosestpoint)
- [getClosestPointToRef](INavigationEnginePlugin.md#getclosestpointtoref)
- [getDefaultQueryExtent](INavigationEnginePlugin.md#getdefaultqueryextent)
- [getDefaultQueryExtentToRef](INavigationEnginePlugin.md#getdefaultqueryextenttoref)
- [getMaximumSubStepCount](INavigationEnginePlugin.md#getmaximumsubstepcount)
- [getNavmeshData](INavigationEnginePlugin.md#getnavmeshdata)
- [getRandomPointAround](INavigationEnginePlugin.md#getrandompointaround)
- [getRandomPointAroundToRef](INavigationEnginePlugin.md#getrandompointaroundtoref)
- [getTimeStep](INavigationEnginePlugin.md#gettimestep)
- [isSupported](INavigationEnginePlugin.md#issupported)
- [moveAlong](INavigationEnginePlugin.md#movealong)
- [moveAlongToRef](INavigationEnginePlugin.md#movealongtoref)
- [removeObstacle](INavigationEnginePlugin.md#removeobstacle)
- [setDefaultQueryExtent](INavigationEnginePlugin.md#setdefaultqueryextent)
- [setMaximumSubStepCount](INavigationEnginePlugin.md#setmaximumsubstepcount)
- [setTimeStep](INavigationEnginePlugin.md#settimestep)

## Properties

### name

• **name**: `string`

plugin name

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:13

## Methods

### addBoxObstacle

▸ **addBoxObstacle**(`position`, `extent`, `angle`): [`IObstacle`](IObstacle.md)

Creates an oriented box obstacle and add it to the navigation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `extent` | [`Vector3`](../classes/Vector3.md) | box size |
| `angle` | `number` | angle in radians of the box orientation on Y axis |

#### Returns

[`IObstacle`](IObstacle.md)

the obstacle freshly created

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:175

___

### addCylinderObstacle

▸ **addCylinderObstacle**(`position`, `radius`, `height`): [`IObstacle`](IObstacle.md)

Creates a cylinder obstacle and add it to the navigation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `radius` | `number` | cylinder radius |
| `height` | `number` | cylinder height |

#### Returns

[`IObstacle`](IObstacle.md)

the obstacle freshly created

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:166

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

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:116

___

### computePath

▸ **computePath**(`start`, `end`): [`Vector3`](../classes/Vector3.md)[]

Compute a navigation path from start to end. Returns an empty array if no path can be computed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Vector3`](../classes/Vector3.md) | world position |
| `end` | [`Vector3`](../classes/Vector3.md) | world position |

#### Returns

[`Vector3`](../classes/Vector3.md)[]

array containing world position composing the path

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:81

___

### createCrowd

▸ **createCrowd**(`maxAgents`, `maxAgentRadius`, `scene`): [`ICrowd`](ICrowd.md)

Create a new Crowd so you can add agents

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxAgents` | `number` | the maximum agent count in the crowd |
| `maxAgentRadius` | `number` | the maximum radius an agent can have |
| `scene` | [`Scene`](../classes/Scene.md) | to attach the crowd to |

#### Returns

[`ICrowd`](ICrowd.md)

the crowd you can add agents to

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:96

___

### createDebugNavMesh

▸ **createDebugNavMesh**(`scene`): [`Mesh`](../classes/Mesh.md)

Create a navigation mesh debug mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](../classes/Scene.md) | is where the mesh will be added |

#### Returns

[`Mesh`](../classes/Mesh.md)

debug display mesh

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:27

___

### createNavMesh

▸ **createNavMesh**(`meshes`, `parameters`): `void`

Creates a navigation mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`Mesh`](../classes/Mesh.md)[] | array of all the geometry used to compute the navigation mesh |
| `parameters` | [`INavMeshParameters`](INavMeshParameters.md) | bunch of parameters used to filter geometry |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:20

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:186

___

### getClosestPoint

▸ **getClosestPoint**(`position`): [`Vector3`](../classes/Vector3.md)

Get a navigation mesh constrained position, closest to the parameter position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |

#### Returns

[`Vector3`](../classes/Vector3.md)

the closest point to position constrained by the navigation mesh

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:34

___

### getClosestPointToRef

▸ **getClosestPointToRef**(`position`, `result`): `void`

Get a navigation mesh constrained position, closest to the parameter position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `result` | [`Vector3`](../classes/Vector3.md) | output the closest point to position constrained by the navigation mesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:41

___

### getDefaultQueryExtent

▸ **getDefaultQueryExtent**(): [`Vector3`](../classes/Vector3.md)

Get the Bounding box extent specified by setDefaultQueryExtent

#### Returns

[`Vector3`](../classes/Vector3.md)

the box extent values

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:110

___

### getDefaultQueryExtentToRef

▸ **getDefaultQueryExtentToRef**(`result`): `void`

Get the Bounding box extent result specified by setDefaultQueryExtent

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](../classes/Vector3.md) | output the box extent values |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:128

___

### getMaximumSubStepCount

▸ **getMaximumSubStepCount**(): `number`

Get the maximum number of iterations per navigation tick update

#### Returns

`number`

the maximum number of iterations

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:157

___

### getNavmeshData

▸ **getNavmeshData**(): `Uint8Array`

returns the navmesh data that can be used later. The navmesh must be built before retrieving the data

#### Returns

`Uint8Array`

data the Uint8Array that can be saved and reused

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:122

___

### getRandomPointAround

▸ **getRandomPointAround**(`position`, `maxRadius`): [`Vector3`](../classes/Vector3.md)

Get a navigation mesh constrained position, within a particular radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `maxRadius` | `number` | the maximum distance to the constrained world position |

#### Returns

[`Vector3`](../classes/Vector3.md)

the closest point to position constrained by the navigation mesh

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:49

___

### getRandomPointAroundToRef

▸ **getRandomPointAroundToRef**(`position`, `maxRadius`, `result`): `void`

Get a navigation mesh constrained position, within a particular radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `maxRadius` | `number` | the maximum distance to the constrained world position |
| `result` | [`Vector3`](../classes/Vector3.md) | output the closest point to position constrained by the navigation mesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:57

___

### getTimeStep

▸ **getTimeStep**(): `number`

Get the time step of the navigation tick update.

#### Returns

`number`

the current time step

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:142

___

### isSupported

▸ **isSupported**(): `boolean`

If this plugin is supported

#### Returns

`boolean`

true if plugin is supported

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:87

___

### moveAlong

▸ **moveAlong**(`position`, `destination`): [`Vector3`](../classes/Vector3.md)

Compute the final position from a segment made of destination-position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `destination` | [`Vector3`](../classes/Vector3.md) | world position |

#### Returns

[`Vector3`](../classes/Vector3.md)

the resulting point along the navmesh

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:65

___

### moveAlongToRef

▸ **moveAlongToRef**(`position`, `destination`, `result`): `void`

Compute the final position from a segment made of destination-position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](../classes/Vector3.md) | world position |
| `destination` | [`Vector3`](../classes/Vector3.md) | world position |
| `result` | [`Vector3`](../classes/Vector3.md) | output the resulting point along the navmesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:73

___

### removeObstacle

▸ **removeObstacle**(`obstacle`): `void`

Removes an obstacle created by addCylinderObstacle or addBoxObstacle

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obstacle` | [`IObstacle`](IObstacle.md) | obstacle to remove from the navigation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:181

___

### setDefaultQueryExtent

▸ **setDefaultQueryExtent**(`extent`): `void`

Set the Bounding box extent for doing spatial queries (getClosestPoint, getRandomPointAround, ...)
The queries will try to find a solution within those bounds
default is (1,1,1)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extent` | [`Vector3`](../classes/Vector3.md) | x,y,z value that define the extent around the queries point of reference |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:104

___

### setMaximumSubStepCount

▸ **setMaximumSubStepCount**(`newStepCount`): `void`

If delta time in navigation tick update is greater than the time step
a number of sub iterations are done. If more iterations are need to reach deltatime
they will be discarded.
A value of 0 will set to no maximum and update will use as many substeps as needed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newStepCount` | `number` | the maximum number of iterations |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:151

___

### setTimeStep

▸ **setTimeStep**(`newTimeStep`): `void`

Set the time step of the navigation tick update.
Default is 1/60.
A value of 0 will disable fixed time update

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTimeStep` | `number` | the new timestep to apply to this world. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:136

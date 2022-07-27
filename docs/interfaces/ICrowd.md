[@dev/core](../README.md) / [Exports](../modules.md) / ICrowd

# Interface: ICrowd

Crowd Interface. A Crowd is a collection of moving agents constrained by a navigation mesh

## Implemented by

- [`RecastJSCrowd`](../classes/RecastJSCrowd.md)

## Table of contents

### Methods

- [addAgent](ICrowd.md#addagent)
- [agentGoto](ICrowd.md#agentgoto)
- [agentTeleport](ICrowd.md#agentteleport)
- [dispose](ICrowd.md#dispose)
- [getAgentNextTargetPath](ICrowd.md#getagentnexttargetpath)
- [getAgentNextTargetPathToRef](ICrowd.md#getagentnexttargetpathtoref)
- [getAgentPosition](ICrowd.md#getagentposition)
- [getAgentPositionToRef](ICrowd.md#getagentpositiontoref)
- [getAgentState](ICrowd.md#getagentstate)
- [getAgentVelocity](ICrowd.md#getagentvelocity)
- [getAgentVelocityToRef](ICrowd.md#getagentvelocitytoref)
- [getAgents](ICrowd.md#getagents)
- [getCorners](ICrowd.md#getcorners)
- [getDefaultQueryExtent](ICrowd.md#getdefaultqueryextent)
- [getDefaultQueryExtentToRef](ICrowd.md#getdefaultqueryextenttoref)
- [overOffmeshConnection](ICrowd.md#overoffmeshconnection)
- [removeAgent](ICrowd.md#removeagent)
- [setDefaultQueryExtent](ICrowd.md#setdefaultqueryextent)
- [update](ICrowd.md#update)
- [updateAgentParameters](ICrowd.md#updateagentparameters)

## Methods

### addAgent

▸ **addAgent**(`pos`, `parameters`, `transform`): `number`

Add a new agent to the crowd with the specified parameter a corresponding transformNode.
You can attach anything to that node. The node position is updated in the scene update tick.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pos` | [`Vector3`](../classes/Vector3.md) | world position that will be constrained by the navigation mesh |
| `parameters` | [`IAgentParameters`](IAgentParameters.md) | agent parameters |
| `transform` | [`TransformNode`](../classes/TransformNode.md) | hooked to the agent that will be update by the scene |

#### Returns

`number`

agent index

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:206

___

### agentGoto

▸ **agentGoto**(`index`, `destination`): `void`

Asks a particular agent to go to a destination. That destination is constrained by the navigation mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `destination` | [`Vector3`](../classes/Vector3.md) | targeted world position |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:287

___

### agentTeleport

▸ **agentTeleport**(`index`, `destination`): `void`

Teleport the agent to a new position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `destination` | [`Vector3`](../classes/Vector3.md) | targeted world position |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:294

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:333

___

### getAgentNextTargetPath

▸ **getAgentNextTargetPath**(`index`): [`Vector3`](../classes/Vector3.md)

Gets the agent next target point on the path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](../classes/Vector3.md)

world space position

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:241

___

### getAgentNextTargetPathToRef

▸ **getAgentNextTargetPathToRef**(`index`, `result`): `void`

Gets the agent next target point on the path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](../classes/Vector3.md) | output world space position |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:262

___

### getAgentPosition

▸ **getAgentPosition**(`index`): [`Vector3`](../classes/Vector3.md)

Returns the agent position in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](../classes/Vector3.md)

world space position

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:213

___

### getAgentPositionToRef

▸ **getAgentPositionToRef**(`index`, `result`): `void`

Gets the agent position result in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](../classes/Vector3.md) | output world space position |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:220

___

### getAgentState

▸ **getAgentState**(`index`): `number`

Gets the agent state

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

`number`

agent state

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:248

___

### getAgentVelocity

▸ **getAgentVelocity**(`index`): [`Vector3`](../classes/Vector3.md)

Gets the agent velocity in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](../classes/Vector3.md)

world space velocity

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:227

___

### getAgentVelocityToRef

▸ **getAgentVelocityToRef**(`index`, `result`): `void`

Gets the agent velocity result in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](../classes/Vector3.md) | output world space velocity |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:234

___

### getAgents

▸ **getAgents**(): `number`[]

get the list of all agents attached to this crowd

#### Returns

`number`[]

list of agent indices

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:274

___

### getCorners

▸ **getCorners**(`index`): [`Vector3`](../classes/Vector3.md)[]

Get the next corner points composing the path (max 4 points)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](../classes/Vector3.md)[]

array containing world position composing the path

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:328

___

### getDefaultQueryExtent

▸ **getDefaultQueryExtent**(): [`Vector3`](../classes/Vector3.md)

Get the Bounding box extent specified by setDefaultQueryExtent

#### Returns

[`Vector3`](../classes/Vector3.md)

the box extent values

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:315

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

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:321

___

### overOffmeshConnection

▸ **overOffmeshConnection**(`index`): `boolean`

returns true if the agent in over an off mesh link connection

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

`boolean`

true if over an off mesh link connection

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:255

___

### removeAgent

▸ **removeAgent**(`index`): `void`

remove a particular agent previously created

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:268

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

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:309

___

### update

▸ **update**(`deltaTime`): `void`

Tick update done by the Scene. Agent position/velocity/acceleration is updated by this function

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `deltaTime` | `number` | in seconds |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:280

___

### updateAgentParameters

▸ **updateAgentParameters**(`index`, `parameters`): `void`

Update agent parameters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `parameters` | [`IAgentParameters`](IAgentParameters.md) | agent parameters |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:301

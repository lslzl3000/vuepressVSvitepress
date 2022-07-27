[@dev/core](../README.md) / [Exports](../modules.md) / RecastJSCrowd

# Class: RecastJSCrowd

Recast detour crowd implementation

## Implements

- [`ICrowd`](../interfaces/ICrowd.md)

## Table of contents

### Constructors

- [constructor](RecastJSCrowd.md#constructor)

### Properties

- [\_agentDestination](RecastJSCrowd.md#_agentdestination)
- [\_agentDestinationArmed](RecastJSCrowd.md#_agentdestinationarmed)
- [\_onBeforeAnimationsObserver](RecastJSCrowd.md#_onbeforeanimationsobserver)
- [\_scene](RecastJSCrowd.md#_scene)
- [agents](RecastJSCrowd.md#agents)
- [bjsRECASTPlugin](RecastJSCrowd.md#bjsrecastplugin)
- [onReachTargetObservable](RecastJSCrowd.md#onreachtargetobservable)
- [reachRadii](RecastJSCrowd.md#reachradii)
- [recastCrowd](RecastJSCrowd.md#recastcrowd)
- [transforms](RecastJSCrowd.md#transforms)

### Methods

- [addAgent](RecastJSCrowd.md#addagent)
- [agentGoto](RecastJSCrowd.md#agentgoto)
- [agentTeleport](RecastJSCrowd.md#agentteleport)
- [dispose](RecastJSCrowd.md#dispose)
- [getAgentNextTargetPath](RecastJSCrowd.md#getagentnexttargetpath)
- [getAgentNextTargetPathToRef](RecastJSCrowd.md#getagentnexttargetpathtoref)
- [getAgentPosition](RecastJSCrowd.md#getagentposition)
- [getAgentPositionToRef](RecastJSCrowd.md#getagentpositiontoref)
- [getAgentState](RecastJSCrowd.md#getagentstate)
- [getAgentVelocity](RecastJSCrowd.md#getagentvelocity)
- [getAgentVelocityToRef](RecastJSCrowd.md#getagentvelocitytoref)
- [getAgents](RecastJSCrowd.md#getagents)
- [getCorners](RecastJSCrowd.md#getcorners)
- [getDefaultQueryExtent](RecastJSCrowd.md#getdefaultqueryextent)
- [getDefaultQueryExtentToRef](RecastJSCrowd.md#getdefaultqueryextenttoref)
- [overOffmeshConnection](RecastJSCrowd.md#overoffmeshconnection)
- [removeAgent](RecastJSCrowd.md#removeagent)
- [setDefaultQueryExtent](RecastJSCrowd.md#setdefaultqueryextent)
- [update](RecastJSCrowd.md#update)
- [updateAgentParameters](RecastJSCrowd.md#updateagentparameters)

## Constructors

### constructor

• **new RecastJSCrowd**(`plugin`, `maxAgents`, `maxAgentRadius`, `scene`)

Constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plugin` | [`RecastJSPlugin`](RecastJSPlugin.md) | recastJS plugin |
| `maxAgents` | `number` | the maximum agent count in the crowd |
| `maxAgentRadius` | `number` | the maximum radius an agent can have |
| `scene` | [`Scene`](Scene.md) | to attach the crowd to |

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:544

## Properties

### \_agentDestination

• `Private` **\_agentDestination**: [`Vector3`](Vector3.md)[]

agent current target

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:520

___

### \_agentDestinationArmed

• `Private` **\_agentDestinationArmed**: `boolean`[]

true when a destination is active for an agent and notifier hasn't been notified of reach

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:516

___

### \_onBeforeAnimationsObserver

• `Private` **\_onBeforeAnimationsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

Observer for crowd updates

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:529

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

Link to the scene is kept to unregister the crowd from the scene

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:524

___

### agents

• **agents**: `number`[]

All agents created

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:508

___

### bjsRECASTPlugin

• **bjsRECASTPlugin**: [`RecastJSPlugin`](RecastJSPlugin.md)

Recast/detour plugin

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:496

___

### onReachTargetObservable

• **onReachTargetObservable**: [`Observable`](Observable.md){ `agentIndex`: `number` ; `destination`: [`Vector3`](Vector3.md)  }

Fires each time an agent is in reach radius of its destination

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:534

___

### reachRadii

• **reachRadii**: `number`[]

agents reach radius

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:512

___

### recastCrowd

• **recastCrowd**: `any` = `{}`

Link to the detour crowd

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:500

___

### transforms

• **transforms**: [`TransformNode`](TransformNode.md)[]

One transform per agent

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:504

## Methods

### addAgent

▸ **addAgent**(`pos`, `parameters`, `transform`): `number`

Add a new agent to the crowd with the specified parameter a corresponding transformNode.
You can attach anything to that node. The node position is updated in the scene update tick.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pos` | [`Vector3`](Vector3.md) | world position that will be constrained by the navigation mesh |
| `parameters` | [`IAgentParameters`](../interfaces/IAgentParameters.md) | agent parameters |
| `transform` | [`TransformNode`](TransformNode.md) | hooked to the agent that will be update by the scene |

#### Returns

`number`

agent index

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[addAgent](../interfaces/ICrowd.md#addagent)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:562

___

### agentGoto

▸ **agentGoto**(`index`, `destination`): `void`

Asks a particular agent to go to a destination. That destination is constrained by the navigation mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `destination` | [`Vector3`](Vector3.md) | targeted world position |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[agentGoto](../interfaces/ICrowd.md#agentgoto)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:668

___

### agentTeleport

▸ **agentTeleport**(`index`, `destination`): `void`

Teleport the agent to a new position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `destination` | [`Vector3`](Vector3.md) | targeted world position |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[agentTeleport](../interfaces/ICrowd.md#agentteleport)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:684

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[dispose](../interfaces/ICrowd.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:844

___

### getAgentNextTargetPath

▸ **getAgentNextTargetPath**(`index`): [`Vector3`](Vector3.md)

Returns the agent next target point on the path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](Vector3.md)

world space position

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentNextTargetPath](../interfaces/ICrowd.md#getagentnexttargetpath)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:630

___

### getAgentNextTargetPathToRef

▸ **getAgentNextTargetPathToRef**(`index`, `result`): `void`

Returns the agent next target point on the path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](Vector3.md) | output world space position |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentNextTargetPathToRef](../interfaces/ICrowd.md#getagentnexttargetpathtoref)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:640

___

### getAgentPosition

▸ **getAgentPosition**(`index`): [`Vector3`](Vector3.md)

Returns the agent position in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](Vector3.md)

world space position

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentPosition](../interfaces/ICrowd.md#getagentposition)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:590

___

### getAgentPositionToRef

▸ **getAgentPositionToRef**(`index`, `result`): `void`

Returns the agent position result in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](Vector3.md) | output world space position |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentPositionToRef](../interfaces/ICrowd.md#getagentpositiontoref)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:600

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

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentState](../interfaces/ICrowd.md#getagentstate)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:650

___

### getAgentVelocity

▸ **getAgentVelocity**(`index`): [`Vector3`](Vector3.md)

Returns the agent velocity in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](Vector3.md)

world space velocity

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentVelocity](../interfaces/ICrowd.md#getagentvelocity)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:610

___

### getAgentVelocityToRef

▸ **getAgentVelocityToRef**(`index`, `result`): `void`

Returns the agent velocity result in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `result` | [`Vector3`](Vector3.md) | output world space velocity |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgentVelocityToRef](../interfaces/ICrowd.md#getagentvelocitytoref)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:620

___

### getAgents

▸ **getAgents**(): `number`[]

get the list of all agents attached to this crowd

#### Returns

`number`[]

list of agent indices

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getAgents](../interfaces/ICrowd.md#getagents)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:742

___

### getCorners

▸ **getCorners**(`index`): [`Vector3`](Vector3.md)[]

Get the next corner points composing the path (max 4 points)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |

#### Returns

[`Vector3`](Vector3.md)[]

array containing world position composing the path

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getCorners](../interfaces/ICrowd.md#getcorners)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:829

___

### getDefaultQueryExtent

▸ **getDefaultQueryExtent**(): [`Vector3`](Vector3.md)

Get the Bounding box extent specified by setDefaultQueryExtent

#### Returns

[`Vector3`](Vector3.md)

the box extent values

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[getDefaultQueryExtent](../interfaces/ICrowd.md#getdefaultqueryextent)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:810

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

[ICrowd](../interfaces/ICrowd.md).[getDefaultQueryExtentToRef](../interfaces/ICrowd.md#getdefaultqueryextenttoref)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:819

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

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[overOffmeshConnection](../interfaces/ICrowd.md#overoffmeshconnection)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:659

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

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[removeAgent](../interfaces/ICrowd.md#removeagent)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:725

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

[ICrowd](../interfaces/ICrowd.md).[setDefaultQueryExtent](../interfaces/ICrowd.md#setdefaultqueryextent)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:801

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

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[update](../interfaces/ICrowd.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:750

___

### updateAgentParameters

▸ **updateAgentParameters**(`index`, `parameters`): `void`

Update agent parameters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | agent index returned by addAgent |
| `parameters` | [`IAgentParameters`](../interfaces/IAgentParameters.md) | agent parameters |

#### Returns

`void`

#### Implementation of

[ICrowd](../interfaces/ICrowd.md).[updateAgentParameters](../interfaces/ICrowd.md#updateagentparameters)

#### Defined in

https://github.com/babylon.js/core/src/Navigation/Plugins/recastJSPlugin.ts:693

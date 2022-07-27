[@dev/core](../README.md) / [Exports](../modules.md) / IAgentParameters

# Interface: IAgentParameters

Configures an agent

## Table of contents

### Properties

- [collisionQueryRange](IAgentParameters.md#collisionqueryrange)
- [height](IAgentParameters.md#height)
- [maxAcceleration](IAgentParameters.md#maxacceleration)
- [maxSpeed](IAgentParameters.md#maxspeed)
- [pathOptimizationRange](IAgentParameters.md#pathoptimizationrange)
- [radius](IAgentParameters.md#radius)
- [reachRadius](IAgentParameters.md#reachradius)
- [separationWeight](IAgentParameters.md#separationweight)

## Properties

### collisionQueryRange

• **collisionQueryRange**: `number`

Defines how close a collision element must be before it is considered for steering behaviors. [Limits: > 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:363

___

### height

• **height**: `number`

Agent height. [Limit: > 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:348

___

### maxAcceleration

• **maxAcceleration**: `number`

Maximum allowed acceleration. [Limit: >= 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:353

___

### maxSpeed

• **maxSpeed**: `number`

Maximum allowed speed. [Limit: >= 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:358

___

### pathOptimizationRange

• **pathOptimizationRange**: `number`

The path visibility optimization range. [Limit: > 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:368

___

### radius

• **radius**: `number`

Agent radius. [Limit: >= 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:343

___

### reachRadius

• `Optional` **reachRadius**: `number`

Observers will be notified when agent gets inside the virtual circle with this Radius around destination point.
Default is agent radius

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:379

___

### separationWeight

• **separationWeight**: `number`

How aggressive the agent manager should be at avoiding collisions with this agent. [Limit: >= 0]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:373

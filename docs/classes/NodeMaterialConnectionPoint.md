[@dev/core](../README.md) / [Exports](../modules.md) / NodeMaterialConnectionPoint

# Class: NodeMaterialConnectionPoint

Defines a connection point for a block

## Hierarchy

- **`NodeMaterialConnectionPoint`**

  ↳ [`NodeMaterialConnectionPointCustomObject`](NodeMaterialConnectionPointCustomObject.md)

## Table of contents

### Constructors

- [constructor](NodeMaterialConnectionPoint.md#constructor)

### Properties

- [\_associatedVariableName](NodeMaterialConnectionPoint.md#_associatedvariablename)
- [\_direction](NodeMaterialConnectionPoint.md#_direction)
- [\_endpoints](NodeMaterialConnectionPoint.md#_endpoints)
- [\_target](NodeMaterialConnectionPoint.md#_target)
- [\_type](NodeMaterialConnectionPoint.md#_type)
- [acceptedConnectionPointTypes](NodeMaterialConnectionPoint.md#acceptedconnectionpointtypes)
- [define](NodeMaterialConnectionPoint.md#define)
- [displayName](NodeMaterialConnectionPoint.md#displayname)
- [excludedConnectionPointTypes](NodeMaterialConnectionPoint.md#excludedconnectionpointtypes)
- [exposedPortPosition](NodeMaterialConnectionPoint.md#exposedportposition)
- [isExposedOnFrame](NodeMaterialConnectionPoint.md#isexposedonframe)
- [isOptional](NodeMaterialConnectionPoint.md#isoptional)
- [name](NodeMaterialConnectionPoint.md#name)
- [needDualDirectionValidation](NodeMaterialConnectionPoint.md#needdualdirectionvalidation)
- [onConnectionObservable](NodeMaterialConnectionPoint.md#onconnectionobservable)

### Accessors

- [associatedVariableName](NodeMaterialConnectionPoint.md#associatedvariablename)
- [connectInputBlock](NodeMaterialConnectionPoint.md#connectinputblock)
- [connectedBlocks](NodeMaterialConnectionPoint.md#connectedblocks)
- [connectedPoint](NodeMaterialConnectionPoint.md#connectedpoint)
- [direction](NodeMaterialConnectionPoint.md#direction)
- [endpoints](NodeMaterialConnectionPoint.md#endpoints)
- [hasEndpoints](NodeMaterialConnectionPoint.md#hasendpoints)
- [innerType](NodeMaterialConnectionPoint.md#innertype)
- [isConnected](NodeMaterialConnectionPoint.md#isconnected)
- [isConnectedInFragmentShader](NodeMaterialConnectionPoint.md#isconnectedinfragmentshader)
- [isConnectedInVertexShader](NodeMaterialConnectionPoint.md#isconnectedinvertexshader)
- [isConnectedToInputBlock](NodeMaterialConnectionPoint.md#isconnectedtoinputblock)
- [isDirectlyConnectedToVertexOutput](NodeMaterialConnectionPoint.md#isdirectlyconnectedtovertexoutput)
- [ownerBlock](NodeMaterialConnectionPoint.md#ownerblock)
- [sourceBlock](NodeMaterialConnectionPoint.md#sourceblock)
- [target](NodeMaterialConnectionPoint.md#target)
- [type](NodeMaterialConnectionPoint.md#type)

### Methods

- [canConnectTo](NodeMaterialConnectionPoint.md#canconnectto)
- [checkCompatibilityState](NodeMaterialConnectionPoint.md#checkcompatibilitystate)
- [connectTo](NodeMaterialConnectionPoint.md#connectto)
- [createCustomInputBlock](NodeMaterialConnectionPoint.md#createcustominputblock)
- [disconnectFrom](NodeMaterialConnectionPoint.md#disconnectfrom)
- [dispose](NodeMaterialConnectionPoint.md#dispose)
- [getClassName](NodeMaterialConnectionPoint.md#getclassname)
- [serialize](NodeMaterialConnectionPoint.md#serialize)
- [AreEquivalentTypes](NodeMaterialConnectionPoint.md#areequivalenttypes)

## Constructors

### constructor

• **new NodeMaterialConnectionPoint**(`name`, `ownerBlock`, `direction`)

Creates a new connection point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `ownerBlock` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the block hosting this connection point |
| `direction` | [`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md) | defines the direction of the connection point |

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:395

## Properties

### \_associatedVariableName

• `Private` **\_associatedVariableName**: `string`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:80

___

### \_direction

• `Private` **\_direction**: [`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:81

___

### \_endpoints

• `Private` **\_endpoints**: [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:79

___

### \_target

• `Private` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) = `NodeMaterialBlockTargets.VertexAndFragment`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:219

___

### \_type

• `Private` **\_type**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) = `NodeMaterialBlockConnectionPointTypes.Float`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:95

___

### acceptedConnectionPointTypes

• **acceptedConnectionPointTypes**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)[]

Gets or sets the additional types supported by this connection point

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:111

___

### define

• **define**: `string`

Gets or sets a string indicating that this uniform must be defined under a #ifdef

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:214

___

### displayName

• **displayName**: `string`

Gets or sets the connection point name

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:194

___

### excludedConnectionPointTypes

• **excludedConnectionPointTypes**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)[]

Gets or sets the additional types excluded by this connection point

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:116

___

### exposedPortPosition

• **exposedPortPosition**: `number` = `-1`

Gets or sets number indicating the position that the port is exposed to on a frame

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:209

___

### isExposedOnFrame

• **isExposedOnFrame**: `boolean` = `false`

Gets or sets a boolean indicating that this connection point is exposed on a frame

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:204

___

### isOptional

• **isOptional**: `boolean`

Gets or sets a boolean indicating that this connection point can be omitted

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:199

___

### name

• **name**: `string`

Gets or sets the connection point name

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:189

___

### needDualDirectionValidation

• **needDualDirectionValidation**: `boolean` = `false`

Indicates that this connection point needs dual validation before being connected to another point

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:106

___

### onConnectionObservable

• **onConnectionObservable**: [`Observable`](Observable.md)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Observable triggered when this point is connected

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:121

## Accessors

### associatedVariableName

• `get` **associatedVariableName**(): `string`

Gets or sets the associated variable name in the shader

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:126

• `set` **associatedVariableName**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:138

___

### connectInputBlock

• `get` **connectInputBlock**(): [`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

Gets a the connected input block (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:259

___

### connectedBlocks

• `get` **connectedBlocks**(): [`NodeMaterialBlock`](NodeMaterialBlock.md)[]

Get the block connected on the endpoints of this connection (if any)

#### Returns

[`NodeMaterialBlock`](NodeMaterialBlock.md)[]

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:287

___

### connectedPoint

• `get` **connectedPoint**(): [`Nullable`](../modules.md#nullable)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Get the other side of the connection (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:268

___

### direction

• `get` **direction**(): [`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md)

Gets the direction of the point

#### Returns

[`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:101

___

### endpoints

• `get` **endpoints**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of connected endpoints

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:296

___

### hasEndpoints

• `get` **hasEndpoints**(): `boolean`

Gets a boolean indicating if that output point is connected to at least one input

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:301

___

### innerType

• `get` **innerType**(): [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

Get the inner type (ie AutoDetect for instance instead of the inferred one)

#### Returns

[`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:143

___

### isConnected

• `get` **isConnected**(): `boolean`

Gets a boolean indicating that the current point is connected to another NodeMaterialBlock

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:245

___

### isConnectedInFragmentShader

• `get` **isConnectedInFragmentShader**(): `boolean`

Gets a boolean indicating that this connection will be used in the fragment shader

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:356

___

### isConnectedInVertexShader

• `get` **isConnectedInVertexShader**(): `boolean`

Gets a boolean indicating that this connection will be used in the vertex shader

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:327

___

### isConnectedToInputBlock

• `get` **isConnectedToInputBlock**(): `boolean`

Gets a boolean indicating that the current point is connected to an input block

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:252

___

### isDirectlyConnectedToVertexOutput

• `get` **isDirectlyConnectedToVertexOutput**(): `boolean`

Gets a boolean indicating that this connection has a path to the vertex output

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:306

___

### ownerBlock

• `get` **ownerBlock**(): [`NodeMaterialBlock`](NodeMaterialBlock.md)

Get the block that owns this connection point

#### Returns

[`NodeMaterialBlock`](NodeMaterialBlock.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:273

___

### sourceBlock

• `get` **sourceBlock**(): [`Nullable`](../modules.md#nullable)[`NodeMaterialBlock`](NodeMaterialBlock.md)

Get the block connected on the other side of this connection (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`NodeMaterialBlock`](NodeMaterialBlock.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:278

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of that connection point

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:222

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:238

___

### type

• `get` **type**(): [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

Gets or sets the connection point type (default is float)

#### Returns

[`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:153

• `set` **type**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:182

## Methods

### canConnectTo

▸ **canConnectTo**(`connectionPoint`): `boolean`

Gets a boolean indicating if the current point can be connected to another point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `connectionPoint` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | defines the other connection point |

#### Returns

`boolean`

a boolean

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:414

___

### checkCompatibilityState

▸ **checkCompatibilityState**(`connectionPoint`): [`NodeMaterialConnectionPointCompatibilityStates`](../enums/NodeMaterialConnectionPointCompatibilityStates.md)

Gets a number indicating if the current point can be connected to another point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `connectionPoint` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | defines the other connection point |

#### Returns

[`NodeMaterialConnectionPointCompatibilityStates`](../enums/NodeMaterialConnectionPointCompatibilityStates.md)

a number defining the compatibility state

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:423

___

### connectTo

▸ **connectTo**(`connectionPoint`, `ignoreConstraints?`): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Connect this point to another connection point

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `connectionPoint` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | `undefined` | defines the other connection point |
| `ignoreConstraints` | `boolean` | `false` | defines if the system will ignore connection type constraints (default is false) |

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the current connection point

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:484

___

### createCustomInputBlock

▸ **createCustomInputBlock**(): [`Nullable`](../modules.md#nullable)[[`NodeMaterialBlock`](NodeMaterialBlock.md), `string`]

Creates a block suitable to be used as an input for this input point.
If null is returned, a block based on the point type will be created.

#### Returns

[`Nullable`](../modules.md#nullable)[[`NodeMaterialBlock`](NodeMaterialBlock.md), `string`]

The returned string parameter is the name of the output point of NodeMaterialBlock (first parameter of the returned array) that can be connected to the input

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:385

___

### disconnectFrom

▸ **disconnectFrom**(`endpoint`): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Disconnect this point from one of his endpoint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `endpoint` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | defines the other connection point |

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the current connection point

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:505

___

### dispose

▸ **dispose**(): `void`

Release resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:549

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name e.g. "NodeMaterialConnectionPoint"

#### Returns

`string`

the class name

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:405

___

### serialize

▸ **serialize**(`isInput?`): `any`

Serializes this point in a JSON representation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `isInput` | `boolean` | `true` | defines if the connection point is an input (default is true) |

#### Returns

`any`

the serialized point object

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:524

___

### AreEquivalentTypes

▸ `Static` **AreEquivalentTypes**(`type1`, `type2`): `boolean`

Checks if two types are equivalent

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type1` | `number` | type 1 to check |
| `type2` | `number` | type 2 to check |

#### Returns

`boolean`

true if both types are equivalent, else false

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:43

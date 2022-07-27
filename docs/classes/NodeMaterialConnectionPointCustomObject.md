[@dev/core](../README.md) / [Exports](../modules.md) / NodeMaterialConnectionPointCustomObject

# Class: NodeMaterialConnectionPointCustomObjectT

Defines a connection point to be used for points with a custom object type

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`NodeMaterialBlock`](NodeMaterialBlock.md) |

## Hierarchy

- [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

  ↳ **`NodeMaterialConnectionPointCustomObject`**

## Table of contents

### Constructors

- [constructor](NodeMaterialConnectionPointCustomObject.md#constructor)

### Properties

- [acceptedConnectionPointTypes](NodeMaterialConnectionPointCustomObject.md#acceptedconnectionpointtypes)
- [define](NodeMaterialConnectionPointCustomObject.md#define)
- [displayName](NodeMaterialConnectionPointCustomObject.md#displayname)
- [excludedConnectionPointTypes](NodeMaterialConnectionPointCustomObject.md#excludedconnectionpointtypes)
- [exposedPortPosition](NodeMaterialConnectionPointCustomObject.md#exposedportposition)
- [isExposedOnFrame](NodeMaterialConnectionPointCustomObject.md#isexposedonframe)
- [isOptional](NodeMaterialConnectionPointCustomObject.md#isoptional)
- [name](NodeMaterialConnectionPointCustomObject.md#name)
- [needDualDirectionValidation](NodeMaterialConnectionPointCustomObject.md#needdualdirectionvalidation)
- [onConnectionObservable](NodeMaterialConnectionPointCustomObject.md#onconnectionobservable)

### Accessors

- [associatedVariableName](NodeMaterialConnectionPointCustomObject.md#associatedvariablename)
- [connectInputBlock](NodeMaterialConnectionPointCustomObject.md#connectinputblock)
- [connectedBlocks](NodeMaterialConnectionPointCustomObject.md#connectedblocks)
- [connectedPoint](NodeMaterialConnectionPointCustomObject.md#connectedpoint)
- [direction](NodeMaterialConnectionPointCustomObject.md#direction)
- [endpoints](NodeMaterialConnectionPointCustomObject.md#endpoints)
- [hasEndpoints](NodeMaterialConnectionPointCustomObject.md#hasendpoints)
- [innerType](NodeMaterialConnectionPointCustomObject.md#innertype)
- [isConnected](NodeMaterialConnectionPointCustomObject.md#isconnected)
- [isConnectedInFragmentShader](NodeMaterialConnectionPointCustomObject.md#isconnectedinfragmentshader)
- [isConnectedInVertexShader](NodeMaterialConnectionPointCustomObject.md#isconnectedinvertexshader)
- [isConnectedToInputBlock](NodeMaterialConnectionPointCustomObject.md#isconnectedtoinputblock)
- [isDirectlyConnectedToVertexOutput](NodeMaterialConnectionPointCustomObject.md#isdirectlyconnectedtovertexoutput)
- [ownerBlock](NodeMaterialConnectionPointCustomObject.md#ownerblock)
- [sourceBlock](NodeMaterialConnectionPointCustomObject.md#sourceblock)
- [target](NodeMaterialConnectionPointCustomObject.md#target)
- [type](NodeMaterialConnectionPointCustomObject.md#type)

### Methods

- [canConnectTo](NodeMaterialConnectionPointCustomObject.md#canconnectto)
- [checkCompatibilityState](NodeMaterialConnectionPointCustomObject.md#checkcompatibilitystate)
- [connectTo](NodeMaterialConnectionPointCustomObject.md#connectto)
- [createCustomInputBlock](NodeMaterialConnectionPointCustomObject.md#createcustominputblock)
- [disconnectFrom](NodeMaterialConnectionPointCustomObject.md#disconnectfrom)
- [dispose](NodeMaterialConnectionPointCustomObject.md#dispose)
- [getClassName](NodeMaterialConnectionPointCustomObject.md#getclassname)
- [serialize](NodeMaterialConnectionPointCustomObject.md#serialize)
- [AreEquivalentTypes](NodeMaterialConnectionPointCustomObject.md#areequivalenttypes)

## Constructors

### constructor

• **new NodeMaterialConnectionPointCustomObject**`T`(`name`, `ownerBlock`, `direction`, `_blockType`, `_blockName`, `_nameForCheking?`)

Creates a new connection point

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`NodeMaterialBlock`](NodeMaterialBlock.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `ownerBlock` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the block hosting this connection point |
| `direction` | [`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md) | defines the direction of the connection point |
| `_blockType` | (...`args`: `any`[]) => `T` |  |
| `_blockName` | `string` |  |
| `_nameForCheking?` | `string` |  |

#### Overrides

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[constructor](NodeMaterialConnectionPoint.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialConnectionPointCustomObject.ts:19

## Properties

### acceptedConnectionPointTypes

• **acceptedConnectionPointTypes**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)[]

Gets or sets the additional types supported by this connection point

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[acceptedConnectionPointTypes](NodeMaterialConnectionPoint.md#acceptedconnectionpointtypes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:111

___

### define

• **define**: `string`

Gets or sets a string indicating that this uniform must be defined under a #ifdef

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[define](NodeMaterialConnectionPoint.md#define)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:214

___

### displayName

• **displayName**: `string`

Gets or sets the connection point name

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[displayName](NodeMaterialConnectionPoint.md#displayname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:194

___

### excludedConnectionPointTypes

• **excludedConnectionPointTypes**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)[]

Gets or sets the additional types excluded by this connection point

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[excludedConnectionPointTypes](NodeMaterialConnectionPoint.md#excludedconnectionpointtypes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:116

___

### exposedPortPosition

• **exposedPortPosition**: `number` = `-1`

Gets or sets number indicating the position that the port is exposed to on a frame

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[exposedPortPosition](NodeMaterialConnectionPoint.md#exposedportposition)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:209

___

### isExposedOnFrame

• **isExposedOnFrame**: `boolean` = `false`

Gets or sets a boolean indicating that this connection point is exposed on a frame

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[isExposedOnFrame](NodeMaterialConnectionPoint.md#isexposedonframe)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:204

___

### isOptional

• **isOptional**: `boolean`

Gets or sets a boolean indicating that this connection point can be omitted

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[isOptional](NodeMaterialConnectionPoint.md#isoptional)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:199

___

### name

• **name**: `string`

Gets or sets the connection point name

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[name](NodeMaterialConnectionPoint.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:189

___

### needDualDirectionValidation

• **needDualDirectionValidation**: `boolean` = `false`

Indicates that this connection point needs dual validation before being connected to another point

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[needDualDirectionValidation](NodeMaterialConnectionPoint.md#needdualdirectionvalidation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:106

___

### onConnectionObservable

• **onConnectionObservable**: [`Observable`](Observable.md)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Observable triggered when this point is connected

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[onConnectionObservable](NodeMaterialConnectionPoint.md#onconnectionobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:121

## Accessors

### associatedVariableName

• `get` **associatedVariableName**(): `string`

Gets or sets the associated variable name in the shader

#### Returns

`string`

#### Inherited from

NodeMaterialConnectionPoint.associatedVariableName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:126

• `set` **associatedVariableName**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

NodeMaterialConnectionPoint.associatedVariableName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:138

___

### connectInputBlock

• `get` **connectInputBlock**(): [`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

Gets a the connected input block (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

#### Inherited from

NodeMaterialConnectionPoint.connectInputBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:259

___

### connectedBlocks

• `get` **connectedBlocks**(): [`NodeMaterialBlock`](NodeMaterialBlock.md)[]

Get the block connected on the endpoints of this connection (if any)

#### Returns

[`NodeMaterialBlock`](NodeMaterialBlock.md)[]

#### Inherited from

NodeMaterialConnectionPoint.connectedBlocks

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:287

___

### connectedPoint

• `get` **connectedPoint**(): [`Nullable`](../modules.md#nullable)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Get the other side of the connection (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Inherited from

NodeMaterialConnectionPoint.connectedPoint

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:268

___

### direction

• `get` **direction**(): [`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md)

Gets the direction of the point

#### Returns

[`NodeMaterialConnectionPointDirection`](../enums/NodeMaterialConnectionPointDirection.md)

#### Inherited from

NodeMaterialConnectionPoint.direction

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:101

___

### endpoints

• `get` **endpoints**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of connected endpoints

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

NodeMaterialConnectionPoint.endpoints

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:296

___

### hasEndpoints

• `get` **hasEndpoints**(): `boolean`

Gets a boolean indicating if that output point is connected to at least one input

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.hasEndpoints

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:301

___

### innerType

• `get` **innerType**(): [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

Get the inner type (ie AutoDetect for instance instead of the inferred one)

#### Returns

[`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Inherited from

NodeMaterialConnectionPoint.innerType

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:143

___

### isConnected

• `get` **isConnected**(): `boolean`

Gets a boolean indicating that the current point is connected to another NodeMaterialBlock

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.isConnected

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:245

___

### isConnectedInFragmentShader

• `get` **isConnectedInFragmentShader**(): `boolean`

Gets a boolean indicating that this connection will be used in the fragment shader

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.isConnectedInFragmentShader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:356

___

### isConnectedInVertexShader

• `get` **isConnectedInVertexShader**(): `boolean`

Gets a boolean indicating that this connection will be used in the vertex shader

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.isConnectedInVertexShader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:327

___

### isConnectedToInputBlock

• `get` **isConnectedToInputBlock**(): `boolean`

Gets a boolean indicating that the current point is connected to an input block

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.isConnectedToInputBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:252

___

### isDirectlyConnectedToVertexOutput

• `get` **isDirectlyConnectedToVertexOutput**(): `boolean`

Gets a boolean indicating that this connection has a path to the vertex output

#### Returns

`boolean`

#### Inherited from

NodeMaterialConnectionPoint.isDirectlyConnectedToVertexOutput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:306

___

### ownerBlock

• `get` **ownerBlock**(): [`NodeMaterialBlock`](NodeMaterialBlock.md)

Get the block that owns this connection point

#### Returns

[`NodeMaterialBlock`](NodeMaterialBlock.md)

#### Inherited from

NodeMaterialConnectionPoint.ownerBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:273

___

### sourceBlock

• `get` **sourceBlock**(): [`Nullable`](../modules.md#nullable)[`NodeMaterialBlock`](NodeMaterialBlock.md)

Get the block connected on the other side of this connection (if any)

#### Returns

[`Nullable`](../modules.md#nullable)[`NodeMaterialBlock`](NodeMaterialBlock.md)

#### Inherited from

NodeMaterialConnectionPoint.sourceBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:278

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of that connection point

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

NodeMaterialConnectionPoint.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:222

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) |

#### Returns

`void`

#### Inherited from

NodeMaterialConnectionPoint.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:238

___

### type

• `get` **type**(): [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

Gets or sets the connection point type (default is float)

#### Returns

[`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Inherited from

NodeMaterialConnectionPoint.type

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:153

• `set` **type**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) |

#### Returns

`void`

#### Inherited from

NodeMaterialConnectionPoint.type

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:182

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

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[canConnectTo](NodeMaterialConnectionPoint.md#canconnectto)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:414

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

#### Overrides

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[checkCompatibilityState](NodeMaterialConnectionPoint.md#checkcompatibilitystate)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialConnectionPointCustomObject.ts:41

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

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[connectTo](NodeMaterialConnectionPoint.md#connectto)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:484

___

### createCustomInputBlock

▸ **createCustomInputBlock**(): [`Nullable`](../modules.md#nullable)[[`NodeMaterialBlock`](NodeMaterialBlock.md), `string`]

Creates a block suitable to be used as an input for this input point.
If null is returned, a block based on the point type will be created.

#### Returns

[`Nullable`](../modules.md#nullable)[[`NodeMaterialBlock`](NodeMaterialBlock.md), `string`]

The returned string parameter is the name of the output point of NodeMaterialBlock (first parameter of the returned array) that can be connected to the input

#### Overrides

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[createCustomInputBlock](NodeMaterialConnectionPoint.md#createcustominputblock)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialConnectionPointCustomObject.ts:52

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

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[disconnectFrom](NodeMaterialConnectionPoint.md#disconnectfrom)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:505

___

### dispose

▸ **dispose**(): `void`

Release resources

#### Returns

`void`

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[dispose](NodeMaterialConnectionPoint.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:549

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name e.g. "NodeMaterialConnectionPoint"

#### Returns

`string`

the class name

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[getClassName](NodeMaterialConnectionPoint.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:405

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

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[serialize](NodeMaterialConnectionPoint.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:524

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

#### Inherited from

[NodeMaterialConnectionPoint](NodeMaterialConnectionPoint.md).[AreEquivalentTypes](NodeMaterialConnectionPoint.md#areequivalenttypes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:43

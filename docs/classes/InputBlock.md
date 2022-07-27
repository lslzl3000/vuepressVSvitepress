[@dev/core](../README.md) / [Exports](../modules.md) / InputBlock

# Class: InputBlock

Block used to expose an input value

## Hierarchy

- [`NodeMaterialBlock`](NodeMaterialBlock.md)

  ↳ **`InputBlock`**

## Table of contents

### Constructors

- [constructor](InputBlock.md#constructor)

### Properties

- [\_animationType](InputBlock.md#_animationtype)
- [\_associatedVariableName](InputBlock.md#_associatedvariablename)
- [\_isUnique](InputBlock.md#_isunique)
- [\_mode](InputBlock.md#_mode)
- [\_storedValue](InputBlock.md#_storedvalue)
- [\_target](InputBlock.md#_target)
- [\_type](InputBlock.md#_type)
- [\_valueCallback](InputBlock.md#_valuecallback)
- [comments](InputBlock.md#comments)
- [convertToGammaSpace](InputBlock.md#converttogammaspace)
- [convertToLinearSpace](InputBlock.md#converttolinearspace)
- [groupInInspector](InputBlock.md#groupininspector)
- [inputsAreExclusive](InputBlock.md#inputsareexclusive)
- [isBoolean](InputBlock.md#isboolean)
- [isConstant](InputBlock.md#isconstant)
- [matrixMode](InputBlock.md#matrixmode)
- [max](InputBlock.md#max)
- [min](InputBlock.md#min)
- [onValueChangedObservable](InputBlock.md#onvaluechangedobservable)
- [uniqueId](InputBlock.md#uniqueid)
- [visibleInInspector](InputBlock.md#visibleininspector)
- [visibleOnFrame](InputBlock.md#visibleonframe)

### Accessors

- [animationType](InputBlock.md#animationtype)
- [associatedVariableName](InputBlock.md#associatedvariablename)
- [buildId](InputBlock.md#buildid)
- [inputs](InputBlock.md#inputs)
- [isAttribute](InputBlock.md#isattribute)
- [isFinalMerger](InputBlock.md#isfinalmerger)
- [isInput](InputBlock.md#isinput)
- [isSystemValue](InputBlock.md#issystemvalue)
- [isUndefined](InputBlock.md#isundefined)
- [isUniform](InputBlock.md#isuniform)
- [isUnique](InputBlock.md#isunique)
- [isVarying](InputBlock.md#isvarying)
- [name](InputBlock.md#name)
- [output](InputBlock.md#output)
- [outputs](InputBlock.md#outputs)
- [systemValue](InputBlock.md#systemvalue)
- [target](InputBlock.md#target)
- [type](InputBlock.md#type)
- [value](InputBlock.md#value)
- [valueCallback](InputBlock.md#valuecallback)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](InputBlock.md#willbegeneratedintovertexshaderfromfragmentshader)

### Methods

- [\_buildBlock](InputBlock.md#_buildblock)
- [\_declareOutput](InputBlock.md#_declareoutput)
- [\_deserialize](InputBlock.md#_deserialize)
- [\_dumpPropertiesCode](InputBlock.md#_dumppropertiescode)
- [\_emit](InputBlock.md#_emit)
- [\_emitConstant](InputBlock.md#_emitconstant)
- [\_emitDefine](InputBlock.md#_emitdefine)
- [\_inputRename](InputBlock.md#_inputrename)
- [\_linkConnectionTypes](InputBlock.md#_linkconnectiontypes)
- [\_outputRename](InputBlock.md#_outputrename)
- [\_writeFloat](InputBlock.md#_writefloat)
- [\_writeVariable](InputBlock.md#_writevariable)
- [animate](InputBlock.md#animate)
- [autoConfigure](InputBlock.md#autoconfigure)
- [bind](InputBlock.md#bind)
- [build](InputBlock.md#build)
- [clone](InputBlock.md#clone)
- [connectTo](InputBlock.md#connectto)
- [dispose](InputBlock.md#dispose)
- [getClassName](InputBlock.md#getclassname)
- [getFirstAvailableInput](InputBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](InputBlock.md#getfirstavailableoutput)
- [getInputByName](InputBlock.md#getinputbyname)
- [getOutputByName](InputBlock.md#getoutputbyname)
- [getSiblingOutput](InputBlock.md#getsiblingoutput)
- [initialize](InputBlock.md#initialize)
- [initializeDefines](InputBlock.md#initializedefines)
- [isAnAncestorOf](InputBlock.md#isanancestorof)
- [isReady](InputBlock.md#isready)
- [prepareDefines](InputBlock.md#preparedefines)
- [provideFallbacks](InputBlock.md#providefallbacks)
- [registerInput](InputBlock.md#registerinput)
- [registerOutput](InputBlock.md#registeroutput)
- [replaceRepeatableContent](InputBlock.md#replacerepeatablecontent)
- [serialize](InputBlock.md#serialize)
- [setAsAttribute](InputBlock.md#setasattribute)
- [setAsSystemValue](InputBlock.md#setassystemvalue)
- [setDefaultValue](InputBlock.md#setdefaultvalue)
- [updateUniformsAndSamples](InputBlock.md#updateuniformsandsamples)
- [validateBlockName](InputBlock.md#validateblockname)

## Constructors

### constructor

• **new InputBlock**(`name`, `target?`, `type?`)

Creates a new InputBlock

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the block name |
| `target` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | `NodeMaterialBlockTargets.Vertex` | defines the target of that block (Vertex by default) |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | `NodeMaterialBlockConnectionPointTypes.AutoDetect` | defines the type of the input (can be set to NodeMaterialBlockConnectionPointTypes.AutoDetect) |

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[constructor](NodeMaterialBlock.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:183

## Properties

### \_animationType

• `Private` **\_animationType**: [`AnimatedInputBlockTypes`](../enums/AnimatedInputBlockTypes.md) = `AnimatedInputBlockTypes.None`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:47

___

### \_associatedVariableName

• `Private` **\_associatedVariableName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:43

___

### \_isUnique

• `Protected` **\_isUnique**: `boolean` = `false`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_isUnique](NodeMaterialBlock.md#_isunique)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:27

___

### \_mode

• `Private` **\_mode**: [`NodeMaterialBlockConnectionPointMode`](../enums/NodeMaterialBlockConnectionPointMode.md) = `NodeMaterialBlockConnectionPointMode.Undefined`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:42

___

### \_storedValue

• `Private` **\_storedValue**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:44

___

### \_target

• `Protected` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_target](NodeMaterialBlock.md#_target)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:23

___

### \_type

• `Private` **\_type**: [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:46

___

### \_valueCallback

• `Private` **\_valueCallback**: () => `any`

#### Type declaration

▸ (): `any`

##### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:45

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[comments](NodeMaterialBlock.md#comments)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### convertToGammaSpace

• **convertToGammaSpace**: `boolean` = `false`

Gets or sets a boolean indicating if content needs to be converted to gamma space (for color3/4 only)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:74

___

### convertToLinearSpace

• **convertToLinearSpace**: `boolean` = `false`

Gets or sets a boolean indicating if content needs to be converted to linear space (for color3/4 only)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:77

___

### groupInInspector

• **groupInInspector**: `string` = `""`

Gets or sets the group to use to display this block in the Inspector

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:68

___

### inputsAreExclusive

• **inputsAreExclusive**: `boolean` = `false`

Gets or sets a boolean indicating that only one input can be connected at a time

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[inputsAreExclusive](NodeMaterialBlock.md#inputsareexclusive)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:30

___

### isBoolean

• **isBoolean**: `boolean` = `false`

Gets or set a value indicating that this input can only get 0 and 1 values

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:56

___

### isConstant

• **isConstant**: `boolean` = `false`

Gets or sets a boolean indicating that the value of this input will not change after a build

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:65

___

### matrixMode

• **matrixMode**: `number` = `0`

Gets or sets a value used by the Node Material editor to determine how to configure the current value if it is a matrix

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:59

___

### max

• **max**: `number` = `0`

Gets or set a value used to limit the range of float values

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:53

___

### min

• **min**: `number` = `0`

Gets or set a value used to limit the range of float values

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:50

___

### onValueChangedObservable

• **onValueChangedObservable**: [`Observable`](Observable.md)[`InputBlock`](InputBlock.md)

Gets an observable raised when the value is changed

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:71

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[uniqueId](NodeMaterialBlock.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:67

___

### visibleInInspector

• **visibleInInspector**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited in the Inspector (false by default)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[visibleInInspector](NodeMaterialBlock.md#visibleininspector)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:163

___

### visibleOnFrame

• **visibleOnFrame**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited from a collapsed frame

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[visibleOnFrame](NodeMaterialBlock.md#visibleonframe)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:166

## Accessors

### animationType

• `get` **animationType**(): [`AnimatedInputBlockTypes`](../enums/AnimatedInputBlockTypes.md)

Gets or sets the type of animation applied to the input

#### Returns

[`AnimatedInputBlockTypes`](../enums/AnimatedInputBlockTypes.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:284

• `set` **animationType**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`AnimatedInputBlockTypes`](../enums/AnimatedInputBlockTypes.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:288

___

### associatedVariableName

• `get` **associatedVariableName**(): `string`

Gets or sets the associated variable name in the shader

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:275

• `set` **associatedVariableName**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:279

___

### buildId

• `get` **buildId**(): `number`

Gets or sets the build Id

#### Returns

`number`

#### Inherited from

NodeMaterialBlock.buildId

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:98

• `set` **buildId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

NodeMaterialBlock.buildId

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:102

___

### inputs

• `get` **inputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of input points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

NodeMaterialBlock.inputs

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:123

___

### isAttribute

• `get` **isAttribute**(): `boolean`

Gets or sets a boolean indicating that this connection point is coming from an attribute.
In this case the connection point name must be the name of the attribute to use
Can only be set on inputs

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:318

• `set` **isAttribute**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:322

___

### isFinalMerger

• `get` **isFinalMerger**(): `boolean`

Gets a boolean indicating that this block is an end block (e.g. it is generating a system value)

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isFinalMerger

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:84

___

### isInput

• `get` **isInput**(): `boolean`

Gets a boolean indicating that this block is an input (e.g. it sends data to the shader)

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isInput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:91

___

### isSystemValue

• `get` **isSystemValue**(): `boolean`

Gets a boolean indicating that the current connection point is a system value

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:343

___

### isUndefined

• `get` **isUndefined**(): `boolean`

Gets a boolean indicating that this connection point not defined yet

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:295

___

### isUniform

• `get` **isUniform**(): `boolean`

Gets or sets a boolean indicating that this connection point is coming from an uniform.
In this case the connection point name must be the name of the uniform to use.
Can only be set on inputs

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:304

• `set` **isUniform**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:308

___

### isUnique

• `get` **isUnique**(): `boolean`

Gets a boolean indicating that this block can only be used once per NodeMaterial

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isUnique

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:77

___

### isVarying

• `get` **isVarying**(): `boolean`

Gets or sets a boolean indicating that this connection point is generating a varying variable.
Can only be set on exit points

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:331

• `set` **isVarying**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:335

___

### name

• `get` **name**(): `string`

Gets the name of the block

#### Returns

`string`

#### Inherited from

NodeMaterialBlock.name

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:49

• `set` **name**(`newName`): `void`

Sets the name of the block. Will check if the name is valid.

#### Parameters

| Name | Type |
| :------ | :------ |
| `newName` | `string` |

#### Returns

`void`

#### Inherited from

NodeMaterialBlock.name

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:56

___

### output

• `get` **output**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:208

___

### outputs

• `get` **outputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of output points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

NodeMaterialBlock.outputs

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:128

___

### systemValue

• `get` **systemValue**(): [`Nullable`](../modules.md#nullable)[`NodeMaterialSystemValues`](../enums/NodeMaterialSystemValues.md)

Gets or sets the current well known value or null if not defined as a system value

#### Returns

[`Nullable`](../modules.md#nullable)[`NodeMaterialSystemValues`](../enums/NodeMaterialSystemValues.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:350

• `set` **systemValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`NodeMaterialSystemValues`](../enums/NodeMaterialSystemValues.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:354

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of the block

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

NodeMaterialBlock.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:109

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) |

#### Returns

`void`

#### Inherited from

NodeMaterialBlock.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:113

___

### type

• `get` **type**(): [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

Gets or sets the connection point type (default is float)

#### Returns

[`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:82

___

### value

• `get` **value**(): `any`

Gets or sets the value of that point.
Please note that this value will be ignored if valueCallback is defined

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:239

• `set` **value**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:243

___

### valueCallback

• `get` **valueCallback**(): () => `any`

Gets or sets a callback used to get the value of that point.
Please note that setting this value will force the connection point to ignore the value property

#### Returns

`fn`

▸ (): `any`

Gets or sets a callback used to get the value of that point.
Please note that setting this value will force the connection point to ignore the value property

##### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:263

• `set` **valueCallback**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | () => `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:267

___

### willBeGeneratedIntoVertexShaderFromFragmentShader

• `get` **willBeGeneratedIntoVertexShaderFromFragmentShader**(): `boolean`

Gets a boolean indicating that the code of this block will be promoted to vertex shader even if connected to fragment output

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.willBeGeneratedIntoVertexShaderFromFragmentShader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:467

## Methods

### \_buildBlock

▸ `Protected` **_buildBlock**(`state`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_buildBlock](NodeMaterialBlock.md#_buildblock)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:681

___

### \_declareOutput

▸ `Protected` **_declareOutput**(`output`, `state`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `output` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) |
| `state` | `NodeMaterialBuildState` |

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_declareOutput](NodeMaterialBlock.md#_declareoutput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:205

___

### \_deserialize

▸ **_deserialize**(`serializationObject`, `scene`, `rootUrl`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `serializationObject` | `any` |
| `scene` | [`Scene`](Scene.md) |
| `rootUrl` | `string` |

#### Returns

`void`

#### Overrides

NodeMaterialBlock.\_deserialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:800

___

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_dumpPropertiesCode](NodeMaterialBlock.md#_dumppropertiescode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:691

___

### \_emit

▸ `Private` **_emit**(`state`, `define?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |
| `define?` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:462

___

### \_emitConstant

▸ `Private` **_emitConstant**(`state`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:424

___

### \_emitDefine

▸ `Private` **_emitDefine**(`define`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `define` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:383

___

### \_inputRename

▸ `Protected` **_inputRename**(`name`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_inputRename](NodeMaterialBlock.md#_inputrename)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:667

___

### \_linkConnectionTypes

▸ `Protected` **_linkConnectionTypes**(`inputIndex0`, `inputIndex1`, `looseCoupling?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `inputIndex0` | `number` | `undefined` |
| `inputIndex1` | `number` | `undefined` |
| `looseCoupling` | `boolean` | `false` |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_linkConnectionTypes](NodeMaterialBlock.md#_linkconnectiontypes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:502

___

### \_outputRename

▸ `Protected` **_outputRename**(`name`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_outputRename](NodeMaterialBlock.md#_outputrename)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:671

___

### \_writeFloat

▸ `Protected` **_writeFloat**(`value`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_writeFloat](NodeMaterialBlock.md#_writefloat)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:219

___

### \_writeVariable

▸ `Protected` **_writeVariable**(`currentPoint`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentPoint` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) |

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_writeVariable](NodeMaterialBlock.md#_writevariable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:209

___

### animate

▸ **animate**(`scene`): `void`

Animate the input if animationType !== None

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the rendering scene |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:372

___

### autoConfigure

▸ **autoConfigure**(`material`): `void`

Lets the block try to connect some inputs automatically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `material` | [`NodeMaterial`](NodeMaterial.md) | defines the hosting NodeMaterial |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[autoConfigure](NodeMaterialBlock.md#autoconfigure)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:450

___

### bind

▸ **bind**(`effect`, `nodeMaterial`, `mesh?`, `subMesh?`): `void`

Bind data to effect. Will only be called for blocks with isBindable === true

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind data to |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the hosting NodeMaterial |
| `mesh?` | [`Mesh`](Mesh.md) | defines the mesh that will be rendered |
| `subMesh?` | [`SubMesh`](SubMesh.md) | defines the submesh that will be rendered |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[bind](NodeMaterialBlock.md#bind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:201

___

### build

▸ **build**(`state`, `activeBlocks`): `boolean`

Compile the current node and generate the shader code

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | defines the current compilation state (uniforms, samplers, current string) |
| `activeBlocks` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] | defines the list of active blocks (i.e. blocks to compile) |

#### Returns

`boolean`

true if already built

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[build](NodeMaterialBlock.md#build)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:580

___

### clone

▸ **clone**(`scene`, `rootUrl?`): ``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

Clone the current block to a new identical block

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

a copy of the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[clone](NodeMaterialBlock.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:781

___

### connectTo

▸ **connectTo**(`other`, `options?`): `undefined` \| [`InputBlock`](InputBlock.md)

Connect current block with another block

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the block to connect with |
| `options?` | `Object` | define the various options to help pick the right connections |
| `options.input?` | `string` |  |
| `options.output?` | `string` |  |
| `options.outputSwizzle?` | `string` |  |

#### Returns

`undefined` \| [`InputBlock`](InputBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[connectTo](NodeMaterialBlock.md#connectto)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:364

___

### dispose

▸ **dispose**(): `void`

Release resources

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[dispose](NodeMaterialBlock.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:765

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name

#### Returns

`string`

the class name

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[getClassName](NodeMaterialBlock.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:364

___

### getFirstAvailableInput

▸ **getFirstAvailableInput**(`forOutput?`): ``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Will return the first available input e.g. the first one which is not an uniform or an attribute

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `forOutput` | [`Nullable`](../modules.md#nullable)[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | `null` | defines an optional connection point to check compatibility with |

#### Returns

``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the first available input or null

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[getFirstAvailableInput](NodeMaterialBlock.md#getfirstavailableinput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:289

___

### getFirstAvailableOutput

▸ **getFirstAvailableOutput**(`forBlock?`): ``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Will return the first available output e.g. the first one which is not yet connected and not a varying

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `forBlock` | [`Nullable`](../modules.md#nullable)[`NodeMaterialBlock`](NodeMaterialBlock.md) | `null` | defines an optional block to check compatibility with |

#### Returns

``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the first available input or null

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[getFirstAvailableOutput](NodeMaterialBlock.md#getfirstavailableoutput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:306

___

### getInputByName

▸ **getInputByName**(`name`): ``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Find an input by its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the input to look for |

#### Returns

``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the input or null if not found

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[getInputByName](NodeMaterialBlock.md#getinputbyname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:137

___

### getOutputByName

▸ **getOutputByName**(`name`): ``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Find an output by its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the output to look for |

#### Returns

``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the output or null if not found

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[getOutputByName](NodeMaterialBlock.md#getoutputbyname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:152

___

### getSiblingOutput

▸ **getSiblingOutput**(`current`): ``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the sibling of the given output

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `current` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | defines the current output |

#### Returns

``null`` \| [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

the next output in the list or null

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[getSiblingOutput](NodeMaterialBlock.md#getsiblingoutput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:321

___

### initialize

▸ **initialize**(): `void`

Initialize the block and prepare the context for build

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[initialize](NodeMaterialBlock.md#initialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:391

___

### initializeDefines

▸ **initializeDefines**(`mesh`, `nodeMaterial`, `defines`, `useInstances?`): `void`

Initialize defines for shader compilation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | `undefined` | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | `undefined` | defines the material defines to update |
| `useInstances` | `boolean` | `false` | specifies that instances should be used |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[initializeDefines](NodeMaterialBlock.md#initializedefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:430

___

### isAnAncestorOf

▸ **isAnAncestorOf**(`block`): `boolean`

Checks if the current block is an ancestor of a given block

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `block` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the potential descendant block to check |

#### Returns

`boolean`

true if block is a descendant

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[isAnAncestorOf](NodeMaterialBlock.md#isanancestorof)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:336

___

### isReady

▸ **isReady**(`mesh`, `nodeMaterial`, `defines`, `useInstances?`): `boolean`

Checks if the block is ready

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | `undefined` | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | `undefined` | defines the material defines to update |
| `useInstances` | `boolean` | `false` | specifies that instances should be used |

#### Returns

`boolean`

true if the block is ready

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[isReady](NodeMaterialBlock.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:498

___

### prepareDefines

▸ **prepareDefines**(`mesh`, `nodeMaterial`, `defines`, `useInstances?`, `subMesh?`): `void`

Update defines for shader compilation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | `undefined` | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | `undefined` | defines the material defines to update |
| `useInstances` | `boolean` | `false` | specifies that instances should be used |
| `subMesh?` | [`SubMesh`](SubMesh.md) | `undefined` | defines which submesh to render |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[prepareDefines](NodeMaterialBlock.md#preparedefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:441

___

### provideFallbacks

▸ **provideFallbacks**(`mesh`, `fallbacks`): `void`

Add potential fallbacks if shader compilation fails

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to be rendered |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | defines the current prioritized list of fallbacks |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[provideFallbacks](NodeMaterialBlock.md#providefallbacks)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:418

___

### registerInput

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`InputBlock`](InputBlock.md)

Register a new input. Must be called inside a block constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | `undefined` | defines the connection point type |
| `isOptional` | `boolean` | `false` | defines a boolean indicating that this input can be omitted |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | `undefined` | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | `undefined` | an already created connection point. If not provided, create a new one |

#### Returns

[`InputBlock`](InputBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerInput](NodeMaterialBlock.md#registerinput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`InputBlock`](InputBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`InputBlock`](InputBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerOutput](NodeMaterialBlock.md#registeroutput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:272

___

### replaceRepeatableContent

▸ **replaceRepeatableContent**(`vertexShaderState`, `fragmentShaderState`, `mesh`, `defines`): `void`

Function called when a block is declared as repeatable content generator

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexShaderState` | `NodeMaterialBuildState` | defines the current compilation state for the vertex shader |
| `fragmentShaderState` | `NodeMaterialBuildState` | defines the current compilation state for the fragment shader |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to be rendered |
| `defines` | `NodeMaterialDefines` | defines the material defines to update |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[replaceRepeatableContent](NodeMaterialBlock.md#replacerepeatablecontent)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:462

___

### serialize

▸ **serialize**(): `any`

Serializes this block in a JSON representation

#### Returns

`any`

the serialized block object

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[serialize](NodeMaterialBlock.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:771

___

### setAsAttribute

▸ **setAsAttribute**(`attributeName?`): [`InputBlock`](InputBlock.md)

Set the source of this connection point to a vertex attribute

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attributeName?` | `string` | defines the attribute name (position, uv, normal, etc...). If not specified it will take the connection point name |

#### Returns

[`InputBlock`](InputBlock.md)

the current connection point

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:217

___

### setAsSystemValue

▸ **setAsSystemValue**(`value`): [`InputBlock`](InputBlock.md)

Set the source of this connection point to a system value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`NodeMaterialSystemValues`](../enums/NodeMaterialSystemValues.md) | define the system value to use (world, view, etc...) or null to switch to manual value |

#### Returns

[`InputBlock`](InputBlock.md)

the current connection point

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:230

___

### setDefaultValue

▸ **setDefaultValue**(): `void`

Set the input block to its default value (based on its type)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:398

___

### updateUniformsAndSamples

▸ **updateUniformsAndSamples**(`state`, `nodeMaterial`, `defines`, `uniformBuffers`): `void`

Add uniforms, samplers and uniform buffers at compilation time

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | defines the state to update |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | defines the material defines to update |
| `uniformBuffers` | `string`[] | defines the list of uniform buffer names |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[updateUniformsAndSamples](NodeMaterialBlock.md#updateuniformsandsamples)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:408

___

### validateBlockName

▸ **validateBlockName**(`newName`): `boolean`

Validates if a name is a reserve word.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newName` | `string` | the new name to be given to the node. |

#### Returns

`boolean`

false if the name is a reserve word, else true.

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[validateBlockName](NodeMaterialBlock.md#validateblockname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Input/inputBlock.ts:198

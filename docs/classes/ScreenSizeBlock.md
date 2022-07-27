[@dev/core](../README.md) / [Exports](../modules.md) / ScreenSizeBlock

# Class: ScreenSizeBlock

Block used to get the screen sizes

## Hierarchy

- [`NodeMaterialBlock`](NodeMaterialBlock.md)

  ↳ **`ScreenSizeBlock`**

## Table of contents

### Constructors

- [constructor](ScreenSizeBlock.md#constructor)

### Properties

- [\_isUnique](ScreenSizeBlock.md#_isunique)
- [\_scene](ScreenSizeBlock.md#_scene)
- [\_target](ScreenSizeBlock.md#_target)
- [\_varName](ScreenSizeBlock.md#_varname)
- [comments](ScreenSizeBlock.md#comments)
- [inputsAreExclusive](ScreenSizeBlock.md#inputsareexclusive)
- [uniqueId](ScreenSizeBlock.md#uniqueid)
- [visibleInInspector](ScreenSizeBlock.md#visibleininspector)
- [visibleOnFrame](ScreenSizeBlock.md#visibleonframe)

### Accessors

- [buildId](ScreenSizeBlock.md#buildid)
- [inputs](ScreenSizeBlock.md#inputs)
- [isFinalMerger](ScreenSizeBlock.md#isfinalmerger)
- [isInput](ScreenSizeBlock.md#isinput)
- [isUnique](ScreenSizeBlock.md#isunique)
- [name](ScreenSizeBlock.md#name)
- [outputs](ScreenSizeBlock.md#outputs)
- [target](ScreenSizeBlock.md#target)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](ScreenSizeBlock.md#willbegeneratedintovertexshaderfromfragmentshader)
- [x](ScreenSizeBlock.md#x)
- [xy](ScreenSizeBlock.md#xy)
- [y](ScreenSizeBlock.md#y)

### Methods

- [\_buildBlock](ScreenSizeBlock.md#_buildblock)
- [\_declareOutput](ScreenSizeBlock.md#_declareoutput)
- [\_dumpPropertiesCode](ScreenSizeBlock.md#_dumppropertiescode)
- [\_inputRename](ScreenSizeBlock.md#_inputrename)
- [\_linkConnectionTypes](ScreenSizeBlock.md#_linkconnectiontypes)
- [\_outputRename](ScreenSizeBlock.md#_outputrename)
- [\_writeFloat](ScreenSizeBlock.md#_writefloat)
- [\_writeVariable](ScreenSizeBlock.md#_writevariable)
- [autoConfigure](ScreenSizeBlock.md#autoconfigure)
- [bind](ScreenSizeBlock.md#bind)
- [build](ScreenSizeBlock.md#build)
- [clone](ScreenSizeBlock.md#clone)
- [connectTo](ScreenSizeBlock.md#connectto)
- [dispose](ScreenSizeBlock.md#dispose)
- [getClassName](ScreenSizeBlock.md#getclassname)
- [getFirstAvailableInput](ScreenSizeBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](ScreenSizeBlock.md#getfirstavailableoutput)
- [getInputByName](ScreenSizeBlock.md#getinputbyname)
- [getOutputByName](ScreenSizeBlock.md#getoutputbyname)
- [getSiblingOutput](ScreenSizeBlock.md#getsiblingoutput)
- [initialize](ScreenSizeBlock.md#initialize)
- [initializeDefines](ScreenSizeBlock.md#initializedefines)
- [isAnAncestorOf](ScreenSizeBlock.md#isanancestorof)
- [isReady](ScreenSizeBlock.md#isready)
- [prepareDefines](ScreenSizeBlock.md#preparedefines)
- [provideFallbacks](ScreenSizeBlock.md#providefallbacks)
- [registerInput](ScreenSizeBlock.md#registerinput)
- [registerOutput](ScreenSizeBlock.md#registeroutput)
- [replaceRepeatableContent](ScreenSizeBlock.md#replacerepeatablecontent)
- [serialize](ScreenSizeBlock.md#serialize)
- [updateUniformsAndSamples](ScreenSizeBlock.md#updateuniformsandsamples)
- [validateBlockName](ScreenSizeBlock.md#validateblockname)
- [writeOutputs](ScreenSizeBlock.md#writeoutputs)

## Constructors

### constructor

• **new ScreenSizeBlock**(`name`)

Creates a new ScreenSizeBlock

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the block name |

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[constructor](NodeMaterialBlock.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:21

## Properties

### \_isUnique

• `Protected` **\_isUnique**: `boolean` = `false`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_isUnique](NodeMaterialBlock.md#_isunique)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:27

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:15

___

### \_target

• `Protected` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_target](NodeMaterialBlock.md#_target)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:23

___

### \_varName

• `Private` **\_varName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:14

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[comments](NodeMaterialBlock.md#comments)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### inputsAreExclusive

• **inputsAreExclusive**: `boolean` = `false`

Gets or sets a boolean indicating that only one input can be connected at a time

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[inputsAreExclusive](NodeMaterialBlock.md#inputsareexclusive)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:30

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

### willBeGeneratedIntoVertexShaderFromFragmentShader

• `get` **willBeGeneratedIntoVertexShaderFromFragmentShader**(): `boolean`

Gets a boolean indicating that the code of this block will be promoted to vertex shader even if connected to fragment output

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.willBeGeneratedIntoVertexShaderFromFragmentShader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:467

___

### x

• `get` **x**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the x component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:47

___

### xy

• `get` **xy**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the xy component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:40

___

### y

• `get` **y**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the y component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:54

## Methods

### \_buildBlock

▸ `Protected` **_buildBlock**(`state`): [`ScreenSizeBlock`](ScreenSizeBlock.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

[`ScreenSizeBlock`](ScreenSizeBlock.md)

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_buildBlock](NodeMaterialBlock.md#_buildblock)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:77

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

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_dumpPropertiesCode](NodeMaterialBlock.md#_dumppropertiescode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:675

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

▸ **bind**(`effect`): `void`

Bind data to effect. Will only be called for blocks with isBindable === true

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind data to |

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[bind](NodeMaterialBlock.md#bind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:58

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

▸ **connectTo**(`other`, `options?`): `undefined` \| [`ScreenSizeBlock`](ScreenSizeBlock.md)

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

`undefined` \| [`ScreenSizeBlock`](ScreenSizeBlock.md)

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

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[dispose](NodeMaterialBlock.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:869

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:33

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

▸ **initialize**(`state`): `void`

Initialize the block and prepare the context for build

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | defines the state that will be used for the build |

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[initialize](NodeMaterialBlock.md#initialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:189

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

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`ScreenSizeBlock`](ScreenSizeBlock.md)

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

[`ScreenSizeBlock`](ScreenSizeBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerInput](NodeMaterialBlock.md#registerinput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`ScreenSizeBlock`](ScreenSizeBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`ScreenSizeBlock`](ScreenSizeBlock.md)

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

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[serialize](NodeMaterialBlock.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:799

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

Validates the new name for the block node.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newName` | `string` | the new name to be given to the node. |

#### Returns

`boolean`

false if the name is a reserve word, else true.

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[validateBlockName](NodeMaterialBlock.md#validateblockname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:543

___

### writeOutputs

▸ `Protected` **writeOutputs**(`state`, `varName`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |
| `varName` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Fragment/screenSizeBlock.ts:65

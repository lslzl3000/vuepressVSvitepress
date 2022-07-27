[@dev/core](../README.md) / [Exports](../modules.md) / ReflectionTextureBlock

# Class: ReflectionTextureBlock

Block used to read a reflection texture from a sampler

## Hierarchy

- `ReflectionTextureBaseBlock`

  ↳ **`ReflectionTextureBlock`**

## Table of contents

### Constructors

- [constructor](ReflectionTextureBlock.md#constructor)

### Properties

- [\_directionWName](ReflectionTextureBlock.md#_directionwname)
- [\_isUnique](ReflectionTextureBlock.md#_isunique)
- [\_positionUVWName](ReflectionTextureBlock.md#_positionuvwname)
- [\_reflectionColorName](ReflectionTextureBlock.md#_reflectioncolorname)
- [\_reflectionVectorName](ReflectionTextureBlock.md#_reflectionvectorname)
- [\_target](ReflectionTextureBlock.md#_target)
- [\_texture](ReflectionTextureBlock.md#_texture)
- [comments](ReflectionTextureBlock.md#comments)
- [inputsAreExclusive](ReflectionTextureBlock.md#inputsareexclusive)
- [uniqueId](ReflectionTextureBlock.md#uniqueid)
- [visibleInInspector](ReflectionTextureBlock.md#visibleininspector)
- [visibleOnFrame](ReflectionTextureBlock.md#visibleonframe)

### Accessors

- [a](ReflectionTextureBlock.md#a)
- [b](ReflectionTextureBlock.md#b)
- [buildId](ReflectionTextureBlock.md#buildid)
- [cameraPosition](ReflectionTextureBlock.md#cameraposition)
- [g](ReflectionTextureBlock.md#g)
- [inputs](ReflectionTextureBlock.md#inputs)
- [isFinalMerger](ReflectionTextureBlock.md#isfinalmerger)
- [isInput](ReflectionTextureBlock.md#isinput)
- [isUnique](ReflectionTextureBlock.md#isunique)
- [name](ReflectionTextureBlock.md#name)
- [outputs](ReflectionTextureBlock.md#outputs)
- [position](ReflectionTextureBlock.md#position)
- [r](ReflectionTextureBlock.md#r)
- [rgb](ReflectionTextureBlock.md#rgb)
- [rgba](ReflectionTextureBlock.md#rgba)
- [target](ReflectionTextureBlock.md#target)
- [texture](ReflectionTextureBlock.md#texture)
- [view](ReflectionTextureBlock.md#view)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](ReflectionTextureBlock.md#willbegeneratedintovertexshaderfromfragmentshader)
- [world](ReflectionTextureBlock.md#world)
- [worldNormal](ReflectionTextureBlock.md#worldnormal)
- [worldPosition](ReflectionTextureBlock.md#worldposition)

### Methods

- [\_buildBlock](ReflectionTextureBlock.md#_buildblock)
- [\_declareOutput](ReflectionTextureBlock.md#_declareoutput)
- [\_deserialize](ReflectionTextureBlock.md#_deserialize)
- [\_dumpPropertiesCode](ReflectionTextureBlock.md#_dumppropertiescode)
- [\_getTexture](ReflectionTextureBlock.md#_gettexture)
- [\_inputRename](ReflectionTextureBlock.md#_inputrename)
- [\_linkConnectionTypes](ReflectionTextureBlock.md#_linkconnectiontypes)
- [\_outputRename](ReflectionTextureBlock.md#_outputrename)
- [\_writeFloat](ReflectionTextureBlock.md#_writefloat)
- [\_writeVariable](ReflectionTextureBlock.md#_writevariable)
- [autoConfigure](ReflectionTextureBlock.md#autoconfigure)
- [bind](ReflectionTextureBlock.md#bind)
- [build](ReflectionTextureBlock.md#build)
- [clone](ReflectionTextureBlock.md#clone)
- [connectTo](ReflectionTextureBlock.md#connectto)
- [dispose](ReflectionTextureBlock.md#dispose)
- [getClassName](ReflectionTextureBlock.md#getclassname)
- [getFirstAvailableInput](ReflectionTextureBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](ReflectionTextureBlock.md#getfirstavailableoutput)
- [getInputByName](ReflectionTextureBlock.md#getinputbyname)
- [getOutputByName](ReflectionTextureBlock.md#getoutputbyname)
- [getSiblingOutput](ReflectionTextureBlock.md#getsiblingoutput)
- [handleFragmentSideCodeReflectionColor](ReflectionTextureBlock.md#handlefragmentsidecodereflectioncolor)
- [handleFragmentSideCodeReflectionCoords](ReflectionTextureBlock.md#handlefragmentsidecodereflectioncoords)
- [handleFragmentSideInits](ReflectionTextureBlock.md#handlefragmentsideinits)
- [handleVertexSide](ReflectionTextureBlock.md#handlevertexside)
- [initialize](ReflectionTextureBlock.md#initialize)
- [initializeDefines](ReflectionTextureBlock.md#initializedefines)
- [isAnAncestorOf](ReflectionTextureBlock.md#isanancestorof)
- [isReady](ReflectionTextureBlock.md#isready)
- [prepareDefines](ReflectionTextureBlock.md#preparedefines)
- [provideFallbacks](ReflectionTextureBlock.md#providefallbacks)
- [registerInput](ReflectionTextureBlock.md#registerinput)
- [registerOutput](ReflectionTextureBlock.md#registeroutput)
- [replaceRepeatableContent](ReflectionTextureBlock.md#replacerepeatablecontent)
- [serialize](ReflectionTextureBlock.md#serialize)
- [updateUniformsAndSamples](ReflectionTextureBlock.md#updateuniformsandsamples)
- [validateBlockName](ReflectionTextureBlock.md#validateblockname)
- [writeOutputs](ReflectionTextureBlock.md#writeoutputs)

## Constructors

### constructor

• **new ReflectionTextureBlock**(`name`)

Create a new ReflectionTextureBlock

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the block name |

#### Overrides

ReflectionTextureBaseBlock.constructor

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:19

## Properties

### \_directionWName

• `Protected` **\_directionWName**: `string`

#### Inherited from

ReflectionTextureBaseBlock.\_directionWName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:60

___

### \_isUnique

• `Protected` **\_isUnique**: `boolean` = `false`

#### Inherited from

ReflectionTextureBaseBlock.\_isUnique

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:27

___

### \_positionUVWName

• `Protected` **\_positionUVWName**: `string`

#### Inherited from

ReflectionTextureBaseBlock.\_positionUVWName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:59

___

### \_reflectionColorName

• `Protected` **\_reflectionColorName**: `string`

#### Inherited from

ReflectionTextureBaseBlock.\_reflectionColorName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:66

___

### \_reflectionVectorName

• `Protected` **\_reflectionVectorName**: `string`

#### Inherited from

ReflectionTextureBaseBlock.\_reflectionVectorName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:61

___

### \_target

• `Protected` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

ReflectionTextureBaseBlock.\_target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:23

___

### \_texture

• `Protected` **\_texture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

ReflectionTextureBaseBlock.\_texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:68

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

ReflectionTextureBaseBlock.comments

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### inputsAreExclusive

• **inputsAreExclusive**: `boolean` = `false`

Gets or sets a boolean indicating that only one input can be connected at a time

#### Inherited from

ReflectionTextureBaseBlock.inputsAreExclusive

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:30

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

ReflectionTextureBaseBlock.uniqueId

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:67

___

### visibleInInspector

• **visibleInInspector**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited in the Inspector (false by default)

#### Inherited from

ReflectionTextureBaseBlock.visibleInInspector

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:163

___

### visibleOnFrame

• **visibleOnFrame**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited from a collapsed frame

#### Inherited from

ReflectionTextureBaseBlock.visibleOnFrame

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:166

## Accessors

### a

• `get` **a**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the a output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:128

___

### b

• `get` **b**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the b output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:121

___

### buildId

• `get` **buildId**(): `number`

Gets or sets the build Id

#### Returns

`number`

#### Inherited from

ReflectionTextureBaseBlock.buildId

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

ReflectionTextureBaseBlock.buildId

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:102

___

### cameraPosition

• `get` **cameraPosition**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the camera (or eye) position component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.cameraPosition

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:79

___

### g

• `get` **g**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the g output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:114

___

### inputs

• `get` **inputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of input points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

ReflectionTextureBaseBlock.inputs

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:123

___

### isFinalMerger

• `get` **isFinalMerger**(): `boolean`

Gets a boolean indicating that this block is an end block (e.g. it is generating a system value)

#### Returns

`boolean`

#### Inherited from

ReflectionTextureBaseBlock.isFinalMerger

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:84

___

### isInput

• `get` **isInput**(): `boolean`

Gets a boolean indicating that this block is an input (e.g. it sends data to the shader)

#### Returns

`boolean`

#### Inherited from

ReflectionTextureBaseBlock.isInput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:91

___

### isUnique

• `get` **isUnique**(): `boolean`

Gets a boolean indicating that this block can only be used once per NodeMaterial

#### Returns

`boolean`

#### Inherited from

ReflectionTextureBaseBlock.isUnique

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:77

___

### name

• `get` **name**(): `string`

Gets the name of the block

#### Returns

`string`

#### Inherited from

ReflectionTextureBaseBlock.name

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

ReflectionTextureBaseBlock.name

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:56

___

### outputs

• `get` **outputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of output points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

ReflectionTextureBaseBlock.outputs

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:128

___

### position

• `get` **position**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.position

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:51

___

### r

• `get` **r**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the r output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:107

___

### rgb

• `get` **rgb**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the rgb output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:93

___

### rgba

• `get` **rgba**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the rgba output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:100

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of the block

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

ReflectionTextureBaseBlock.target

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

ReflectionTextureBaseBlock.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:113

___

### texture

• `get` **texture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets or sets the texture associated with the node

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

ReflectionTextureBaseBlock.texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:72

• `set` **texture**(`texture`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Inherited from

ReflectionTextureBaseBlock.texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:76

___

### view

• `get` **view**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the view input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.view

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:86

___

### willBeGeneratedIntoVertexShaderFromFragmentShader

• `get` **willBeGeneratedIntoVertexShaderFromFragmentShader**(): `boolean`

Gets a boolean indicating that the code of this block will be promoted to vertex shader even if connected to fragment output

#### Returns

`boolean`

#### Inherited from

ReflectionTextureBaseBlock.willBeGeneratedIntoVertexShaderFromFragmentShader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:467

___

### world

• `get` **world**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.world

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:72

___

### worldNormal

• `get` **worldNormal**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world normal input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.worldNormal

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:65

___

### worldPosition

• `get` **worldPosition**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.worldPosition

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:58

## Methods

### \_buildBlock

▸ `Protected` **_buildBlock**(`state`): [`ReflectionTextureBlock`](ReflectionTextureBlock.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

[`ReflectionTextureBlock`](ReflectionTextureBlock.md)

#### Overrides

ReflectionTextureBaseBlock.\_buildBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:146

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

ReflectionTextureBaseBlock.\_declareOutput

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

#### Inherited from

ReflectionTextureBaseBlock.\_deserialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:504

___

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Inherited from

ReflectionTextureBaseBlock.\_dumpPropertiesCode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:474

___

### \_getTexture

▸ `Protected` **_getTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

ReflectionTextureBaseBlock.\_getTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:144

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

ReflectionTextureBaseBlock.\_inputRename

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

ReflectionTextureBaseBlock.\_linkConnectionTypes

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

ReflectionTextureBaseBlock.\_outputRename

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

ReflectionTextureBaseBlock.\_writeFloat

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

ReflectionTextureBaseBlock.\_writeVariable

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:209

___

### autoConfigure

▸ **autoConfigure**(`material`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `material` | [`NodeMaterial`](NodeMaterial.md) |

#### Returns

`void`

#### Overrides

ReflectionTextureBaseBlock.autoConfigure

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:132

___

### bind

▸ **bind**(`effect`, `nodeMaterial`, `mesh?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `effect` | [`Effect`](Effect.md) |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) |
| `mesh?` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Inherited from

ReflectionTextureBaseBlock.bind

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:215

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

ReflectionTextureBaseBlock.build

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

ReflectionTextureBaseBlock.clone

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:781

___

### connectTo

▸ **connectTo**(`other`, `options?`): `undefined` \| [`ReflectionTextureBlock`](ReflectionTextureBlock.md)

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

`undefined` \| [`ReflectionTextureBlock`](ReflectionTextureBlock.md)

the current block

#### Inherited from

ReflectionTextureBaseBlock.connectTo

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:364

___

### dispose

▸ **dispose**(): `void`

Release resources

#### Returns

`void`

#### Inherited from

ReflectionTextureBaseBlock.dispose

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

ReflectionTextureBaseBlock.getClassName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBlock.ts:44

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

ReflectionTextureBaseBlock.getFirstAvailableInput

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

ReflectionTextureBaseBlock.getFirstAvailableOutput

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

ReflectionTextureBaseBlock.getInputByName

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

ReflectionTextureBaseBlock.getOutputByName

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

ReflectionTextureBaseBlock.getSiblingOutput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:321

___

### handleFragmentSideCodeReflectionColor

▸ **handleFragmentSideCodeReflectionColor**(`lodVarName?`, `swizzleLookupTexture?`): `string`

Generates the reflection color code for the fragment code path

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `lodVarName?` | `string` | `undefined` | name of the lod variable |
| `swizzleLookupTexture` | `string` | `".rgb"` | swizzle to use for the final color variable |

#### Returns

`string`

the shader code

#### Inherited from

ReflectionTextureBaseBlock.handleFragmentSideCodeReflectionColor

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:423

___

### handleFragmentSideCodeReflectionCoords

▸ **handleFragmentSideCodeReflectionCoords**(`worldNormalVarName`, `worldPos?`, `onlyReflectionVector?`, `doNotEmitInvertZ?`): `string`

Generates the reflection coords code for the fragment code path

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `worldNormalVarName` | `string` | `undefined` | name of the world normal variable |
| `worldPos?` | `string` | `undefined` | name of the world position variable. If not provided, will use the world position connected to this block |
| `onlyReflectionVector` | `boolean` | `false` | if true, generates code only for the reflection vector computation, not for the reflection coordinates |
| `doNotEmitInvertZ` | `boolean` | `false` | if true, does not emit the invertZ code |

#### Returns

`string`

the shader code

#### Inherited from

ReflectionTextureBaseBlock.handleFragmentSideCodeReflectionCoords

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:342

___

### handleFragmentSideInits

▸ **handleFragmentSideInits**(`state`): `void`

Handles the inits for the fragment code path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | node material build state |

#### Returns

`void`

#### Inherited from

ReflectionTextureBaseBlock.handleFragmentSideInits

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:295

___

### handleVertexSide

▸ **handleVertexSide**(`state`): `string`

Gets the code to inject in the vertex shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | current state of the node material building |

#### Returns

`string`

the shader code

#### Inherited from

ReflectionTextureBaseBlock.handleVertexSide

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:242

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

ReflectionTextureBaseBlock.initialize

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

ReflectionTextureBaseBlock.initializeDefines

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

ReflectionTextureBaseBlock.isAnAncestorOf

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:336

___

### isReady

▸ **isReady**(): `boolean`

#### Returns

`boolean`

#### Inherited from

ReflectionTextureBaseBlock.isReady

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:205

___

### prepareDefines

▸ **prepareDefines**(`mesh`, `nodeMaterial`, `defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) |
| `defines` | `NodeMaterialDefines` |

#### Returns

`void`

#### Inherited from

ReflectionTextureBaseBlock.prepareDefines

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:180

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

ReflectionTextureBaseBlock.provideFallbacks

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:418

___

### registerInput

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`ReflectionTextureBlock`](ReflectionTextureBlock.md)

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

[`ReflectionTextureBlock`](ReflectionTextureBlock.md)

the current block

#### Inherited from

ReflectionTextureBaseBlock.registerInput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`ReflectionTextureBlock`](ReflectionTextureBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`ReflectionTextureBlock`](ReflectionTextureBlock.md)

the current block

#### Inherited from

ReflectionTextureBaseBlock.registerOutput

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

ReflectionTextureBaseBlock.replaceRepeatableContent

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:462

___

### serialize

▸ **serialize**(): `any`

#### Returns

`any`

#### Inherited from

ReflectionTextureBaseBlock.serialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:494

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

ReflectionTextureBaseBlock.updateUniformsAndSamples

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

ReflectionTextureBaseBlock.validateBlockName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:543

___

### writeOutputs

▸ **writeOutputs**(`state`, `varName`): `string`

Generates the code corresponding to the connected output points

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | node material build state |
| `varName` | `string` | name of the variable to output |

#### Returns

`string`

the shader code

#### Inherited from

ReflectionTextureBaseBlock.writeOutputs

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:455

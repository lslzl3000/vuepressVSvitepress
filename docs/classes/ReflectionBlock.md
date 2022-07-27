[@dev/core](../README.md) / [Exports](../modules.md) / ReflectionBlock

# Class: ReflectionBlock

Block used to implement the reflection module of the PBR material

## Hierarchy

- `ReflectionTextureBaseBlock`

  ↳ **`ReflectionBlock`**

## Table of contents

### Constructors

- [constructor](ReflectionBlock.md#constructor)

### Properties

- [\_directionWName](ReflectionBlock.md#_directionwname)
- [\_isUnique](ReflectionBlock.md#_isunique)
- [\_positionUVWName](ReflectionBlock.md#_positionuvwname)
- [\_reflectionColorName](ReflectionBlock.md#_reflectioncolorname)
- [\_reflectionVectorName](ReflectionBlock.md#_reflectionvectorname)
- [\_scene](ReflectionBlock.md#_scene)
- [\_target](ReflectionBlock.md#_target)
- [\_texture](ReflectionBlock.md#_texture)
- [\_vEnvironmentIrradianceName](ReflectionBlock.md#_venvironmentirradiancename)
- [comments](ReflectionBlock.md#comments)
- [forceIrradianceInFragment](ReflectionBlock.md#forceirradianceinfragment)
- [inputsAreExclusive](ReflectionBlock.md#inputsareexclusive)
- [uniqueId](ReflectionBlock.md#uniqueid)
- [useSphericalHarmonics](ReflectionBlock.md#usesphericalharmonics)
- [visibleInInspector](ReflectionBlock.md#visibleininspector)
- [visibleOnFrame](ReflectionBlock.md#visibleonframe)

### Accessors

- [buildId](ReflectionBlock.md#buildid)
- [cameraPosition](ReflectionBlock.md#cameraposition)
- [color](ReflectionBlock.md#color)
- [hasTexture](ReflectionBlock.md#hastexture)
- [inputs](ReflectionBlock.md#inputs)
- [isFinalMerger](ReflectionBlock.md#isfinalmerger)
- [isInput](ReflectionBlock.md#isinput)
- [isUnique](ReflectionBlock.md#isunique)
- [name](ReflectionBlock.md#name)
- [outputs](ReflectionBlock.md#outputs)
- [position](ReflectionBlock.md#position)
- [reflection](ReflectionBlock.md#reflection)
- [reflectionColor](ReflectionBlock.md#reflectioncolor)
- [target](ReflectionBlock.md#target)
- [texture](ReflectionBlock.md#texture)
- [view](ReflectionBlock.md#view)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](ReflectionBlock.md#willbegeneratedintovertexshaderfromfragmentshader)
- [world](ReflectionBlock.md#world)
- [worldNormal](ReflectionBlock.md#worldnormal)
- [worldPosition](ReflectionBlock.md#worldposition)

### Methods

- [\_buildBlock](ReflectionBlock.md#_buildblock)
- [\_declareOutput](ReflectionBlock.md#_declareoutput)
- [\_deserialize](ReflectionBlock.md#_deserialize)
- [\_dumpPropertiesCode](ReflectionBlock.md#_dumppropertiescode)
- [\_getTexture](ReflectionBlock.md#_gettexture)
- [\_inputRename](ReflectionBlock.md#_inputrename)
- [\_linkConnectionTypes](ReflectionBlock.md#_linkconnectiontypes)
- [\_outputRename](ReflectionBlock.md#_outputrename)
- [\_writeFloat](ReflectionBlock.md#_writefloat)
- [\_writeVariable](ReflectionBlock.md#_writevariable)
- [autoConfigure](ReflectionBlock.md#autoconfigure)
- [bind](ReflectionBlock.md#bind)
- [build](ReflectionBlock.md#build)
- [clone](ReflectionBlock.md#clone)
- [connectTo](ReflectionBlock.md#connectto)
- [dispose](ReflectionBlock.md#dispose)
- [getClassName](ReflectionBlock.md#getclassname)
- [getCode](ReflectionBlock.md#getcode)
- [getFirstAvailableInput](ReflectionBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](ReflectionBlock.md#getfirstavailableoutput)
- [getInputByName](ReflectionBlock.md#getinputbyname)
- [getOutputByName](ReflectionBlock.md#getoutputbyname)
- [getSiblingOutput](ReflectionBlock.md#getsiblingoutput)
- [handleFragmentSideCodeReflectionColor](ReflectionBlock.md#handlefragmentsidecodereflectioncolor)
- [handleFragmentSideCodeReflectionCoords](ReflectionBlock.md#handlefragmentsidecodereflectioncoords)
- [handleFragmentSideInits](ReflectionBlock.md#handlefragmentsideinits)
- [handleVertexSide](ReflectionBlock.md#handlevertexside)
- [initialize](ReflectionBlock.md#initialize)
- [initializeDefines](ReflectionBlock.md#initializedefines)
- [isAnAncestorOf](ReflectionBlock.md#isanancestorof)
- [isReady](ReflectionBlock.md#isready)
- [prepareDefines](ReflectionBlock.md#preparedefines)
- [provideFallbacks](ReflectionBlock.md#providefallbacks)
- [registerInput](ReflectionBlock.md#registerinput)
- [registerOutput](ReflectionBlock.md#registeroutput)
- [replaceRepeatableContent](ReflectionBlock.md#replacerepeatablecontent)
- [serialize](ReflectionBlock.md#serialize)
- [updateUniformsAndSamples](ReflectionBlock.md#updateuniformsandsamples)
- [validateBlockName](ReflectionBlock.md#validateblockname)
- [writeOutputs](ReflectionBlock.md#writeoutputs)

## Constructors

### constructor

• **new ReflectionBlock**(`name`)

Create a new ReflectionBlock

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the block name |

#### Overrides

ReflectionTextureBaseBlock.constructor

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:70

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

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:36

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

### \_vEnvironmentIrradianceName

• `Private` **\_vEnvironmentIrradianceName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:29

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

ReflectionTextureBaseBlock.comments

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### forceIrradianceInFragment

• **forceIrradianceInFragment**: `boolean` = `false`

Force the shader to compute irradiance in the fragment shader in order to take bump in account.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:64

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

### useSphericalHarmonics

• **useSphericalHarmonics**: `boolean` = `true`

Defines if the material uses spherical harmonics vs spherical polynomials for the
diffuse part of the IBL.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:58

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:126

___

### color

• `get` **color**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the color input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:140

___

### hasTexture

• `get` **hasTexture**(): `boolean`

Returns true if the block has a texture (either its own texture or the environment texture from the scene, if set)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:154

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

Gets the position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.position

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:98

___

### reflection

• `get` **reflection**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the reflection object output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:147

___

### reflectionColor

• `get` **reflectionColor**(): `string`

Gets the reflection color (either the name of the variable if the color input is connected, else a default value)

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:161

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:133

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:119

___

### worldNormal

• `get` **worldNormal**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world normal input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.worldNormal

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:112

___

### worldPosition

• `get` **worldPosition**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Overrides

ReflectionTextureBaseBlock.worldPosition

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:105

## Methods

### \_buildBlock

▸ `Protected` **_buildBlock**(`state`): [`ReflectionBlock`](ReflectionBlock.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

[`ReflectionBlock`](ReflectionBlock.md)

#### Overrides

ReflectionTextureBaseBlock.\_buildBlock

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:421

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

#### Overrides

ReflectionTextureBaseBlock.\_deserialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:454

___

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Overrides

ReflectionTextureBaseBlock.\_dumpPropertiesCode

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:432

___

### \_getTexture

▸ `Protected` **_getTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Overrides

ReflectionTextureBaseBlock.\_getTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:165

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

#### Inherited from

ReflectionTextureBaseBlock.autoConfigure

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/reflectionTextureBaseBlock.ts:148

___

### bind

▸ **bind**(`effect`, `nodeMaterial`, `mesh?`, `subMesh?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `effect` | [`Effect`](Effect.md) |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) |
| `mesh?` | [`Mesh`](Mesh.md) |
| `subMesh?` | [`SubMesh`](SubMesh.md) |

#### Returns

`void`

#### Overrides

ReflectionTextureBaseBlock.bind

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:206

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

▸ **connectTo**(`other`, `options?`): `undefined` \| [`ReflectionBlock`](ReflectionBlock.md)

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

`undefined` \| [`ReflectionBlock`](ReflectionBlock.md)

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:91

___

### getCode

▸ **getCode**(`state`, `normalVarName`): `string`

Gets the main code of the block (fragment side)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | current state of the node material building |
| `normalVarName` | `string` | name of the existing variable corresponding to the normal |

#### Returns

`string`

the shader code

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:313

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

#### Overrides

ReflectionTextureBaseBlock.handleVertexSide

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:260

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

#### Overrides

ReflectionTextureBaseBlock.prepareDefines

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:173

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

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`ReflectionBlock`](ReflectionBlock.md)

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

[`ReflectionBlock`](ReflectionBlock.md)

the current block

#### Inherited from

ReflectionTextureBaseBlock.registerInput

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`ReflectionBlock`](ReflectionBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`ReflectionBlock`](ReflectionBlock.md)

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

#### Overrides

ReflectionTextureBaseBlock.serialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/PBR/reflectionBlock.ts:444

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

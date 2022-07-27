[@dev/core](../README.md) / [Exports](../modules.md) / TextureBlock

# Class: TextureBlock

Block used to read a texture from a sampler

## Hierarchy

- [`NodeMaterialBlock`](NodeMaterialBlock.md)

  ↳ **`TextureBlock`**

## Table of contents

### Constructors

- [constructor](TextureBlock.md#constructor)

### Properties

- [\_convertToGammaSpace](TextureBlock.md#_converttogammaspace)
- [\_convertToLinearSpace](TextureBlock.md#_converttolinearspace)
- [\_defineName](TextureBlock.md#_definename)
- [\_fragmentOnly](TextureBlock.md#_fragmentonly)
- [\_gammaDefineName](TextureBlock.md#_gammadefinename)
- [\_imageSource](TextureBlock.md#_imagesource)
- [\_isUnique](TextureBlock.md#_isunique)
- [\_linearDefineName](TextureBlock.md#_lineardefinename)
- [\_mainUVDefineName](TextureBlock.md#_mainuvdefinename)
- [\_mainUVName](TextureBlock.md#_mainuvname)
- [\_samplerName](TextureBlock.md#_samplername)
- [\_target](TextureBlock.md#_target)
- [\_tempTextureRead](TextureBlock.md#_temptextureread)
- [\_texture](TextureBlock.md#_texture)
- [\_textureInfoName](TextureBlock.md#_textureinfoname)
- [\_textureTransformName](TextureBlock.md#_texturetransformname)
- [\_transformedUVName](TextureBlock.md#_transformeduvname)
- [comments](TextureBlock.md#comments)
- [disableLevelMultiplication](TextureBlock.md#disablelevelmultiplication)
- [inputsAreExclusive](TextureBlock.md#inputsareexclusive)
- [uniqueId](TextureBlock.md#uniqueid)
- [visibleInInspector](TextureBlock.md#visibleininspector)
- [visibleOnFrame](TextureBlock.md#visibleonframe)

### Accessors

- [\_isMixed](TextureBlock.md#_ismixed)
- [a](TextureBlock.md#a)
- [b](TextureBlock.md#b)
- [buildId](TextureBlock.md#buildid)
- [convertToGammaSpace](TextureBlock.md#converttogammaspace)
- [convertToLinearSpace](TextureBlock.md#converttolinearspace)
- [g](TextureBlock.md#g)
- [hasImageSource](TextureBlock.md#hasimagesource)
- [inputs](TextureBlock.md#inputs)
- [isFinalMerger](TextureBlock.md#isfinalmerger)
- [isInput](TextureBlock.md#isinput)
- [isUnique](TextureBlock.md#isunique)
- [level](TextureBlock.md#level)
- [name](TextureBlock.md#name)
- [outputs](TextureBlock.md#outputs)
- [r](TextureBlock.md#r)
- [rgb](TextureBlock.md#rgb)
- [rgba](TextureBlock.md#rgba)
- [samplerName](TextureBlock.md#samplername)
- [source](TextureBlock.md#source)
- [target](TextureBlock.md#target)
- [texture](TextureBlock.md#texture)
- [uv](TextureBlock.md#uv)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](TextureBlock.md#willbegeneratedintovertexshaderfromfragmentshader)

### Methods

- [\_buildBlock](TextureBlock.md#_buildblock)
- [\_declareOutput](TextureBlock.md#_declareoutput)
- [\_deserialize](TextureBlock.md#_deserialize)
- [\_dumpPropertiesCode](TextureBlock.md#_dumppropertiescode)
- [\_generateConversionCode](TextureBlock.md#_generateconversioncode)
- [\_generateTextureLookup](TextureBlock.md#_generatetexturelookup)
- [\_injectVertexCode](TextureBlock.md#_injectvertexcode)
- [\_inputRename](TextureBlock.md#_inputrename)
- [\_linkConnectionTypes](TextureBlock.md#_linkconnectiontypes)
- [\_outputRename](TextureBlock.md#_outputrename)
- [\_writeFloat](TextureBlock.md#_writefloat)
- [\_writeOutput](TextureBlock.md#_writeoutput)
- [\_writeTextureRead](TextureBlock.md#_writetextureread)
- [\_writeVariable](TextureBlock.md#_writevariable)
- [autoConfigure](TextureBlock.md#autoconfigure)
- [bind](TextureBlock.md#bind)
- [build](TextureBlock.md#build)
- [clone](TextureBlock.md#clone)
- [connectTo](TextureBlock.md#connectto)
- [dispose](TextureBlock.md#dispose)
- [getClassName](TextureBlock.md#getclassname)
- [getFirstAvailableInput](TextureBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](TextureBlock.md#getfirstavailableoutput)
- [getInputByName](TextureBlock.md#getinputbyname)
- [getOutputByName](TextureBlock.md#getoutputbyname)
- [getSiblingOutput](TextureBlock.md#getsiblingoutput)
- [initialize](TextureBlock.md#initialize)
- [initializeDefines](TextureBlock.md#initializedefines)
- [isAnAncestorOf](TextureBlock.md#isanancestorof)
- [isReady](TextureBlock.md#isready)
- [prepareDefines](TextureBlock.md#preparedefines)
- [provideFallbacks](TextureBlock.md#providefallbacks)
- [registerInput](TextureBlock.md#registerinput)
- [registerOutput](TextureBlock.md#registeroutput)
- [replaceRepeatableContent](TextureBlock.md#replacerepeatablecontent)
- [serialize](TextureBlock.md#serialize)
- [updateUniformsAndSamples](TextureBlock.md#updateuniformsandsamples)
- [validateBlockName](TextureBlock.md#validateblockname)

## Constructors

### constructor

• **new TextureBlock**(`name`, `fragmentOnly?`)

Create a new TextureBlock

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the block name |
| `fragmentOnly` | `boolean` | `false` |  |

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[constructor](NodeMaterialBlock.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:142

## Properties

### \_convertToGammaSpace

• `Private` **\_convertToGammaSpace**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:90

___

### \_convertToLinearSpace

• `Private` **\_convertToLinearSpace**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:111

___

### \_defineName

• `Private` **\_defineName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:27

___

### \_fragmentOnly

• `Private` **\_fragmentOnly**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:37

___

### \_gammaDefineName

• `Private` **\_gammaDefineName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:29

___

### \_imageSource

• `Private` **\_imageSource**: [`Nullable`](../modules.md#nullable)[`ImageSourceBlock`](ImageSourceBlock.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:38

___

### \_isUnique

• `Protected` **\_isUnique**: `boolean` = `false`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_isUnique](NodeMaterialBlock.md#_isunique)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:27

___

### \_linearDefineName

• `Private` **\_linearDefineName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:28

___

### \_mainUVDefineName

• `Private` **\_mainUVDefineName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:36

___

### \_mainUVName

• `Private` **\_mainUVName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:35

___

### \_samplerName

• `Private` **\_samplerName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:31

___

### \_target

• `Protected` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_target](NodeMaterialBlock.md#_target)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:23

___

### \_tempTextureRead

• `Private` **\_tempTextureRead**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:30

___

### \_texture

• `Protected` **\_texture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:40

___

### \_textureInfoName

• `Private` **\_textureInfoName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:34

___

### \_textureTransformName

• `Private` **\_textureTransformName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:33

___

### \_transformedUVName

• `Private` **\_transformedUVName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:32

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[comments](NodeMaterialBlock.md#comments)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### disableLevelMultiplication

• **disableLevelMultiplication**: `boolean` = `false`

Gets or sets a boolean indicating if multiplication of texture with level should be disabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:135

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

### \_isMixed

• `Private` `get` **_isMixed**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:378

___

### a

• `get` **a**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the a output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:231

___

### b

• `get` **b**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the b output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:224

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

### convertToGammaSpace

• `get` **convertToGammaSpace**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:107

• `set` **convertToGammaSpace**(`value`): `void`

Gets or sets a boolean indicating if content needs to be converted to gamma space

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:94

___

### convertToLinearSpace

• `get` **convertToLinearSpace**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:128

• `set` **convertToLinearSpace**(`value`): `void`

Gets or sets a boolean indicating if content needs to be converted to linear space

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:115

___

### g

• `get` **g**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the g output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:217

___

### hasImageSource

• `get` **hasImageSource**(): `boolean`

Gets a boolean indicating that this block is linked to an ImageSourceBlock

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:86

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

### level

• `get` **level**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the level output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:238

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

### r

• `get` **r**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the r output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:210

___

### rgb

• `get` **rgb**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the rgb output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:203

___

### rgba

• `get` **rgba**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the rgba output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:196

___

### samplerName

• `get` **samplerName**(): `string`

Gets the sampler name associated with this texture

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:76

___

### source

• `get` **source**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the source input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:189

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of the block

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Overrides

NodeMaterialBlock.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:242

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) |

#### Returns

`void`

#### Overrides

NodeMaterialBlock.target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:288

___

### texture

• `get` **texture**(): [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md)

Gets or sets the texture associated with the node

#### Returns

[`Nullable`](../modules.md#nullable)[`Texture`](Texture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:44

• `set` **texture**(`texture`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:51

___

### uv

• `get` **uv**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the uv input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:182

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

▸ `Protected` **_buildBlock**(`state`): `undefined` \| [`TextureBlock`](TextureBlock.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`undefined` \| [`TextureBlock`](TextureBlock.md)

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_buildBlock](NodeMaterialBlock.md#_buildblock)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:493

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:596

___

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_dumpPropertiesCode](NodeMaterialBlock.md#_dumppropertiescode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:556

___

### \_generateConversionCode

▸ `Private` **_generateConversionCode**(`state`, `output`, `swizzle`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |
| `output` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) |
| `swizzle` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:450

___

### \_generateTextureLookup

▸ `Private` **_generateTextureLookup**(`state`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:420

___

### \_injectVertexCode

▸ `Private` **_injectVertexCode**(`state`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:382

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

### \_writeOutput

▸ `Private` **_writeOutput**(`state`, `output`, `swizzle`, `vertexMode?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | `undefined` |
| `output` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | `undefined` |
| `swizzle` | `string` | `undefined` |
| `vertexMode` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:467

___

### \_writeTextureRead

▸ `Private` **_writeTextureRead**(`state`, `vertexMode?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `state` | `NodeMaterialBuildState` | `undefined` |
| `vertexMode` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:430

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

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[autoConfigure](NodeMaterialBlock.md#autoconfigure)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:290

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:363

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

▸ **connectTo**(`other`, `options?`): `undefined` \| [`TextureBlock`](TextureBlock.md)

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

`undefined` \| [`TextureBlock`](TextureBlock.md)

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:175

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

▸ **initializeDefines**(`mesh`, `nodeMaterial`, `defines`): `void`

Initialize defines for shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | defines the material defines to update |

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[initializeDefines](NodeMaterialBlock.md#initializedefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:312

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

▸ **isReady**(): `boolean`

Checks if the block is ready

#### Returns

`boolean`

true if the block is ready

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[isReady](NodeMaterialBlock.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:355

___

### prepareDefines

▸ **prepareDefines**(`mesh`, `nodeMaterial`, `defines`): `void`

Update defines for shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | defines the material defines to update |

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[prepareDefines](NodeMaterialBlock.md#preparedefines)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:322

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

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`TextureBlock`](TextureBlock.md)

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

[`TextureBlock`](TextureBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerInput](NodeMaterialBlock.md#registerinput)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`TextureBlock`](TextureBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`TextureBlock`](TextureBlock.md)

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

https://github.com/babylon.js/core/src/Materials/Node/Blocks/Dual/textureBlock.ts:582

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

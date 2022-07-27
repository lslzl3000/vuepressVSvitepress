[@dev/core](../README.md) / [Exports](../modules.md) / PBRMetallicRoughnessBlock

# Class: PBRMetallicRoughnessBlock

Block used to implement the PBR metallic/roughness model

## Hierarchy

- [`NodeMaterialBlock`](NodeMaterialBlock.md)

  ↳ **`PBRMetallicRoughnessBlock`**

## Table of contents

### Constructors

- [constructor](PBRMetallicRoughnessBlock.md#constructor)

### Properties

- [\_environmentBRDFTexture](PBRMetallicRoughnessBlock.md#_environmentbrdftexture)
- [\_environmentBrdfSamplerName](PBRMetallicRoughnessBlock.md#_environmentbrdfsamplername)
- [\_invertNormalName](PBRMetallicRoughnessBlock.md#_invertnormalname)
- [\_isUnique](PBRMetallicRoughnessBlock.md#_isunique)
- [\_lightId](PBRMetallicRoughnessBlock.md#_lightid)
- [\_metallicF0Factor](PBRMetallicRoughnessBlock.md#_metallicf0factor)
- [\_metallicReflectanceColor](PBRMetallicRoughnessBlock.md#_metallicreflectancecolor)
- [\_scene](PBRMetallicRoughnessBlock.md#_scene)
- [\_target](PBRMetallicRoughnessBlock.md#_target)
- [\_vMetallicReflectanceFactorsName](PBRMetallicRoughnessBlock.md#_vmetallicreflectancefactorsname)
- [\_vNormalWName](PBRMetallicRoughnessBlock.md#_vnormalwname)
- [alphaTestCutoff](PBRMetallicRoughnessBlock.md#alphatestcutoff)
- [comments](PBRMetallicRoughnessBlock.md#comments)
- [debugFactor](PBRMetallicRoughnessBlock.md#debugfactor)
- [debugLimit](PBRMetallicRoughnessBlock.md#debuglimit)
- [debugMode](PBRMetallicRoughnessBlock.md#debugmode)
- [directIntensity](PBRMetallicRoughnessBlock.md#directintensity)
- [enableSpecularAntiAliasing](PBRMetallicRoughnessBlock.md#enablespecularantialiasing)
- [environmentIntensity](PBRMetallicRoughnessBlock.md#environmentintensity)
- [forceNormalForward](PBRMetallicRoughnessBlock.md#forcenormalforward)
- [inputsAreExclusive](PBRMetallicRoughnessBlock.md#inputsareexclusive)
- [light](PBRMetallicRoughnessBlock.md#light)
- [lightFalloff](PBRMetallicRoughnessBlock.md#lightfalloff)
- [realTimeFiltering](PBRMetallicRoughnessBlock.md#realtimefiltering)
- [realTimeFilteringQuality](PBRMetallicRoughnessBlock.md#realtimefilteringquality)
- [specularIntensity](PBRMetallicRoughnessBlock.md#specularintensity)
- [uniqueId](PBRMetallicRoughnessBlock.md#uniqueid)
- [unlit](PBRMetallicRoughnessBlock.md#unlit)
- [useAlphaBlending](PBRMetallicRoughnessBlock.md#usealphablending)
- [useAlphaTest](PBRMetallicRoughnessBlock.md#usealphatest)
- [useEnergyConservation](PBRMetallicRoughnessBlock.md#useenergyconservation)
- [useHorizonOcclusion](PBRMetallicRoughnessBlock.md#usehorizonocclusion)
- [useRadianceOcclusion](PBRMetallicRoughnessBlock.md#useradianceocclusion)
- [useRadianceOverAlpha](PBRMetallicRoughnessBlock.md#useradianceoveralpha)
- [useSpecularOverAlpha](PBRMetallicRoughnessBlock.md#usespecularoveralpha)
- [visibleInInspector](PBRMetallicRoughnessBlock.md#visibleininspector)
- [visibleOnFrame](PBRMetallicRoughnessBlock.md#visibleonframe)

### Accessors

- [alpha](PBRMetallicRoughnessBlock.md#alpha)
- [ambientClr](PBRMetallicRoughnessBlock.md#ambientclr)
- [ambientColor](PBRMetallicRoughnessBlock.md#ambientcolor)
- [ambientOcc](PBRMetallicRoughnessBlock.md#ambientocc)
- [anisotropy](PBRMetallicRoughnessBlock.md#anisotropy)
- [baseColor](PBRMetallicRoughnessBlock.md#basecolor)
- [buildId](PBRMetallicRoughnessBlock.md#buildid)
- [cameraPosition](PBRMetallicRoughnessBlock.md#cameraposition)
- [clearcoat](PBRMetallicRoughnessBlock.md#clearcoat)
- [clearcoatDir](PBRMetallicRoughnessBlock.md#clearcoatdir)
- [clearcoatInd](PBRMetallicRoughnessBlock.md#clearcoatind)
- [diffuseDir](PBRMetallicRoughnessBlock.md#diffusedir)
- [diffuseInd](PBRMetallicRoughnessBlock.md#diffuseind)
- [indexOfRefraction](PBRMetallicRoughnessBlock.md#indexofrefraction)
- [inputs](PBRMetallicRoughnessBlock.md#inputs)
- [iridescence](PBRMetallicRoughnessBlock.md#iridescence)
- [isFinalMerger](PBRMetallicRoughnessBlock.md#isfinalmerger)
- [isInput](PBRMetallicRoughnessBlock.md#isinput)
- [isUnique](PBRMetallicRoughnessBlock.md#isunique)
- [lighting](PBRMetallicRoughnessBlock.md#lighting)
- [metallic](PBRMetallicRoughnessBlock.md#metallic)
- [name](PBRMetallicRoughnessBlock.md#name)
- [opacity](PBRMetallicRoughnessBlock.md#opacity)
- [outputs](PBRMetallicRoughnessBlock.md#outputs)
- [perturbedNormal](PBRMetallicRoughnessBlock.md#perturbednormal)
- [reflection](PBRMetallicRoughnessBlock.md#reflection)
- [refraction](PBRMetallicRoughnessBlock.md#refraction)
- [roughness](PBRMetallicRoughnessBlock.md#roughness)
- [shadow](PBRMetallicRoughnessBlock.md#shadow)
- [sheen](PBRMetallicRoughnessBlock.md#sheen)
- [sheenDir](PBRMetallicRoughnessBlock.md#sheendir)
- [sheenInd](PBRMetallicRoughnessBlock.md#sheenind)
- [specularDir](PBRMetallicRoughnessBlock.md#speculardir)
- [specularInd](PBRMetallicRoughnessBlock.md#specularind)
- [subsurface](PBRMetallicRoughnessBlock.md#subsurface)
- [target](PBRMetallicRoughnessBlock.md#target)
- [view](PBRMetallicRoughnessBlock.md#view)
- [willBeGeneratedIntoVertexShaderFromFragmentShader](PBRMetallicRoughnessBlock.md#willbegeneratedintovertexshaderfromfragmentshader)
- [worldNormal](PBRMetallicRoughnessBlock.md#worldnormal)
- [worldPosition](PBRMetallicRoughnessBlock.md#worldposition)

### Methods

- [\_buildBlock](PBRMetallicRoughnessBlock.md#_buildblock)
- [\_declareOutput](PBRMetallicRoughnessBlock.md#_declareoutput)
- [\_deserialize](PBRMetallicRoughnessBlock.md#_deserialize)
- [\_dumpPropertiesCode](PBRMetallicRoughnessBlock.md#_dumppropertiescode)
- [\_getAlbedoOpacityCode](PBRMetallicRoughnessBlock.md#_getalbedoopacitycode)
- [\_getAmbientOcclusionCode](PBRMetallicRoughnessBlock.md#_getambientocclusioncode)
- [\_getReflectivityCode](PBRMetallicRoughnessBlock.md#_getreflectivitycode)
- [\_injectVertexCode](PBRMetallicRoughnessBlock.md#_injectvertexcode)
- [\_inputRename](PBRMetallicRoughnessBlock.md#_inputrename)
- [\_linkConnectionTypes](PBRMetallicRoughnessBlock.md#_linkconnectiontypes)
- [\_outputRename](PBRMetallicRoughnessBlock.md#_outputrename)
- [\_writeFloat](PBRMetallicRoughnessBlock.md#_writefloat)
- [\_writeVariable](PBRMetallicRoughnessBlock.md#_writevariable)
- [autoConfigure](PBRMetallicRoughnessBlock.md#autoconfigure)
- [bind](PBRMetallicRoughnessBlock.md#bind)
- [build](PBRMetallicRoughnessBlock.md#build)
- [clone](PBRMetallicRoughnessBlock.md#clone)
- [connectTo](PBRMetallicRoughnessBlock.md#connectto)
- [dispose](PBRMetallicRoughnessBlock.md#dispose)
- [getClassName](PBRMetallicRoughnessBlock.md#getclassname)
- [getFirstAvailableInput](PBRMetallicRoughnessBlock.md#getfirstavailableinput)
- [getFirstAvailableOutput](PBRMetallicRoughnessBlock.md#getfirstavailableoutput)
- [getInputByName](PBRMetallicRoughnessBlock.md#getinputbyname)
- [getOutputByName](PBRMetallicRoughnessBlock.md#getoutputbyname)
- [getSiblingOutput](PBRMetallicRoughnessBlock.md#getsiblingoutput)
- [initialize](PBRMetallicRoughnessBlock.md#initialize)
- [initializeDefines](PBRMetallicRoughnessBlock.md#initializedefines)
- [isAnAncestorOf](PBRMetallicRoughnessBlock.md#isanancestorof)
- [isReady](PBRMetallicRoughnessBlock.md#isready)
- [prepareDefines](PBRMetallicRoughnessBlock.md#preparedefines)
- [provideFallbacks](PBRMetallicRoughnessBlock.md#providefallbacks)
- [registerInput](PBRMetallicRoughnessBlock.md#registerinput)
- [registerOutput](PBRMetallicRoughnessBlock.md#registeroutput)
- [replaceRepeatableContent](PBRMetallicRoughnessBlock.md#replacerepeatablecontent)
- [serialize](PBRMetallicRoughnessBlock.md#serialize)
- [updateUniformsAndSamples](PBRMetallicRoughnessBlock.md#updateuniformsandsamples)
- [validateBlockName](PBRMetallicRoughnessBlock.md#validateblockname)

## Constructors

### constructor

• **new PBRMetallicRoughnessBlock**(`name`)

Create a new ReflectionBlock

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the block name |

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[constructor](NodeMaterialBlock.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:74

## Properties

### \_environmentBRDFTexture

• `Private` **\_environmentBRDFTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:62

___

### \_environmentBrdfSamplerName

• `Private` **\_environmentBrdfSamplerName**: `string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:63

___

### \_invertNormalName

• `Private` **\_invertNormalName**: `string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:65

___

### \_isUnique

• `Protected` **\_isUnique**: `boolean` = `false`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_isUnique](NodeMaterialBlock.md#_isunique)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:27

___

### \_lightId

• `Private` **\_lightId**: `number`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:60

___

### \_metallicF0Factor

• `Private` **\_metallicF0Factor**: `number` = `1`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:67

___

### \_metallicReflectanceColor

• `Private` **\_metallicReflectanceColor**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:66

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:61

___

### \_target

• `Protected` **\_target**: [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[_target](NodeMaterialBlock.md#_target)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:23

___

### \_vMetallicReflectanceFactorsName

• `Private` **\_vMetallicReflectanceFactorsName**: `string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:68

___

### \_vNormalWName

• `Private` **\_vNormalWName**: `string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:64

___

### alphaTestCutoff

• **alphaTestCutoff**: `number` = `0.5`

Defines the alpha limits in alpha test mode.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:194

___

### comments

• **comments**: `string` = `""`

Gets or sets the comments associated with this block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[comments](NodeMaterialBlock.md#comments)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:72

___

### debugFactor

• **debugFactor**: `number` = `1`

As the default viewing range might not be enough (if the ambient is really small for instance)
You can use the factor to better multiply the final value.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:350

___

### debugLimit

• **debugLimit**: `number` = `0`

Specify from where on screen the debug mode should start.
The value goes from -1 (full screen) to 1 (not visible)
It helps with side by side comparison against the final render
This defaults to 0

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:343

___

### debugMode

• **debugMode**: `number` = `0`

Defines the material debug mode.
It helps seeing only some components of the material while troubleshooting.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:334

___

### directIntensity

• **directIntensity**: `number` = `1.0`

Intensity of the direct lights e.g. the four lights available in your scene.
This impacts both the direct diffuse and specular highlights.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:154

___

### enableSpecularAntiAliasing

• **enableSpecularAntiAliasing**: `boolean` = `false`

Enables specular anti aliasing in the PBR shader.
It will both interacts on the Geometry for analytical and IBL lighting.
It also prefilter the roughness map based on the bump values.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:222

___

### environmentIntensity

• **environmentIntensity**: `number` = `1.0`

Intensity of the environment e.g. how much the environment will light the object
either through harmonics for rough material or through the reflection for shiny ones.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:161

___

### forceNormalForward

• **forceNormalForward**: `boolean` = `false`

Force normal to face away from face.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:273

___

### inputsAreExclusive

• **inputsAreExclusive**: `boolean` = `false`

Gets or sets a boolean indicating that only one input can be connected at a time

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[inputsAreExclusive](NodeMaterialBlock.md#inputsareexclusive)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:30

___

### light

• **light**: [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Gets or sets the light associated with this block

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:58

___

### lightFalloff

• **lightFalloff**: `number` = `0`

Defines the  falloff type used in this material.
It by default is Physical.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:182

___

### realTimeFiltering

• **realTimeFiltering**: `boolean` = `false`

Enables realtime filtering on the texture.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:228

___

### realTimeFilteringQuality

• **realTimeFilteringQuality**: `number` = `Constants.TEXTURE_FILTERING_QUALITY_LOW`

Quality switch for realtime filtering

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:241

___

### specularIntensity

• **specularIntensity**: `number` = `1.0`

This is a special control allowing the reduction of the specular highlights coming from the
four lights of the scene. Those highlights may not be needed in full environment lighting.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:168

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[uniqueId](NodeMaterialBlock.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:67

___

### unlit

• **unlit**: `boolean` = `false`

If set to true, no lighting calculations will be applied.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:267

___

### useAlphaBlending

• **useAlphaBlending**: `boolean` = `false`

Specifies that alpha blending should be used

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:200

___

### useAlphaTest

• **useAlphaTest**: `boolean` = `false`

Specifies that alpha test should be used

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:188

___

### useEnergyConservation

• **useEnergyConservation**: `boolean` = `true`

Defines if the material uses energy conservation.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:247

___

### useHorizonOcclusion

• **useHorizonOcclusion**: `boolean` = `true`

This parameters will enable/disable Horizon occlusion to prevent normal maps to look shiny when the normal
makes the reflect vector face the model (under horizon).

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:261

___

### useRadianceOcclusion

• **useRadianceOcclusion**: `boolean` = `true`

This parameters will enable/disable radiance occlusion by preventing the radiance to lit
too much the area relying on ambient texture to define their ambient occlusion.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:254

___

### useRadianceOverAlpha

• **useRadianceOverAlpha**: `boolean` = `true`

Specifies that the material will keeps the reflection highlights over a transparent surface (only the most luminous ones).
A car glass is a good example of that. When the street lights reflects on it you can not see what is behind.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:207

___

### useSpecularOverAlpha

• **useSpecularOverAlpha**: `boolean` = `true`

Specifies that the material will keeps the specular highlights over a transparent surface (only the most luminous ones).
A car glass is a good example of that. When sun reflects on it you can not see what is behind.

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:214

___

### visibleInInspector

• **visibleInInspector**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited in the Inspector (false by default)

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[visibleInInspector](NodeMaterialBlock.md#visibleininspector)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:163

___

### visibleOnFrame

• **visibleOnFrame**: `boolean` = `false`

Gets or sets a boolean indicating that this input can be edited from a collapsed frame

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[visibleOnFrame](NodeMaterialBlock.md#visibleonframe)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:166

## Accessors

### alpha

• `get` **alpha**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the alpha output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:624

___

### ambientClr

• `get` **ambientClr**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the ambient output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:540

___

### ambientColor

• `get` **ambientColor**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the ambient color input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:491

___

### ambientOcc

• `get` **ambientOcc**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the ambient occlusion input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:470

___

### anisotropy

• `get` **anisotropy**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the anisotropy object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:526

___

### baseColor

• `get` **baseColor**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the base color input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:449

___

### buildId

• `get` **buildId**(): `number`

Gets or sets the build Id

#### Returns

`number`

#### Inherited from

NodeMaterialBlock.buildId

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:98

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:102

___

### cameraPosition

• `get` **cameraPosition**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the camera position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:435

___

### clearcoat

• `get` **clearcoat**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the clear coat object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:505

___

### clearcoatDir

• `get` **clearcoatDir**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the clear coat output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:561

___

### clearcoatInd

• `get` **clearcoatInd**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the indirect clear coat output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:589

___

### diffuseDir

• `get` **diffuseDir**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the diffuse output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:547

___

### diffuseInd

• `get` **diffuseInd**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the indirect diffuse output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:575

___

### indexOfRefraction

• `get` **indexOfRefraction**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the index of refraction input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:484

___

### inputs

• `get` **inputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of input points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

NodeMaterialBlock.inputs

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:123

___

### iridescence

• `get` **iridescence**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the iridescence object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:533

___

### isFinalMerger

• `get` **isFinalMerger**(): `boolean`

Gets a boolean indicating that this block is an end block (e.g. it is generating a system value)

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isFinalMerger

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:84

___

### isInput

• `get` **isInput**(): `boolean`

Gets a boolean indicating that this block is an input (e.g. it sends data to the shader)

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isInput

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:91

___

### isUnique

• `get` **isUnique**(): `boolean`

Gets a boolean indicating that this block can only be used once per NodeMaterial

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.isUnique

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:77

___

### lighting

• `get` **lighting**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the global lighting output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:610

___

### metallic

• `get` **metallic**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the metallic input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:456

___

### name

• `get` **name**(): `string`

Gets the name of the block

#### Returns

`string`

#### Inherited from

NodeMaterialBlock.name

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:49

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:56

___

### opacity

• `get` **opacity**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the opacity input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:477

___

### outputs

• `get` **outputs**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

Gets the list of output points

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)[]

#### Inherited from

NodeMaterialBlock.outputs

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:128

___

### perturbedNormal

• `get` **perturbedNormal**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the perturbed normal input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:442

___

### reflection

• `get` **reflection**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the reflection object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:498

___

### refraction

• `get` **refraction**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the refraction output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:603

___

### roughness

• `get` **roughness**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the roughness input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:463

___

### shadow

• `get` **shadow**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the shadow output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:617

___

### sheen

• `get` **sheen**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the sheen object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:512

___

### sheenDir

• `get` **sheenDir**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the sheen output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:568

___

### sheenInd

• `get` **sheenInd**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the indirect sheen output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:596

___

### specularDir

• `get` **specularDir**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the specular output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:554

___

### specularInd

• `get` **specularInd**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the indirect specular output component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:582

___

### subsurface

• `get` **subsurface**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the sub surface object parameters

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:519

___

### target

• `get` **target**(): [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

Gets or sets the target of the block

#### Returns

[`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md)

#### Inherited from

NodeMaterialBlock.target

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:109

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:113

___

### view

• `get` **view**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the view matrix parameter

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:428

___

### willBeGeneratedIntoVertexShaderFromFragmentShader

• `get` **willBeGeneratedIntoVertexShaderFromFragmentShader**(): `boolean`

Gets a boolean indicating that the code of this block will be promoted to vertex shader even if connected to fragment output

#### Returns

`boolean`

#### Inherited from

NodeMaterialBlock.willBeGeneratedIntoVertexShaderFromFragmentShader

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:467

___

### worldNormal

• `get` **worldNormal**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world normal input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:421

___

### worldPosition

• `get` **worldPosition**(): [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

Gets the world position input component

#### Returns

[`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:414

## Methods

### \_buildBlock

▸ `Protected` **_buildBlock**(`state`): [`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

[`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_buildBlock](NodeMaterialBlock.md#_buildblock)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:989

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:205

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:1407

___

### \_dumpPropertiesCode

▸ `Protected` **_dumpPropertiesCode**(): `string`

#### Returns

`string`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[_dumpPropertiesCode](NodeMaterialBlock.md#_dumppropertiescode)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:1355

___

### \_getAlbedoOpacityCode

▸ `Private` **_getAlbedoOpacityCode**(): `string`

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:906

___

### \_getAmbientOcclusionCode

▸ `Private` **_getAmbientOcclusionCode**(): `string`

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:931

___

### \_getReflectivityCode

▸ `Private` **_getReflectivityCode**(`state`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `state` | `NodeMaterialBuildState` |

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:947

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:838

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:667

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:502

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:671

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:219

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:209

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:628

___

### bind

▸ **bind**(`effect`, `nodeMaterial`, `mesh?`): `void`

Bind data to effect. Will only be called for blocks with isBindable === true

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind data to |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the hosting NodeMaterial |
| `mesh?` | [`Mesh`](Mesh.md) | defines the mesh that will be rendered |

#### Returns

`void`

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[bind](NodeMaterialBlock.md#bind)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:789

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:580

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:781

___

### connectTo

▸ **connectTo**(`other`, `options?`): `undefined` \| [`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

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

`undefined` \| [`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[connectTo](NodeMaterialBlock.md#connectto)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:364

___

### dispose

▸ **dispose**(): `void`

Release resources

#### Returns

`void`

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[dispose](NodeMaterialBlock.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:869

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:407

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:289

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:306

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:137

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:152

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:321

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

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[initialize](NodeMaterialBlock.md#initialize)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:356

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:430

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:336

___

### isReady

▸ **isReady**(`mesh`, `nodeMaterial`, `defines`): `boolean`

Checks if the block is ready

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to be rendered |
| `nodeMaterial` | [`NodeMaterial`](NodeMaterial.md) | defines the node material requesting the update |
| `defines` | `NodeMaterialDefines` | defines the material defines to update |

#### Returns

`boolean`

true if the block is ready

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[isReady](NodeMaterialBlock.md#isready)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:775

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:650

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:418

___

### registerInput

▸ **registerInput**(`name`, `type`, `isOptional?`, `target?`, `point?`): [`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

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

[`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerInput](NodeMaterialBlock.md#registerinput)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:245

___

### registerOutput

▸ **registerOutput**(`name`, `type`, `target?`, `point?`): [`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

Register a new output. Must be called inside a block constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the connection point name |
| `type` | [`NodeMaterialBlockConnectionPointTypes`](../enums/NodeMaterialBlockConnectionPointTypes.md) | defines the connection point type |
| `target?` | [`NodeMaterialBlockTargets`](../enums/NodeMaterialBlockTargets.md) | defines the target to use to limit the connection point (will be VertexAndFragment by default) |
| `point?` | [`NodeMaterialConnectionPoint`](NodeMaterialConnectionPoint.md) | an already created connection point. If not provided, create a new one |

#### Returns

[`PBRMetallicRoughnessBlock`](PBRMetallicRoughnessBlock.md)

the current block

#### Inherited from

[NodeMaterialBlock](NodeMaterialBlock.md).[registerOutput](NodeMaterialBlock.md#registeroutput)

#### Defined in

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:272

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:462

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

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:1379

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

#### Overrides

[NodeMaterialBlock](NodeMaterialBlock.md).[updateUniformsAndSamples](NodeMaterialBlock.md#updateuniformsandsamples)

#### Defined in

packages/dev/core/src/Materials/Node/Blocks/PBR/pbrMetallicRoughnessBlock.ts:758

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

packages/dev/core/src/Materials/Node/nodeMaterialBlock.ts:543

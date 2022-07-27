[@dev/core](../README.md) / [Exports](../modules.md) / SpotLight

# Class: SpotLight

A spot light is defined by a position, a direction, an angle, and an exponent.
These values define a cone of light starting from the position, emitting toward the direction.
The angle, in radians, defines the size (field of illumination) of the spotlight's conical beam,
and the exponent defines the speed of the decay of the light with distance (reach).
Documentation: https://doc.babylonjs.com/babylon101/lights

## Hierarchy

- [`ShadowLight`](ShadowLight.md)

  ↳ **`SpotLight`**

## Table of contents

### Constructors

- [constructor](SpotLight.md#constructor)

### Properties

- [\_angle](SpotLight.md#_angle)
- [\_cosHalfAngle](SpotLight.md#_coshalfangle)
- [\_direction](SpotLight.md#_direction)
- [\_innerAngle](SpotLight.md#_innerangle)
- [\_inverseSquaredRange](SpotLight.md#_inversesquaredrange)
- [\_isDirty](SpotLight.md#_isdirty)
- [\_lightAngleOffset](SpotLight.md#_lightangleoffset)
- [\_lightAngleScale](SpotLight.md#_lightanglescale)
- [\_parentNode](SpotLight.md#_parentnode)
- [\_position](SpotLight.md#_position)
- [\_projectionTexture](SpotLight.md#_projectiontexture)
- [\_projectionTextureDirty](SpotLight.md#_projectiontexturedirty)
- [\_projectionTextureLightFar](SpotLight.md#_projectiontexturelightfar)
- [\_projectionTextureLightNear](SpotLight.md#_projectiontexturelightnear)
- [\_projectionTextureMatrix](SpotLight.md#_projectiontexturematrix)
- [\_projectionTextureProjectionLightDirty](SpotLight.md#_projectiontextureprojectionlightdirty)
- [\_projectionTextureProjectionLightMatrix](SpotLight.md#_projectiontextureprojectionlightmatrix)
- [\_projectionTextureScalingMatrix](SpotLight.md#_projectiontexturescalingmatrix)
- [\_projectionTextureUpDirection](SpotLight.md#_projectiontextureupdirection)
- [\_projectionTextureViewLightDirty](SpotLight.md#_projectiontextureviewlightdirty)
- [\_projectionTextureViewLightMatrix](SpotLight.md#_projectiontextureviewlightmatrix)
- [\_projectionTextureViewTargetVector](SpotLight.md#_projectiontextureviewtargetvector)
- [\_ranges](SpotLight.md#_ranges)
- [\_shadowAngleScale](SpotLight.md#_shadowanglescale)
- [\_shadowMaxZ](SpotLight.md#_shadowmaxz)
- [\_shadowMinZ](SpotLight.md#_shadowminz)
- [animations](SpotLight.md#animations)
- [customProjectionMatrixBuilder](SpotLight.md#customprojectionmatrixbuilder)
- [diffuse](SpotLight.md#diffuse)
- [exponent](SpotLight.md#exponent)
- [falloffType](SpotLight.md#fallofftype)
- [id](SpotLight.md#id)
- [inspectableCustomProperties](SpotLight.md#inspectablecustomproperties)
- [intensity](SpotLight.md#intensity)
- [metadata](SpotLight.md#metadata)
- [name](SpotLight.md#name)
- [onDisposeObservable](SpotLight.md#ondisposeobservable)
- [onReady](SpotLight.md#onready)
- [renderPriority](SpotLight.md#renderpriority)
- [reservedDataStore](SpotLight.md#reserveddatastore)
- [specular](SpotLight.md#specular)
- [state](SpotLight.md#state)
- [transformedDirection](SpotLight.md#transformeddirection)
- [transformedPosition](SpotLight.md#transformedposition)
- [uniqueId](SpotLight.md#uniqueid)
- [FALLOFF\_DEFAULT](SpotLight.md#falloff_default)
- [FALLOFF\_GLTF](SpotLight.md#falloff_gltf)
- [FALLOFF\_PHYSICAL](SpotLight.md#falloff_physical)
- [FALLOFF\_STANDARD](SpotLight.md#falloff_standard)
- [INTENSITYMODE\_AUTOMATIC](SpotLight.md#intensitymode_automatic)
- [INTENSITYMODE\_ILLUMINANCE](SpotLight.md#intensitymode_illuminance)
- [INTENSITYMODE\_LUMINANCE](SpotLight.md#intensitymode_luminance)
- [INTENSITYMODE\_LUMINOUSINTENSITY](SpotLight.md#intensitymode_luminousintensity)
- [INTENSITYMODE\_LUMINOUSPOWER](SpotLight.md#intensitymode_luminouspower)
- [LIGHTMAP\_DEFAULT](SpotLight.md#lightmap_default)
- [LIGHTMAP\_SHADOWSONLY](SpotLight.md#lightmap_shadowsonly)
- [LIGHTMAP\_SPECULAR](SpotLight.md#lightmap_specular)
- [LIGHTTYPEID\_DIRECTIONALLIGHT](SpotLight.md#lighttypeid_directionallight)
- [LIGHTTYPEID\_HEMISPHERICLIGHT](SpotLight.md#lighttypeid_hemisphericlight)
- [LIGHTTYPEID\_POINTLIGHT](SpotLight.md#lighttypeid_pointlight)
- [LIGHTTYPEID\_SPOTLIGHT](SpotLight.md#lighttypeid_spotlight)

### Accessors

- [angle](SpotLight.md#angle)
- [animationPropertiesOverride](SpotLight.md#animationpropertiesoverride)
- [behaviors](SpotLight.md#behaviors)
- [direction](SpotLight.md#direction)
- [doNotSerialize](SpotLight.md#donotserialize)
- [excludeWithLayerMask](SpotLight.md#excludewithlayermask)
- [excludedMeshes](SpotLight.md#excludedmeshes)
- [includeOnlyWithLayerMask](SpotLight.md#includeonlywithlayermask)
- [includedOnlyMeshes](SpotLight.md#includedonlymeshes)
- [innerAngle](SpotLight.md#innerangle)
- [intensityMode](SpotLight.md#intensitymode)
- [lightmapMode](SpotLight.md#lightmapmode)
- [onClonedObservable](SpotLight.md#onclonedobservable)
- [onDispose](SpotLight.md#ondispose)
- [onEnabledStateChangedObservable](SpotLight.md#onenabledstatechangedobservable)
- [parent](SpotLight.md#parent)
- [position](SpotLight.md#position)
- [projectionTexture](SpotLight.md#projectiontexture)
- [projectionTextureLightFar](SpotLight.md#projectiontexturelightfar)
- [projectionTextureLightNear](SpotLight.md#projectiontexturelightnear)
- [projectionTextureMatrix](SpotLight.md#projectiontexturematrix)
- [projectionTextureProjectionLightMatrix](SpotLight.md#projectiontextureprojectionlightmatrix)
- [projectionTextureUpDirection](SpotLight.md#projectiontextureupdirection)
- [radius](SpotLight.md#radius)
- [range](SpotLight.md#range)
- [shadowAngleScale](SpotLight.md#shadowanglescale)
- [shadowEnabled](SpotLight.md#shadowenabled)
- [shadowMaxZ](SpotLight.md#shadowmaxz)
- [shadowMinZ](SpotLight.md#shadowminz)
- [worldMatrixFromCache](SpotLight.md#worldmatrixfromcache)

### Methods

- [\_bindLight](SpotLight.md#_bindlight)
- [\_buildUniformLayout](SpotLight.md#_builduniformlayout)
- [\_computeAngleValues](SpotLight.md#_computeanglevalues)
- [\_computeProjectionTextureMatrix](SpotLight.md#_computeprojectiontexturematrix)
- [\_computeProjectionTextureProjectionLightMatrix](SpotLight.md#_computeprojectiontextureprojectionlightmatrix)
- [\_computeProjectionTextureViewLightMatrix](SpotLight.md#_computeprojectiontextureviewlightmatrix)
- [\_setDefaultShadowProjectionMatrix](SpotLight.md#_setdefaultshadowprojectionmatrix)
- [\_setDirection](SpotLight.md#_setdirection)
- [\_setPosition](SpotLight.md#_setposition)
- [addBehavior](SpotLight.md#addbehavior)
- [beginAnimation](SpotLight.md#beginanimation)
- [canAffectMesh](SpotLight.md#canaffectmesh)
- [clone](SpotLight.md#clone)
- [computeTransformedInformation](SpotLight.md#computetransformedinformation)
- [computeWorldMatrix](SpotLight.md#computeworldmatrix)
- [createAnimationRange](SpotLight.md#createanimationrange)
- [deleteAnimationRange](SpotLight.md#deleteanimationrange)
- [dispose](SpotLight.md#dispose)
- [forceProjectionMatrixCompute](SpotLight.md#forceprojectionmatrixcompute)
- [getAbsolutePosition](SpotLight.md#getabsoluteposition)
- [getAnimationByName](SpotLight.md#getanimationbyname)
- [getAnimationRange](SpotLight.md#getanimationrange)
- [getAnimationRanges](SpotLight.md#getanimationranges)
- [getBehaviorByName](SpotLight.md#getbehaviorbyname)
- [getChildMeshes](SpotLight.md#getchildmeshes)
- [getChildren](SpotLight.md#getchildren)
- [getClassName](SpotLight.md#getclassname)
- [getDepthMaxZ](SpotLight.md#getdepthmaxz)
- [getDepthMinZ](SpotLight.md#getdepthminz)
- [getDepthScale](SpotLight.md#getdepthscale)
- [getDescendants](SpotLight.md#getdescendants)
- [getEngine](SpotLight.md#getengine)
- [getHierarchyBoundingVectors](SpotLight.md#gethierarchyboundingvectors)
- [getRotation](SpotLight.md#getrotation)
- [getScaledIntensity](SpotLight.md#getscaledintensity)
- [getScene](SpotLight.md#getscene)
- [getShadowDirection](SpotLight.md#getshadowdirection)
- [getShadowGenerator](SpotLight.md#getshadowgenerator)
- [getTypeID](SpotLight.md#gettypeid)
- [getWorldMatrix](SpotLight.md#getworldmatrix)
- [isDescendantOf](SpotLight.md#isdescendantof)
- [isDisposed](SpotLight.md#isdisposed)
- [isEnabled](SpotLight.md#isenabled)
- [isReady](SpotLight.md#isready)
- [markAsDirty](SpotLight.md#markasdirty)
- [needCube](SpotLight.md#needcube)
- [needProjectionMatrixCompute](SpotLight.md#needprojectionmatrixcompute)
- [prepareLightSpecificDefines](SpotLight.md#preparelightspecificdefines)
- [removeBehavior](SpotLight.md#removebehavior)
- [serialize](SpotLight.md#serialize)
- [serializeAnimationRanges](SpotLight.md#serializeanimationranges)
- [setDirectionToTarget](SpotLight.md#setdirectiontotarget)
- [setEnabled](SpotLight.md#setenabled)
- [setShadowProjectionMatrix](SpotLight.md#setshadowprojectionmatrix)
- [toString](SpotLight.md#tostring)
- [transferTexturesToEffect](SpotLight.md#transfertexturestoeffect)
- [transferToEffect](SpotLight.md#transfertoeffect)
- [transferToNodeMaterialEffect](SpotLight.md#transfertonodematerialeffect)
- [AddNodeConstructor](SpotLight.md#addnodeconstructor)
- [Construct](SpotLight.md#construct)
- [GetConstructorFromName](SpotLight.md#getconstructorfromname)
- [Parse](SpotLight.md#parse)
- [ParseAnimationRanges](SpotLight.md#parseanimationranges)
- [\_IsProceduralTexture](SpotLight.md#_isproceduraltexture)
- [\_IsTexture](SpotLight.md#_istexture)

## Constructors

### constructor

• **new SpotLight**(`name`, `position`, `direction`, `angle`, `exponent`, `scene`)

Creates a SpotLight object in the scene. A spot light is a simply light oriented cone.
It can cast shadows.
Documentation : https://doc.babylonjs.com/babylon101/lights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The light friendly name |
| `position` | [`Vector3`](Vector3.md) | The position of the spot light in the scene |
| `direction` | [`Vector3`](Vector3.md) | The direction of the light in the scene |
| `angle` | `number` | The cone angle of the light in Radians |
| `exponent` | `number` | The light decay speed with the distance from the emission spot |
| `scene` | [`Scene`](Scene.md) | The scene the lights belongs to |

#### Overrides

[ShadowLight](ShadowLight.md).[constructor](ShadowLight.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:234

## Properties

### \_angle

• `Private` **\_angle**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:40

___

### \_cosHalfAngle

• `Private` **\_cosHalfAngle**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:42

___

### \_direction

• `Protected` **\_direction**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowLight](ShadowLight.md).[_direction](ShadowLight.md#_direction)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:146

___

### \_innerAngle

• `Private` **\_innerAngle**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:41

___

### \_inverseSquaredRange

• `Protected` **\_inverseSquaredRange**: `number` = `0`

#### Inherited from

[ShadowLight](ShadowLight.md).[_inverseSquaredRange](ShadowLight.md#_inversesquaredrange)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:140

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[ShadowLight](ShadowLight.md).[_isDirty](ShadowLight.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_lightAngleOffset

• `Private` **\_lightAngleOffset**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:45

___

### \_lightAngleScale

• `Private` **\_lightAngleScale**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:44

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[ShadowLight](ShadowLight.md).[_parentNode](ShadowLight.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_position

• `Protected` **\_position**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowLight](ShadowLight.md).[_position](ShadowLight.md#_position)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:126

___

### \_projectionTexture

• `Private` **\_projectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:163

___

### \_projectionTextureDirty

• `Private` **\_projectionTextureDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:203

___

### \_projectionTextureLightFar

• `Protected` **\_projectionTextureLightFar**: `number` = `1000.0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:130

___

### \_projectionTextureLightNear

• `Protected` **\_projectionTextureLightNear**: `number` = `1e-6`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:114

___

### \_projectionTextureMatrix

• `Private` **\_projectionTextureMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:106

___

### \_projectionTextureProjectionLightDirty

• `Private` **\_projectionTextureProjectionLightDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:202

___

### \_projectionTextureProjectionLightMatrix

• `Private` **\_projectionTextureProjectionLightMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:207

___

### \_projectionTextureScalingMatrix

• `Private` **\_projectionTextureScalingMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:221

___

### \_projectionTextureUpDirection

• `Protected` **\_projectionTextureUpDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:146

___

### \_projectionTextureViewLightDirty

• `Private` **\_projectionTextureViewLightDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:201

___

### \_projectionTextureViewLightMatrix

• `Private` **\_projectionTextureViewLightMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:205

___

### \_projectionTextureViewTargetVector

• `Private` **\_projectionTextureViewTargetVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:204

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[ShadowLight](ShadowLight.md).[_ranges](ShadowLight.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### \_shadowAngleScale

• `Private` **\_shadowAngleScale**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:84

___

### \_shadowMaxZ

• `Protected` **\_shadowMaxZ**: `number`

#### Inherited from

[ShadowLight](ShadowLight.md).[_shadowMaxZ](ShadowLight.md#_shadowmaxz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:182

___

### \_shadowMinZ

• `Protected` **\_shadowMinZ**: `number`

#### Inherited from

[ShadowLight](ShadowLight.md).[_shadowMinZ](ShadowLight.md#_shadowminz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:166

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[ShadowLight](ShadowLight.md).[animations](ShadowLight.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:153

___

### customProjectionMatrixBuilder

• **customProjectionMatrixBuilder**: (`viewMatrix`: [`Matrix`](Matrix.md), `renderList`: [`AbstractMesh`](AbstractMesh.md)[], `result`: [`Matrix`](Matrix.md)) => `void`

#### Type declaration

▸ (`viewMatrix`, `renderList`, `result`): `void`

Callback defining a custom Projection Matrix Builder.
This can be used to override the default projection matrix computation.

##### Parameters

| Name | Type |
| :------ | :------ |
| `viewMatrix` | [`Matrix`](Matrix.md) |
| `renderList` | [`AbstractMesh`](AbstractMesh.md)[] |
| `result` | [`Matrix`](Matrix.md) |

##### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[customProjectionMatrixBuilder](ShadowLight.md#customprojectionmatrixbuilder)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:202

___

### diffuse

• **diffuse**: [`Color3`](Color3.md)

Diffuse gives the basic color to an object.

#### Inherited from

[ShadowLight](ShadowLight.md).[diffuse](ShadowLight.md#diffuse)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:111

___

### exponent

• **exponent**: `number`

The light decay speed with the distance from the emission spot.

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:104

___

### falloffType

• **falloffType**: `number` = `Light.FALLOFF_DEFAULT`

Defines the falloff type for this light. This lets overriding how punctual light are
falling off base on range or angle.
This can be set to any values in Light.FALLOFF_x.

Note: This is only useful for PBR Materials at the moment. This could be extended if required to
other types of materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[falloffType](ShadowLight.md#fallofftype)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:129

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[id](ShadowLight.md#id)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:97

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[ShadowLight](ShadowLight.md).[inspectableCustomProperties](ShadowLight.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:126

___

### intensity

• **intensity**: `number` = `1.0`

Strength of the light.
Note: By default it is define in the framework own unit.
Note: In PBR materials the intensityMode can be use to chose what unit the intensity is defined in.

#### Inherited from

[ShadowLight](ShadowLight.md).[intensity](ShadowLight.md#intensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:137

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[ShadowLight](ShadowLight.md).[metadata](ShadowLight.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[name](ShadowLight.md#name)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:91

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[ShadowLight](ShadowLight.md).[onDisposeObservable](ShadowLight.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[ShadowLight](ShadowLight.md).[onReady](ShadowLight.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### renderPriority

• **renderPriority**: `number` = `0`

Defines the rendering priority of the lights. It can help in case of fallback or number of lights
exceeding the number allowed of the materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[renderPriority](ShadowLight.md#renderpriority)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:206

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[ShadowLight](ShadowLight.md).[reservedDataStore](ShadowLight.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### specular

• **specular**: [`Color3`](Color3.md)

Specular produces a highlight color on an object.
Note: This is not affecting PBR materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[specular](ShadowLight.md#specular)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:118

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[ShadowLight](ShadowLight.md).[state](ShadowLight.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### transformedDirection

• **transformedDirection**: [`Vector3`](Vector3.md)

The transformed direction. Direction of the light in world space taking parenting in account.

#### Inherited from

[ShadowLight](ShadowLight.md).[transformedDirection](ShadowLight.md#transformeddirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:212

___

### transformedPosition

• **transformedPosition**: [`Vector3`](Vector3.md)

The transformed position. Position of the light in world space taking parenting in account.

#### Inherited from

[ShadowLight](ShadowLight.md).[transformedPosition](ShadowLight.md#transformedposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:207

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[uniqueId](ShadowLight.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

___

### FALLOFF\_DEFAULT

▪ `Static` `Readonly` **FALLOFF\_DEFAULT**: ``0``

Falloff Default: light is falling off following the material specification:
standard material is using standard falloff whereas pbr material can request special falloff per materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_DEFAULT](ShadowLight.md#falloff_default)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:25

___

### FALLOFF\_GLTF

▪ `Static` `Readonly` **FALLOFF\_GLTF**: ``2``

Falloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_GLTF](ShadowLight.md#falloff_gltf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:36

___

### FALLOFF\_PHYSICAL

▪ `Static` `Readonly` **FALLOFF\_PHYSICAL**: ``1``

Falloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_PHYSICAL](ShadowLight.md#falloff_physical)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:30

___

### FALLOFF\_STANDARD

▪ `Static` `Readonly` **FALLOFF\_STANDARD**: ``3``

Falloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_STANDARD](ShadowLight.md#falloff_standard)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:42

___

### INTENSITYMODE\_AUTOMATIC

▪ `Static` `Readonly` **INTENSITYMODE\_AUTOMATIC**: ``0``

Each light type uses the default quantity according to its type:
     point/spot lights use luminous intensity
     directional lights use illuminance

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_AUTOMATIC](ShadowLight.md#intensitymode_automatic)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:71

___

### INTENSITYMODE\_ILLUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_ILLUMINANCE**: ``3``

lux (lm/m^2)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_ILLUMINANCE](ShadowLight.md#intensitymode_illuminance)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:83

___

### INTENSITYMODE\_LUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINANCE**: ``4``

nit (cd/m^2)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINANCE](ShadowLight.md#intensitymode_luminance)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:87

___

### INTENSITYMODE\_LUMINOUSINTENSITY

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSINTENSITY**: ``2``

candela (lm/sr)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINOUSINTENSITY](ShadowLight.md#intensitymode_luminousintensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:79

___

### INTENSITYMODE\_LUMINOUSPOWER

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSPOWER**: ``1``

lumen (lm)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINOUSPOWER](ShadowLight.md#intensitymode_luminouspower)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:75

___

### LIGHTMAP\_DEFAULT

▪ `Static` `Readonly` **LIGHTMAP\_DEFAULT**: ``0``

If every light affecting the material is in this lightmapMode,
material.lightmapTexture adds or multiplies
(depends on material.useLightmapAsShadowmap)
after every other light calculations.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTMAP_DEFAULT](ShadowLight.md#lightmap_default)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:51

___

### LIGHTMAP\_SHADOWSONLY

▪ `Static` `Readonly` **LIGHTMAP\_SHADOWSONLY**: ``2``

material.lightmapTexture as only lighting
no light calculation from this light
only adds dynamic shadows from this light

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTMAP_SHADOWSONLY](ShadowLight.md#lightmap_shadowsonly)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:63

___

### LIGHTMAP\_SPECULAR

▪ `Static` `Readonly` **LIGHTMAP\_SPECULAR**: ``1``

material.lightmapTexture as only diffuse lighting from this light
adds only specular lighting from this light
adds dynamic shadows

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTMAP_SPECULAR](ShadowLight.md#lightmap_specular)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:57

___

### LIGHTTYPEID\_DIRECTIONALLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_DIRECTIONALLIGHT**: ``1``

Light type const id of the directional light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_DIRECTIONALLIGHT](ShadowLight.md#lighttypeid_directionallight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:97

___

### LIGHTTYPEID\_HEMISPHERICLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_HEMISPHERICLIGHT**: ``3``

Light type const id of the hemispheric light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_HEMISPHERICLIGHT](ShadowLight.md#lighttypeid_hemisphericlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:105

___

### LIGHTTYPEID\_POINTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_POINTLIGHT**: ``0``

Light type const id of the point light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_POINTLIGHT](ShadowLight.md#lighttypeid_pointlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:93

___

### LIGHTTYPEID\_SPOTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_SPOTLIGHT**: ``2``

Light type const id of the spot light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_SPOTLIGHT](ShadowLight.md#lighttypeid_spotlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:101

## Accessors

### angle

• `get` **angle**(): `number`

Gets the cone angle of the spot light in Radians.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:50

• `set` **angle**(`value`): `void`

Sets the cone angle of the spot light in Radians.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:57

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

ShadowLight.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:275

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Inherited from

ShadowLight.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:282

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

ShadowLight.behaviors

#### Defined in

https://github.com/babylon.js/core/src/node.ts:410

___

### direction

• `get` **direction**(): [`Vector3`](Vector3.md)

In 2d mode (needCube being false), gets the direction used to cast the shadow.
Also use as the light direction on spot and directional lights.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ShadowLight.direction

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:154

• `set` **direction**(`value`): `void`

In 2d mode (needCube being false), sets the direction used to cast the shadow.
Also use as the light direction on spot and directional lights.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

ShadowLight.direction

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:162

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

ShadowLight.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:131

• `set` **doNotSerialize**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ShadowLight.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:143

___

### excludeWithLayerMask

• `get` **excludeWithLayerMask**(): `number`

Gets the layer id use to find what meshes are not impacted by the light.
Inactive if 0

#### Returns

`number`

#### Inherited from

ShadowLight.excludeWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:266

• `set` **excludeWithLayerMask**(`value`): `void`

Sets the layer id use to find what meshes are not impacted by the light.
Inactive if 0

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.excludeWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:273

___

### excludedMeshes

• `get` **excludedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes not impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

ShadowLight.excludedMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:249

• `set` **excludedMeshes**(`value`): `void`

Sets the meshes not impacted by this light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Inherited from

ShadowLight.excludedMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:255

___

### includeOnlyWithLayerMask

• `get` **includeOnlyWithLayerMask**(): `number`

Gets the layer id use to find what meshes are impacted by the light.
Inactive if 0

#### Returns

`number`

#### Inherited from

ShadowLight.includeOnlyWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:284

• `set` **includeOnlyWithLayerMask**(`value`): `void`

Sets the layer id use to find what meshes are impacted by the light.
Inactive if 0

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.includeOnlyWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:291

___

### includedOnlyMeshes

• `get` **includedOnlyMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the only meshes impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

ShadowLight.includedOnlyMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:234

• `set` **includedOnlyMeshes**(`value`): `void`

Sets the only meshes impacted by this light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Inherited from

ShadowLight.includedOnlyMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:240

___

### innerAngle

• `get` **innerAngle**(): `number`

Only used in gltf falloff mode, this defines the angle where
the directional falloff will start before cutting at angle which could be seen
as outer angle.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:70

• `set` **innerAngle**(`value`): `void`

Only used in gltf falloff mode, this defines the angle where
the directional falloff will start before cutting at angle which could be seen
as outer angle.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:79

___

### intensityMode

• `get` **intensityMode**(): `number`

Gets the photometric scale used to interpret the intensity.
This is only relevant with PBR Materials where the light intensity can be defined in a physical way.

#### Returns

`number`

#### Inherited from

ShadowLight.intensityMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:170

• `set` **intensityMode**(`value`): `void`

Sets the photometric scale used to interpret the intensity.
This is only relevant with PBR Materials where the light intensity can be defined in a physical way.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.intensityMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:178

___

### lightmapMode

• `get` **lightmapMode**(): `number`

Gets the lightmap mode of this light (should be one of the constants defined by Light.LIGHTMAP_x)

#### Returns

`number`

#### Inherited from

ShadowLight.lightmapMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:301

• `set` **lightmapMode**(`value`): `void`

Sets the lightmap mode of this light (should be one of the constants defined by Light.LIGHTMAP_x)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.lightmapMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:307

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

ShadowLight.onClonedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:323

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Sets a callback that will be raised when the node will be disposed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

ShadowLight.onDispose

#### Defined in

https://github.com/babylon.js/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

ShadowLight.onEnabledStateChangedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

ShadowLight.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:238

• `set` **parent**(`parent`): `void`

Gets or sets the parent of the node (without keeping the current position in the scene)

**`See`**

https://doc.babylonjs.com/how_to/parenting

#### Parameters

| Name | Type |
| :------ | :------ |
| `parent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Inherited from

ShadowLight.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Sets the position the shadow will be casted from. Also use as the light position for both
point and spot lights.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ShadowLight.position

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:134

• `set` **position**(`value`): `void`

Sets the position the shadow will be casted from. Also use as the light position for both
point and spot lights.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

ShadowLight.position

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:142

___

### projectionTexture

• `get` **projectionTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the projection texture of the light.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:168

• `set` **projectionTexture**(`value`): `void`

Sets the projection texture of the light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:174

___

### projectionTextureLightFar

• `get` **projectionTextureLightFar**(): `number`

Gets the far clip of the Spotlight for texture projection.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:134

• `set` **projectionTextureLightFar**(`value`): `void`

Sets the far clip of the Spotlight for texture projection.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:141

___

### projectionTextureLightNear

• `get` **projectionTextureLightNear**(): `number`

Gets the near clip of the Spotlight for texture projection.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:118

• `set` **projectionTextureLightNear**(`value`): `void`

Sets the near clip of the Spotlight for texture projection.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:125

___

### projectionTextureMatrix

• `get` **projectionTextureMatrix**(): [`Matrix`](Matrix.md)

Allows reading the projection texture

#### Returns

[`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:110

___

### projectionTextureProjectionLightMatrix

• `get` **projectionTextureProjectionLightMatrix**(): [`Matrix`](Matrix.md)

Gets or sets the light projection matrix as used by the projection texture

#### Returns

[`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:211

• `set` **projectionTextureProjectionLightMatrix**(`projection`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `projection` | [`Matrix`](Matrix.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:215

___

### projectionTextureUpDirection

• `get` **projectionTextureUpDirection**(): [`Vector3`](Vector3.md)

Gets the Up vector of the Spotlight for texture projection.

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:150

• `set` **projectionTextureUpDirection**(`value`): `void`

Sets the Up vector of the Spotlight for texture projection.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:157

___

### radius

• `get` **radius**(): `number`

Gets the light radius used by PBR Materials to simulate soft area lights.

#### Returns

`number`

#### Inherited from

ShadowLight.radius

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:187

• `set` **radius**(`value`): `void`

sets the light radius used by PBR Materials to simulate soft area lights.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.radius

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:194

___

### range

• `get` **range**(): `number`

Defines how far from the source the light is impacting in scene units.
Note: Unused in PBR material as the distance light falloff is defined following the inverse squared falloff.

#### Returns

`number`

#### Inherited from

ShadowLight.range

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:146

• `set` **range**(`value`): `void`

Defines how far from the source the light is impacting in scene units.
Note: Unused in PBR material as the distance light falloff is defined following the inverse squared falloff.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.range

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:154

___

### shadowAngleScale

• `get` **shadowAngleScale**(): `number`

Allows scaling the angle of the light for shadow generation only.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:88

• `set` **shadowAngleScale**(`value`): `void`

Allows scaling the angle of the light for shadow generation only.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:95

___

### shadowEnabled

• `get` **shadowEnabled**(): `boolean`

Gets whether or not the shadows are enabled for this light. This can help turning off/on shadow without detaching
the current shadow generator.

#### Returns

`boolean`

#### Inherited from

ShadowLight.shadowEnabled

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:214

• `set` **shadowEnabled**(`value`): `void`

Sets whether or not the shadows are enabled for this light. This can help turning off/on shadow without detaching
the current shadow generator.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ShadowLight.shadowEnabled

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:221

___

### shadowMaxZ

• `get` **shadowMaxZ**(): `number`

Sets the shadow projection clipping maximum z value.

#### Returns

`number`

#### Inherited from

ShadowLight.shadowMaxZ

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:186

• `set` **shadowMaxZ**(`value`): `void`

Gets the shadow projection clipping maximum z value.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.shadowMaxZ

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:193

___

### shadowMinZ

• `get` **shadowMinZ**(): `number`

Gets the shadow projection clipping minimum z value.

#### Returns

`number`

#### Inherited from

ShadowLight.shadowMinZ

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:170

• `set` **shadowMinZ**(`value`): `void`

Sets the shadow projection clipping minimum z value.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowLight.shadowMinZ

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:177

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

ShadowLight.worldMatrixFromCache

#### Defined in

https://github.com/babylon.js/core/src/node.ts:454

## Methods

### \_bindLight

▸ **_bindLight**(`lightIndex`, `scene`, `effect`, `useSpecular`, `receiveShadows?`): `void`

Binds the lights information from the scene to the effect for the given mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `lightIndex` | `number` | `undefined` | Light index |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene where the light belongs to |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect we are binding the data to |
| `useSpecular` | `boolean` | `undefined` | Defines if specular is supported |
| `receiveShadows` | `boolean` | `true` | Defines if the effect (mesh) we bind the light for receives shadows |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[_bindLight](ShadowLight.md#_bindlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:391

___

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[_buildUniformLayout](ShadowLight.md#_builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:351

___

### \_computeAngleValues

▸ `Private` **_computeAngleValues**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:362

___

### \_computeProjectionTextureMatrix

▸ `Protected` **_computeProjectionTextureMatrix**(): `void`

Main function for light texture projection matrix computing.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:339

___

### \_computeProjectionTextureProjectionLightMatrix

▸ `Protected` **_computeProjectionTextureProjectionLightMatrix**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:321

___

### \_computeProjectionTextureViewLightMatrix

▸ `Protected` **_computeProjectionTextureViewLightMatrix**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:313

___

### \_setDefaultShadowProjectionMatrix

▸ `Protected` **_setDefaultShadowProjectionMatrix**(`matrix`, `viewMatrix`, `renderList`): `void`

Sets the passed matrix "matrix" as perspective projection matrix for the shadows and the passed view matrix with the fov equal to the SpotLight angle and and aspect ratio of 1.0.
Returns the SpotLight.

#### Parameters

| Name | Type |
| :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) |
| `viewMatrix` | [`Matrix`](Matrix.md) |
| `renderList` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[_setDefaultShadowProjectionMatrix](ShadowLight.md#_setdefaultshadowprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:285

___

### \_setDirection

▸ `Protected` **_setDirection**(`value`): `void`

Overrides the direction setter to recompute the projection texture view light Matrix.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[_setDirection](ShadowLight.md#_setdirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:263

___

### \_setPosition

▸ `Protected` **_setPosition**(`value`): `void`

Overrides the position setter to recompute the projection texture view light Matrix.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[_setPosition](ShadowLight.md#_setposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:272

___

### addBehavior

▸ **addBehavior**(`behavior`, `attachImmediately?`): [`Node`](Node.md)

Attach a behavior to the node

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `behavior` | [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md) | `undefined` | defines the behavior to attach |
| `attachImmediately` | `boolean` | `false` | defines that the behavior must be attached even if the scene is still loading |

#### Returns

[`Node`](Node.md)

the current Node

#### Inherited from

[ShadowLight](ShadowLight.md).[addBehavior](ShadowLight.md#addbehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:366

___

### beginAnimation

▸ **beginAnimation**(`name`, `loop?`, `speedRatio?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Will start the animation sequence

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the range frames for animation sequence |
| `loop?` | `boolean` | defines if the animation should loop (false by default) |
| `speedRatio?` | `number` | defines the speed factor in which to run the animation (1 by default) |
| `onAnimationEnd?` | () => `void` | defines a function to be executed when the animation ended (undefined by default) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

the object created for this animation. If range does not exist, it will return null

#### Inherited from

[ShadowLight](ShadowLight.md).[beginAnimation](ShadowLight.md#beginanimation)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:833

___

### canAffectMesh

▸ **canAffectMesh**(`mesh`): `boolean`

Specifies if the light will affect the passed mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to test against the light |

#### Returns

`boolean`

true the mesh is affected otherwise, false.

#### Inherited from

[ShadowLight](ShadowLight.md).[canAffectMesh](ShadowLight.md#canaffectmesh)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:507

___

### clone

▸ **clone**(`name`, `newParent?`): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Returns a new Light object, named "name", from the current one.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the cloned light |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `null` | The parent of this light, if it has one |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

the new created light

#### Inherited from

[ShadowLight](ShadowLight.md).[clone](ShadowLight.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:587

___

### computeTransformedInformation

▸ **computeTransformedInformation**(): `boolean`

Computes the transformed information (transformedPosition and transformedDirection in World space) of the current light

#### Returns

`boolean`

true if the information has been computed, false if it does not need to (no parenting)

#### Inherited from

[ShadowLight](ShadowLight.md).[computeTransformedInformation](ShadowLight.md#computetransformedinformation)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:220

___

### computeWorldMatrix

▸ **computeWorldMatrix**(`force?`): [`Matrix`](Matrix.md)

Computes the world matrix of the node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | defines if the cache version should be invalidated forcing the world matrix to be created from scratch |

#### Returns

[`Matrix`](Matrix.md)

the world matrix

#### Inherited from

[ShadowLight](ShadowLight.md).[computeWorldMatrix](ShadowLight.md#computeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:330

___

### createAnimationRange

▸ **createAnimationRange**(`name`, `from`, `to`): `void`

Creates an animation range for this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the range |
| `from` | `number` | defines the starting key |
| `to` | `number` | defines the end key |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[createAnimationRange](ShadowLight.md#createanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:777

___

### deleteAnimationRange

▸ **deleteAnimationRange**(`name`, `deleteFrames?`): `void`

Delete a specific animation range

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the range to delete |
| `deleteFrames` | `boolean` | `true` | defines if animation frames from the range must be deleted as well |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[deleteAnimationRange](ShadowLight.md#deleteanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:794

___

### dispose

▸ **dispose**(): `void`

Disposes the light and the associated resources.

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[dispose](ShadowLight.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:436

___

### forceProjectionMatrixCompute

▸ **forceProjectionMatrixCompute**(): `void`

Forces the shadow generator to recompute the projection matrix even if position and direction did not changed.

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[forceProjectionMatrixCompute](ShadowLight.md#forceprojectionmatrixcompute)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:305

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns the ShadowLight absolute position in the World.

#### Returns

[`Vector3`](Vector3.md)

the position vector in world space

#### Inherited from

[ShadowLight](ShadowLight.md).[getAbsolutePosition](ShadowLight.md#getabsoluteposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:261

___

### getAnimationByName

▸ **getAnimationByName**(`name`): [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

Get an animation by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

null if not found else the requested animation

#### Inherited from

[ShadowLight](ShadowLight.md).[getAnimationByName](ShadowLight.md#getanimationbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:759

___

### getAnimationRange

▸ **getAnimationRange**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

Get an animation range by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation range to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

null if not found else the requested animation range

#### Inherited from

[ShadowLight](ShadowLight.md).[getAnimationRange](ShadowLight.md#getanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:808

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

Gets the list of all animation ranges defined on this node

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

an array

#### Inherited from

[ShadowLight](ShadowLight.md).[getAnimationRanges](ShadowLight.md#getanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:816

___

### getBehaviorByName

▸ **getBehaviorByName**(`name`): [`Nullable`](../modules.md#nullable)[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)

Gets an attached behavior by name

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the behavior to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)

null if behavior was not found else the requested behavior

#### Inherited from

[ShadowLight](ShadowLight.md).[getBehaviorByName](ShadowLight.md#getbehaviorbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:420

___

### getChildMeshes

▸ **getChildMeshes**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Get all child-meshes of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`AbstractMesh`](AbstractMesh.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

an array of AbstractMesh

#### Inherited from

[ShadowLight](ShadowLight.md).[getChildMeshes](ShadowLight.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:684

▸ **getChildMeshes**(`directDescendantsOnly?`, `predicate?`): [`AbstractMesh`](AbstractMesh.md)[]

Get all child-meshes of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of AbstractMesh

#### Inherited from

[ShadowLight](ShadowLight.md).[getChildMeshes](ShadowLight.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:692

___

### getChildren

▸ **getChildren**`T`(`predicate?`, `directDescendantsOnly?`): `T`[]

Get all direct children of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

`T`[]

an array of Node

#### Inherited from

[ShadowLight](ShadowLight.md).[getChildren](ShadowLight.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:714

▸ **getChildren**(`predicate?`, `directDescendantsOnly?`): [`Node`](Node.md)[]

Get all direct children of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

[`Node`](Node.md)[]

an array of Node

#### Inherited from

[ShadowLight](ShadowLight.md).[getChildren](ShadowLight.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "SpotLight".

#### Returns

`string`

the class name

#### Overrides

[ShadowLight](ShadowLight.md).[getClassName](ShadowLight.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:247

___

### getDepthMaxZ

▸ **getDepthMaxZ**(`activeCamera`): `number`

Gets the maxZ used for shadow according to both the scene and the light.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeCamera` | [`Camera`](Camera.md) | The camera we are returning the max for |

#### Returns

`number`

the depth max z

#### Overrides

[ShadowLight](ShadowLight.md).[getDepthMaxZ](ShadowLight.md#getdepthmaxz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:460

___

### getDepthMinZ

▸ **getDepthMinZ**(`activeCamera`): `number`

Gets the minZ used for shadow according to both the scene and the light.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeCamera` | [`Camera`](Camera.md) | The camera we are returning the min for |

#### Returns

`number`

the depth min z

#### Overrides

[ShadowLight](ShadowLight.md).[getDepthMinZ](ShadowLight.md#getdepthminz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:448

___

### getDepthScale

▸ **getDepthScale**(): `number`

Return the depth scale used for the shadow map.

#### Returns

`number`

the depth scale.

#### Inherited from

[ShadowLight](ShadowLight.md).[getDepthScale](ShadowLight.md#getdepthscale)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:243

___

### getDescendants

▸ **getDescendants**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Will return all nodes that have this node as ascendant

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

all children nodes of all types

#### Inherited from

[ShadowLight](ShadowLight.md).[getDescendants](ShadowLight.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:654

▸ **getDescendants**(`directDescendantsOnly?`, `predicate?`): [`Node`](Node.md)[]

Will return all nodes that have this node as ascendant

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`Node`](Node.md)[]

all children nodes of all types

#### Inherited from

[ShadowLight](ShadowLight.md).[getDescendants](ShadowLight.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:662

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[ShadowLight](ShadowLight.md).[getEngine](ShadowLight.md#getengine)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:352

___

### getHierarchyBoundingVectors

▸ **getHierarchyBoundingVectors**(`includeDescendants?`, `predicate?`): `Object`

Return the minimum and maximum world vectors of the entire hierarchy under current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `includeDescendants` | `boolean` | `true` | Include bounding info from descendants as well (true by default) |
| `predicate` | [`Nullable`](../modules.md#nullable)(`abstractMesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | `null` | defines a callback function that can be customize to filter what meshes should be included in the list used to compute the bounding vectors |

#### Returns

`Object`

the new bounding vectors

| Name | Type |
| :------ | :------ |
| `max` | [`Vector3`](Vector3.md) |
| `min` | [`Vector3`](Vector3.md) |

#### Inherited from

[ShadowLight](ShadowLight.md).[getHierarchyBoundingVectors](ShadowLight.md#gethierarchyboundingvectors)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:933

___

### getRotation

▸ **getRotation**(): [`Vector3`](Vector3.md)

Returns the light rotation in euler definition.

#### Returns

[`Vector3`](Vector3.md)

the x y z rotation in local space.

#### Inherited from

[ShadowLight](ShadowLight.md).[getRotation](ShadowLight.md#getrotation)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:279

___

### getScaledIntensity

▸ **getScaledIntensity**(): `number`

Returns the intensity scaled by the Photometric Scale according to the light type and intensity mode.

#### Returns

`number`

the scaled intensity in intensity mode unit

#### Inherited from

[ShadowLight](ShadowLight.md).[getScaledIntensity](ShadowLight.md#getscaledintensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:577

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[ShadowLight](ShadowLight.md).[getScene](ShadowLight.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:344

___

### getShadowDirection

▸ **getShadowDirection**(`faceIndex?`): [`Vector3`](Vector3.md)

Get the direction to use to render the shadow map. In case of cube texture, the face index can be passed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `faceIndex?` | `number` | The index of the face we are computed the direction to generate shadow |

#### Returns

[`Vector3`](Vector3.md)

The set direction in 2d mode otherwise the direction to the cubemap face if needCube() is true

#### Inherited from

[ShadowLight](ShadowLight.md).[getShadowDirection](ShadowLight.md#getshadowdirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:253

___

### getShadowGenerator

▸ **getShadowGenerator**(): [`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

Returns the Light associated shadow generator if any.

#### Returns

[`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

the associated shadow generator.

#### Inherited from

[ShadowLight](ShadowLight.md).[getShadowGenerator](ShadowLight.md#getshadowgenerator)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:490

___

### getTypeID

▸ **getTypeID**(): `number`

Returns the integer 2.

#### Returns

`number`

The light Type id as a constant defines in Light.LIGHTTYPEID_x

#### Overrides

[ShadowLight](ShadowLight.md).[getTypeID](ShadowLight.md#gettypeid)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:255

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Returns the latest update of the World matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[ShadowLight](ShadowLight.md).[getWorldMatrix](ShadowLight.md#getworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:434

___

### isDescendantOf

▸ **isDescendantOf**(`ancestor`): `boolean`

Is this node a descendant of the given node?
The function will iterate up the hierarchy until the ancestor was found or no more parents defined

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ancestor` | [`Node`](Node.md) | defines the parent node to inspect |

#### Returns

`boolean`

a boolean indicating if this node is a descendant of the given node

#### Inherited from

[ShadowLight](ShadowLight.md).[isDescendantOf](ShadowLight.md#isdescendantof)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:613

___

### isDisposed

▸ **isDisposed**(): `boolean`

Gets a boolean indicating if the node has been disposed

#### Returns

`boolean`

true if the node was disposed

#### Inherited from

[ShadowLight](ShadowLight.md).[isDisposed](ShadowLight.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:192

___

### isEnabled

▸ **isEnabled**(`checkAncestors?`): `boolean`

Is this node enabled?
If the node has a parent, all ancestors will be checked and false will be returned if any are false (not enabled), otherwise will return true

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `checkAncestors` | `boolean` | `true` | indicates if this method should check the ancestors. The default is to check the ancestors. If set to false, the method will return the value of this node without checking ancestors |

#### Returns

`boolean`

whether this node (and its parent) is enabled

#### Inherited from

[ShadowLight](ShadowLight.md).[isEnabled](ShadowLight.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:569

___

### isReady

▸ **isReady**(`completeCheck?`): `boolean`

Is this node ready to be used/rendered

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `completeCheck` | `boolean` | `false` | defines if a complete check (including materials and lights) has to be done (false by default) |

#### Returns

`boolean`

true if the node is ready

#### Inherited from

[ShadowLight](ShadowLight.md).[isReady](ShadowLight.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:548

___

### markAsDirty

▸ **markAsDirty**(`property?`): [`Node`](Node.md)

Flag the  node as dirty (Forcing it to update everything)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property?` | `string` | helps children apply precise "dirtyfication" |

#### Returns

[`Node`](Node.md)

this node

#### Inherited from

[ShadowLight](ShadowLight.md).[markAsDirty](ShadowLight.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:557

___

### needCube

▸ **needCube**(): `boolean`

Returns whether or not the shadow generation require a cube texture or a 2d texture.

#### Returns

`boolean`

true if a cube texture needs to be use

#### Inherited from

[ShadowLight](ShadowLight.md).[needCube](ShadowLight.md#needcube)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:290

___

### needProjectionMatrixCompute

▸ **needProjectionMatrixCompute**(): `boolean`

Detects if the projection matrix requires to be recomputed this frame.

#### Returns

`boolean`

true if it requires to be recomputed otherwise, false.

#### Inherited from

[ShadowLight](ShadowLight.md).[needProjectionMatrixCompute](ShadowLight.md#needprojectionmatrixcompute)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:298

___

### prepareLightSpecificDefines

▸ **prepareLightSpecificDefines**(`defines`, `lightIndex`): `void`

Prepares the list of defines specific to the light type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `any` | the list of defines |
| `lightIndex` | `number` | defines the index of the light for the effect |

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[prepareLightSpecificDefines](ShadowLight.md#preparelightspecificdefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:472

___

### removeBehavior

▸ **removeBehavior**(`behavior`): [`Node`](Node.md)

Remove an attached behavior

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `behavior` | [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md) | defines the behavior to attach |

#### Returns

[`Node`](Node.md)

the current Node

#### Inherited from

[ShadowLight](ShadowLight.md).[removeBehavior](ShadowLight.md#removebehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:393

___

### serialize

▸ **serialize**(): `any`

Serializes the current light into a Serialization object.

#### Returns

`any`

the serialized object.

#### Inherited from

[ShadowLight](ShadowLight.md).[serialize](ShadowLight.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:611

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[ShadowLight](ShadowLight.md).[serializeAnimationRanges](ShadowLight.md#serializeanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:847

___

### setDirectionToTarget

▸ **setDirectionToTarget**(`target`): [`Vector3`](Vector3.md)

Sets the ShadowLight direction toward the passed target.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Vector3`](Vector3.md) | The point to target in local space |

#### Returns

[`Vector3`](Vector3.md)

the updated ShadowLight direction

#### Inherited from

[ShadowLight](ShadowLight.md).[setDirectionToTarget](ShadowLight.md#setdirectiontotarget)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:270

___

### setEnabled

▸ **setEnabled**(`value`): `void`

Set the enabled state of this node.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | the new enabled state |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[setEnabled](ShadowLight.md#setenabled)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:480

___

### setShadowProjectionMatrix

▸ **setShadowProjectionMatrix**(`matrix`, `viewMatrix`, `renderList`): [`IShadowLight`](../interfaces/IShadowLight.md)

Sets the shadow projection matrix in parameter to the generated projection matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | The matrix to updated with the projection information |
| `viewMatrix` | [`Matrix`](Matrix.md) | The transform matrix of the light |
| `renderList` | [`AbstractMesh`](AbstractMesh.md)[] | The list of mesh to render in the map |

#### Returns

[`IShadowLight`](../interfaces/IShadowLight.md)

The current light

#### Inherited from

[ShadowLight](ShadowLight.md).[setShadowProjectionMatrix](ShadowLight.md#setshadowprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:382

___

### toString

▸ **toString**(`fullDetails?`): `string`

Converts the light information to a readable string for debug purpose.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | Supports for multiple levels of logging within scene loading |

#### Returns

`string`

the human readable light info

#### Inherited from

[ShadowLight](ShadowLight.md).[toString](ShadowLight.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:457

___

### transferTexturesToEffect

▸ **transferTexturesToEffect**(`effect`, `lightIndex`): [`Light`](Light.md)

Sets the passed Effect "effect" with the Light textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`Light`](Light.md)

The light

#### Overrides

[ShadowLight](ShadowLight.md).[transferTexturesToEffect](ShadowLight.md#transfertexturestoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:373

___

### transferToEffect

▸ **transferToEffect**(`effect`, `lightIndex`): [`SpotLight`](SpotLight.md)

Sets the passed Effect object with the SpotLight transformed position (or position if not parented) and normalized direction.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`SpotLight`](SpotLight.md)

The spot light

#### Overrides

[ShadowLight](ShadowLight.md).[transferToEffect](ShadowLight.md#transfertoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:396

___

### transferToNodeMaterialEffect

▸ **transferToNodeMaterialEffect**(`effect`, `lightDataUniformName`): [`SpotLight`](SpotLight.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightDataUniformName` | `string` | The uniform used to store light data (position or direction) |

#### Returns

[`SpotLight`](SpotLight.md)

The light

#### Overrides

[ShadowLight](ShadowLight.md).[transferToNodeMaterialEffect](ShadowLight.md#transfertonodematerialeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:415

___

### AddNodeConstructor

▸ `Static` **AddNodeConstructor**(`type`, `constructorFunc`): `void`

Add a new node constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | defines the type name of the node to construct |
| `constructorFunc` | [`NodeConstructor`](../modules.md#nodeconstructor) | defines the constructor function |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[AddNodeConstructor](ShadowLight.md#addnodeconstructor)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:63

___

### Construct

▸ `Static` **Construct**(`type`, `name`, `scene`, `options?`): [`Nullable`](../modules.md#nullable)() => [`Node`](Node.md)

Returns a node constructor based on type name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | defines the type name |
| `name` | `string` | defines the new node name |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `options?` | `any` | defines optional options to transmit to constructors |

#### Returns

[`Nullable`](../modules.md#nullable)() => [`Node`](Node.md)

the new constructor or null

#### Inherited from

[ShadowLight](ShadowLight.md).[Construct](ShadowLight.md#construct)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:75

___

### GetConstructorFromName

▸ `Static` **GetConstructorFromName**(`type`, `name`, `scene`): [`Nullable`](../modules.md#nullable)() => [`Light`](Light.md)

Creates a new typed light from the passed type (integer) : point light = 0, directional light = 1, spot light = 2, hemispheric light = 3.
This new light is named "name" and added to the passed scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Type according to the types available in Light.LIGHTTYPEID_x |
| `name` | `string` | The friendly name of the light |
| `scene` | [`Scene`](Scene.md) | The scene the new light will belong to |

#### Returns

[`Nullable`](../modules.md#nullable)() => [`Light`](Light.md)

the constructor function

#### Inherited from

[ShadowLight](ShadowLight.md).[GetConstructorFromName](ShadowLight.md#getconstructorfromname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:655

___

### Parse

▸ `Static` **Parse**(`parsedLight`, `scene`): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Parses the passed "parsedLight" and returns a new instanced Light from this parsing.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedLight` | `any` | The JSON representation of the light |
| `scene` | [`Scene`](Scene.md) | The scene to create the parsed light in |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

the created light after parsing

#### Inherited from

[ShadowLight](ShadowLight.md).[Parse](ShadowLight.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:672

___

### ParseAnimationRanges

▸ `Static` **ParseAnimationRanges**(`node`, `parsedNode`, `scene`): `void`

Parse animation range data from a serialization object and store them into a given node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`Node`](Node.md) | defines where to store the animation ranges |
| `parsedNode` | `any` | defines the serialization object to read data from |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[ParseAnimationRanges](ShadowLight.md#parseanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:919

___

### \_IsProceduralTexture

▸ `Static` `Private` **_IsProceduralTexture**(`texture`): texture is ProceduralTexture

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) |

#### Returns

texture is ProceduralTexture

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:193

___

### \_IsTexture

▸ `Static` `Private` **_IsTexture**(`texture`): texture is Texture

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) |

#### Returns

texture is Texture

#### Defined in

https://github.com/babylon.js/core/src/Lights/spotLight.ts:197

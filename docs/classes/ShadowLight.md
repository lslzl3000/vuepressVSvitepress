[@dev/core](../README.md) / [Exports](../modules.md) / ShadowLight

# Class: ShadowLight

Base implementation IShadowLight
It groups all the common behaviour in order to reduce duplication and better follow the DRY pattern.

## Hierarchy

- [`Light`](Light.md)

  ↳ **`ShadowLight`**

  ↳↳ [`DirectionalLight`](DirectionalLight.md)

  ↳↳ [`PointLight`](PointLight.md)

  ↳↳ [`SpotLight`](SpotLight.md)

## Implements

- [`IShadowLight`](../interfaces/IShadowLight.md)

## Table of contents

### Constructors

- [constructor](ShadowLight.md#constructor)

### Properties

- [\_direction](ShadowLight.md#_direction)
- [\_inverseSquaredRange](ShadowLight.md#_inversesquaredrange)
- [\_isDirty](ShadowLight.md#_isdirty)
- [\_needProjectionMatrixCompute](ShadowLight.md#_needprojectionmatrixcompute)
- [\_parentNode](ShadowLight.md#_parentnode)
- [\_position](ShadowLight.md#_position)
- [\_ranges](ShadowLight.md#_ranges)
- [\_shadowMaxZ](ShadowLight.md#_shadowmaxz)
- [\_shadowMinZ](ShadowLight.md#_shadowminz)
- [animations](ShadowLight.md#animations)
- [customProjectionMatrixBuilder](ShadowLight.md#customprojectionmatrixbuilder)
- [diffuse](ShadowLight.md#diffuse)
- [falloffType](ShadowLight.md#fallofftype)
- [id](ShadowLight.md#id)
- [inspectableCustomProperties](ShadowLight.md#inspectablecustomproperties)
- [intensity](ShadowLight.md#intensity)
- [metadata](ShadowLight.md#metadata)
- [name](ShadowLight.md#name)
- [onDisposeObservable](ShadowLight.md#ondisposeobservable)
- [onReady](ShadowLight.md#onready)
- [renderPriority](ShadowLight.md#renderpriority)
- [reservedDataStore](ShadowLight.md#reserveddatastore)
- [specular](ShadowLight.md#specular)
- [state](ShadowLight.md#state)
- [transformedDirection](ShadowLight.md#transformeddirection)
- [transformedPosition](ShadowLight.md#transformedposition)
- [uniqueId](ShadowLight.md#uniqueid)
- [FALLOFF\_DEFAULT](ShadowLight.md#falloff_default)
- [FALLOFF\_GLTF](ShadowLight.md#falloff_gltf)
- [FALLOFF\_PHYSICAL](ShadowLight.md#falloff_physical)
- [FALLOFF\_STANDARD](ShadowLight.md#falloff_standard)
- [INTENSITYMODE\_AUTOMATIC](ShadowLight.md#intensitymode_automatic)
- [INTENSITYMODE\_ILLUMINANCE](ShadowLight.md#intensitymode_illuminance)
- [INTENSITYMODE\_LUMINANCE](ShadowLight.md#intensitymode_luminance)
- [INTENSITYMODE\_LUMINOUSINTENSITY](ShadowLight.md#intensitymode_luminousintensity)
- [INTENSITYMODE\_LUMINOUSPOWER](ShadowLight.md#intensitymode_luminouspower)
- [LIGHTMAP\_DEFAULT](ShadowLight.md#lightmap_default)
- [LIGHTMAP\_SHADOWSONLY](ShadowLight.md#lightmap_shadowsonly)
- [LIGHTMAP\_SPECULAR](ShadowLight.md#lightmap_specular)
- [LIGHTTYPEID\_DIRECTIONALLIGHT](ShadowLight.md#lighttypeid_directionallight)
- [LIGHTTYPEID\_HEMISPHERICLIGHT](ShadowLight.md#lighttypeid_hemisphericlight)
- [LIGHTTYPEID\_POINTLIGHT](ShadowLight.md#lighttypeid_pointlight)
- [LIGHTTYPEID\_SPOTLIGHT](ShadowLight.md#lighttypeid_spotlight)

### Accessors

- [animationPropertiesOverride](ShadowLight.md#animationpropertiesoverride)
- [behaviors](ShadowLight.md#behaviors)
- [direction](ShadowLight.md#direction)
- [doNotSerialize](ShadowLight.md#donotserialize)
- [excludeWithLayerMask](ShadowLight.md#excludewithlayermask)
- [excludedMeshes](ShadowLight.md#excludedmeshes)
- [includeOnlyWithLayerMask](ShadowLight.md#includeonlywithlayermask)
- [includedOnlyMeshes](ShadowLight.md#includedonlymeshes)
- [intensityMode](ShadowLight.md#intensitymode)
- [lightmapMode](ShadowLight.md#lightmapmode)
- [onClonedObservable](ShadowLight.md#onclonedobservable)
- [onDispose](ShadowLight.md#ondispose)
- [onEnabledStateChangedObservable](ShadowLight.md#onenabledstatechangedobservable)
- [parent](ShadowLight.md#parent)
- [position](ShadowLight.md#position)
- [radius](ShadowLight.md#radius)
- [range](ShadowLight.md#range)
- [shadowEnabled](ShadowLight.md#shadowenabled)
- [shadowMaxZ](ShadowLight.md#shadowmaxz)
- [shadowMinZ](ShadowLight.md#shadowminz)
- [worldMatrixFromCache](ShadowLight.md#worldmatrixfromcache)

### Methods

- [\_bindLight](ShadowLight.md#_bindlight)
- [\_buildUniformLayout](ShadowLight.md#_builduniformlayout)
- [\_setDefaultShadowProjectionMatrix](ShadowLight.md#_setdefaultshadowprojectionmatrix)
- [\_setDirection](ShadowLight.md#_setdirection)
- [\_setPosition](ShadowLight.md#_setposition)
- [addBehavior](ShadowLight.md#addbehavior)
- [beginAnimation](ShadowLight.md#beginanimation)
- [canAffectMesh](ShadowLight.md#canaffectmesh)
- [clone](ShadowLight.md#clone)
- [computeTransformedInformation](ShadowLight.md#computetransformedinformation)
- [computeWorldMatrix](ShadowLight.md#computeworldmatrix)
- [createAnimationRange](ShadowLight.md#createanimationrange)
- [deleteAnimationRange](ShadowLight.md#deleteanimationrange)
- [dispose](ShadowLight.md#dispose)
- [forceProjectionMatrixCompute](ShadowLight.md#forceprojectionmatrixcompute)
- [getAbsolutePosition](ShadowLight.md#getabsoluteposition)
- [getAnimationByName](ShadowLight.md#getanimationbyname)
- [getAnimationRange](ShadowLight.md#getanimationrange)
- [getAnimationRanges](ShadowLight.md#getanimationranges)
- [getBehaviorByName](ShadowLight.md#getbehaviorbyname)
- [getChildMeshes](ShadowLight.md#getchildmeshes)
- [getChildren](ShadowLight.md#getchildren)
- [getClassName](ShadowLight.md#getclassname)
- [getDepthMaxZ](ShadowLight.md#getdepthmaxz)
- [getDepthMinZ](ShadowLight.md#getdepthminz)
- [getDepthScale](ShadowLight.md#getdepthscale)
- [getDescendants](ShadowLight.md#getdescendants)
- [getEngine](ShadowLight.md#getengine)
- [getHierarchyBoundingVectors](ShadowLight.md#gethierarchyboundingvectors)
- [getRotation](ShadowLight.md#getrotation)
- [getScaledIntensity](ShadowLight.md#getscaledintensity)
- [getScene](ShadowLight.md#getscene)
- [getShadowDirection](ShadowLight.md#getshadowdirection)
- [getShadowGenerator](ShadowLight.md#getshadowgenerator)
- [getTypeID](ShadowLight.md#gettypeid)
- [getWorldMatrix](ShadowLight.md#getworldmatrix)
- [isDescendantOf](ShadowLight.md#isdescendantof)
- [isDisposed](ShadowLight.md#isdisposed)
- [isEnabled](ShadowLight.md#isenabled)
- [isReady](ShadowLight.md#isready)
- [markAsDirty](ShadowLight.md#markasdirty)
- [needCube](ShadowLight.md#needcube)
- [needProjectionMatrixCompute](ShadowLight.md#needprojectionmatrixcompute)
- [prepareLightSpecificDefines](ShadowLight.md#preparelightspecificdefines)
- [removeBehavior](ShadowLight.md#removebehavior)
- [serialize](ShadowLight.md#serialize)
- [serializeAnimationRanges](ShadowLight.md#serializeanimationranges)
- [setDirectionToTarget](ShadowLight.md#setdirectiontotarget)
- [setEnabled](ShadowLight.md#setenabled)
- [setShadowProjectionMatrix](ShadowLight.md#setshadowprojectionmatrix)
- [toString](ShadowLight.md#tostring)
- [transferTexturesToEffect](ShadowLight.md#transfertexturestoeffect)
- [transferToEffect](ShadowLight.md#transfertoeffect)
- [transferToNodeMaterialEffect](ShadowLight.md#transfertonodematerialeffect)
- [AddNodeConstructor](ShadowLight.md#addnodeconstructor)
- [Construct](ShadowLight.md#construct)
- [GetConstructorFromName](ShadowLight.md#getconstructorfromname)
- [Parse](ShadowLight.md#parse)
- [ParseAnimationRanges](ShadowLight.md#parseanimationranges)

## Constructors

### constructor

• **new ShadowLight**(`name`, `scene`)

Creates a Light object in the scene.
Documentation : https://doc.babylonjs.com/babylon101/lights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The friendly name of the light |
| `scene` | [`Scene`](Scene.md) | The scene the light belongs too |

#### Inherited from

[Light](Light.md).[constructor](Light.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:349

## Properties

### \_direction

• `Protected` **\_direction**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:146

___

### \_inverseSquaredRange

• `Protected` **\_inverseSquaredRange**: `number` = `0`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_inverseSquaredRange](../interfaces/IShadowLight.md#_inversesquaredrange)

#### Inherited from

[Light](Light.md).[_inverseSquaredRange](Light.md#_inversesquaredrange)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:140

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_isDirty](../interfaces/IShadowLight.md#_isdirty)

#### Inherited from

[Light](Light.md).[_isDirty](Light.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_needProjectionMatrixCompute

• `Private` **\_needProjectionMatrixCompute**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:214

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_parentNode](../interfaces/IShadowLight.md#_parentnode)

#### Inherited from

[Light](Light.md).[_parentNode](Light.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_position

• `Protected` **\_position**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:126

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_ranges](../interfaces/IShadowLight.md#_ranges)

#### Inherited from

[Light](Light.md).[_ranges](Light.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### \_shadowMaxZ

• `Protected` **\_shadowMaxZ**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:182

___

### \_shadowMinZ

• `Protected` **\_shadowMinZ**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:166

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[animations](../interfaces/IShadowLight.md#animations)

#### Inherited from

[Light](Light.md).[animations](Light.md#animations)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[customProjectionMatrixBuilder](../interfaces/IShadowLight.md#customprojectionmatrixbuilder)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:202

___

### diffuse

• **diffuse**: [`Color3`](Color3.md)

Diffuse gives the basic color to an object.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[diffuse](../interfaces/IShadowLight.md#diffuse)

#### Inherited from

[Light](Light.md).[diffuse](Light.md#diffuse)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:111

___

### falloffType

• **falloffType**: `number` = `Light.FALLOFF_DEFAULT`

Defines the falloff type for this light. This lets overriding how punctual light are
falling off base on range or angle.
This can be set to any values in Light.FALLOFF_x.

Note: This is only useful for PBR Materials at the moment. This could be extended if required to
other types of materials.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[falloffType](../interfaces/IShadowLight.md#fallofftype)

#### Inherited from

[Light](Light.md).[falloffType](Light.md#fallofftype)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:129

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[id](../interfaces/IShadowLight.md#id)

#### Inherited from

[Light](Light.md).[id](Light.md#id)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:97

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[inspectableCustomProperties](../interfaces/IShadowLight.md#inspectablecustomproperties)

#### Inherited from

[Light](Light.md).[inspectableCustomProperties](Light.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:126

___

### intensity

• **intensity**: `number` = `1.0`

Strength of the light.
Note: By default it is define in the framework own unit.
Note: In PBR materials the intensityMode can be use to chose what unit the intensity is defined in.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[intensity](../interfaces/IShadowLight.md#intensity)

#### Inherited from

[Light](Light.md).[intensity](Light.md#intensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:137

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[metadata](../interfaces/IShadowLight.md#metadata)

#### Inherited from

[Light](Light.md).[metadata](Light.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[name](../interfaces/IShadowLight.md#name)

#### Inherited from

[Light](Light.md).[name](Light.md#name)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:91

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[onDisposeObservable](../interfaces/IShadowLight.md#ondisposeobservable)

#### Inherited from

[Light](Light.md).[onDisposeObservable](Light.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[onReady](../interfaces/IShadowLight.md#onready)

#### Inherited from

[Light](Light.md).[onReady](Light.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### renderPriority

• **renderPriority**: `number` = `0`

Defines the rendering priority of the lights. It can help in case of fallback or number of lights
exceeding the number allowed of the materials.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[renderPriority](../interfaces/IShadowLight.md#renderpriority)

#### Inherited from

[Light](Light.md).[renderPriority](Light.md#renderpriority)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:206

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[reservedDataStore](../interfaces/IShadowLight.md#reserveddatastore)

#### Inherited from

[Light](Light.md).[reservedDataStore](Light.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### specular

• **specular**: [`Color3`](Color3.md)

Specular produces a highlight color on an object.
Note: This is not affecting PBR materials.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[specular](../interfaces/IShadowLight.md#specular)

#### Inherited from

[Light](Light.md).[specular](Light.md#specular)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:118

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[state](../interfaces/IShadowLight.md#state)

#### Inherited from

[Light](Light.md).[state](Light.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### transformedDirection

• **transformedDirection**: [`Vector3`](Vector3.md)

The transformed direction. Direction of the light in world space taking parenting in account.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[transformedDirection](../interfaces/IShadowLight.md#transformeddirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:212

___

### transformedPosition

• **transformedPosition**: [`Vector3`](Vector3.md)

The transformed position. Position of the light in world space taking parenting in account.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[transformedPosition](../interfaces/IShadowLight.md#transformedposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:207

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[uniqueId](../interfaces/IShadowLight.md#uniqueid)

#### Inherited from

[Light](Light.md).[uniqueId](Light.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

___

### FALLOFF\_DEFAULT

▪ `Static` `Readonly` **FALLOFF\_DEFAULT**: ``0``

Falloff Default: light is falling off following the material specification:
standard material is using standard falloff whereas pbr material can request special falloff per materials.

#### Inherited from

[Light](Light.md).[FALLOFF_DEFAULT](Light.md#falloff_default)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:25

___

### FALLOFF\_GLTF

▪ `Static` `Readonly` **FALLOFF\_GLTF**: ``2``

Falloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[Light](Light.md).[FALLOFF_GLTF](Light.md#falloff_gltf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:36

___

### FALLOFF\_PHYSICAL

▪ `Static` `Readonly` **FALLOFF\_PHYSICAL**: ``1``

Falloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[Light](Light.md).[FALLOFF_PHYSICAL](Light.md#falloff_physical)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:30

___

### FALLOFF\_STANDARD

▪ `Static` `Readonly` **FALLOFF\_STANDARD**: ``3``

Falloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[Light](Light.md).[FALLOFF_STANDARD](Light.md#falloff_standard)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:42

___

### INTENSITYMODE\_AUTOMATIC

▪ `Static` `Readonly` **INTENSITYMODE\_AUTOMATIC**: ``0``

Each light type uses the default quantity according to its type:
     point/spot lights use luminous intensity
     directional lights use illuminance

#### Inherited from

[Light](Light.md).[INTENSITYMODE_AUTOMATIC](Light.md#intensitymode_automatic)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:71

___

### INTENSITYMODE\_ILLUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_ILLUMINANCE**: ``3``

lux (lm/m^2)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_ILLUMINANCE](Light.md#intensitymode_illuminance)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:83

___

### INTENSITYMODE\_LUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINANCE**: ``4``

nit (cd/m^2)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINANCE](Light.md#intensitymode_luminance)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:87

___

### INTENSITYMODE\_LUMINOUSINTENSITY

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSINTENSITY**: ``2``

candela (lm/sr)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINOUSINTENSITY](Light.md#intensitymode_luminousintensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:79

___

### INTENSITYMODE\_LUMINOUSPOWER

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSPOWER**: ``1``

lumen (lm)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINOUSPOWER](Light.md#intensitymode_luminouspower)

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

[Light](Light.md).[LIGHTMAP_DEFAULT](Light.md#lightmap_default)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:51

___

### LIGHTMAP\_SHADOWSONLY

▪ `Static` `Readonly` **LIGHTMAP\_SHADOWSONLY**: ``2``

material.lightmapTexture as only lighting
no light calculation from this light
only adds dynamic shadows from this light

#### Inherited from

[Light](Light.md).[LIGHTMAP_SHADOWSONLY](Light.md#lightmap_shadowsonly)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:63

___

### LIGHTMAP\_SPECULAR

▪ `Static` `Readonly` **LIGHTMAP\_SPECULAR**: ``1``

material.lightmapTexture as only diffuse lighting from this light
adds only specular lighting from this light
adds dynamic shadows

#### Inherited from

[Light](Light.md).[LIGHTMAP_SPECULAR](Light.md#lightmap_specular)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:57

___

### LIGHTTYPEID\_DIRECTIONALLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_DIRECTIONALLIGHT**: ``1``

Light type const id of the directional light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_DIRECTIONALLIGHT](Light.md#lighttypeid_directionallight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:97

___

### LIGHTTYPEID\_HEMISPHERICLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_HEMISPHERICLIGHT**: ``3``

Light type const id of the hemispheric light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_HEMISPHERICLIGHT](Light.md#lighttypeid_hemisphericlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:105

___

### LIGHTTYPEID\_POINTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_POINTLIGHT**: ``0``

Light type const id of the point light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_POINTLIGHT](Light.md#lighttypeid_pointlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:93

___

### LIGHTTYPEID\_SPOTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_SPOTLIGHT**: ``2``

Light type const id of the spot light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_SPOTLIGHT](Light.md#lighttypeid_spotlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:101

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Implementation of

IShadowLight.animationPropertiesOverride

#### Inherited from

Light.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:275

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Implementation of

IShadowLight.animationPropertiesOverride

#### Inherited from

Light.animationPropertiesOverride

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

#### Implementation of

IShadowLight.behaviors

#### Inherited from

Light.behaviors

#### Defined in

https://github.com/babylon.js/core/src/node.ts:410

___

### direction

• `get` **direction**(): [`Vector3`](Vector3.md)

In 2d mode (needCube being false), gets the direction used to cast the shadow.
Also use as the light direction on spot and directional lights.

#### Returns

[`Vector3`](Vector3.md)

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[direction](../interfaces/IShadowLight.md#direction)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[direction](../interfaces/IShadowLight.md#direction)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:162

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Implementation of

IShadowLight.doNotSerialize

#### Inherited from

Light.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:131

• `set` **doNotSerialize**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Implementation of

IShadowLight.doNotSerialize

#### Inherited from

Light.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:143

___

### excludeWithLayerMask

• `get` **excludeWithLayerMask**(): `number`

Gets the layer id use to find what meshes are not impacted by the light.
Inactive if 0

#### Returns

`number`

#### Implementation of

IShadowLight.excludeWithLayerMask

#### Inherited from

Light.excludeWithLayerMask

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

#### Implementation of

IShadowLight.excludeWithLayerMask

#### Inherited from

Light.excludeWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:273

___

### excludedMeshes

• `get` **excludedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes not impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Implementation of

IShadowLight.excludedMeshes

#### Inherited from

Light.excludedMeshes

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

#### Implementation of

IShadowLight.excludedMeshes

#### Inherited from

Light.excludedMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:255

___

### includeOnlyWithLayerMask

• `get` **includeOnlyWithLayerMask**(): `number`

Gets the layer id use to find what meshes are impacted by the light.
Inactive if 0

#### Returns

`number`

#### Implementation of

IShadowLight.includeOnlyWithLayerMask

#### Inherited from

Light.includeOnlyWithLayerMask

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

#### Implementation of

IShadowLight.includeOnlyWithLayerMask

#### Inherited from

Light.includeOnlyWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:291

___

### includedOnlyMeshes

• `get` **includedOnlyMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the only meshes impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Implementation of

IShadowLight.includedOnlyMeshes

#### Inherited from

Light.includedOnlyMeshes

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

#### Implementation of

IShadowLight.includedOnlyMeshes

#### Inherited from

Light.includedOnlyMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:240

___

### intensityMode

• `get` **intensityMode**(): `number`

Gets the photometric scale used to interpret the intensity.
This is only relevant with PBR Materials where the light intensity can be defined in a physical way.

#### Returns

`number`

#### Implementation of

IShadowLight.intensityMode

#### Inherited from

Light.intensityMode

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

#### Implementation of

IShadowLight.intensityMode

#### Inherited from

Light.intensityMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:178

___

### lightmapMode

• `get` **lightmapMode**(): `number`

Gets the lightmap mode of this light (should be one of the constants defined by Light.LIGHTMAP_x)

#### Returns

`number`

#### Implementation of

IShadowLight.lightmapMode

#### Inherited from

Light.lightmapMode

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

#### Implementation of

IShadowLight.lightmapMode

#### Inherited from

Light.lightmapMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:307

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Implementation of

IShadowLight.onClonedObservable

#### Inherited from

Light.onClonedObservable

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

#### Implementation of

IShadowLight.onDispose

#### Inherited from

Light.onDispose

#### Defined in

https://github.com/babylon.js/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Implementation of

IShadowLight.onEnabledStateChangedObservable

#### Inherited from

Light.onEnabledStateChangedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Implementation of

IShadowLight.parent

#### Inherited from

Light.parent

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

#### Implementation of

IShadowLight.parent

#### Inherited from

Light.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Sets the position the shadow will be casted from. Also use as the light position for both
point and spot lights.

#### Returns

[`Vector3`](Vector3.md)

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[position](../interfaces/IShadowLight.md#position)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[position](../interfaces/IShadowLight.md#position)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:142

___

### radius

• `get` **radius**(): `number`

Gets the light radius used by PBR Materials to simulate soft area lights.

#### Returns

`number`

#### Implementation of

IShadowLight.radius

#### Inherited from

Light.radius

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

#### Implementation of

IShadowLight.radius

#### Inherited from

Light.radius

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:194

___

### range

• `get` **range**(): `number`

Defines how far from the source the light is impacting in scene units.
Note: Unused in PBR material as the distance light falloff is defined following the inverse squared falloff.

#### Returns

`number`

#### Implementation of

IShadowLight.range

#### Inherited from

Light.range

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

#### Implementation of

IShadowLight.range

#### Inherited from

Light.range

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:154

___

### shadowEnabled

• `get` **shadowEnabled**(): `boolean`

Gets whether or not the shadows are enabled for this light. This can help turning off/on shadow without detaching
the current shadow generator.

#### Returns

`boolean`

#### Implementation of

IShadowLight.shadowEnabled

#### Inherited from

Light.shadowEnabled

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

#### Implementation of

IShadowLight.shadowEnabled

#### Inherited from

Light.shadowEnabled

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:221

___

### shadowMaxZ

• `get` **shadowMaxZ**(): `number`

Sets the shadow projection clipping maximum z value.

#### Returns

`number`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[shadowMaxZ](../interfaces/IShadowLight.md#shadowmaxz)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[shadowMaxZ](../interfaces/IShadowLight.md#shadowmaxz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:193

___

### shadowMinZ

• `get` **shadowMinZ**(): `number`

Gets the shadow projection clipping minimum z value.

#### Returns

`number`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[shadowMinZ](../interfaces/IShadowLight.md#shadowminz)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[shadowMinZ](../interfaces/IShadowLight.md#shadowminz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:177

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Implementation of

IShadowLight.worldMatrixFromCache

#### Inherited from

Light.worldMatrixFromCache

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_bindLight](../interfaces/IShadowLight.md#_bindlight)

#### Inherited from

[Light](Light.md).[_bindLight](Light.md#_bindlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:391

___

### \_buildUniformLayout

▸ `Protected` `Abstract` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[_buildUniformLayout](../interfaces/IShadowLight.md#_builduniformlayout)

#### Inherited from

[Light](Light.md).[_buildUniformLayout](Light.md#_builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:361

___

### \_setDefaultShadowProjectionMatrix

▸ `Protected` `Abstract` **_setDefaultShadowProjectionMatrix**(`matrix`, `viewMatrix`, `renderList`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) |
| `viewMatrix` | [`Matrix`](Matrix.md) |
| `renderList` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:124

___

### \_setDirection

▸ `Protected` **_setDirection**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:147

___

### \_setPosition

▸ `Protected` **_setPosition**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:127

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[addBehavior](../interfaces/IShadowLight.md#addbehavior)

#### Inherited from

[Light](Light.md).[addBehavior](Light.md#addbehavior)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[beginAnimation](../interfaces/IShadowLight.md#beginanimation)

#### Inherited from

[Light](Light.md).[beginAnimation](Light.md#beginanimation)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[canAffectMesh](../interfaces/IShadowLight.md#canaffectmesh)

#### Inherited from

[Light](Light.md).[canAffectMesh](Light.md#canaffectmesh)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[clone](../interfaces/IShadowLight.md#clone)

#### Inherited from

[Light](Light.md).[clone](Light.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:587

___

### computeTransformedInformation

▸ **computeTransformedInformation**(): `boolean`

Computes the transformed information (transformedPosition and transformedDirection in World space) of the current light

#### Returns

`boolean`

true if the information has been computed, false if it does not need to (no parenting)

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[computeTransformedInformation](../interfaces/IShadowLight.md#computetransformedinformation)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[computeWorldMatrix](../interfaces/IShadowLight.md#computeworldmatrix)

#### Overrides

[Light](Light.md).[computeWorldMatrix](Light.md#computeworldmatrix)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[createAnimationRange](../interfaces/IShadowLight.md#createanimationrange)

#### Inherited from

[Light](Light.md).[createAnimationRange](Light.md#createanimationrange)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[deleteAnimationRange](../interfaces/IShadowLight.md#deleteanimationrange)

#### Inherited from

[Light](Light.md).[deleteAnimationRange](Light.md#deleteanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:794

___

### dispose

▸ **dispose**(`doNotRecurse?`, `disposeMaterialAndTextures?`): `void`

Releases resources associated with this node.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `doNotRecurse?` | `boolean` | `undefined` | Set to true to not recurse into each children (recurse into each children by default) |
| `disposeMaterialAndTextures` | `boolean` | `false` | Set to true to also dispose referenced materials and textures (false by default) |

#### Returns

`void`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[dispose](../interfaces/IShadowLight.md#dispose)

#### Inherited from

[Light](Light.md).[dispose](Light.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:536

___

### forceProjectionMatrixCompute

▸ **forceProjectionMatrixCompute**(): `void`

Forces the shadow generator to recompute the projection matrix even if position and direction did not changed.

#### Returns

`void`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[forceProjectionMatrixCompute](../interfaces/IShadowLight.md#forceprojectionmatrixcompute)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:305

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns the ShadowLight absolute position in the World.

#### Returns

[`Vector3`](Vector3.md)

the position vector in world space

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getAbsolutePosition](../interfaces/IShadowLight.md#getabsoluteposition)

#### Overrides

[Light](Light.md).[getAbsolutePosition](Light.md#getabsoluteposition)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getAnimationByName](../interfaces/IShadowLight.md#getanimationbyname)

#### Inherited from

[Light](Light.md).[getAnimationByName](Light.md#getanimationbyname)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getAnimationRange](../interfaces/IShadowLight.md#getanimationrange)

#### Inherited from

[Light](Light.md).[getAnimationRange](Light.md#getanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:808

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

Gets the list of all animation ranges defined on this node

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

an array

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getAnimationRanges](../interfaces/IShadowLight.md#getanimationranges)

#### Inherited from

[Light](Light.md).[getAnimationRanges](Light.md#getanimationranges)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getBehaviorByName](../interfaces/IShadowLight.md#getbehaviorbyname)

#### Inherited from

[Light](Light.md).[getBehaviorByName](Light.md#getbehaviorbyname)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getChildMeshes](../interfaces/IShadowLight.md#getchildmeshes)

#### Inherited from

[Light](Light.md).[getChildMeshes](Light.md#getchildmeshes)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getChildMeshes](../interfaces/IShadowLight.md#getchildmeshes)

#### Inherited from

[Light](Light.md).[getChildMeshes](Light.md#getchildmeshes)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getChildren](../interfaces/IShadowLight.md#getchildren)

#### Inherited from

[Light](Light.md).[getChildren](Light.md#getchildren)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getChildren](../interfaces/IShadowLight.md#getchildren)

#### Inherited from

[Light](Light.md).[getChildren](Light.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "Light".

#### Returns

`string`

the class name

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getClassName](../interfaces/IShadowLight.md#getclassname)

#### Inherited from

[Light](Light.md).[getClassName](Light.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:445

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getDepthMaxZ](../interfaces/IShadowLight.md#getdepthmaxz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:371

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getDepthMinZ](../interfaces/IShadowLight.md#getdepthminz)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:362

___

### getDepthScale

▸ **getDepthScale**(): `number`

Return the depth scale used for the shadow map.

#### Returns

`number`

the depth scale.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getDepthScale](../interfaces/IShadowLight.md#getdepthscale)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getDescendants](../interfaces/IShadowLight.md#getdescendants)

#### Inherited from

[Light](Light.md).[getDescendants](Light.md#getdescendants)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getDescendants](../interfaces/IShadowLight.md#getdescendants)

#### Inherited from

[Light](Light.md).[getDescendants](Light.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:662

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getEngine](../interfaces/IShadowLight.md#getengine)

#### Inherited from

[Light](Light.md).[getEngine](Light.md#getengine)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getHierarchyBoundingVectors](../interfaces/IShadowLight.md#gethierarchyboundingvectors)

#### Inherited from

[Light](Light.md).[getHierarchyBoundingVectors](Light.md#gethierarchyboundingvectors)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:933

___

### getRotation

▸ **getRotation**(): [`Vector3`](Vector3.md)

Returns the light rotation in euler definition.

#### Returns

[`Vector3`](Vector3.md)

the x y z rotation in local space.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:279

___

### getScaledIntensity

▸ **getScaledIntensity**(): `number`

Returns the intensity scaled by the Photometric Scale according to the light type and intensity mode.

#### Returns

`number`

the scaled intensity in intensity mode unit

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getScaledIntensity](../interfaces/IShadowLight.md#getscaledintensity)

#### Inherited from

[Light](Light.md).[getScaledIntensity](Light.md#getscaledintensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:577

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getScene](../interfaces/IShadowLight.md#getscene)

#### Inherited from

[Light](Light.md).[getScene](Light.md#getscene)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getShadowDirection](../interfaces/IShadowLight.md#getshadowdirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:253

___

### getShadowGenerator

▸ **getShadowGenerator**(): [`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

Returns the Light associated shadow generator if any.

#### Returns

[`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

the associated shadow generator.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getShadowGenerator](../interfaces/IShadowLight.md#getshadowgenerator)

#### Inherited from

[Light](Light.md).[getShadowGenerator](Light.md#getshadowgenerator)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:490

___

### getTypeID

▸ **getTypeID**(): `number`

Returns the light type ID (integer).

#### Returns

`number`

The light Type id as a constant defines in Light.LIGHTTYPEID_x

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getTypeID](../interfaces/IShadowLight.md#gettypeid)

#### Inherited from

[Light](Light.md).[getTypeID](Light.md#gettypeid)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:569

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Returns the latest update of the World matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[getWorldMatrix](../interfaces/IShadowLight.md#getworldmatrix)

#### Inherited from

[Light](Light.md).[getWorldMatrix](Light.md#getworldmatrix)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[isDescendantOf](../interfaces/IShadowLight.md#isdescendantof)

#### Inherited from

[Light](Light.md).[isDescendantOf](Light.md#isdescendantof)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:613

___

### isDisposed

▸ **isDisposed**(): `boolean`

Gets a boolean indicating if the node has been disposed

#### Returns

`boolean`

true if the node was disposed

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[isDisposed](../interfaces/IShadowLight.md#isdisposed)

#### Inherited from

[Light](Light.md).[isDisposed](Light.md#isdisposed)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[isEnabled](../interfaces/IShadowLight.md#isenabled)

#### Inherited from

[Light](Light.md).[isEnabled](Light.md#isenabled)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[isReady](../interfaces/IShadowLight.md#isready)

#### Inherited from

[Light](Light.md).[isReady](Light.md#isready)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[markAsDirty](../interfaces/IShadowLight.md#markasdirty)

#### Inherited from

[Light](Light.md).[markAsDirty](Light.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:557

___

### needCube

▸ **needCube**(): `boolean`

Returns whether or not the shadow generation require a cube texture or a 2d texture.

#### Returns

`boolean`

true if a cube texture needs to be use

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[needCube](../interfaces/IShadowLight.md#needcube)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:290

___

### needProjectionMatrixCompute

▸ **needProjectionMatrixCompute**(): `boolean`

Detects if the projection matrix requires to be recomputed this frame.

#### Returns

`boolean`

true if it requires to be recomputed otherwise, false.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[needProjectionMatrixCompute](../interfaces/IShadowLight.md#needprojectionmatrixcompute)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:298

___

### prepareLightSpecificDefines

▸ `Abstract` **prepareLightSpecificDefines**(`defines`, `lightIndex`): `void`

Prepares the list of defines specific to the light type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `any` | the list of defines |
| `lightIndex` | `number` | defines the index of the light for the effect |

#### Returns

`void`

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[prepareLightSpecificDefines](../interfaces/IShadowLight.md#preparelightspecificdefines)

#### Inherited from

[Light](Light.md).[prepareLightSpecificDefines](Light.md#preparelightspecificdefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:886

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[removeBehavior](../interfaces/IShadowLight.md#removebehavior)

#### Inherited from

[Light](Light.md).[removeBehavior](Light.md#removebehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:393

___

### serialize

▸ **serialize**(): `any`

Serializes the current light into a Serialization object.

#### Returns

`any`

the serialized object.

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[serialize](../interfaces/IShadowLight.md#serialize)

#### Inherited from

[Light](Light.md).[serialize](Light.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:611

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[serializeAnimationRanges](../interfaces/IShadowLight.md#serializeanimationranges)

#### Inherited from

[Light](Light.md).[serializeAnimationRanges](Light.md#serializeanimationranges)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[setEnabled](../interfaces/IShadowLight.md#setenabled)

#### Inherited from

[Light](Light.md).[setEnabled](Light.md#setenabled)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[setShadowProjectionMatrix](../interfaces/IShadowLight.md#setshadowprojectionmatrix)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[toString](../interfaces/IShadowLight.md#tostring)

#### Inherited from

[Light](Light.md).[toString](Light.md#tostring)

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

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[transferTexturesToEffect](../interfaces/IShadowLight.md#transfertexturestoeffect)

#### Inherited from

[Light](Light.md).[transferTexturesToEffect](Light.md#transfertexturestoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:378

___

### transferToEffect

▸ `Abstract` **transferToEffect**(`effect`, `lightIndex`): [`Light`](Light.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`Light`](Light.md)

The light

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[transferToEffect](../interfaces/IShadowLight.md#transfertoeffect)

#### Inherited from

[Light](Light.md).[transferToEffect](Light.md#transfertoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:369

___

### transferToNodeMaterialEffect

▸ `Abstract` **transferToNodeMaterialEffect**(`effect`, `lightDataUniformName`): [`Light`](Light.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightDataUniformName` | `string` | The uniform used to store light data (position or direction) |

#### Returns

[`Light`](Light.md)

The light

#### Implementation of

[IShadowLight](../interfaces/IShadowLight.md).[transferToNodeMaterialEffect](../interfaces/IShadowLight.md#transfertonodematerialeffect)

#### Inherited from

[Light](Light.md).[transferToNodeMaterialEffect](Light.md#transfertonodematerialeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:439

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

[Light](Light.md).[AddNodeConstructor](Light.md#addnodeconstructor)

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

[Light](Light.md).[Construct](Light.md#construct)

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

[Light](Light.md).[GetConstructorFromName](Light.md#getconstructorfromname)

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

[Light](Light.md).[Parse](Light.md#parse)

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

[Light](Light.md).[ParseAnimationRanges](Light.md#parseanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:919

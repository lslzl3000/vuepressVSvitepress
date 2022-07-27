[@dev/core](../README.md) / [Exports](../modules.md) / PointLight

# Class: PointLight

A point light is a light defined by an unique point in world space.
The light is emitted in every direction from this point.
A good example of a point light is a standard light bulb.
Documentation: https://doc.babylonjs.com/babylon101/lights

## Hierarchy

- [`ShadowLight`](ShadowLight.md)

  ↳ **`PointLight`**

## Table of contents

### Constructors

- [constructor](PointLight.md#constructor)

### Properties

- [\_direction](PointLight.md#_direction)
- [\_inverseSquaredRange](PointLight.md#_inversesquaredrange)
- [\_isDirty](PointLight.md#_isdirty)
- [\_parentNode](PointLight.md#_parentnode)
- [\_position](PointLight.md#_position)
- [\_ranges](PointLight.md#_ranges)
- [\_shadowAngle](PointLight.md#_shadowangle)
- [\_shadowMaxZ](PointLight.md#_shadowmaxz)
- [\_shadowMinZ](PointLight.md#_shadowminz)
- [animations](PointLight.md#animations)
- [customProjectionMatrixBuilder](PointLight.md#customprojectionmatrixbuilder)
- [diffuse](PointLight.md#diffuse)
- [falloffType](PointLight.md#fallofftype)
- [id](PointLight.md#id)
- [inspectableCustomProperties](PointLight.md#inspectablecustomproperties)
- [intensity](PointLight.md#intensity)
- [metadata](PointLight.md#metadata)
- [name](PointLight.md#name)
- [onDisposeObservable](PointLight.md#ondisposeobservable)
- [onReady](PointLight.md#onready)
- [renderPriority](PointLight.md#renderpriority)
- [reservedDataStore](PointLight.md#reserveddatastore)
- [specular](PointLight.md#specular)
- [state](PointLight.md#state)
- [transformedDirection](PointLight.md#transformeddirection)
- [transformedPosition](PointLight.md#transformedposition)
- [uniqueId](PointLight.md#uniqueid)
- [FALLOFF\_DEFAULT](PointLight.md#falloff_default)
- [FALLOFF\_GLTF](PointLight.md#falloff_gltf)
- [FALLOFF\_PHYSICAL](PointLight.md#falloff_physical)
- [FALLOFF\_STANDARD](PointLight.md#falloff_standard)
- [INTENSITYMODE\_AUTOMATIC](PointLight.md#intensitymode_automatic)
- [INTENSITYMODE\_ILLUMINANCE](PointLight.md#intensitymode_illuminance)
- [INTENSITYMODE\_LUMINANCE](PointLight.md#intensitymode_luminance)
- [INTENSITYMODE\_LUMINOUSINTENSITY](PointLight.md#intensitymode_luminousintensity)
- [INTENSITYMODE\_LUMINOUSPOWER](PointLight.md#intensitymode_luminouspower)
- [LIGHTMAP\_DEFAULT](PointLight.md#lightmap_default)
- [LIGHTMAP\_SHADOWSONLY](PointLight.md#lightmap_shadowsonly)
- [LIGHTMAP\_SPECULAR](PointLight.md#lightmap_specular)
- [LIGHTTYPEID\_DIRECTIONALLIGHT](PointLight.md#lighttypeid_directionallight)
- [LIGHTTYPEID\_HEMISPHERICLIGHT](PointLight.md#lighttypeid_hemisphericlight)
- [LIGHTTYPEID\_POINTLIGHT](PointLight.md#lighttypeid_pointlight)
- [LIGHTTYPEID\_SPOTLIGHT](PointLight.md#lighttypeid_spotlight)

### Accessors

- [animationPropertiesOverride](PointLight.md#animationpropertiesoverride)
- [behaviors](PointLight.md#behaviors)
- [direction](PointLight.md#direction)
- [doNotSerialize](PointLight.md#donotserialize)
- [excludeWithLayerMask](PointLight.md#excludewithlayermask)
- [excludedMeshes](PointLight.md#excludedmeshes)
- [includeOnlyWithLayerMask](PointLight.md#includeonlywithlayermask)
- [includedOnlyMeshes](PointLight.md#includedonlymeshes)
- [intensityMode](PointLight.md#intensitymode)
- [lightmapMode](PointLight.md#lightmapmode)
- [onClonedObservable](PointLight.md#onclonedobservable)
- [onDispose](PointLight.md#ondispose)
- [onEnabledStateChangedObservable](PointLight.md#onenabledstatechangedobservable)
- [parent](PointLight.md#parent)
- [position](PointLight.md#position)
- [radius](PointLight.md#radius)
- [range](PointLight.md#range)
- [shadowAngle](PointLight.md#shadowangle)
- [shadowEnabled](PointLight.md#shadowenabled)
- [shadowMaxZ](PointLight.md#shadowmaxz)
- [shadowMinZ](PointLight.md#shadowminz)
- [worldMatrixFromCache](PointLight.md#worldmatrixfromcache)

### Methods

- [\_bindLight](PointLight.md#_bindlight)
- [\_buildUniformLayout](PointLight.md#_builduniformlayout)
- [\_setDefaultShadowProjectionMatrix](PointLight.md#_setdefaultshadowprojectionmatrix)
- [\_setDirection](PointLight.md#_setdirection)
- [\_setPosition](PointLight.md#_setposition)
- [addBehavior](PointLight.md#addbehavior)
- [beginAnimation](PointLight.md#beginanimation)
- [canAffectMesh](PointLight.md#canaffectmesh)
- [clone](PointLight.md#clone)
- [computeTransformedInformation](PointLight.md#computetransformedinformation)
- [computeWorldMatrix](PointLight.md#computeworldmatrix)
- [createAnimationRange](PointLight.md#createanimationrange)
- [deleteAnimationRange](PointLight.md#deleteanimationrange)
- [dispose](PointLight.md#dispose)
- [forceProjectionMatrixCompute](PointLight.md#forceprojectionmatrixcompute)
- [getAbsolutePosition](PointLight.md#getabsoluteposition)
- [getAnimationByName](PointLight.md#getanimationbyname)
- [getAnimationRange](PointLight.md#getanimationrange)
- [getAnimationRanges](PointLight.md#getanimationranges)
- [getBehaviorByName](PointLight.md#getbehaviorbyname)
- [getChildMeshes](PointLight.md#getchildmeshes)
- [getChildren](PointLight.md#getchildren)
- [getClassName](PointLight.md#getclassname)
- [getDepthMaxZ](PointLight.md#getdepthmaxz)
- [getDepthMinZ](PointLight.md#getdepthminz)
- [getDepthScale](PointLight.md#getdepthscale)
- [getDescendants](PointLight.md#getdescendants)
- [getEngine](PointLight.md#getengine)
- [getHierarchyBoundingVectors](PointLight.md#gethierarchyboundingvectors)
- [getRotation](PointLight.md#getrotation)
- [getScaledIntensity](PointLight.md#getscaledintensity)
- [getScene](PointLight.md#getscene)
- [getShadowDirection](PointLight.md#getshadowdirection)
- [getShadowGenerator](PointLight.md#getshadowgenerator)
- [getTypeID](PointLight.md#gettypeid)
- [getWorldMatrix](PointLight.md#getworldmatrix)
- [isDescendantOf](PointLight.md#isdescendantof)
- [isDisposed](PointLight.md#isdisposed)
- [isEnabled](PointLight.md#isenabled)
- [isReady](PointLight.md#isready)
- [markAsDirty](PointLight.md#markasdirty)
- [needCube](PointLight.md#needcube)
- [needProjectionMatrixCompute](PointLight.md#needprojectionmatrixcompute)
- [prepareLightSpecificDefines](PointLight.md#preparelightspecificdefines)
- [removeBehavior](PointLight.md#removebehavior)
- [serialize](PointLight.md#serialize)
- [serializeAnimationRanges](PointLight.md#serializeanimationranges)
- [setDirectionToTarget](PointLight.md#setdirectiontotarget)
- [setEnabled](PointLight.md#setenabled)
- [setShadowProjectionMatrix](PointLight.md#setshadowprojectionmatrix)
- [toString](PointLight.md#tostring)
- [transferTexturesToEffect](PointLight.md#transfertexturestoeffect)
- [transferToEffect](PointLight.md#transfertoeffect)
- [transferToNodeMaterialEffect](PointLight.md#transfertonodematerialeffect)
- [AddNodeConstructor](PointLight.md#addnodeconstructor)
- [Construct](PointLight.md#construct)
- [GetConstructorFromName](PointLight.md#getconstructorfromname)
- [Parse](PointLight.md#parse)
- [ParseAnimationRanges](PointLight.md#parseanimationranges)

## Constructors

### constructor

• **new PointLight**(`name`, `position`, `scene`)

Creates a PointLight object from the passed name and position (Vector3) and adds it in the scene.
A PointLight emits the light in every direction.
It can cast shadows.
If the scene camera is already defined and you want to set your PointLight at the camera position, just set it :
```javascript
var pointLight = new PointLight("pl", camera.position, scene);
```
Documentation : https://doc.babylonjs.com/babylon101/lights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The light friendly name |
| `position` | [`Vector3`](Vector3.md) | The position of the point light in the scene |
| `scene` | [`Scene`](Scene.md) | The scene the lights belongs to |

#### Overrides

[ShadowLight](ShadowLight.md).[constructor](ShadowLight.md#constructor)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:75

## Properties

### \_direction

• `Protected` **\_direction**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowLight](ShadowLight.md).[_direction](ShadowLight.md#_direction)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:146

___

### \_inverseSquaredRange

• `Protected` **\_inverseSquaredRange**: `number` = `0`

#### Inherited from

[ShadowLight](ShadowLight.md).[_inverseSquaredRange](ShadowLight.md#_inversesquaredrange)

#### Defined in

packages/dev/core/src/Lights/light.ts:140

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[ShadowLight](ShadowLight.md).[_isDirty](ShadowLight.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[ShadowLight](ShadowLight.md).[_parentNode](ShadowLight.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_position

• `Protected` **\_position**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowLight](ShadowLight.md).[_position](ShadowLight.md#_position)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:126

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[ShadowLight](ShadowLight.md).[_ranges](ShadowLight.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_shadowAngle

• `Private` **\_shadowAngle**: `number`

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:21

___

### \_shadowMaxZ

• `Protected` **\_shadowMaxZ**: `number`

#### Inherited from

[ShadowLight](ShadowLight.md).[_shadowMaxZ](ShadowLight.md#_shadowmaxz)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:182

___

### \_shadowMinZ

• `Protected` **\_shadowMinZ**: `number`

#### Inherited from

[ShadowLight](ShadowLight.md).[_shadowMinZ](ShadowLight.md#_shadowminz)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:166

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[ShadowLight](ShadowLight.md).[animations](ShadowLight.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

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

packages/dev/core/src/Lights/shadowLight.ts:202

___

### diffuse

• **diffuse**: [`Color3`](Color3.md)

Diffuse gives the basic color to an object.

#### Inherited from

[ShadowLight](ShadowLight.md).[diffuse](ShadowLight.md#diffuse)

#### Defined in

packages/dev/core/src/Lights/light.ts:111

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

packages/dev/core/src/Lights/light.ts:129

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[id](ShadowLight.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[ShadowLight](ShadowLight.md).[inspectableCustomProperties](ShadowLight.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### intensity

• **intensity**: `number` = `1.0`

Strength of the light.
Note: By default it is define in the framework own unit.
Note: In PBR materials the intensityMode can be use to chose what unit the intensity is defined in.

#### Inherited from

[ShadowLight](ShadowLight.md).[intensity](ShadowLight.md#intensity)

#### Defined in

packages/dev/core/src/Lights/light.ts:137

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[ShadowLight](ShadowLight.md).[metadata](ShadowLight.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[name](ShadowLight.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[ShadowLight](ShadowLight.md).[onDisposeObservable](ShadowLight.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[ShadowLight](ShadowLight.md).[onReady](ShadowLight.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### renderPriority

• **renderPriority**: `number` = `0`

Defines the rendering priority of the lights. It can help in case of fallback or number of lights
exceeding the number allowed of the materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[renderPriority](ShadowLight.md#renderpriority)

#### Defined in

packages/dev/core/src/Lights/light.ts:206

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[ShadowLight](ShadowLight.md).[reservedDataStore](ShadowLight.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### specular

• **specular**: [`Color3`](Color3.md)

Specular produces a highlight color on an object.
Note: This is not affecting PBR materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[specular](ShadowLight.md#specular)

#### Defined in

packages/dev/core/src/Lights/light.ts:118

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[ShadowLight](ShadowLight.md).[state](ShadowLight.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### transformedDirection

• **transformedDirection**: [`Vector3`](Vector3.md)

The transformed direction. Direction of the light in world space taking parenting in account.

#### Inherited from

[ShadowLight](ShadowLight.md).[transformedDirection](ShadowLight.md#transformeddirection)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:212

___

### transformedPosition

• **transformedPosition**: [`Vector3`](Vector3.md)

The transformed position. Position of the light in world space taking parenting in account.

#### Inherited from

[ShadowLight](ShadowLight.md).[transformedPosition](ShadowLight.md#transformedposition)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:207

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[ShadowLight](ShadowLight.md).[uniqueId](ShadowLight.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### FALLOFF\_DEFAULT

▪ `Static` `Readonly` **FALLOFF\_DEFAULT**: ``0``

Falloff Default: light is falling off following the material specification:
standard material is using standard falloff whereas pbr material can request special falloff per materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_DEFAULT](ShadowLight.md#falloff_default)

#### Defined in

packages/dev/core/src/Lights/light.ts:25

___

### FALLOFF\_GLTF

▪ `Static` `Readonly` **FALLOFF\_GLTF**: ``2``

Falloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_GLTF](ShadowLight.md#falloff_gltf)

#### Defined in

packages/dev/core/src/Lights/light.ts:36

___

### FALLOFF\_PHYSICAL

▪ `Static` `Readonly` **FALLOFF\_PHYSICAL**: ``1``

Falloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_PHYSICAL](ShadowLight.md#falloff_physical)

#### Defined in

packages/dev/core/src/Lights/light.ts:30

___

### FALLOFF\_STANDARD

▪ `Static` `Readonly` **FALLOFF\_STANDARD**: ``3``

Falloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[ShadowLight](ShadowLight.md).[FALLOFF_STANDARD](ShadowLight.md#falloff_standard)

#### Defined in

packages/dev/core/src/Lights/light.ts:42

___

### INTENSITYMODE\_AUTOMATIC

▪ `Static` `Readonly` **INTENSITYMODE\_AUTOMATIC**: ``0``

Each light type uses the default quantity according to its type:
     point/spot lights use luminous intensity
     directional lights use illuminance

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_AUTOMATIC](ShadowLight.md#intensitymode_automatic)

#### Defined in

packages/dev/core/src/Lights/light.ts:71

___

### INTENSITYMODE\_ILLUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_ILLUMINANCE**: ``3``

lux (lm/m^2)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_ILLUMINANCE](ShadowLight.md#intensitymode_illuminance)

#### Defined in

packages/dev/core/src/Lights/light.ts:83

___

### INTENSITYMODE\_LUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINANCE**: ``4``

nit (cd/m^2)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINANCE](ShadowLight.md#intensitymode_luminance)

#### Defined in

packages/dev/core/src/Lights/light.ts:87

___

### INTENSITYMODE\_LUMINOUSINTENSITY

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSINTENSITY**: ``2``

candela (lm/sr)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINOUSINTENSITY](ShadowLight.md#intensitymode_luminousintensity)

#### Defined in

packages/dev/core/src/Lights/light.ts:79

___

### INTENSITYMODE\_LUMINOUSPOWER

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSPOWER**: ``1``

lumen (lm)

#### Inherited from

[ShadowLight](ShadowLight.md).[INTENSITYMODE_LUMINOUSPOWER](ShadowLight.md#intensitymode_luminouspower)

#### Defined in

packages/dev/core/src/Lights/light.ts:75

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

packages/dev/core/src/Lights/light.ts:51

___

### LIGHTMAP\_SHADOWSONLY

▪ `Static` `Readonly` **LIGHTMAP\_SHADOWSONLY**: ``2``

material.lightmapTexture as only lighting
no light calculation from this light
only adds dynamic shadows from this light

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTMAP_SHADOWSONLY](ShadowLight.md#lightmap_shadowsonly)

#### Defined in

packages/dev/core/src/Lights/light.ts:63

___

### LIGHTMAP\_SPECULAR

▪ `Static` `Readonly` **LIGHTMAP\_SPECULAR**: ``1``

material.lightmapTexture as only diffuse lighting from this light
adds only specular lighting from this light
adds dynamic shadows

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTMAP_SPECULAR](ShadowLight.md#lightmap_specular)

#### Defined in

packages/dev/core/src/Lights/light.ts:57

___

### LIGHTTYPEID\_DIRECTIONALLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_DIRECTIONALLIGHT**: ``1``

Light type const id of the directional light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_DIRECTIONALLIGHT](ShadowLight.md#lighttypeid_directionallight)

#### Defined in

packages/dev/core/src/Lights/light.ts:97

___

### LIGHTTYPEID\_HEMISPHERICLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_HEMISPHERICLIGHT**: ``3``

Light type const id of the hemispheric light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_HEMISPHERICLIGHT](ShadowLight.md#lighttypeid_hemisphericlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:105

___

### LIGHTTYPEID\_POINTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_POINTLIGHT**: ``0``

Light type const id of the point light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_POINTLIGHT](ShadowLight.md#lighttypeid_pointlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:93

___

### LIGHTTYPEID\_SPOTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_SPOTLIGHT**: ``2``

Light type const id of the spot light.

#### Inherited from

[ShadowLight](ShadowLight.md).[LIGHTTYPEID_SPOTLIGHT](ShadowLight.md#lighttypeid_spotlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:101

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

ShadowLight.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:275

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

packages/dev/core/src/node.ts:282

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

packages/dev/core/src/node.ts:410

___

### direction

• `get` **direction**(): [`Vector3`](Vector3.md)

Gets the direction if it has been set.
In case of direction provided, the shadow will not use a cube texture but simulate a spot shadow as a fallback

#### Returns

[`Vector3`](Vector3.md)

#### Overrides

ShadowLight.direction

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:47

• `set` **direction**(`value`): `void`

In case of direction provided, the shadow will not use a cube texture but simulate a spot shadow as a fallback

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Overrides

ShadowLight.direction

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:54

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

ShadowLight.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:131

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

packages/dev/core/src/node.ts:143

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

packages/dev/core/src/Lights/light.ts:266

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

packages/dev/core/src/Lights/light.ts:273

___

### excludedMeshes

• `get` **excludedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes not impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

ShadowLight.excludedMeshes

#### Defined in

packages/dev/core/src/Lights/light.ts:249

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

packages/dev/core/src/Lights/light.ts:255

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

packages/dev/core/src/Lights/light.ts:284

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

packages/dev/core/src/Lights/light.ts:291

___

### includedOnlyMeshes

• `get` **includedOnlyMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the only meshes impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

ShadowLight.includedOnlyMeshes

#### Defined in

packages/dev/core/src/Lights/light.ts:234

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

packages/dev/core/src/Lights/light.ts:240

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

packages/dev/core/src/Lights/light.ts:170

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

packages/dev/core/src/Lights/light.ts:178

___

### lightmapMode

• `get` **lightmapMode**(): `number`

Gets the lightmap mode of this light (should be one of the constants defined by Light.LIGHTMAP_x)

#### Returns

`number`

#### Inherited from

ShadowLight.lightmapMode

#### Defined in

packages/dev/core/src/Lights/light.ts:301

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

packages/dev/core/src/Lights/light.ts:307

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

ShadowLight.onClonedObservable

#### Defined in

packages/dev/core/src/node.ts:323

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

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

ShadowLight.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

ShadowLight.parent

#### Defined in

packages/dev/core/src/node.ts:238

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

packages/dev/core/src/node.ts:200

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

packages/dev/core/src/Lights/shadowLight.ts:134

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

packages/dev/core/src/Lights/shadowLight.ts:142

___

### radius

• `get` **radius**(): `number`

Gets the light radius used by PBR Materials to simulate soft area lights.

#### Returns

`number`

#### Inherited from

ShadowLight.radius

#### Defined in

packages/dev/core/src/Lights/light.ts:187

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

packages/dev/core/src/Lights/light.ts:194

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

packages/dev/core/src/Lights/light.ts:146

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

packages/dev/core/src/Lights/light.ts:154

___

### shadowAngle

• `get` **shadowAngle**(): `number`

Getter: In case of direction provided, the shadow will not use a cube texture but simulate a spot shadow as a fallback
This specifies what angle the shadow will use to be created.

It default to 90 degrees to work nicely with the cube texture generation for point lights shadow maps.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:28

• `set` **shadowAngle**(`value`): `void`

Setter: In case of direction provided, the shadow will not use a cube texture but simulate a spot shadow as a fallback
This specifies what angle the shadow will use to be created.

It default to 90 degrees to work nicely with the cube texture generation for point lights shadow maps.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:38

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

packages/dev/core/src/Lights/light.ts:214

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

packages/dev/core/src/Lights/light.ts:221

___

### shadowMaxZ

• `get` **shadowMaxZ**(): `number`

Sets the shadow projection clipping maximum z value.

#### Returns

`number`

#### Inherited from

ShadowLight.shadowMaxZ

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:186

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

packages/dev/core/src/Lights/shadowLight.ts:193

___

### shadowMinZ

• `get` **shadowMinZ**(): `number`

Gets the shadow projection clipping minimum z value.

#### Returns

`number`

#### Inherited from

ShadowLight.shadowMinZ

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:170

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

packages/dev/core/src/Lights/shadowLight.ts:177

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

packages/dev/core/src/node.ts:454

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

packages/dev/core/src/Lights/light.ts:391

___

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Overrides

[ShadowLight](ShadowLight.md).[_buildUniformLayout](ShadowLight.md#_builduniformlayout)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:168

___

### \_setDefaultShadowProjectionMatrix

▸ `Protected` **_setDefaultShadowProjectionMatrix**(`matrix`, `viewMatrix`, `renderList`): `void`

Sets the passed matrix "matrix" as a left-handed perspective projection matrix with the following settings :
- fov = PI / 2
- aspect ratio : 1.0
- z-near and far equal to the active camera minZ and maxZ.
Returns the PointLight.

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

packages/dev/core/src/Lights/pointLight.ts:143

___

### \_setDirection

▸ `Protected` **_setDirection**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[_setDirection](ShadowLight.md#_setdirection)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:147

___

### \_setPosition

▸ `Protected` **_setPosition**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[_setPosition](ShadowLight.md#_setposition)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:127

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

packages/dev/core/src/node.ts:366

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

packages/dev/core/src/node.ts:833

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

packages/dev/core/src/Lights/light.ts:507

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

packages/dev/core/src/Lights/light.ts:587

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

packages/dev/core/src/Lights/shadowLight.ts:220

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

packages/dev/core/src/Lights/shadowLight.ts:330

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

packages/dev/core/src/node.ts:777

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

packages/dev/core/src/node.ts:794

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

#### Inherited from

[ShadowLight](ShadowLight.md).[dispose](ShadowLight.md#dispose)

#### Defined in

packages/dev/core/src/Lights/light.ts:536

___

### forceProjectionMatrixCompute

▸ **forceProjectionMatrixCompute**(): `void`

Forces the shadow generator to recompute the projection matrix even if position and direction did not changed.

#### Returns

`void`

#### Inherited from

[ShadowLight](ShadowLight.md).[forceProjectionMatrixCompute](ShadowLight.md#forceprojectionmatrixcompute)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:305

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

packages/dev/core/src/Lights/shadowLight.ts:261

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

packages/dev/core/src/node.ts:759

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

packages/dev/core/src/node.ts:808

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

packages/dev/core/src/node.ts:816

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

packages/dev/core/src/node.ts:420

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

packages/dev/core/src/node.ts:684

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

packages/dev/core/src/node.ts:692

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

packages/dev/core/src/node.ts:714

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

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "PointLight"

#### Returns

`string`

the class name

#### Overrides

[ShadowLight](ShadowLight.md).[getClassName](ShadowLight.md#getclassname)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:84

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

#### Inherited from

[ShadowLight](ShadowLight.md).[getDepthMaxZ](ShadowLight.md#getdepthmaxz)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:371

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

#### Inherited from

[ShadowLight](ShadowLight.md).[getDepthMinZ](ShadowLight.md#getdepthminz)

#### Defined in

packages/dev/core/src/Lights/shadowLight.ts:362

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

packages/dev/core/src/Lights/shadowLight.ts:243

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

packages/dev/core/src/node.ts:654

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

packages/dev/core/src/node.ts:662

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

packages/dev/core/src/node.ts:352

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

packages/dev/core/src/node.ts:933

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

packages/dev/core/src/Lights/shadowLight.ts:279

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

packages/dev/core/src/Lights/light.ts:577

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

packages/dev/core/src/node.ts:344

___

### getShadowDirection

▸ **getShadowDirection**(`faceIndex?`): [`Vector3`](Vector3.md)

Returns a new Vector3 aligned with the PointLight cube system according to the passed cube face index (integer).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `faceIndex?` | `number` | The index of the face we are computed the direction to generate shadow |

#### Returns

[`Vector3`](Vector3.md)

The set direction in 2d mode otherwise the direction to the cubemap face if needCube() is true

#### Overrides

[ShadowLight](ShadowLight.md).[getShadowDirection](ShadowLight.md#getshadowdirection)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:109

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

packages/dev/core/src/Lights/light.ts:490

___

### getTypeID

▸ **getTypeID**(): `number`

Returns the integer 0.

#### Returns

`number`

The light Type id as a constant defines in Light.LIGHTTYPEID_x

#### Overrides

[ShadowLight](ShadowLight.md).[getTypeID](ShadowLight.md#gettypeid)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:92

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

packages/dev/core/src/node.ts:434

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

packages/dev/core/src/node.ts:613

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

packages/dev/core/src/node.ts:192

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

packages/dev/core/src/node.ts:569

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

packages/dev/core/src/node.ts:548

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

packages/dev/core/src/node.ts:557

___

### needCube

▸ **needCube**(): `boolean`

Specifies whether or not the shadowmap should be a cube texture.

#### Returns

`boolean`

true if the shadowmap needs to be a cube texture.

#### Overrides

[ShadowLight](ShadowLight.md).[needCube](ShadowLight.md#needcube)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:100

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

packages/dev/core/src/Lights/shadowLight.ts:298

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

packages/dev/core/src/Lights/pointLight.ts:210

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

packages/dev/core/src/node.ts:393

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

packages/dev/core/src/Lights/light.ts:611

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

packages/dev/core/src/node.ts:847

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

packages/dev/core/src/Lights/shadowLight.ts:270

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

packages/dev/core/src/Lights/light.ts:480

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

packages/dev/core/src/Lights/shadowLight.ts:382

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

packages/dev/core/src/Lights/light.ts:457

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

#### Inherited from

[ShadowLight](ShadowLight.md).[transferTexturesToEffect](ShadowLight.md#transfertexturestoeffect)

#### Defined in

packages/dev/core/src/Lights/light.ts:378

___

### transferToEffect

▸ **transferToEffect**(`effect`, `lightIndex`): [`PointLight`](PointLight.md)

Sets the passed Effect "effect" with the PointLight transformed position (or position, if none) and passed name (string).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`PointLight`](PointLight.md)

The point light

#### Overrides

[ShadowLight](ShadowLight.md).[transferToEffect](ShadowLight.md#transfertoeffect)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:184

___

### transferToNodeMaterialEffect

▸ **transferToNodeMaterialEffect**(`effect`, `lightDataUniformName`): [`PointLight`](PointLight.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightDataUniformName` | `string` | The uniform used to store light data (position or direction) |

#### Returns

[`PointLight`](PointLight.md)

The light

#### Overrides

[ShadowLight](ShadowLight.md).[transferToNodeMaterialEffect](ShadowLight.md#transfertonodematerialeffect)

#### Defined in

packages/dev/core/src/Lights/pointLight.ts:195

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

packages/dev/core/src/node.ts:63

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

packages/dev/core/src/node.ts:75

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

packages/dev/core/src/Lights/light.ts:655

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

packages/dev/core/src/Lights/light.ts:672

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

packages/dev/core/src/node.ts:919

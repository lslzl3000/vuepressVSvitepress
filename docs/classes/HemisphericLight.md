[@dev/core](../README.md) / [Exports](../modules.md) / HemisphericLight

# Class: HemisphericLight

The HemisphericLight simulates the ambient environment light,
so the passed direction is the light reflection direction, not the incoming direction.

## Hierarchy

- [`Light`](Light.md)

  ↳ **`HemisphericLight`**

## Table of contents

### Constructors

- [constructor](HemisphericLight.md#constructor)

### Properties

- [\_inverseSquaredRange](HemisphericLight.md#_inversesquaredrange)
- [\_isDirty](HemisphericLight.md#_isdirty)
- [\_parentNode](HemisphericLight.md#_parentnode)
- [\_ranges](HemisphericLight.md#_ranges)
- [animations](HemisphericLight.md#animations)
- [diffuse](HemisphericLight.md#diffuse)
- [direction](HemisphericLight.md#direction)
- [falloffType](HemisphericLight.md#fallofftype)
- [groundColor](HemisphericLight.md#groundcolor)
- [id](HemisphericLight.md#id)
- [inspectableCustomProperties](HemisphericLight.md#inspectablecustomproperties)
- [intensity](HemisphericLight.md#intensity)
- [metadata](HemisphericLight.md#metadata)
- [name](HemisphericLight.md#name)
- [onDisposeObservable](HemisphericLight.md#ondisposeobservable)
- [onReady](HemisphericLight.md#onready)
- [renderPriority](HemisphericLight.md#renderpriority)
- [reservedDataStore](HemisphericLight.md#reserveddatastore)
- [specular](HemisphericLight.md#specular)
- [state](HemisphericLight.md#state)
- [uniqueId](HemisphericLight.md#uniqueid)
- [FALLOFF\_DEFAULT](HemisphericLight.md#falloff_default)
- [FALLOFF\_GLTF](HemisphericLight.md#falloff_gltf)
- [FALLOFF\_PHYSICAL](HemisphericLight.md#falloff_physical)
- [FALLOFF\_STANDARD](HemisphericLight.md#falloff_standard)
- [INTENSITYMODE\_AUTOMATIC](HemisphericLight.md#intensitymode_automatic)
- [INTENSITYMODE\_ILLUMINANCE](HemisphericLight.md#intensitymode_illuminance)
- [INTENSITYMODE\_LUMINANCE](HemisphericLight.md#intensitymode_luminance)
- [INTENSITYMODE\_LUMINOUSINTENSITY](HemisphericLight.md#intensitymode_luminousintensity)
- [INTENSITYMODE\_LUMINOUSPOWER](HemisphericLight.md#intensitymode_luminouspower)
- [LIGHTMAP\_DEFAULT](HemisphericLight.md#lightmap_default)
- [LIGHTMAP\_SHADOWSONLY](HemisphericLight.md#lightmap_shadowsonly)
- [LIGHTMAP\_SPECULAR](HemisphericLight.md#lightmap_specular)
- [LIGHTTYPEID\_DIRECTIONALLIGHT](HemisphericLight.md#lighttypeid_directionallight)
- [LIGHTTYPEID\_HEMISPHERICLIGHT](HemisphericLight.md#lighttypeid_hemisphericlight)
- [LIGHTTYPEID\_POINTLIGHT](HemisphericLight.md#lighttypeid_pointlight)
- [LIGHTTYPEID\_SPOTLIGHT](HemisphericLight.md#lighttypeid_spotlight)

### Accessors

- [animationPropertiesOverride](HemisphericLight.md#animationpropertiesoverride)
- [behaviors](HemisphericLight.md#behaviors)
- [doNotSerialize](HemisphericLight.md#donotserialize)
- [excludeWithLayerMask](HemisphericLight.md#excludewithlayermask)
- [excludedMeshes](HemisphericLight.md#excludedmeshes)
- [includeOnlyWithLayerMask](HemisphericLight.md#includeonlywithlayermask)
- [includedOnlyMeshes](HemisphericLight.md#includedonlymeshes)
- [intensityMode](HemisphericLight.md#intensitymode)
- [lightmapMode](HemisphericLight.md#lightmapmode)
- [onClonedObservable](HemisphericLight.md#onclonedobservable)
- [onDispose](HemisphericLight.md#ondispose)
- [onEnabledStateChangedObservable](HemisphericLight.md#onenabledstatechangedobservable)
- [parent](HemisphericLight.md#parent)
- [radius](HemisphericLight.md#radius)
- [range](HemisphericLight.md#range)
- [shadowEnabled](HemisphericLight.md#shadowenabled)
- [worldMatrixFromCache](HemisphericLight.md#worldmatrixfromcache)

### Methods

- [\_bindLight](HemisphericLight.md#_bindlight)
- [\_buildUniformLayout](HemisphericLight.md#_builduniformlayout)
- [addBehavior](HemisphericLight.md#addbehavior)
- [beginAnimation](HemisphericLight.md#beginanimation)
- [canAffectMesh](HemisphericLight.md#canaffectmesh)
- [clone](HemisphericLight.md#clone)
- [computeWorldMatrix](HemisphericLight.md#computeworldmatrix)
- [createAnimationRange](HemisphericLight.md#createanimationrange)
- [deleteAnimationRange](HemisphericLight.md#deleteanimationrange)
- [dispose](HemisphericLight.md#dispose)
- [getAbsolutePosition](HemisphericLight.md#getabsoluteposition)
- [getAnimationByName](HemisphericLight.md#getanimationbyname)
- [getAnimationRange](HemisphericLight.md#getanimationrange)
- [getAnimationRanges](HemisphericLight.md#getanimationranges)
- [getBehaviorByName](HemisphericLight.md#getbehaviorbyname)
- [getChildMeshes](HemisphericLight.md#getchildmeshes)
- [getChildren](HemisphericLight.md#getchildren)
- [getClassName](HemisphericLight.md#getclassname)
- [getDescendants](HemisphericLight.md#getdescendants)
- [getEngine](HemisphericLight.md#getengine)
- [getHierarchyBoundingVectors](HemisphericLight.md#gethierarchyboundingvectors)
- [getScaledIntensity](HemisphericLight.md#getscaledintensity)
- [getScene](HemisphericLight.md#getscene)
- [getShadowGenerator](HemisphericLight.md#getshadowgenerator)
- [getTypeID](HemisphericLight.md#gettypeid)
- [getWorldMatrix](HemisphericLight.md#getworldmatrix)
- [isDescendantOf](HemisphericLight.md#isdescendantof)
- [isDisposed](HemisphericLight.md#isdisposed)
- [isEnabled](HemisphericLight.md#isenabled)
- [isReady](HemisphericLight.md#isready)
- [markAsDirty](HemisphericLight.md#markasdirty)
- [prepareLightSpecificDefines](HemisphericLight.md#preparelightspecificdefines)
- [removeBehavior](HemisphericLight.md#removebehavior)
- [serialize](HemisphericLight.md#serialize)
- [serializeAnimationRanges](HemisphericLight.md#serializeanimationranges)
- [setDirectionToTarget](HemisphericLight.md#setdirectiontotarget)
- [setEnabled](HemisphericLight.md#setenabled)
- [toString](HemisphericLight.md#tostring)
- [transferTexturesToEffect](HemisphericLight.md#transfertexturestoeffect)
- [transferToEffect](HemisphericLight.md#transfertoeffect)
- [transferToNodeMaterialEffect](HemisphericLight.md#transfertonodematerialeffect)
- [AddNodeConstructor](HemisphericLight.md#addnodeconstructor)
- [Construct](HemisphericLight.md#construct)
- [GetConstructorFromName](HemisphericLight.md#getconstructorfromname)
- [Parse](HemisphericLight.md#parse)
- [ParseAnimationRanges](HemisphericLight.md#parseanimationranges)

## Constructors

### constructor

• **new HemisphericLight**(`name`, `direction`, `scene`)

Creates a HemisphericLight object in the scene according to the passed direction (Vector3).
The HemisphericLight simulates the ambient environment light, so the passed direction is the light reflection direction, not the incoming direction.
The HemisphericLight can't cast shadows.
Documentation : https://doc.babylonjs.com/babylon101/lights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The friendly name of the light |
| `direction` | [`Vector3`](Vector3.md) | The direction of the light reflection |
| `scene` | [`Scene`](Scene.md) | The scene the light belongs to |

#### Overrides

[Light](Light.md).[constructor](Light.md#constructor)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:42

## Properties

### \_inverseSquaredRange

• `Protected` **\_inverseSquaredRange**: `number` = `0`

#### Inherited from

[Light](Light.md).[_inverseSquaredRange](Light.md#_inversesquaredrange)

#### Defined in

packages/dev/core/src/Lights/light.ts:140

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Light](Light.md).[_isDirty](Light.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[Light](Light.md).[_parentNode](Light.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Light](Light.md).[_ranges](Light.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[Light](Light.md).[animations](Light.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

___

### diffuse

• **diffuse**: [`Color3`](Color3.md)

Diffuse gives the basic color to an object.

#### Inherited from

[Light](Light.md).[diffuse](Light.md#diffuse)

#### Defined in

packages/dev/core/src/Lights/light.ts:111

___

### direction

• **direction**: [`Vector3`](Vector3.md)

The light reflection direction, not the incoming direction.

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:31

___

### falloffType

• **falloffType**: `number` = `Light.FALLOFF_DEFAULT`

Defines the falloff type for this light. This lets overriding how punctual light are
falling off base on range or angle.
This can be set to any values in Light.FALLOFF_x.

Note: This is only useful for PBR Materials at the moment. This could be extended if required to
other types of materials.

#### Inherited from

[Light](Light.md).[falloffType](Light.md#fallofftype)

#### Defined in

packages/dev/core/src/Lights/light.ts:129

___

### groundColor

• **groundColor**: [`Color3`](Color3.md)

The groundColor is the light in the opposite direction to the one specified during creation.
You can think of the diffuse and specular light as coming from the centre of the object in the given direction and the groundColor light in the opposite direction.

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:25

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[Light](Light.md).[id](Light.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Light](Light.md).[inspectableCustomProperties](Light.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### intensity

• **intensity**: `number` = `1.0`

Strength of the light.
Note: By default it is define in the framework own unit.
Note: In PBR materials the intensityMode can be use to chose what unit the intensity is defined in.

#### Inherited from

[Light](Light.md).[intensity](Light.md#intensity)

#### Defined in

packages/dev/core/src/Lights/light.ts:137

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Light](Light.md).[metadata](Light.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[Light](Light.md).[name](Light.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Light](Light.md).[onDisposeObservable](Light.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Light](Light.md).[onReady](Light.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### renderPriority

• **renderPriority**: `number` = `0`

Defines the rendering priority of the lights. It can help in case of fallback or number of lights
exceeding the number allowed of the materials.

#### Inherited from

[Light](Light.md).[renderPriority](Light.md#renderpriority)

#### Defined in

packages/dev/core/src/Lights/light.ts:206

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Light](Light.md).[reservedDataStore](Light.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### specular

• **specular**: [`Color3`](Color3.md)

Specular produces a highlight color on an object.
Note: This is not affecting PBR materials.

#### Inherited from

[Light](Light.md).[specular](Light.md#specular)

#### Defined in

packages/dev/core/src/Lights/light.ts:118

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Light](Light.md).[state](Light.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Light](Light.md).[uniqueId](Light.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### FALLOFF\_DEFAULT

▪ `Static` `Readonly` **FALLOFF\_DEFAULT**: ``0``

Falloff Default: light is falling off following the material specification:
standard material is using standard falloff whereas pbr material can request special falloff per materials.

#### Inherited from

[Light](Light.md).[FALLOFF_DEFAULT](Light.md#falloff_default)

#### Defined in

packages/dev/core/src/Lights/light.ts:25

___

### FALLOFF\_GLTF

▪ `Static` `Readonly` **FALLOFF\_GLTF**: ``2``

Falloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[Light](Light.md).[FALLOFF_GLTF](Light.md#falloff_gltf)

#### Defined in

packages/dev/core/src/Lights/light.ts:36

___

### FALLOFF\_PHYSICAL

▪ `Static` `Readonly` **FALLOFF\_PHYSICAL**: ``1``

Falloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[Light](Light.md).[FALLOFF_PHYSICAL](Light.md#falloff_physical)

#### Defined in

packages/dev/core/src/Lights/light.ts:30

___

### FALLOFF\_STANDARD

▪ `Static` `Readonly` **FALLOFF\_STANDARD**: ``3``

Falloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[Light](Light.md).[FALLOFF_STANDARD](Light.md#falloff_standard)

#### Defined in

packages/dev/core/src/Lights/light.ts:42

___

### INTENSITYMODE\_AUTOMATIC

▪ `Static` `Readonly` **INTENSITYMODE\_AUTOMATIC**: ``0``

Each light type uses the default quantity according to its type:
     point/spot lights use luminous intensity
     directional lights use illuminance

#### Inherited from

[Light](Light.md).[INTENSITYMODE_AUTOMATIC](Light.md#intensitymode_automatic)

#### Defined in

packages/dev/core/src/Lights/light.ts:71

___

### INTENSITYMODE\_ILLUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_ILLUMINANCE**: ``3``

lux (lm/m^2)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_ILLUMINANCE](Light.md#intensitymode_illuminance)

#### Defined in

packages/dev/core/src/Lights/light.ts:83

___

### INTENSITYMODE\_LUMINANCE

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINANCE**: ``4``

nit (cd/m^2)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINANCE](Light.md#intensitymode_luminance)

#### Defined in

packages/dev/core/src/Lights/light.ts:87

___

### INTENSITYMODE\_LUMINOUSINTENSITY

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSINTENSITY**: ``2``

candela (lm/sr)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINOUSINTENSITY](Light.md#intensitymode_luminousintensity)

#### Defined in

packages/dev/core/src/Lights/light.ts:79

___

### INTENSITYMODE\_LUMINOUSPOWER

▪ `Static` `Readonly` **INTENSITYMODE\_LUMINOUSPOWER**: ``1``

lumen (lm)

#### Inherited from

[Light](Light.md).[INTENSITYMODE_LUMINOUSPOWER](Light.md#intensitymode_luminouspower)

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

[Light](Light.md).[LIGHTMAP_DEFAULT](Light.md#lightmap_default)

#### Defined in

packages/dev/core/src/Lights/light.ts:51

___

### LIGHTMAP\_SHADOWSONLY

▪ `Static` `Readonly` **LIGHTMAP\_SHADOWSONLY**: ``2``

material.lightmapTexture as only lighting
no light calculation from this light
only adds dynamic shadows from this light

#### Inherited from

[Light](Light.md).[LIGHTMAP_SHADOWSONLY](Light.md#lightmap_shadowsonly)

#### Defined in

packages/dev/core/src/Lights/light.ts:63

___

### LIGHTMAP\_SPECULAR

▪ `Static` `Readonly` **LIGHTMAP\_SPECULAR**: ``1``

material.lightmapTexture as only diffuse lighting from this light
adds only specular lighting from this light
adds dynamic shadows

#### Inherited from

[Light](Light.md).[LIGHTMAP_SPECULAR](Light.md#lightmap_specular)

#### Defined in

packages/dev/core/src/Lights/light.ts:57

___

### LIGHTTYPEID\_DIRECTIONALLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_DIRECTIONALLIGHT**: ``1``

Light type const id of the directional light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_DIRECTIONALLIGHT](Light.md#lighttypeid_directionallight)

#### Defined in

packages/dev/core/src/Lights/light.ts:97

___

### LIGHTTYPEID\_HEMISPHERICLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_HEMISPHERICLIGHT**: ``3``

Light type const id of the hemispheric light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_HEMISPHERICLIGHT](Light.md#lighttypeid_hemisphericlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:105

___

### LIGHTTYPEID\_POINTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_POINTLIGHT**: ``0``

Light type const id of the point light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_POINTLIGHT](Light.md#lighttypeid_pointlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:93

___

### LIGHTTYPEID\_SPOTLIGHT

▪ `Static` `Readonly` **LIGHTTYPEID\_SPOTLIGHT**: ``2``

Light type const id of the spot light.

#### Inherited from

[Light](Light.md).[LIGHTTYPEID_SPOTLIGHT](Light.md#lighttypeid_spotlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:101

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

Light.animationPropertiesOverride

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

Light.animationPropertiesOverride

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

Light.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

Light.doNotSerialize

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

Light.doNotSerialize

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

Light.excludeWithLayerMask

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

Light.excludeWithLayerMask

#### Defined in

packages/dev/core/src/Lights/light.ts:273

___

### excludedMeshes

• `get` **excludedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes not impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

Light.excludedMeshes

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

Light.excludedMeshes

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

Light.includeOnlyWithLayerMask

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

Light.includeOnlyWithLayerMask

#### Defined in

packages/dev/core/src/Lights/light.ts:291

___

### includedOnlyMeshes

• `get` **includedOnlyMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the only meshes impacted by this light.

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

Light.includedOnlyMeshes

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

Light.includedOnlyMeshes

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

Light.intensityMode

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

Light.intensityMode

#### Defined in

packages/dev/core/src/Lights/light.ts:178

___

### lightmapMode

• `get` **lightmapMode**(): `number`

Gets the lightmap mode of this light (should be one of the constants defined by Light.LIGHTMAP_x)

#### Returns

`number`

#### Inherited from

Light.lightmapMode

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

Light.lightmapMode

#### Defined in

packages/dev/core/src/Lights/light.ts:307

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

Light.onClonedObservable

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

Light.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

Light.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

Light.parent

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

Light.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### radius

• `get` **radius**(): `number`

Gets the light radius used by PBR Materials to simulate soft area lights.

#### Returns

`number`

#### Inherited from

Light.radius

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

Light.radius

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

Light.range

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

Light.range

#### Defined in

packages/dev/core/src/Lights/light.ts:154

___

### shadowEnabled

• `get` **shadowEnabled**(): `boolean`

Gets whether or not the shadows are enabled for this light. This can help turning off/on shadow without detaching
the current shadow generator.

#### Returns

`boolean`

#### Inherited from

Light.shadowEnabled

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

Light.shadowEnabled

#### Defined in

packages/dev/core/src/Lights/light.ts:221

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

Light.worldMatrixFromCache

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

[Light](Light.md).[_bindLight](Light.md#_bindlight)

#### Defined in

packages/dev/core/src/Lights/light.ts:391

___

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Overrides

[Light](Light.md).[_buildUniformLayout](Light.md#_builduniformlayout)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:47

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

[Light](Light.md).[addBehavior](Light.md#addbehavior)

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

[Light](Light.md).[beginAnimation](Light.md#beginanimation)

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

[Light](Light.md).[canAffectMesh](Light.md#canaffectmesh)

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

[Light](Light.md).[clone](Light.md#clone)

#### Defined in

packages/dev/core/src/Lights/light.ts:587

___

### computeWorldMatrix

▸ **computeWorldMatrix**(): [`Matrix`](Matrix.md)

Computes the world matrix of the node

#### Returns

[`Matrix`](Matrix.md)

the world matrix

#### Overrides

[Light](Light.md).[computeWorldMatrix](Light.md#computeworldmatrix)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:107

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

[Light](Light.md).[createAnimationRange](Light.md#createanimationrange)

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

[Light](Light.md).[deleteAnimationRange](Light.md#deleteanimationrange)

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

[Light](Light.md).[dispose](Light.md#dispose)

#### Defined in

packages/dev/core/src/Lights/light.ts:536

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns a Vector3, the absolute light position in the World.

#### Returns

[`Vector3`](Vector3.md)

the world space position of the light

#### Inherited from

[Light](Light.md).[getAbsolutePosition](Light.md#getabsoluteposition)

#### Defined in

packages/dev/core/src/Lights/light.ts:498

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

[Light](Light.md).[getAnimationByName](Light.md#getanimationbyname)

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

[Light](Light.md).[getAnimationRange](Light.md#getanimationrange)

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

[Light](Light.md).[getAnimationRanges](Light.md#getanimationranges)

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

[Light](Light.md).[getBehaviorByName](Light.md#getbehaviorbyname)

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

[Light](Light.md).[getChildMeshes](Light.md#getchildmeshes)

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

[Light](Light.md).[getChildMeshes](Light.md#getchildmeshes)

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

[Light](Light.md).[getChildren](Light.md#getchildren)

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

[Light](Light.md).[getChildren](Light.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "HemisphericLight".

#### Returns

`string`

The class name

#### Overrides

[Light](Light.md).[getClassName](Light.md#getclassname)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:61

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

[Light](Light.md).[getDescendants](Light.md#getdescendants)

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

[Light](Light.md).[getDescendants](Light.md#getdescendants)

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

[Light](Light.md).[getEngine](Light.md#getengine)

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

[Light](Light.md).[getHierarchyBoundingVectors](Light.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getScaledIntensity

▸ **getScaledIntensity**(): `number`

Returns the intensity scaled by the Photometric Scale according to the light type and intensity mode.

#### Returns

`number`

the scaled intensity in intensity mode unit

#### Inherited from

[Light](Light.md).[getScaledIntensity](Light.md#getscaledintensity)

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

[Light](Light.md).[getScene](Light.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getShadowGenerator

▸ **getShadowGenerator**(): [`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

Returns the shadow generator associated to the light.

#### Returns

[`Nullable`](../modules.md#nullable)[`IShadowGenerator`](../interfaces/IShadowGenerator.md)

Always null for hemispheric lights because it does not support shadows.

#### Overrides

[Light](Light.md).[getShadowGenerator](Light.md#getshadowgenerator)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:80

___

### getTypeID

▸ **getTypeID**(): `number`

Returns the integer 3.

#### Returns

`number`

The light Type id as a constant defines in Light.LIGHTTYPEID_x

#### Overrides

[Light](Light.md).[getTypeID](Light.md#gettypeid)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:118

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Returns the latest update of the World matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[Light](Light.md).[getWorldMatrix](Light.md#getworldmatrix)

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

[Light](Light.md).[isDescendantOf](Light.md#isdescendantof)

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

[Light](Light.md).[isDisposed](Light.md#isdisposed)

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

[Light](Light.md).[isEnabled](Light.md#isenabled)

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

[Light](Light.md).[isReady](Light.md#isready)

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

[Light](Light.md).[markAsDirty](Light.md#markasdirty)

#### Defined in

packages/dev/core/src/node.ts:557

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

[Light](Light.md).[prepareLightSpecificDefines](Light.md#preparelightspecificdefines)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:127

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

[Light](Light.md).[removeBehavior](Light.md#removebehavior)

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

[Light](Light.md).[serialize](Light.md#serialize)

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

[Light](Light.md).[serializeAnimationRanges](Light.md#serializeanimationranges)

#### Defined in

packages/dev/core/src/node.ts:847

___

### setDirectionToTarget

▸ **setDirectionToTarget**(`target`): [`Vector3`](Vector3.md)

Sets the HemisphericLight direction towards the passed target (Vector3).
Returns the updated direction.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Vector3`](Vector3.md) | The target the direction should point to |

#### Returns

[`Vector3`](Vector3.md)

The computed direction

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:71

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

[Light](Light.md).[setEnabled](Light.md#setenabled)

#### Defined in

packages/dev/core/src/Lights/light.ts:480

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

[Light](Light.md).[toString](Light.md#tostring)

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

[Light](Light.md).[transferTexturesToEffect](Light.md#transfertexturestoeffect)

#### Defined in

packages/dev/core/src/Lights/light.ts:378

___

### transferToEffect

▸ **transferToEffect**(`_effect`, `lightIndex`): [`HemisphericLight`](HemisphericLight.md)

Sets the passed Effect object with the HemisphericLight normalized direction and color and the passed name (string).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_effect` | [`Effect`](Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`HemisphericLight`](HemisphericLight.md)

The hemispheric light

#### Overrides

[Light](Light.md).[transferToEffect](Light.md#transfertoeffect)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:90

___

### transferToNodeMaterialEffect

▸ **transferToNodeMaterialEffect**(`effect`, `lightDataUniformName`): [`HemisphericLight`](HemisphericLight.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to update |
| `lightDataUniformName` | `string` | The uniform used to store light data (position or direction) |

#### Returns

[`HemisphericLight`](HemisphericLight.md)

The light

#### Overrides

[Light](Light.md).[transferToNodeMaterialEffect](Light.md#transfertonodematerialeffect)

#### Defined in

packages/dev/core/src/Lights/hemisphericLight.ts:97

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

[Light](Light.md).[Construct](Light.md#construct)

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

[Light](Light.md).[GetConstructorFromName](Light.md#getconstructorfromname)

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

[Light](Light.md).[Parse](Light.md#parse)

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

[Light](Light.md).[ParseAnimationRanges](Light.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919

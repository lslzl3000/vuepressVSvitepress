[@dev/core](../README.md) / [Exports](../modules.md) / IShadowLight

# Interface: IShadowLight

Interface describing all the common properties and methods a shadow light needs to implement.
This helps both the shadow generator and materials to generate the corresponding shadow maps
as well as binding the different shadow properties to the effects.

## Hierarchy

- [`Light`](../classes/Light.md)

  ↳ **`IShadowLight`**

## Implemented by

- [`ShadowLight`](../classes/ShadowLight.md)

## Table of contents

### Properties

- [\_inverseSquaredRange](IShadowLight.md#_inversesquaredrange)
- [\_isDirty](IShadowLight.md#_isdirty)
- [\_parentNode](IShadowLight.md#_parentnode)
- [\_ranges](IShadowLight.md#_ranges)
- [animations](IShadowLight.md#animations)
- [customProjectionMatrixBuilder](IShadowLight.md#customprojectionmatrixbuilder)
- [diffuse](IShadowLight.md#diffuse)
- [direction](IShadowLight.md#direction)
- [falloffType](IShadowLight.md#fallofftype)
- [id](IShadowLight.md#id)
- [inspectableCustomProperties](IShadowLight.md#inspectablecustomproperties)
- [intensity](IShadowLight.md#intensity)
- [metadata](IShadowLight.md#metadata)
- [name](IShadowLight.md#name)
- [onDisposeObservable](IShadowLight.md#ondisposeobservable)
- [onReady](IShadowLight.md#onready)
- [position](IShadowLight.md#position)
- [renderPriority](IShadowLight.md#renderpriority)
- [reservedDataStore](IShadowLight.md#reserveddatastore)
- [shadowMaxZ](IShadowLight.md#shadowmaxz)
- [shadowMinZ](IShadowLight.md#shadowminz)
- [specular](IShadowLight.md#specular)
- [state](IShadowLight.md#state)
- [transformedDirection](IShadowLight.md#transformeddirection)
- [transformedPosition](IShadowLight.md#transformedposition)
- [uniqueId](IShadowLight.md#uniqueid)

### Accessors

- [animationPropertiesOverride](IShadowLight.md#animationpropertiesoverride)
- [behaviors](IShadowLight.md#behaviors)
- [doNotSerialize](IShadowLight.md#donotserialize)
- [excludeWithLayerMask](IShadowLight.md#excludewithlayermask)
- [excludedMeshes](IShadowLight.md#excludedmeshes)
- [includeOnlyWithLayerMask](IShadowLight.md#includeonlywithlayermask)
- [includedOnlyMeshes](IShadowLight.md#includedonlymeshes)
- [intensityMode](IShadowLight.md#intensitymode)
- [lightmapMode](IShadowLight.md#lightmapmode)
- [onClonedObservable](IShadowLight.md#onclonedobservable)
- [onDispose](IShadowLight.md#ondispose)
- [onEnabledStateChangedObservable](IShadowLight.md#onenabledstatechangedobservable)
- [parent](IShadowLight.md#parent)
- [radius](IShadowLight.md#radius)
- [range](IShadowLight.md#range)
- [shadowEnabled](IShadowLight.md#shadowenabled)
- [worldMatrixFromCache](IShadowLight.md#worldmatrixfromcache)

### Methods

- [\_bindLight](IShadowLight.md#_bindlight)
- [\_buildUniformLayout](IShadowLight.md#_builduniformlayout)
- [addBehavior](IShadowLight.md#addbehavior)
- [beginAnimation](IShadowLight.md#beginanimation)
- [canAffectMesh](IShadowLight.md#canaffectmesh)
- [clone](IShadowLight.md#clone)
- [computeTransformedInformation](IShadowLight.md#computetransformedinformation)
- [computeWorldMatrix](IShadowLight.md#computeworldmatrix)
- [createAnimationRange](IShadowLight.md#createanimationrange)
- [deleteAnimationRange](IShadowLight.md#deleteanimationrange)
- [dispose](IShadowLight.md#dispose)
- [forceProjectionMatrixCompute](IShadowLight.md#forceprojectionmatrixcompute)
- [getAbsolutePosition](IShadowLight.md#getabsoluteposition)
- [getAnimationByName](IShadowLight.md#getanimationbyname)
- [getAnimationRange](IShadowLight.md#getanimationrange)
- [getAnimationRanges](IShadowLight.md#getanimationranges)
- [getBehaviorByName](IShadowLight.md#getbehaviorbyname)
- [getChildMeshes](IShadowLight.md#getchildmeshes)
- [getChildren](IShadowLight.md#getchildren)
- [getClassName](IShadowLight.md#getclassname)
- [getDepthMaxZ](IShadowLight.md#getdepthmaxz)
- [getDepthMinZ](IShadowLight.md#getdepthminz)
- [getDepthScale](IShadowLight.md#getdepthscale)
- [getDescendants](IShadowLight.md#getdescendants)
- [getEngine](IShadowLight.md#getengine)
- [getHierarchyBoundingVectors](IShadowLight.md#gethierarchyboundingvectors)
- [getScaledIntensity](IShadowLight.md#getscaledintensity)
- [getScene](IShadowLight.md#getscene)
- [getShadowDirection](IShadowLight.md#getshadowdirection)
- [getShadowGenerator](IShadowLight.md#getshadowgenerator)
- [getTypeID](IShadowLight.md#gettypeid)
- [getWorldMatrix](IShadowLight.md#getworldmatrix)
- [isDescendantOf](IShadowLight.md#isdescendantof)
- [isDisposed](IShadowLight.md#isdisposed)
- [isEnabled](IShadowLight.md#isenabled)
- [isReady](IShadowLight.md#isready)
- [markAsDirty](IShadowLight.md#markasdirty)
- [needCube](IShadowLight.md#needcube)
- [needProjectionMatrixCompute](IShadowLight.md#needprojectionmatrixcompute)
- [prepareLightSpecificDefines](IShadowLight.md#preparelightspecificdefines)
- [removeBehavior](IShadowLight.md#removebehavior)
- [serialize](IShadowLight.md#serialize)
- [serializeAnimationRanges](IShadowLight.md#serializeanimationranges)
- [setEnabled](IShadowLight.md#setenabled)
- [setShadowProjectionMatrix](IShadowLight.md#setshadowprojectionmatrix)
- [toString](IShadowLight.md#tostring)
- [transferTexturesToEffect](IShadowLight.md#transfertexturestoeffect)
- [transferToEffect](IShadowLight.md#transfertoeffect)
- [transferToNodeMaterialEffect](IShadowLight.md#transfertonodematerialeffect)

## Properties

### \_inverseSquaredRange

• `Protected` **\_inverseSquaredRange**: `number` = `0`

#### Inherited from

[Light](../classes/Light.md).[_inverseSquaredRange](../classes/Light.md#_inversesquaredrange)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:140

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Light](../classes/Light.md).[_isDirty](../classes/Light.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](../classes/Node.md) = `null`

#### Inherited from

[Light](../classes/Light.md).[_parentNode](../classes/Light.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Light](../classes/Light.md).[_ranges](../classes/Light.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### animations

• **animations**: [`Animation`](../classes/Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[Light](../classes/Light.md).[animations](../classes/Light.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:153

___

### customProjectionMatrixBuilder

• **customProjectionMatrixBuilder**: (`viewMatrix`: [`Matrix`](../classes/Matrix.md), `renderList`: [`AbstractMesh`](../classes/AbstractMesh.md)[], `result`: [`Matrix`](../classes/Matrix.md)) => `void`

#### Type declaration

▸ (`viewMatrix`, `renderList`, `result`): `void`

Callback defining a custom Projection Matrix Builder.
This can be used to override the default projection matrix computation.

##### Parameters

| Name | Type |
| :------ | :------ |
| `viewMatrix` | [`Matrix`](../classes/Matrix.md) |
| `renderList` | [`AbstractMesh`](../classes/AbstractMesh.md)[] |
| `result` | [`Matrix`](../classes/Matrix.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:63

___

### diffuse

• **diffuse**: [`Color3`](../classes/Color3.md)

Diffuse gives the basic color to an object.

#### Inherited from

[Light](../classes/Light.md).[diffuse](../classes/Light.md#diffuse)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:111

___

### direction

• **direction**: [`Vector3`](../classes/Vector3.md)

In 2d mode (needCube being false), the direction used to cast the shadow.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:25

___

### falloffType

• **falloffType**: `number` = `Light.FALLOFF_DEFAULT`

Defines the falloff type for this light. This lets overriding how punctual light are
falling off base on range or angle.
This can be set to any values in Light.FALLOFF_x.

Note: This is only useful for PBR Materials at the moment. This could be extended if required to
other types of materials.

#### Inherited from

[Light](../classes/Light.md).[falloffType](../classes/Light.md#fallofftype)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:129

___

### id

• **id**: `string`

The light id in the scene (used in scene.getLightById for instance)

#### Overrides

[Light](../classes/Light.md).[id](../classes/Light.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:17

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Light](../classes/Light.md).[inspectableCustomProperties](../classes/Light.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:126

___

### intensity

• **intensity**: `number` = `1.0`

Strength of the light.
Note: By default it is define in the framework own unit.
Note: In PBR materials the intensityMode can be use to chose what unit the intensity is defined in.

#### Inherited from

[Light](../classes/Light.md).[intensity](../classes/Light.md#intensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:137

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Light](../classes/Light.md).[metadata](../classes/Light.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### name

• **name**: `string`

The friendly name of the light in the scene.

#### Overrides

[Light](../classes/Light.md).[name](../classes/Light.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:37

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](../classes/Observable.md)[`Node`](../classes/Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Light](../classes/Light.md).[onDisposeObservable](../classes/Light.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](../classes/Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Light](../classes/Light.md).[onReady](../classes/Light.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### position

• **position**: [`Vector3`](../classes/Vector3.md)

The position the shadow will be casted from.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:21

___

### renderPriority

• **renderPriority**: `number` = `0`

Defines the rendering priority of the lights. It can help in case of fallback or number of lights
exceeding the number allowed of the materials.

#### Inherited from

[Light](../classes/Light.md).[renderPriority](../classes/Light.md#renderpriority)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:206

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Light](../classes/Light.md).[reservedDataStore](../classes/Light.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### shadowMaxZ

• **shadowMaxZ**: `number`

Defines the shadow projection clipping maximum z value.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:45

___

### shadowMinZ

• **shadowMinZ**: `number`

Defines the shadow projection clipping minimum z value.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:41

___

### specular

• **specular**: [`Color3`](../classes/Color3.md)

Specular produces a highlight color on an object.
Note: This is not affecting PBR materials.

#### Inherited from

[Light](../classes/Light.md).[specular](../classes/Light.md#specular)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:118

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Light](../classes/Light.md).[state](../classes/Light.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### transformedDirection

• **transformedDirection**: [`Vector3`](../classes/Vector3.md)

The transformed direction. Direction of the light in world space taking parenting in account.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:33

___

### transformedPosition

• **transformedPosition**: [`Vector3`](../classes/Vector3.md)

The transformed position. Position of the light in world space taking parenting in account.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:29

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Light](../classes/Light.md).[uniqueId](../classes/Light.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](../classes/AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](../classes/AnimationPropertiesOverride.md)

#### Inherited from

Light.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:275

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](../classes/AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Inherited from

Light.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:282

___

### behaviors

• `get` **behaviors**(): [`Behavior`](Behavior.md)[`Node`](../classes/Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](Behavior.md)[`Node`](../classes/Node.md)[]

#### Inherited from

Light.behaviors

#### Defined in

https://github.com/babylon.js/core/src/node.ts:410

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

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

#### Inherited from

Light.excludeWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:273

___

### excludedMeshes

• `get` **excludedMeshes**(): [`AbstractMesh`](../classes/AbstractMesh.md)[]

Gets the meshes not impacted by this light.

#### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)[]

#### Inherited from

Light.excludedMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:249

• `set` **excludedMeshes**(`value`): `void`

Sets the meshes not impacted by this light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`AbstractMesh`](../classes/AbstractMesh.md)[] |

#### Returns

`void`

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

#### Inherited from

Light.includeOnlyWithLayerMask

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:291

___

### includedOnlyMeshes

• `get` **includedOnlyMeshes**(): [`AbstractMesh`](../classes/AbstractMesh.md)[]

Gets the only meshes impacted by this light.

#### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)[]

#### Inherited from

Light.includedOnlyMeshes

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:234

• `set` **includedOnlyMeshes**(`value`): `void`

Sets the only meshes impacted by this light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`AbstractMesh`](../classes/AbstractMesh.md)[] |

#### Returns

`void`

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

#### Inherited from

Light.lightmapMode

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:307

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](../classes/Observable.md)[`Node`](../classes/Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](../classes/Observable.md)[`Node`](../classes/Node.md)

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

#### Inherited from

Light.onDispose

#### Defined in

https://github.com/babylon.js/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](../classes/Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](../classes/Observable.md)`boolean`

#### Inherited from

Light.onEnabledStateChangedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](../classes/Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](../classes/Node.md)

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
| `parent` | [`Nullable`](../modules.md#nullable)[`Node`](../classes/Node.md) |

#### Returns

`void`

#### Inherited from

Light.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:200

___

### radius

• `get` **radius**(): `number`

Gets the light radius used by PBR Materials to simulate soft area lights.

#### Returns

`number`

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

#### Inherited from

Light.shadowEnabled

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:221

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](../classes/Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](../classes/Matrix.md)

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
| `scene` | [`Scene`](../classes/Scene.md) | `undefined` | The scene where the light belongs to |
| `effect` | [`Effect`](../classes/Effect.md) | `undefined` | The effect we are binding the data to |
| `useSpecular` | `boolean` | `undefined` | Defines if specular is supported |
| `receiveShadows` | `boolean` | `true` | Defines if the effect (mesh) we bind the light for receives shadows |

#### Returns

`void`

#### Inherited from

[Light](../classes/Light.md).[_bindLight](../classes/Light.md#_bindlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:391

___

### \_buildUniformLayout

▸ `Protected` `Abstract` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Inherited from

[Light](../classes/Light.md).[_buildUniformLayout](../classes/Light.md#_builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:361

___

### addBehavior

▸ **addBehavior**(`behavior`, `attachImmediately?`): [`Node`](../classes/Node.md)

Attach a behavior to the node

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `behavior` | [`Behavior`](Behavior.md)[`Node`](../classes/Node.md) | `undefined` | defines the behavior to attach |
| `attachImmediately` | `boolean` | `false` | defines that the behavior must be attached even if the scene is still loading |

#### Returns

[`Node`](../classes/Node.md)

the current Node

#### Inherited from

[Light](../classes/Light.md).[addBehavior](../classes/Light.md#addbehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:366

___

### beginAnimation

▸ **beginAnimation**(`name`, `loop?`, `speedRatio?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](../classes/Animatable.md)

Will start the animation sequence

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the range frames for animation sequence |
| `loop?` | `boolean` | defines if the animation should loop (false by default) |
| `speedRatio?` | `number` | defines the speed factor in which to run the animation (1 by default) |
| `onAnimationEnd?` | () => `void` | defines a function to be executed when the animation ended (undefined by default) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](../classes/Animatable.md)

the object created for this animation. If range does not exist, it will return null

#### Inherited from

[Light](../classes/Light.md).[beginAnimation](../classes/Light.md#beginanimation)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:833

___

### canAffectMesh

▸ **canAffectMesh**(`mesh`): `boolean`

Specifies if the light will affect the passed mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](../classes/AbstractMesh.md) | The mesh to test against the light |

#### Returns

`boolean`

true the mesh is affected otherwise, false.

#### Inherited from

[Light](../classes/Light.md).[canAffectMesh](../classes/Light.md#canaffectmesh)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:507

___

### clone

▸ **clone**(`name`, `newParent?`): [`Nullable`](../modules.md#nullable)[`Light`](../classes/Light.md)

Returns a new Light object, named "name", from the current one.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the cloned light |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](../classes/Node.md) | `null` | The parent of this light, if it has one |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](../classes/Light.md)

the new created light

#### Inherited from

[Light](../classes/Light.md).[clone](../classes/Light.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:587

___

### computeTransformedInformation

▸ **computeTransformedInformation**(): `boolean`

Computes the transformed information (transformedPosition and transformedDirection in World space) of the current light

#### Returns

`boolean`

true if the information has been computed, false if it does not need to (no parenting)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:51

___

### computeWorldMatrix

▸ **computeWorldMatrix**(`force?`): [`Matrix`](../classes/Matrix.md)

Computes the world matrix of the node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | defines if the cache version should be invalidated forcing the world matrix to be created from scratch |

#### Returns

[`Matrix`](../classes/Matrix.md)

the world matrix

#### Inherited from

[Light](../classes/Light.md).[computeWorldMatrix](../classes/Light.md#computeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:868

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

[Light](../classes/Light.md).[createAnimationRange](../classes/Light.md#createanimationrange)

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

[Light](../classes/Light.md).[deleteAnimationRange](../classes/Light.md#deleteanimationrange)

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

#### Inherited from

[Light](../classes/Light.md).[dispose](../classes/Light.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:536

___

### forceProjectionMatrixCompute

▸ **forceProjectionMatrixCompute**(): `void`

Forces the shadow generator to recompute the projection matrix even if position and direction did not changed.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:95

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](../classes/Vector3.md)

Returns a Vector3, the absolute light position in the World.

#### Returns

[`Vector3`](../classes/Vector3.md)

the world space position of the light

#### Inherited from

[Light](../classes/Light.md).[getAbsolutePosition](../classes/Light.md#getabsoluteposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:498

___

### getAnimationByName

▸ **getAnimationByName**(`name`): [`Nullable`](../modules.md#nullable)[`Animation`](../classes/Animation.md)

Get an animation by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animation`](../classes/Animation.md)

null if not found else the requested animation

#### Inherited from

[Light](../classes/Light.md).[getAnimationByName](../classes/Light.md#getanimationbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:759

___

### getAnimationRange

▸ **getAnimationRange**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationRange`](../classes/AnimationRange.md)

Get an animation range by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation range to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](../classes/AnimationRange.md)

null if not found else the requested animation range

#### Inherited from

[Light](../classes/Light.md).[getAnimationRange](../classes/Light.md#getanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:808

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](../classes/AnimationRange.md)[]

Gets the list of all animation ranges defined on this node

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](../classes/AnimationRange.md)[]

an array

#### Inherited from

[Light](../classes/Light.md).[getAnimationRanges](../classes/Light.md#getanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:816

___

### getBehaviorByName

▸ **getBehaviorByName**(`name`): [`Nullable`](../modules.md#nullable)[`Behavior`](Behavior.md)[`Node`](../classes/Node.md)

Gets an attached behavior by name

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the behavior to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Behavior`](Behavior.md)[`Node`](../classes/Node.md)

null if behavior was not found else the requested behavior

#### Inherited from

[Light](../classes/Light.md).[getBehaviorByName](../classes/Light.md#getbehaviorbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:420

___

### getChildMeshes

▸ **getChildMeshes**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Get all child-meshes of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`AbstractMesh`](../classes/AbstractMesh.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

an array of AbstractMesh

#### Inherited from

[Light](../classes/Light.md).[getChildMeshes](../classes/Light.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:684

▸ **getChildMeshes**(`directDescendantsOnly?`, `predicate?`): [`AbstractMesh`](../classes/AbstractMesh.md)[]

Get all child-meshes of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)[]

an array of AbstractMesh

#### Inherited from

[Light](../classes/Light.md).[getChildMeshes](../classes/Light.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:692

___

### getChildren

▸ **getChildren**`T`(`predicate?`, `directDescendantsOnly?`): `T`[]

Get all direct children of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](../classes/Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

`T`[]

an array of Node

#### Inherited from

[Light](../classes/Light.md).[getChildren](../classes/Light.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:714

▸ **getChildren**(`predicate?`, `directDescendantsOnly?`): [`Node`](../classes/Node.md)[]

Get all direct children of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

[`Node`](../classes/Node.md)[]

an array of Node

#### Inherited from

[Light](../classes/Light.md).[getChildren](../classes/Light.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "Light".

#### Returns

`string`

the class name

#### Inherited from

[Light](../classes/Light.md).[getClassName](../classes/Light.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:445

___

### getDepthMaxZ

▸ **getDepthMaxZ**(`activeCamera`): `number`

Gets the maxZ used for shadow according to both the scene and the light.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeCamera` | [`Camera`](../classes/Camera.md) | The camera we are returning the max for |

#### Returns

`number`

the depth max z

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:116

___

### getDepthMinZ

▸ **getDepthMinZ**(`activeCamera`): `number`

Gets the minZ used for shadow according to both the scene and the light.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeCamera` | [`Camera`](../classes/Camera.md) | The camera we are returning the min for |

#### Returns

`number`

the depth min z

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:109

___

### getDepthScale

▸ **getDepthScale**(): `number`

Gets the current depth scale used in ESM.

#### Returns

`number`

The scale

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:78

___

### getDescendants

▸ **getDescendants**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Will return all nodes that have this node as ascendant

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](../classes/Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

all children nodes of all types

#### Inherited from

[Light](../classes/Light.md).[getDescendants](../classes/Light.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:654

▸ **getDescendants**(`directDescendantsOnly?`, `predicate?`): [`Node`](../classes/Node.md)[]

Will return all nodes that have this node as ascendant

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](../classes/Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`Node`](../classes/Node.md)[]

all children nodes of all types

#### Inherited from

[Light](../classes/Light.md).[getDescendants](../classes/Light.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:662

___

### getEngine

▸ **getEngine**(): [`Engine`](../classes/Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](../classes/Engine.md)

a Engine

#### Inherited from

[Light](../classes/Light.md).[getEngine](../classes/Light.md#getengine)

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
| `predicate` | [`Nullable`](../modules.md#nullable)(`abstractMesh`: [`AbstractMesh`](../classes/AbstractMesh.md)) => `boolean` | `null` | defines a callback function that can be customize to filter what meshes should be included in the list used to compute the bounding vectors |

#### Returns

`Object`

the new bounding vectors

| Name | Type |
| :------ | :------ |
| `max` | [`Vector3`](../classes/Vector3.md) |
| `min` | [`Vector3`](../classes/Vector3.md) |

#### Inherited from

[Light](../classes/Light.md).[getHierarchyBoundingVectors](../classes/Light.md#gethierarchyboundingvectors)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:933

___

### getScaledIntensity

▸ **getScaledIntensity**(): `number`

Returns the intensity scaled by the Photometric Scale according to the light type and intensity mode.

#### Returns

`number`

the scaled intensity in intensity mode unit

#### Inherited from

[Light](../classes/Light.md).[getScaledIntensity](../classes/Light.md#getscaledintensity)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:577

___

### getScene

▸ **getScene**(): [`Scene`](../classes/Scene.md)

Gets the scene the light belongs to.

#### Returns

[`Scene`](../classes/Scene.md)

The scene

#### Overrides

[Light](../classes/Light.md).[getScene](../classes/Light.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:57

___

### getShadowDirection

▸ **getShadowDirection**(`faceIndex?`): [`Vector3`](../classes/Vector3.md)

Get the direction to use to render the shadow map. In case of cube texture, the face index can be passed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `faceIndex?` | `number` | The index of the face we are computed the direction to generate shadow |

#### Returns

[`Vector3`](../classes/Vector3.md)

The set direction in 2d mode otherwise the direction to the cubemap face if needCube() is true

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:102

___

### getShadowGenerator

▸ **getShadowGenerator**(): [`Nullable`](../modules.md#nullable)[`IShadowGenerator`](IShadowGenerator.md)

Returns the Light associated shadow generator if any.

#### Returns

[`Nullable`](../modules.md#nullable)[`IShadowGenerator`](IShadowGenerator.md)

the associated shadow generator.

#### Inherited from

[Light](../classes/Light.md).[getShadowGenerator](../classes/Light.md#getshadowgenerator)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:490

___

### getTypeID

▸ **getTypeID**(): `number`

Returns the light type ID (integer).

#### Returns

`number`

The light Type id as a constant defines in Light.LIGHTTYPEID_x

#### Inherited from

[Light](../classes/Light.md).[getTypeID](../classes/Light.md#gettypeid)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:569

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](../classes/Matrix.md)

Returns the latest update of the World matrix

#### Returns

[`Matrix`](../classes/Matrix.md)

a Matrix

#### Inherited from

[Light](../classes/Light.md).[getWorldMatrix](../classes/Light.md#getworldmatrix)

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
| `ancestor` | [`Node`](../classes/Node.md) | defines the parent node to inspect |

#### Returns

`boolean`

a boolean indicating if this node is a descendant of the given node

#### Inherited from

[Light](../classes/Light.md).[isDescendantOf](../classes/Light.md#isdescendantof)

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

[Light](../classes/Light.md).[isDisposed](../classes/Light.md#isdisposed)

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

[Light](../classes/Light.md).[isEnabled](../classes/Light.md#isenabled)

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

[Light](../classes/Light.md).[isReady](../classes/Light.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:548

___

### markAsDirty

▸ **markAsDirty**(`property?`): [`Node`](../classes/Node.md)

Flag the  node as dirty (Forcing it to update everything)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property?` | `string` | helps children apply precise "dirtyfication" |

#### Returns

[`Node`](../classes/Node.md)

this node

#### Inherited from

[Light](../classes/Light.md).[markAsDirty](../classes/Light.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:557

___

### needCube

▸ **needCube**(): `boolean`

Returns whether or not the shadow generation require a cube texture or a 2d texture.

#### Returns

`boolean`

true if a cube texture needs to be use

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:84

___

### needProjectionMatrixCompute

▸ **needProjectionMatrixCompute**(): `boolean`

Detects if the projection matrix requires to be recomputed this frame.

#### Returns

`boolean`

true if it requires to be recomputed otherwise, false.

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:90

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

#### Inherited from

[Light](../classes/Light.md).[prepareLightSpecificDefines](../classes/Light.md#preparelightspecificdefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:886

___

### removeBehavior

▸ **removeBehavior**(`behavior`): [`Node`](../classes/Node.md)

Remove an attached behavior

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `behavior` | [`Behavior`](Behavior.md)[`Node`](../classes/Node.md) | defines the behavior to attach |

#### Returns

[`Node`](../classes/Node.md)

the current Node

#### Inherited from

[Light](../classes/Light.md).[removeBehavior](../classes/Light.md#removebehavior)

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

[Light](../classes/Light.md).[serialize](../classes/Light.md#serialize)

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

[Light](../classes/Light.md).[serializeAnimationRanges](../classes/Light.md#serializeanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:847

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

[Light](../classes/Light.md).[setEnabled](../classes/Light.md#setenabled)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:480

___

### setShadowProjectionMatrix

▸ **setShadowProjectionMatrix**(`matrix`, `viewMatrix`, `renderList`): [`IShadowLight`](IShadowLight.md)

Sets the shadow projection matrix in parameter to the generated projection matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](../classes/Matrix.md) | The matrix to updated with the projection information |
| `viewMatrix` | [`Matrix`](../classes/Matrix.md) | The transform matrix of the light |
| `renderList` | [`AbstractMesh`](../classes/AbstractMesh.md)[] | The list of mesh to render in the map |

#### Returns

[`IShadowLight`](IShadowLight.md)

The current light

#### Defined in

https://github.com/babylon.js/core/src/Lights/shadowLight.ts:72

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

[Light](../classes/Light.md).[toString](../classes/Light.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:457

___

### transferTexturesToEffect

▸ **transferTexturesToEffect**(`effect`, `lightIndex`): [`Light`](../classes/Light.md)

Sets the passed Effect "effect" with the Light textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](../classes/Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`Light`](../classes/Light.md)

The light

#### Inherited from

[Light](../classes/Light.md).[transferTexturesToEffect](../classes/Light.md#transfertexturestoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:378

___

### transferToEffect

▸ `Abstract` **transferToEffect**(`effect`, `lightIndex`): [`Light`](../classes/Light.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](../classes/Effect.md) | The effect to update |
| `lightIndex` | `string` | The index of the light in the effect to update |

#### Returns

[`Light`](../classes/Light.md)

The light

#### Inherited from

[Light](../classes/Light.md).[transferToEffect](../classes/Light.md#transfertoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:369

___

### transferToNodeMaterialEffect

▸ `Abstract` **transferToNodeMaterialEffect**(`effect`, `lightDataUniformName`): [`Light`](../classes/Light.md)

Sets the passed Effect "effect" with the Light information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](../classes/Effect.md) | The effect to update |
| `lightDataUniformName` | `string` | The uniform used to store light data (position or direction) |

#### Returns

[`Light`](../classes/Light.md)

The light

#### Inherited from

[Light](../classes/Light.md).[transferToNodeMaterialEffect](../classes/Light.md#transfertonodematerialeffect)

#### Defined in

https://github.com/babylon.js/core/src/Lights/light.ts:439

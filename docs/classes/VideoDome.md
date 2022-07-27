[@dev/core](../README.md) / [Exports](../modules.md) / VideoDome

# Class: VideoDome

Display a 360/180 degree video on an approximately spherical surface, useful for VR applications or skyboxes.
As a subclass of TransformNode, this allow parenting to the camera or multiple videos with different locations in the scene.
This class achieves its effect with a VideoTexture and a correctly configured BackgroundMaterial on an inverted sphere.
Potential additions to this helper include zoom and and non-infinite distance rendering effects.

## Hierarchy

- `TextureDome`[`VideoTexture`](VideoTexture.md)

  ↳ **`VideoDome`**

## Table of contents

### Constructors

- [constructor](VideoDome.md#constructor)

### Properties

- [\_isDirty](VideoDome.md#_isdirty)
- [\_isWorldMatrixFrozen](VideoDome.md#_isworldmatrixfrozen)
- [\_material](VideoDome.md#_material)
- [\_mesh](VideoDome.md#_mesh)
- [\_parentNode](VideoDome.md#_parentnode)
- [\_pointerObserver](VideoDome.md#_pointerobserver)
- [\_ranges](VideoDome.md#_ranges)
- [\_scaling](VideoDome.md#_scaling)
- [\_texture](VideoDome.md#_texture)
- [\_textureMode](VideoDome.md#_texturemode)
- [\_textureObserver](VideoDome.md#_textureobserver)
- [\_useDirectMapping](VideoDome.md#_usedirectmapping)
- [animations](VideoDome.md#animations)
- [id](VideoDome.md#id)
- [ignoreNonUniformScaling](VideoDome.md#ignorenonuniformscaling)
- [inspectableCustomProperties](VideoDome.md#inspectablecustomproperties)
- [metadata](VideoDome.md#metadata)
- [name](VideoDome.md#name)
- [onAfterWorldMatrixUpdateObservable](VideoDome.md#onafterworldmatrixupdateobservable)
- [onDisposeObservable](VideoDome.md#ondisposeobservable)
- [onError](VideoDome.md#onerror)
- [onLoadErrorObservable](VideoDome.md#onloaderrorobservable)
- [onLoadObservable](VideoDome.md#onloadobservable)
- [onReady](VideoDome.md#onready)
- [reIntegrateRotationIntoRotationQuaternion](VideoDome.md#reintegraterotationintorotationquaternion)
- [reservedDataStore](VideoDome.md#reserveddatastore)
- [scalingDeterminant](VideoDome.md#scalingdeterminant)
- [state](VideoDome.md#state)
- [uniqueId](VideoDome.md#uniqueid)
- [BILLBOARDMODE\_ALL](VideoDome.md#billboardmode_all)
- [BILLBOARDMODE\_NONE](VideoDome.md#billboardmode_none)
- [BILLBOARDMODE\_USE\_POSITION](VideoDome.md#billboardmode_use_position)
- [BILLBOARDMODE\_X](VideoDome.md#billboardmode_x)
- [BILLBOARDMODE\_Y](VideoDome.md#billboardmode_y)
- [BILLBOARDMODE\_Z](VideoDome.md#billboardmode_z)
- [MODE\_MONOSCOPIC](VideoDome.md#mode_monoscopic)
- [MODE\_SIDEBYSIDE](VideoDome.md#mode_sidebyside)
- [MODE\_TOPBOTTOM](VideoDome.md#mode_topbottom)

### Accessors

- [absolutePosition](VideoDome.md#absoluteposition)
- [absoluteRotationQuaternion](VideoDome.md#absoluterotationquaternion)
- [absoluteScaling](VideoDome.md#absolutescaling)
- [animationPropertiesOverride](VideoDome.md#animationpropertiesoverride)
- [behaviors](VideoDome.md#behaviors)
- [billboardMode](VideoDome.md#billboardmode)
- [crossEye](VideoDome.md#crosseye)
- [doNotSerialize](VideoDome.md#donotserialize)
- [forward](VideoDome.md#forward)
- [fovMultiplier](VideoDome.md#fovmultiplier)
- [halfDome](VideoDome.md#halfdome)
- [infiniteDistance](VideoDome.md#infinitedistance)
- [isWorldMatrixFrozen](VideoDome.md#isworldmatrixfrozen)
- [material](VideoDome.md#material)
- [mesh](VideoDome.md#mesh)
- [nonUniformScaling](VideoDome.md#nonuniformscaling)
- [onClonedObservable](VideoDome.md#onclonedobservable)
- [onDispose](VideoDome.md#ondispose)
- [onEnabledStateChangedObservable](VideoDome.md#onenabledstatechangedobservable)
- [parent](VideoDome.md#parent)
- [position](VideoDome.md#position)
- [preserveParentRotationForBillboard](VideoDome.md#preserveparentrotationforbillboard)
- [right](VideoDome.md#right)
- [rotation](VideoDome.md#rotation)
- [rotationQuaternion](VideoDome.md#rotationquaternion)
- [scaling](VideoDome.md#scaling)
- [texture](VideoDome.md#texture)
- [textureMode](VideoDome.md#texturemode)
- [up](VideoDome.md#up)
- [videoMode](VideoDome.md#videomode)
- [videoTexture](VideoDome.md#videotexture)
- [worldMatrixFromCache](VideoDome.md#worldmatrixfromcache)

### Methods

- [\_afterComputeWorldMatrix](VideoDome.md#_aftercomputeworldmatrix)
- [\_changeTextureMode](VideoDome.md#_changetexturemode)
- [\_initTexture](VideoDome.md#_inittexture)
- [addBehavior](VideoDome.md#addbehavior)
- [addRotation](VideoDome.md#addrotation)
- [attachToBone](VideoDome.md#attachtobone)
- [beginAnimation](VideoDome.md#beginanimation)
- [clone](VideoDome.md#clone)
- [computeWorldMatrix](VideoDome.md#computeworldmatrix)
- [createAnimationRange](VideoDome.md#createanimationrange)
- [deleteAnimationRange](VideoDome.md#deleteanimationrange)
- [detachFromBone](VideoDome.md#detachfrombone)
- [dispose](VideoDome.md#dispose)
- [freezeWorldMatrix](VideoDome.md#freezeworldmatrix)
- [getAbsolutePivotPoint](VideoDome.md#getabsolutepivotpoint)
- [getAbsolutePivotPointToRef](VideoDome.md#getabsolutepivotpointtoref)
- [getAbsolutePosition](VideoDome.md#getabsoluteposition)
- [getAnimationByName](VideoDome.md#getanimationbyname)
- [getAnimationRange](VideoDome.md#getanimationrange)
- [getAnimationRanges](VideoDome.md#getanimationranges)
- [getBehaviorByName](VideoDome.md#getbehaviorbyname)
- [getChildMeshes](VideoDome.md#getchildmeshes)
- [getChildTransformNodes](VideoDome.md#getchildtransformnodes)
- [getChildren](VideoDome.md#getchildren)
- [getClassName](VideoDome.md#getclassname)
- [getDescendants](VideoDome.md#getdescendants)
- [getDirection](VideoDome.md#getdirection)
- [getDirectionToRef](VideoDome.md#getdirectiontoref)
- [getDistanceToCamera](VideoDome.md#getdistancetocamera)
- [getEngine](VideoDome.md#getengine)
- [getHierarchyBoundingVectors](VideoDome.md#gethierarchyboundingvectors)
- [getPivotMatrix](VideoDome.md#getpivotmatrix)
- [getPivotPoint](VideoDome.md#getpivotpoint)
- [getPivotPointToRef](VideoDome.md#getpivotpointtoref)
- [getPoseMatrix](VideoDome.md#getposematrix)
- [getPositionExpressedInLocalSpace](VideoDome.md#getpositionexpressedinlocalspace)
- [getPositionInCameraSpace](VideoDome.md#getpositionincameraspace)
- [getScene](VideoDome.md#getscene)
- [getWorldMatrix](VideoDome.md#getworldmatrix)
- [instantiateHierarchy](VideoDome.md#instantiatehierarchy)
- [isDescendantOf](VideoDome.md#isdescendantof)
- [isDisposed](VideoDome.md#isdisposed)
- [isEnabled](VideoDome.md#isenabled)
- [isReady](VideoDome.md#isready)
- [isUsingPivotMatrix](VideoDome.md#isusingpivotmatrix)
- [locallyTranslate](VideoDome.md#locallytranslate)
- [lookAt](VideoDome.md#lookat)
- [markAsDirty](VideoDome.md#markasdirty)
- [normalizeToUnitCube](VideoDome.md#normalizetounitcube)
- [registerAfterWorldMatrixUpdate](VideoDome.md#registerafterworldmatrixupdate)
- [removeBehavior](VideoDome.md#removebehavior)
- [resetLocalMatrix](VideoDome.md#resetlocalmatrix)
- [rotate](VideoDome.md#rotate)
- [rotateAround](VideoDome.md#rotatearound)
- [serialize](VideoDome.md#serialize)
- [serializeAnimationRanges](VideoDome.md#serializeanimationranges)
- [setAbsolutePosition](VideoDome.md#setabsoluteposition)
- [setDirection](VideoDome.md#setdirection)
- [setEnabled](VideoDome.md#setenabled)
- [setParent](VideoDome.md#setparent)
- [setPivotMatrix](VideoDome.md#setpivotmatrix)
- [setPivotPoint](VideoDome.md#setpivotpoint)
- [setPositionWithLocalVector](VideoDome.md#setpositionwithlocalvector)
- [setPreTransformMatrix](VideoDome.md#setpretransformmatrix)
- [translate](VideoDome.md#translate)
- [unfreezeWorldMatrix](VideoDome.md#unfreezeworldmatrix)
- [unregisterAfterWorldMatrixUpdate](VideoDome.md#unregisterafterworldmatrixupdate)
- [updatePoseMatrix](VideoDome.md#updateposematrix)
- [AddNodeConstructor](VideoDome.md#addnodeconstructor)
- [Construct](VideoDome.md#construct)
- [Parse](VideoDome.md#parse)
- [ParseAnimationRanges](VideoDome.md#parseanimationranges)

## Constructors

### constructor

• **new VideoDome**(`name`, `textureUrlOrElement`, `options`, `scene`, `onError?`)

Create an instance of this class and pass through the parameters to the relevant classes- Texture, StandardMaterial, and Mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Element's name, child elements will append suffixes for their own names. |
| `textureUrlOrElement` | `string` \| `string`[] \| `HTMLVideoElement` | `undefined` | defines the url(s) or the (video) HTML element to use |
| `options` | `Object` | `undefined` | An object containing optional or exposed sub element properties |
| `options.autoPlay?` | `boolean` | `undefined` |  |
| `options.clickToPlay?` | `boolean` | `undefined` |  |
| `options.crossEyeMode?` | `boolean` | `undefined` |  |
| `options.faceForward?` | `boolean` | `undefined` |  |
| `options.generateMipMaps?` | `boolean` | `undefined` |  |
| `options.halfDomeMode?` | `boolean` | `undefined` |  |
| `options.loop?` | `boolean` | `undefined` |  |
| `options.mesh?` | [`Mesh`](Mesh.md) | `undefined` |  |
| `options.poster?` | `string` | `undefined` |  |
| `options.resolution?` | `number` | `undefined` |  |
| `options.size?` | `number` | `undefined` |  |
| `options.useDirectMapping?` | `boolean` | `undefined` |  |
| `scene` | [`Scene`](Scene.md) | `undefined` |  |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` |  |

#### Inherited from

TextureDomeVideoTexture.constructor

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:199

## Properties

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

TextureDome.\_isDirty

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_isWorldMatrixFrozen

• `Protected` **\_isWorldMatrixFrozen**: `boolean` = `false`

#### Inherited from

TextureDome.\_isWorldMatrixFrozen

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:161

___

### \_material

• `Protected` **\_material**: [`BackgroundMaterial`](BackgroundMaterial.md)

The skybox material

#### Inherited from

TextureDome.\_material

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:75

___

### \_mesh

• `Protected` **\_mesh**: [`Mesh`](Mesh.md)

The surface used for the dome

#### Inherited from

TextureDome.\_mesh

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:80

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

TextureDome.\_parentNode

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:51

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

TextureDome.\_ranges

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_scaling

• `Protected` **\_scaling**: [`Vector3`](Vector3.md)

#### Inherited from

TextureDome.\_scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:62

___

### \_texture

• `Protected` **\_texture**: [`VideoTexture`](VideoTexture.md)

The texture being displayed on the sphere

#### Inherited from

TextureDome.\_texture

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:43

___

### \_textureMode

• `Protected` **\_textureMode**: `number` = `TextureDome.MODE_MONOSCOPIC`

#### Inherited from

TextureDome.\_textureMode

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:104

___

### \_textureObserver

• `Private` **\_textureObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Texture`](Texture.md)

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:52

___

### \_useDirectMapping

• `Protected` **\_useDirectMapping**: `boolean` = `false`

#### Inherited from

TextureDome.\_useDirectMapping

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:38

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

TextureDome.animations

#### Defined in

packages/dev/core/src/node.ts:153

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

TextureDome.id

#### Defined in

packages/dev/core/src/node.ts:97

___

### ignoreNonUniformScaling

• **ignoreNonUniformScaling**: `boolean` = `false`

Gets or sets a boolean indicating that non uniform scaling (when at least one component is different from others) should be ignored.
By default the system will update normals to compensate

#### Inherited from

TextureDome.ignoreNonUniformScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:138

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

TextureDome.inspectableCustomProperties

#### Defined in

packages/dev/core/src/node.ts:126

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

TextureDome.metadata

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

TextureDome.name

#### Defined in

packages/dev/core/src/node.ts:91

___

### onAfterWorldMatrixUpdateObservable

• **onAfterWorldMatrixUpdateObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered after the world matrix is updated

#### Inherited from

TextureDome.onAfterWorldMatrixUpdateObservable

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:169

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

TextureDome.onDisposeObservable

#### Defined in

packages/dev/core/src/node.ts:300

___

### onError

• `Protected` **onError**: [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` = `null`

#### Inherited from

TextureDome.onError

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:218

___

### onLoadErrorObservable

• **onLoadErrorObservable**: [`Observable`](Observable.md)`string`

Observable raised when an error occurred while loading the texture

#### Inherited from

TextureDome.onLoadErrorObservable

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:173

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)`void`

Observable raised when the texture finished loading

#### Inherited from

TextureDome.onLoadObservable

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:177

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

TextureDome.onReady

#### Defined in

packages/dev/core/src/node.ts:159

___

### reIntegrateRotationIntoRotationQuaternion

• **reIntegrateRotationIntoRotationQuaternion**: `boolean` = `false`

Gets or sets a boolean indicating that even if rotationQuaternion is defined, you can keep updating rotation property and Babylon.js will just mix both

#### Inherited from

TextureDome.reIntegrateRotationIntoRotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:144

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

TextureDome.reservedDataStore

#### Defined in

packages/dev/core/src/node.ts:120

___

### scalingDeterminant

• **scalingDeterminant**: `number` = `1`

Multiplication factor on scale x/y/z when computing the world matrix. Eg. for a 1x1x1 cube setting this to 2 will make it a 2x2x2 cube

#### Inherited from

TextureDome.scalingDeterminant

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:113

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

TextureDome.state

#### Defined in

packages/dev/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

TextureDome.uniqueId

#### Defined in

packages/dev/core/src/node.ts:103

___

### BILLBOARDMODE\_ALL

▪ `Static` **BILLBOARDMODE\_ALL**: `number` = `7`

Object will rotate to face the camera

#### Inherited from

TextureDome.BILLBOARDMODE\_ALL

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:37

___

### BILLBOARDMODE\_NONE

▪ `Static` **BILLBOARDMODE\_NONE**: `number` = `0`

Object will not rotate to face the camera

#### Inherited from

TextureDome.BILLBOARDMODE\_NONE

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:21

___

### BILLBOARDMODE\_USE\_POSITION

▪ `Static` **BILLBOARDMODE\_USE\_POSITION**: `number` = `128`

Object will rotate to face the camera's position instead of orientation

#### Inherited from

TextureDome.BILLBOARDMODE\_USE\_POSITION

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:41

___

### BILLBOARDMODE\_X

▪ `Static` **BILLBOARDMODE\_X**: `number` = `1`

Object will rotate to face the camera but only on the x axis

#### Inherited from

TextureDome.BILLBOARDMODE\_X

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:25

___

### BILLBOARDMODE\_Y

▪ `Static` **BILLBOARDMODE\_Y**: `number` = `2`

Object will rotate to face the camera but only on the y axis

#### Inherited from

TextureDome.BILLBOARDMODE\_Y

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:29

___

### BILLBOARDMODE\_Z

▪ `Static` **BILLBOARDMODE\_Z**: `number` = `4`

Object will rotate to face the camera but only on the z axis

#### Inherited from

TextureDome.BILLBOARDMODE\_Z

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:33

___

### MODE\_MONOSCOPIC

▪ `Static` `Readonly` **MODE\_MONOSCOPIC**: ``0``

Define the video source as a Monoscopic panoramic 360 video.

#### Overrides

TextureDome.MODE\_MONOSCOPIC

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:21

___

### MODE\_SIDEBYSIDE

▪ `Static` `Readonly` **MODE\_SIDEBYSIDE**: ``2``

Define the video source as a Stereoscopic Side by Side panoramic 360 video.

#### Overrides

TextureDome.MODE\_SIDEBYSIDE

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:29

___

### MODE\_TOPBOTTOM

▪ `Static` `Readonly` **MODE\_TOPBOTTOM**: ``1``

Define the video source as a Stereoscopic TopBottom/OverUnder panoramic 360 video.

#### Overrides

TextureDome.MODE\_TOPBOTTOM

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:25

## Accessors

### absolutePosition

• `get` **absolutePosition**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute position.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.absolutePosition

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:344

___

### absoluteRotationQuaternion

• `get` **absoluteRotationQuaternion**(): [`Quaternion`](Quaternion.md)

Returns the current mesh absolute rotation.
Returns a Quaternion.

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

TextureDome.absoluteRotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:361

___

### absoluteScaling

• `get` **absoluteScaling**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute scaling.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.absoluteScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:352

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

TextureDome.animationPropertiesOverride

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

TextureDome.animationPropertiesOverride

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

TextureDome.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### billboardMode

• `get` **billboardMode**(): `number`

Gets or sets the billboard mode. Default is 0.

| Value | Type | Description |
| --- | --- | --- |
| 0 | BILLBOARDMODE_NONE |  |
| 1 | BILLBOARDMODE_X |  |
| 2 | BILLBOARDMODE_Y |  |
| 4 | BILLBOARDMODE_Z |  |
| 7 | BILLBOARDMODE_ALL |  |

#### Returns

`number`

#### Inherited from

TextureDome.billboardMode

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:82

• `set` **billboardMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TextureDome.billboardMode

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:86

___

### crossEye

• `get` **crossEye**(): `boolean`

Is it a cross-eye texture?

#### Returns

`boolean`

#### Inherited from

TextureDome.crossEye

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:155

• `set` **crossEye**(`enabled`): `void`

Set the cross-eye mode. If set, images that can be seen when crossing eyes will render correctly

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Inherited from

TextureDome.crossEye

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:147

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

TextureDome.doNotSerialize

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

TextureDome.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### forward

• `get` **forward**(): [`Vector3`](Vector3.md)

The forward direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.forward

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:253

___

### fovMultiplier

• `get` **fovMultiplier**(): `number`

The current fov(field of view) multiplier, 0.0 - 2.0. Defaults to 1.0. Lower values "zoom in" and higher values "zoom out".
Also see the options.resolution property.

#### Returns

`number`

#### Inherited from

TextureDome.fovMultiplier

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:97

• `set` **fovMultiplier**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TextureDome.fovMultiplier

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:100

___

### halfDome

• `get` **halfDome**(): `boolean`

Is it a 180 degrees dome (half dome) or 360 texture (full dome)

#### Returns

`boolean`

#### Inherited from

TextureDome.halfDome

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:131

• `set` **halfDome**(`enabled`): `void`

Set the halfDome mode. If set, only the front (180 degrees) will be displayed and the back will be blacked out.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Inherited from

TextureDome.halfDome

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:138

___

### infiniteDistance

• `get` **infiniteDistance**(): `boolean`

Gets or sets the distance of the object to max, often used by skybox

#### Returns

`boolean`

#### Inherited from

TextureDome.infiniteDistance

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:121

• `set` **infiniteDistance**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

TextureDome.infiniteDistance

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:125

___

### isWorldMatrixFrozen

• `get` **isWorldMatrixFrozen**(): `boolean`

True if the World matrix has been frozen.

#### Returns

`boolean`

#### Inherited from

TextureDome.isWorldMatrixFrozen

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:476

___

### material

• `get` **material**(): [`BackgroundMaterial`](BackgroundMaterial.md)

The background material of this dome.

#### Returns

[`BackgroundMaterial`](BackgroundMaterial.md)

#### Inherited from

TextureDome.material

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:162

___

### mesh

• `get` **mesh**(): [`Mesh`](Mesh.md)

Gets the mesh used for the dome.

#### Returns

[`Mesh`](Mesh.md)

#### Inherited from

TextureDome.mesh

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:84

___

### nonUniformScaling

• `get` **nonUniformScaling**(): `boolean`

True if the scaling property of this object is non uniform eg. (1,2,1)

#### Returns

`boolean`

#### Inherited from

TextureDome.nonUniformScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:799

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

TextureDome.onClonedObservable

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

TextureDome.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

TextureDome.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

TextureDome.parent

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

TextureDome.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or set the node position (default is (0.0, 0.0, 0.0))

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.position

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:190

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TextureDome.position

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:194

___

### preserveParentRotationForBillboard

• `get` **preserveParentRotationForBillboard**(): `boolean`

Gets or sets a boolean indicating that parent rotation should be preserved when using billboards.
This could be useful for glTF objects where parent rotation helps converting from right handed to left handed

#### Returns

`boolean`

#### Inherited from

TextureDome.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:98

• `set` **preserveParentRotationForBillboard**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

TextureDome.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:102

___

### right

• `get` **right**(): [`Vector3`](Vector3.md)

The right direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.right

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:269

___

### rotation

• `get` **rotation**(): [`Vector3`](Vector3.md)

Gets or sets the rotation property : a Vector3 defining the rotation value in radians around each local axis X, Y, Z  (default is (0.0, 0.0, 0.0)).
If rotation quaternion is set, this Vector3 will be ignored and copy from the quaternion

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.rotation

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:211

• `set` **rotation**(`newRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newRotation` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TextureDome.rotation

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:215

___

### rotationQuaternion

• `get` **rotationQuaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Gets or sets the rotation Quaternion property : this a Quaternion object defining the node rotation by using a unit quaternion (undefined by default, but can be null).
If set, only the rotationQuaternion is then used to compute the node rotation (ie. node.rotation will be ignored)

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Inherited from

TextureDome.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:237

• `set` **rotationQuaternion**(`quaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `quaternion` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Inherited from

TextureDome.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:241

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets the scaling property : a Vector3 defining the node scaling along each local axis X, Y, Z (default is (1.0, 1.0, 1.0)).

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:224

• `set` **scaling**(`newScaling`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newScaling` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TextureDome.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:228

___

### texture

• `get` **texture**(): `T`

Gets the texture being displayed on the sphere

#### Returns

`T`

#### Inherited from

TextureDome.texture

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:48

• `set` **texture**(`newTexture`): `void`

Sets the texture being displayed on the sphere

#### Parameters

| Name | Type |
| :------ | :------ |
| `newTexture` | `T` |

#### Returns

`void`

#### Inherited from

TextureDome.texture

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:55

___

### textureMode

• `get` **textureMode**(): `number`

Gets or set the current texture mode for the texture. It can be:
* TextureDome.MODE_MONOSCOPIC : Define the texture source as a Monoscopic panoramic 360.
* TextureDome.MODE_TOPBOTTOM  : Define the texture source as a Stereoscopic TopBottom/OverUnder panoramic 360.
* TextureDome.MODE_SIDEBYSIDE : Define the texture source as a Stereoscopic Side by Side panoramic 360.

#### Returns

`number`

#### Inherited from

TextureDome.textureMode

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:111

• `set` **textureMode**(`value`): `void`

Sets the current texture mode for the texture. It can be:
* TextureDome.MODE_MONOSCOPIC : Define the texture source as a Monoscopic panoramic 360.
* TextureDome.MODE_TOPBOTTOM  : Define the texture source as a Stereoscopic TopBottom/OverUnder panoramic 360.
* TextureDome.MODE_SIDEBYSIDE : Define the texture source as a Stereoscopic Side by Side panoramic 360.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TextureDome.textureMode

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:120

___

### up

• `get` **up**(): [`Vector3`](Vector3.md)

The up direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TextureDome.up

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:261

___

### videoMode

• `get` **videoMode**(): `number`

Get the video mode of this dome

#### Returns

`number`

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:40

• `set` **videoMode**(`value`): `void`

Set the video mode of this dome.

**`See`**

textureMode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:47

___

### videoTexture

• `get` **videoTexture**(): [`VideoTexture`](VideoTexture.md)

Get the video texture associated with this video dome

#### Returns

[`VideoTexture`](VideoTexture.md)

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:34

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

TextureDome.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

## Methods

### \_afterComputeWorldMatrix

▸ `Protected` **_afterComputeWorldMatrix**(): `void`

#### Returns

`void`

#### Inherited from

TextureDome.\_afterComputeWorldMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1275

___

### \_changeTextureMode

▸ `Protected` **_changeTextureMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TextureDome.\_changeTextureMode

#### Defined in

packages/dev/core/src/Helpers/textureDome.ts:293

___

### \_initTexture

▸ `Protected` **_initTexture**(`urlsOrElement`, `scene`, `options`): [`VideoTexture`](VideoTexture.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlsOrElement` | `string` \| `string`[] \| `HTMLVideoElement` |
| `scene` | [`Scene`](Scene.md) |
| `options` | `any` |

#### Returns

[`VideoTexture`](VideoTexture.md)

#### Overrides

TextureDome.\_initTexture

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:54

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

TextureDome.addBehavior

#### Defined in

packages/dev/core/src/node.ts:366

___

### addRotation

▸ **addRotation**(`x`, `y`, `z`): [`TransformNode`](TransformNode.md)

Adds a rotation step to the mesh current rotation.
x, y, z are Euler angles expressed in radians.
This methods updates the current mesh rotation, either mesh.rotation, either mesh.rotationQuaternion if it's set.
This means this rotation is made in the mesh local space only.
It's useful to set a custom rotation order different from the BJS standard one YXZ.
Example : this rotates the mesh first around its local X axis, then around its local Z axis, finally around its local Y axis.
```javascript
mesh.addRotation(x1, 0, 0).addRotation(0, 0, z2).addRotation(0, 0, y3);
```
Note that `addRotation()` accumulates the passed rotation values to the current ones and computes the .rotation or .rotationQuaternion updated values.
Under the hood, only quaternions are used. So it's a little faster is you use .rotationQuaternion because it doesn't need to translate them back to Euler angles.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Rotation to add |
| `y` | `number` | Rotation to add |
| `z` | `number` | Rotation to add |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.addRotation

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:973

___

### attachToBone

▸ **attachToBone**(`bone`, `affectedTransformNode`): [`TransformNode`](TransformNode.md)

Attach the current TransformNode to another TransformNode associated with a bone

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bone` | [`Bone`](Bone.md) | Bone affecting the TransformNode |
| `affectedTransformNode` | [`TransformNode`](TransformNode.md) | TransformNode associated with the bone |

#### Returns

[`TransformNode`](TransformNode.md)

this object

#### Inherited from

TextureDome.attachToBone

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:822

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

TextureDome.beginAnimation

#### Defined in

packages/dev/core/src/node.ts:833

___

### clone

▸ **clone**(`name`, `newParent`, `doNotCloneChildren?`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Clone the current transform node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the new clone |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | New parent for the clone |
| `doNotCloneChildren?` | `boolean` | Do not clone children hierarchy |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

the new transform node

#### Inherited from

TextureDome.clone

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1330

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

TextureDome.computeWorldMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1002

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

TextureDome.createAnimationRange

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

TextureDome.deleteAnimationRange

#### Defined in

packages/dev/core/src/node.ts:794

___

### detachFromBone

▸ **detachFromBone**(`resetToPreviousParent?`): [`TransformNode`](TransformNode.md)

Detach the transform node if its associated with a bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `resetToPreviousParent` | `boolean` | `false` | Indicates if the parent that was in effect when attachToBone was called should be set back or if we should set parent to null instead (defaults to the latter) |

#### Returns

[`TransformNode`](TransformNode.md)

this object

#### Inherited from

TextureDome.detachFromBone

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:840

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

#### Overrides

TextureDome.dispose

#### Defined in

packages/dev/core/src/Helpers/videoDome.ts:84

___

### freezeWorldMatrix

▸ **freezeWorldMatrix**(`newWorldMatrix?`, `decompose?`): [`TransformNode`](TransformNode.md)

Prevents the World matrix to be computed any longer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newWorldMatrix` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `null` | defines an optional matrix to use as world matrix |
| `decompose` | `boolean` | `false` | defines whether to decompose the given newWorldMatrix or directly assign |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.freezeWorldMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:442

___

### getAbsolutePivotPoint

▸ **getAbsolutePivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point World coordinates.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 set with the mesh pivot point World coordinates.

#### Inherited from

TextureDome.getAbsolutePivotPoint

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:707

___

### getAbsolutePivotPointToRef

▸ **getAbsolutePivotPointToRef**(`result`): [`TransformNode`](TransformNode.md)

Sets the Vector3 "result" coordinates with the mesh pivot point World coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | vector3 to store the result |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

TextureDome.getAbsolutePivotPointToRef

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:718

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns the mesh absolute position in the World.

#### Returns

[`Vector3`](Vector3.md)

a Vector3.

#### Inherited from

TextureDome.getAbsolutePosition

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:484

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

TextureDome.getAnimationByName

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

TextureDome.getAnimationRange

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

TextureDome.getAnimationRanges

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

TextureDome.getBehaviorByName

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

TextureDome.getChildMeshes

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

TextureDome.getChildMeshes

#### Defined in

packages/dev/core/src/node.ts:692

___

### getChildTransformNodes

▸ **getChildTransformNodes**(`directDescendantsOnly?`, `predicate?`): [`TransformNode`](TransformNode.md)[]

Get all child-transformNodes of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`TransformNode`](TransformNode.md)[]

an array of TransformNode

#### Inherited from

TextureDome.getChildTransformNodes

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1414

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

TextureDome.getChildren

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

TextureDome.getChildren

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"TransformNode" string

#### Inherited from

TextureDome.getClassName

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:183

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

TextureDome.getDescendants

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

TextureDome.getDescendants

#### Defined in

packages/dev/core/src/node.ts:662

___

### getDirection

▸ **getDirection**(`localAxis`): [`Vector3`](Vector3.md)

Returns a new Vector3 that is the localAxis, expressed in the mesh local space, rotated like the mesh.
This Vector3 is expressed in the World space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | axis to rotate |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 that is the localAxis, expressed in the mesh local space, rotated like the mesh.

#### Inherited from

TextureDome.getDirection

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:616

___

### getDirectionToRef

▸ **getDirectionToRef**(`localAxis`, `result`): [`TransformNode`](TransformNode.md)

Sets the Vector3 "result" as the rotated Vector3 "localAxis" in the same rotation than the mesh.
localAxis is expressed in the mesh local space.
result is computed in the World space from the mesh World matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | axis to rotate |
| `result` | [`Vector3`](Vector3.md) | the resulting transformnode |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

TextureDome.getDirectionToRef

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:632

___

### getDistanceToCamera

▸ **getDistanceToCamera**(`camera?`): `number`

Returns the distance from the mesh to the active camera

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `null` | defines the camera to use |

#### Returns

`number`

the distance

#### Inherited from

TextureDome.getDistanceToCamera

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1316

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

TextureDome.getEngine

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

TextureDome.getHierarchyBoundingVectors

#### Defined in

packages/dev/core/src/node.ts:933

___

### getPivotMatrix

▸ **getPivotMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh pivot matrix.
Default : Identity.

#### Returns

[`Matrix`](Matrix.md)

the matrix

#### Inherited from

TextureDome.getPivotMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:404

___

### getPivotPoint

▸ **getPivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point coordinates in the local space.

#### Returns

[`Vector3`](Vector3.md)

the pivot point

#### Inherited from

TextureDome.getPivotPoint

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:685

___

### getPivotPointToRef

▸ **getPivotPointToRef**(`result`): [`TransformNode`](TransformNode.md)

Sets the passed Vector3 "result" with the coordinates of the mesh pivot point in the local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | the vector3 to store the result |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

TextureDome.getPivotPointToRef

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:696

___

### getPoseMatrix

▸ **getPoseMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh Pose matrix.

#### Returns

[`Matrix`](Matrix.md)

the pose matrix

#### Inherited from

TextureDome.getPoseMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:292

___

### getPositionExpressedInLocalSpace

▸ **getPositionExpressedInLocalSpace**(): [`Vector3`](Vector3.md)

Returns the mesh position in the local space from the current World matrix values.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3.

#### Inherited from

TextureDome.getPositionExpressedInLocalSpace

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:542

___

### getPositionInCameraSpace

▸ **getPositionInCameraSpace**(`camera?`): [`Vector3`](Vector3.md)

Gets the position of the current mesh in camera space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `null` | defines the camera to use |

#### Returns

[`Vector3`](Vector3.md)

a position

#### Inherited from

TextureDome.getPositionInCameraSpace

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1303

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

TextureDome.getScene

#### Defined in

packages/dev/core/src/node.ts:344

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Returns the latest update of the World matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

TextureDome.getWorldMatrix

#### Defined in

packages/dev/core/src/node.ts:434

___

### instantiateHierarchy

▸ **instantiateHierarchy**(`newParent?`, `options?`, `onNewNodeCreated?`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Instantiate (when possible) or clone that node with its hierarchy

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newParent` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | defines the new parent to use for the instance (or clone) |
| `options?` | `Object` | `undefined` | defines options to configure how copy is done |
| `options.doNotInstantiate` | `boolean` \| (`node`: [`TransformNode`](TransformNode.md)) => `boolean` | `undefined` | defines if the model must be instantiated or just cloned |
| `onNewNodeCreated?` | (`source`: [`TransformNode`](TransformNode.md), `clone`: [`TransformNode`](TransformNode.md)) => `void` | `undefined` | defines an option callback to call when a clone or an instance is created |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

an instance (or a clone) of the current node with its hierarchy

#### Inherited from

TextureDome.instantiateHierarchy

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:416

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

TextureDome.isDescendantOf

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

TextureDome.isDisposed

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

TextureDome.isEnabled

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

TextureDome.isReady

#### Defined in

packages/dev/core/src/node.ts:548

___

### isUsingPivotMatrix

▸ **isUsingPivotMatrix**(): `boolean`

return true if a pivot has been set

#### Returns

`boolean`

true if a pivot matrix is used

#### Inherited from

TextureDome.isUsingPivotMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:203

___

### locallyTranslate

▸ **locallyTranslate**(`vector3`): [`TransformNode`](TransformNode.md)

Translates the mesh along the passed Vector3 in its local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector3` | [`Vector3`](Vector3.md) | the distance to translate in localspace |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.locallyTranslate

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:554

___

### lookAt

▸ **lookAt**(`targetPoint`, `yawCor?`, `pitchCor?`, `rollCor?`, `space?`): [`TransformNode`](TransformNode.md)

Orients a mesh towards a target point. Mesh must be drawn facing user.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `targetPoint` | [`Vector3`](Vector3.md) | `undefined` | the position (must be in same space as current mesh) to look at |
| `yawCor` | `number` | `0` | optional yaw (y-axis) correction in radians |
| `pitchCor` | `number` | `0` | optional pitch (x-axis) correction in radians |
| `rollCor` | `number` | `0` | optional roll (z-axis) correction in radians |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | the chosen space of the target |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.lookAt

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:571

___

### markAsDirty

▸ **markAsDirty**(`property?`): [`Node`](Node.md)

Flag the transform node as dirty (Forcing it to update everything)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property?` | `string` | if set to "rotation" the objects rotationQuaternion will be set to null |

#### Returns

[`Node`](Node.md)

this  node

#### Inherited from

TextureDome.markAsDirty

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:729

___

### normalizeToUnitCube

▸ **normalizeToUnitCube**(`includeDescendants?`, `ignoreRotation?`, `predicate?`): [`TransformNode`](TransformNode.md)

Uniformly scales the mesh to fit inside of a unit cube (1 X 1 X 1 units)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `includeDescendants` | `boolean` | `true` | Use the hierarchy's bounding box instead of the mesh's bounding box. Default is false |
| `ignoreRotation` | `boolean` | `false` | ignore rotation when computing the scale (ie. object will be axis aligned). Default is false |
| `predicate?` | [`Nullable`](../modules.md#nullable)(`node`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | `undefined` | predicate that is passed in to getHierarchyBoundingVectors when selecting which object should be included when scaling |

#### Returns

[`TransformNode`](TransformNode.md)

the current mesh

#### Inherited from

TextureDome.normalizeToUnitCube

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1462

___

### registerAfterWorldMatrixUpdate

▸ **registerAfterWorldMatrixUpdate**(`func`): [`TransformNode`](TransformNode.md)

If you'd like to be called back after the mesh position, rotation or scaling has been updated.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`TransformNode`](TransformNode.md)) => `void` | callback function to add |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.registerAfterWorldMatrixUpdate

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1283

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

TextureDome.removeBehavior

#### Defined in

packages/dev/core/src/node.ts:393

___

### resetLocalMatrix

▸ **resetLocalMatrix**(`independentOfChildren?`): `void`

Resets this nodeTransform's local matrix to Matrix.Identity().

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `independentOfChildren` | `boolean` | `true` | indicates if all child nodeTransform's world-space transform should be preserved. |

#### Returns

`void`

#### Inherited from

TextureDome.resetLocalMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1244

___

### rotate

▸ **rotate**(`axis`, `amount`, `space?`): [`TransformNode`](TransformNode.md)

Rotates the mesh around the axis vector for the passed angle (amount) expressed in radians, in the given space.
space (default LOCAL) can be either Space.LOCAL, either Space.WORLD.
Note that the property `rotationQuaternion` is then automatically updated and the property `rotation` is set to (0,0,0) and no longer used.
The passed axis is also normalized.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | the axis to rotate around |
| `amount` | `number` | the amount to rotate in radians |
| `space?` | [`Space`](../enums/Space.md) | Space to rotate in (Default: local) |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.rotate

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:871

___

### rotateAround

▸ **rotateAround**(`point`, `axis`, `amount`): [`TransformNode`](TransformNode.md)

Rotates the mesh around the axis vector for the passed angle (amount) expressed in radians, in world space.
Note that the property `rotationQuaternion` is then automatically updated and the property `rotation` is set to (0,0,0) and no longer used.
The passed axis is also normalized. .
Method is based on http://www.euclideanspace.com/maths/geometry/affine/aroundPoint/index.htm

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | the point to rotate around |
| `axis` | [`Vector3`](Vector3.md) | the axis to rotate around |
| `amount` | `number` | the amount to rotate in radians |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode

#### Inherited from

TextureDome.rotateAround

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:903

___

### serialize

▸ **serialize**(`currentSerializationObject?`): `any`

Serializes the objects information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentSerializationObject?` | `any` | defines the object to serialize in |

#### Returns

`any`

the serialized object

#### Inherited from

TextureDome.serialize

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1360

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

TextureDome.serializeAnimationRanges

#### Defined in

packages/dev/core/src/node.ts:847

___

### setAbsolutePosition

▸ **setAbsolutePosition**(`absolutePosition`): [`TransformNode`](TransformNode.md)

Sets the mesh absolute position in the World from a Vector3 or an Array(3).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `absolutePosition` | [`Vector3`](Vector3.md) | the absolute position to set |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.setAbsolutePosition

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:494

___

### setDirection

▸ **setDirection**(`localAxis`, `yawCor?`, `pitchCor?`, `rollCor?`): [`TransformNode`](TransformNode.md)

Sets this transform node rotation to the given local axis.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | `undefined` | the axis in local space |
| `yawCor` | `number` | `0` | optional yaw (y-axis) correction in radians |
| `pitchCor` | `number` | `0` | optional pitch (x-axis) correction in radians |
| `rollCor` | `number` | `0` | optional roll (z-axis) correction in radians |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode

#### Inherited from

TextureDome.setDirection

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:645

___

### setEnabled

▸ **setEnabled**(`value`): `void`

Set the enabled state of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | defines the new enabled state |

#### Returns

`void`

#### Inherited from

TextureDome.setEnabled

#### Defined in

packages/dev/core/src/node.ts:596

___

### setParent

▸ **setParent**(`node`, `preserveScalingSign?`): [`TransformNode`](TransformNode.md)

Defines the passed node as the parent of the current node.
The node will remain exactly where it is and its position / rotation will be updated accordingly.
Note that if the mesh has a pivot matrix / point defined it will be applied after the parent was updated.
In that case the node will not remain in the same space as it is, as the pivot will be applied.

**`See`**

https://doc.babylonjs.com/how_to/parenting

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `node` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `undefined` | the node ot set as the parent |
| `preserveScalingSign` | `boolean` | `false` | if true, keep scaling sign of child. Otherwise, scaling sign might change. |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

TextureDome.setParent

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:750

___

### setPivotMatrix

▸ **setPivotMatrix**(`matrix`, `postMultiplyPivotMatrix?`): [`TransformNode`](TransformNode.md)

Sets a new pivot matrix to the current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` | defines the new pivot matrix to use |
| `postMultiplyPivotMatrix` | `boolean` | `true` | defines if the pivot matrix must be cancelled in the world matrix. When this parameter is set to true (default), the inverse of the pivot matrix is also applied at the end to cancel the transformation effect |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

TextureDome.setPivotMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:381

___

### setPivotPoint

▸ **setPivotPoint**(`point`, `space?`): [`TransformNode`](TransformNode.md)

Sets a new pivot point to the current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | `undefined` | defines the new pivot point to use |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | defines if the point is in world or local space (local by default) |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

TextureDome.setPivotPoint

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:665

___

### setPositionWithLocalVector

▸ **setPositionWithLocalVector**(`vector3`): [`TransformNode`](TransformNode.md)

Sets the mesh position in its local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector3` | [`Vector3`](Vector3.md) | the position to set in localspace |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.setPositionWithLocalVector

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:532

___

### setPreTransformMatrix

▸ **setPreTransformMatrix**(`matrix`): [`TransformNode`](TransformNode.md)

Sets a new matrix to apply before all other transformation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | defines the transform matrix |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

TextureDome.setPreTransformMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:371

___

### translate

▸ **translate**(`axis`, `distance`, `space?`): [`TransformNode`](TransformNode.md)

Translates the mesh along the axis vector for the passed distance in the given space.
space (default LOCAL) can be either Space.LOCAL, either Space.WORLD.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | the axis to translate in |
| `distance` | `number` | the distance to translate |
| `space?` | [`Space`](../enums/Space.md) | Space to rotate in (Default: local) |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.translate

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:945

___

### unfreezeWorldMatrix

▸ **unfreezeWorldMatrix**(): [`VideoDome`](VideoDome.md)

Allows back the World matrix computation.

#### Returns

[`VideoDome`](VideoDome.md)

the TransformNode.

#### Inherited from

TextureDome.unfreezeWorldMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:467

___

### unregisterAfterWorldMatrixUpdate

▸ **unregisterAfterWorldMatrixUpdate**(`func`): [`TransformNode`](TransformNode.md)

Removes a registered callback function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`TransformNode`](TransformNode.md)) => `void` | callback function to remove |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

TextureDome.unregisterAfterWorldMatrixUpdate

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1293

___

### updatePoseMatrix

▸ **updatePoseMatrix**(`matrix`): [`TransformNode`](TransformNode.md)

Copies the parameter passed Matrix into the mesh Pose matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | the matrix to copy the pose from |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

TextureDome.updatePoseMatrix

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:279

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

TextureDome.AddNodeConstructor

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

TextureDome.Construct

#### Defined in

packages/dev/core/src/node.ts:75

___

### Parse

▸ `Static` **Parse**(`parsedTransformNode`, `scene`, `rootUrl`): [`TransformNode`](TransformNode.md)

Returns a new TransformNode object parsed from the source provided.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTransformNode` | `any` | is the source. |
| `scene` | [`Scene`](Scene.md) | the scene the object belongs to |
| `rootUrl` | `string` | is a string, it's the root URL to prefix the `delayLoadingFile` property with |

#### Returns

[`TransformNode`](TransformNode.md)

a new TransformNode object parsed from the source provided.

#### Inherited from

TextureDome.Parse

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1385

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

TextureDome.ParseAnimationRanges

#### Defined in

packages/dev/core/src/node.ts:919

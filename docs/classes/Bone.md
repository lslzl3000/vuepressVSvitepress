[@dev/core](../README.md) / [Exports](../modules.md) / Bone

# Class: Bone

Class used to store bone information

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

## Hierarchy

- [`Node`](Node.md)

  ↳ **`Bone`**

## Table of contents

### Constructors

- [constructor](Bone.md#constructor)

### Properties

- [\_absoluteTransform](Bone.md#_absolutetransform)
- [\_baseMatrix](Bone.md#_basematrix)
- [\_invertedAbsoluteTransform](Bone.md#_invertedabsolutetransform)
- [\_isDirty](Bone.md#_isdirty)
- [\_localMatrix](Bone.md#_localmatrix)
- [\_localPosition](Bone.md#_localposition)
- [\_localRotation](Bone.md#_localrotation)
- [\_localScaling](Bone.md#_localscaling)
- [\_needToCompose](Bone.md#_needtocompose)
- [\_needToDecompose](Bone.md#_needtodecompose)
- [\_parentNode](Bone.md#_parentnode)
- [\_ranges](Bone.md#_ranges)
- [\_restPose](Bone.md#_restpose)
- [\_scalingDeterminant](Bone.md#_scalingdeterminant)
- [\_skeleton](Bone.md#_skeleton)
- [\_worldTransform](Bone.md#_worldtransform)
- [animations](Bone.md#animations)
- [children](Bone.md#children)
- [id](Bone.md#id)
- [inspectableCustomProperties](Bone.md#inspectablecustomproperties)
- [length](Bone.md#length)
- [metadata](Bone.md#metadata)
- [name](Bone.md#name)
- [onDisposeObservable](Bone.md#ondisposeobservable)
- [onReady](Bone.md#onready)
- [reservedDataStore](Bone.md#reserveddatastore)
- [state](Bone.md#state)
- [uniqueId](Bone.md#uniqueid)
- [\_TmpMats](Bone.md#_tmpmats)
- [\_TmpQuat](Bone.md#_tmpquat)
- [\_TmpVecs](Bone.md#_tmpvecs)

### Accessors

- [animationPropertiesOverride](Bone.md#animationpropertiesoverride)
- [behaviors](Bone.md#behaviors)
- [doNotSerialize](Bone.md#donotserialize)
- [onClonedObservable](Bone.md#onclonedobservable)
- [onDispose](Bone.md#ondispose)
- [onEnabledStateChangedObservable](Bone.md#onenabledstatechangedobservable)
- [parent](Bone.md#parent)
- [position](Bone.md#position)
- [rotation](Bone.md#rotation)
- [rotationQuaternion](Bone.md#rotationquaternion)
- [scaling](Bone.md#scaling)
- [worldMatrixFromCache](Bone.md#worldmatrixfromcache)

### Methods

- [\_compose](Bone.md#_compose)
- [\_decompose](Bone.md#_decompose)
- [\_getNegativeRotationToRef](Bone.md#_getnegativerotationtoref)
- [\_markAsDirtyAndDecompose](Bone.md#_markasdirtyanddecompose)
- [\_rotateWithMatrix](Bone.md#_rotatewithmatrix)
- [addBehavior](Bone.md#addbehavior)
- [beginAnimation](Bone.md#beginanimation)
- [computeAbsoluteTransforms](Bone.md#computeabsolutetransforms)
- [computeWorldMatrix](Bone.md#computeworldmatrix)
- [copyAnimationRange](Bone.md#copyanimationrange)
- [createAnimationRange](Bone.md#createanimationrange)
- [deleteAnimationRange](Bone.md#deleteanimationrange)
- [dispose](Bone.md#dispose)
- [getAbsolutePosition](Bone.md#getabsoluteposition)
- [getAbsolutePositionFromLocal](Bone.md#getabsolutepositionfromlocal)
- [getAbsolutePositionFromLocalToRef](Bone.md#getabsolutepositionfromlocaltoref)
- [getAbsolutePositionToRef](Bone.md#getabsolutepositiontoref)
- [getAbsoluteTransform](Bone.md#getabsolutetransform)
- [getAnimationByName](Bone.md#getanimationbyname)
- [getAnimationRange](Bone.md#getanimationrange)
- [getAnimationRanges](Bone.md#getanimationranges)
- [getBaseMatrix](Bone.md#getbasematrix)
- [getBehaviorByName](Bone.md#getbehaviorbyname)
- [getBindPose](Bone.md#getbindpose)
- [getChildMeshes](Bone.md#getchildmeshes)
- [getChildren](Bone.md#getchildren)
- [getClassName](Bone.md#getclassname)
- [getDescendants](Bone.md#getdescendants)
- [getDirection](Bone.md#getdirection)
- [getDirectionToRef](Bone.md#getdirectiontoref)
- [getEngine](Bone.md#getengine)
- [getHierarchyBoundingVectors](Bone.md#gethierarchyboundingvectors)
- [getIndex](Bone.md#getindex)
- [getInvertedAbsoluteTransform](Bone.md#getinvertedabsolutetransform)
- [getLocalMatrix](Bone.md#getlocalmatrix)
- [getLocalPositionFromAbsolute](Bone.md#getlocalpositionfromabsolute)
- [getLocalPositionFromAbsoluteToRef](Bone.md#getlocalpositionfromabsolutetoref)
- [getParent](Bone.md#getparent)
- [getPosition](Bone.md#getposition)
- [getPositionToRef](Bone.md#getpositiontoref)
- [getRestPose](Bone.md#getrestpose)
- [getRotation](Bone.md#getrotation)
- [getRotationMatrix](Bone.md#getrotationmatrix)
- [getRotationMatrixToRef](Bone.md#getrotationmatrixtoref)
- [getRotationQuaternion](Bone.md#getrotationquaternion)
- [getRotationQuaternionToRef](Bone.md#getrotationquaterniontoref)
- [getRotationToRef](Bone.md#getrotationtoref)
- [getScale](Bone.md#getscale)
- [getScaleToRef](Bone.md#getscaletoref)
- [getScene](Bone.md#getscene)
- [getSkeleton](Bone.md#getskeleton)
- [getTransformNode](Bone.md#gettransformnode)
- [getWorldMatrix](Bone.md#getworldmatrix)
- [isDescendantOf](Bone.md#isdescendantof)
- [isDisposed](Bone.md#isdisposed)
- [isEnabled](Bone.md#isenabled)
- [isReady](Bone.md#isready)
- [linkTransformNode](Bone.md#linktransformnode)
- [markAsDirty](Bone.md#markasdirty)
- [removeBehavior](Bone.md#removebehavior)
- [returnToRest](Bone.md#returntorest)
- [rotate](Bone.md#rotate)
- [scale](Bone.md#scale)
- [serializeAnimationRanges](Bone.md#serializeanimationranges)
- [setAbsolutePosition](Bone.md#setabsoluteposition)
- [setAxisAngle](Bone.md#setaxisangle)
- [setBindPose](Bone.md#setbindpose)
- [setCurrentPoseAsRest](Bone.md#setcurrentposeasrest)
- [setEnabled](Bone.md#setenabled)
- [setParent](Bone.md#setparent)
- [setPosition](Bone.md#setposition)
- [setRestPose](Bone.md#setrestpose)
- [setRotation](Bone.md#setrotation)
- [setRotationMatrix](Bone.md#setrotationmatrix)
- [setRotationQuaternion](Bone.md#setrotationquaternion)
- [setScale](Bone.md#setscale)
- [setYawPitchRoll](Bone.md#setyawpitchroll)
- [translate](Bone.md#translate)
- [updateMatrix](Bone.md#updatematrix)
- [AddNodeConstructor](Bone.md#addnodeconstructor)
- [Construct](Bone.md#construct)
- [ParseAnimationRanges](Bone.md#parseanimationranges)

## Constructors

### constructor

• **new Bone**(`name`, `skeleton`, `parentBone?`, `localMatrix?`, `restPose?`, `baseMatrix?`, `index?`)

Create a new bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the bone name |
| `skeleton` | [`Skeleton`](Skeleton.md) | `undefined` | defines the parent skeleton |
| `parentBone` | [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md) | `null` | defines the parent (can be null if the bone is the root) |
| `localMatrix` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `null` | defines the local matrix |
| `restPose` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `null` | defines the rest pose matrix |
| `baseMatrix` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `null` | defines the base matrix |
| `index` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines index of the bone in the hierarchy |

#### Overrides

[Node](Node.md).[constructor](Node.md#constructor)

#### Defined in

packages/dev/core/src/Bones/bone.ts:91

## Properties

### \_absoluteTransform

• `Private` **\_absoluteTransform**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:45

___

### \_baseMatrix

• `Private` **\_baseMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:44

___

### \_invertedAbsoluteTransform

• `Private` **\_invertedAbsoluteTransform**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:46

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Node](Node.md).[_isDirty](Node.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_localMatrix

• `Private` **\_localMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:42

___

### \_localPosition

• `Private` **\_localPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:52

___

### \_localRotation

• `Private` **\_localRotation**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:51

___

### \_localScaling

• `Private` **\_localScaling**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:50

___

### \_needToCompose

• `Private` **\_needToCompose**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Bones/bone.ts:54

___

### \_needToDecompose

• `Private` **\_needToDecompose**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Bones/bone.ts:53

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[Node](Node.md).[_parentNode](Node.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Node](Node.md).[_ranges](Node.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_restPose

• `Private` **\_restPose**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:43

___

### \_scalingDeterminant

• `Private` **\_scalingDeterminant**: `number` = `1`

#### Defined in

packages/dev/core/src/Bones/bone.ts:47

___

### \_skeleton

• `Private` **\_skeleton**: [`Skeleton`](Skeleton.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:41

___

### \_worldTransform

• `Private` **\_worldTransform**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:48

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets the animations associated with this bone

#### Overrides

[Node](Node.md).[animations](Node.md#animations)

#### Defined in

packages/dev/core/src/Bones/bone.ts:27

___

### children

• **children**: [`Bone`](Bone.md)[]

Gets the list of child bones

#### Defined in

packages/dev/core/src/Bones/bone.ts:24

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[Node](Node.md).[id](Node.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Node](Node.md).[inspectableCustomProperties](Node.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### length

• **length**: `number`

Gets or sets bone length

#### Defined in

packages/dev/core/src/Bones/bone.ts:32

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Node](Node.md).[metadata](Node.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[Node](Node.md).[name](Node.md#name)

#### Defined in

packages/dev/core/src/Bones/bone.ts:95

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Node](Node.md).[onDisposeObservable](Node.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Node](Node.md).[onReady](Node.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Node](Node.md).[reservedDataStore](Node.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Node](Node.md).[state](Node.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Node](Node.md).[uniqueId](Node.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### \_TmpMats

▪ `Static` `Private` **\_TmpMats**: [`Matrix`](Matrix.md)[]

#### Defined in

packages/dev/core/src/Bones/bone.ts:19

___

### \_TmpQuat

▪ `Static` `Private` **\_TmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:18

___

### \_TmpVecs

▪ `Static` `Private` **\_TmpVecs**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Bones/bone.ts:17

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Overrides

Node.animationPropertiesOverride

#### Defined in

packages/dev/core/src/Bones/bone.ts:365

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

Node.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

Node.doNotSerialize

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

Node.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

Node.onClonedObservable

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

Node.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

Node.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Bone`](Bone.md)

#### Returns

[`Bone`](Bone.md)

#### Overrides

Node.parent

#### Defined in

packages/dev/core/src/Bones/bone.ts:137

• `set` **parent**(`newParent`): `void`

Gets or sets the parent of the node (without keeping the current position in the scene)

**`See`**

https://doc.babylonjs.com/how_to/parenting

#### Parameters

| Name | Type |
| :------ | :------ |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md) |

#### Returns

`void`

#### Overrides

Node.parent

#### Defined in

packages/dev/core/src/Bones/bone.ts:165

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or sets current position (in local space)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:322

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:327

___

### rotation

• `get` **rotation**(): [`Vector3`](Vector3.md)

Gets or sets current rotation (in local space)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:335

• `set` **rotation**(`newRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newRotation` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:339

___

### rotationQuaternion

• `get` **rotationQuaternion**(): [`Quaternion`](Quaternion.md)

Gets or sets current rotation quaternion (in local space)

#### Returns

[`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:344

• `set` **rotationQuaternion**(`newRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newRotation` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:349

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets current scaling (in local space)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Bones/bone.ts:354

• `set` **scaling**(`newScaling`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newScaling` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:358

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

Node.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

## Methods

### \_compose

▸ `Private` **_compose**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:385

___

### \_decompose

▸ `Private` **_decompose**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:370

___

### \_getNegativeRotationToRef

▸ `Private` **_getNegativeRotationToRef**(`rotMatInv`, `tNode?`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rotMatInv` | [`Matrix`](Matrix.md) |
| `tNode?` | [`TransformNode`](TransformNode.md) |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Bones/bone.ts:809

___

### \_markAsDirtyAndDecompose

▸ `Private` **_markAsDirtyAndDecompose**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:463

___

### \_rotateWithMatrix

▸ `Private` **_rotateWithMatrix**(`rmat`, `space?`, `tNode?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `rmat` | [`Matrix`](Matrix.md) | `undefined` |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:769

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

[Node](Node.md).[addBehavior](Node.md#addbehavior)

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

[Node](Node.md).[beginAnimation](Node.md#beginanimation)

#### Defined in

packages/dev/core/src/node.ts:833

___

### computeAbsoluteTransforms

▸ **computeAbsoluteTransforms**(): `void`

Compute the absolute transforms of this bone and its children

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:910

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

[Node](Node.md).[computeWorldMatrix](Node.md#computeworldmatrix)

#### Defined in

packages/dev/core/src/node.ts:868

___

### copyAnimationRange

▸ **copyAnimationRange**(`source`, `rangeName`, `frameOffset`, `rescaleAsRequired`, `skelDimensionsRatio`): `boolean`

Copy an animation range from another bone

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Bone`](Bone.md) | defines the source bone |
| `rangeName` | `string` | defines the range name to copy |
| `frameOffset` | `number` | defines the frame offset |
| `rescaleAsRequired` | `boolean` | defines if rescaling must be applied if required |
| `skelDimensionsRatio` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | defines the scaling ratio |

#### Returns

`boolean`

true if operation was successful

#### Defined in

packages/dev/core/src/Animations/animatable.ts:1178

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

[Node](Node.md).[createAnimationRange](Node.md#createanimationrange)

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

[Node](Node.md).[deleteAnimationRange](Node.md#deleteanimationrange)

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

[Node](Node.md).[dispose](Node.md#dispose)

#### Defined in

packages/dev/core/src/node.ts:880

___

### getAbsolutePosition

▸ **getAbsolutePosition**(`tNode?`): [`Vector3`](Vector3.md)

Get the absolute position of the bone (world space)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |

#### Returns

[`Vector3`](Vector3.md)

The absolute position of the bone

#### Defined in

packages/dev/core/src/Bones/bone.ts:890

___

### getAbsolutePositionFromLocal

▸ **getAbsolutePositionFromLocal**(`position`, `tNode?`): [`Vector3`](Vector3.md)

Get the world position of a point that is in the local space of the bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | The local position |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |

#### Returns

[`Vector3`](Vector3.md)

The world position

#### Defined in

packages/dev/core/src/Bones/bone.ts:1093

___

### getAbsolutePositionFromLocalToRef

▸ **getAbsolutePositionFromLocalToRef**(`position`, `tNode?`, `result`): `void`

Get the world position of a point that is in the local space of the bone and copy it to the result param

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | The local position |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |
| `result` | [`Vector3`](Vector3.md) | `undefined` | The vector3 that the world position should be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:1107

___

### getAbsolutePositionToRef

▸ **getAbsolutePositionToRef**(`tNode`, `result`): `void`

Copy the absolute position of the bone (world space) to the result param

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tNode` | [`TransformNode`](TransformNode.md) | The TransformNode that this bone is attached to |
| `result` | [`Vector3`](Vector3.md) | The vector3 to copy the absolute position to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:903

___

### getAbsoluteTransform

▸ **getAbsoluteTransform**(): [`Matrix`](Matrix.md)

Gets the absolute transform matrix (ie base matrix * parent world matrix)

#### Returns

[`Matrix`](Matrix.md)

a matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:290

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

[Node](Node.md).[getAnimationByName](Node.md#getanimationbyname)

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

[Node](Node.md).[getAnimationRange](Node.md#getanimationrange)

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

[Node](Node.md).[getAnimationRanges](Node.md#getanimationranges)

#### Defined in

packages/dev/core/src/node.ts:816

___

### getBaseMatrix

▸ **getBaseMatrix**(): [`Matrix`](Matrix.md)

Gets the base matrix (initial matrix which remains unchanged)

#### Returns

[`Matrix`](Matrix.md)

the base matrix (as known as bind pose matrix)

#### Defined in

packages/dev/core/src/Bones/bone.ts:212

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

[Node](Node.md).[getBehaviorByName](Node.md#getbehaviorbyname)

#### Defined in

packages/dev/core/src/node.ts:420

___

### getBindPose

▸ **getBindPose**(): [`Matrix`](Matrix.md)

Gets the bind pose matrix

**`Deprecated`**

Please use getBaseMatrix instead

#### Returns

[`Matrix`](Matrix.md)

the bind pose matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:237

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

[Node](Node.md).[getChildMeshes](Node.md#getchildmeshes)

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

[Node](Node.md).[getChildMeshes](Node.md#getchildmeshes)

#### Defined in

packages/dev/core/src/node.ts:692

___

### getChildren

▸ **getChildren**(): [`Bone`](Bone.md)[]

Returns an array containing the root bones

#### Returns

[`Bone`](Bone.md)[]

an array containing the root bones

#### Overrides

[Node](Node.md).[getChildren](Node.md#getchildren)

#### Defined in

packages/dev/core/src/Bones/bone.ts:153

___

### getClassName

▸ **getClassName**(): `string`

Gets the current object class name.

#### Returns

`string`

the class name

#### Overrides

[Node](Node.md).[getClassName](Node.md#getclassname)

#### Defined in

packages/dev/core/src/Bones/bone.ts:123

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

[Node](Node.md).[getDescendants](Node.md#getdescendants)

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

[Node](Node.md).[getDescendants](Node.md#getdescendants)

#### Defined in

packages/dev/core/src/node.ts:662

___

### getDirection

▸ **getDirection**(`localAxis`, `tNode?`): [`Vector3`](Vector3.md)

Get the world direction from an axis that is in the local space of the bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | `undefined` | The local direction that is used to compute the world direction |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |

#### Returns

[`Vector3`](Vector3.md)

The world direction

#### Defined in

packages/dev/core/src/Bones/bone.ts:939

___

### getDirectionToRef

▸ **getDirectionToRef**(`localAxis`, `tNode?`, `result`): `void`

Copy the world direction to a vector3 from an axis that is in the local space of the bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | `undefined` | The local direction that is used to compute the world direction |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |
| `result` | [`Vector3`](Vector3.md) | `undefined` | The vector3 that the world direction will be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:953

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[Node](Node.md).[getEngine](Node.md#getengine)

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

[Node](Node.md).[getHierarchyBoundingVectors](Node.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getIndex

▸ **getIndex**(): `number`

Gets the node index in matrix array generated for rendering

#### Returns

`number`

the node index

#### Defined in

packages/dev/core/src/Bones/bone.ts:161

___

### getInvertedAbsoluteTransform

▸ **getInvertedAbsoluteTransform**(): [`Matrix`](Matrix.md)

Gets the inverse of the absolute transform matrix.
This matrix will be multiplied by local matrix to get the difference matrix (ie. the difference between original state and current state)

#### Returns

[`Matrix`](Matrix.md)

a matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:282

___

### getLocalMatrix

▸ **getLocalMatrix**(): [`Matrix`](Matrix.md)

Gets the local matrix

#### Returns

[`Matrix`](Matrix.md)

a matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:203

___

### getLocalPositionFromAbsolute

▸ **getLocalPositionFromAbsolute**(`position`, `tNode?`): [`Vector3`](Vector3.md)

Get the local position of a point that is in world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | The world position |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |

#### Returns

[`Vector3`](Vector3.md)

The local position

#### Defined in

packages/dev/core/src/Bones/bone.ts:1135

___

### getLocalPositionFromAbsoluteToRef

▸ **getLocalPositionFromAbsoluteToRef**(`position`, `tNode?`, `result`): `void`

Get the local position of a point that is in world space and copy it to the result param

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | The world position |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to |
| `result` | [`Vector3`](Vector3.md) | `undefined` | The vector3 that the local position should be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:1149

___

### getParent

▸ **getParent**(): [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

Gets parent bone

#### Returns

[`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

a bone or null if the bone is the root of the bone hierarchy

#### Defined in

packages/dev/core/src/Bones/bone.ts:145

___

### getPosition

▸ **getPosition**(`space?`, `tNode?`): [`Vector3`](Vector3.md)

Get the position of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the returned position is in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

[`Vector3`](Vector3.md)

The position of the bone

#### Defined in

packages/dev/core/src/Bones/bone.ts:839

___

### getPositionToRef

▸ **getPositionToRef**(`space?`, `tNode`, `result`): `void`

Copy the position of the bone to a vector3 in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the returned position is in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |
| `result` | [`Vector3`](Vector3.md) | `undefined` | The vector3 to copy the position to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:853

___

### getRestPose

▸ **getRestPose**(): [`Matrix`](Matrix.md)

Gets the rest pose matrix

#### Returns

[`Matrix`](Matrix.md)

a matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:220

___

### getRotation

▸ **getRotation**(`space?`, `tNode?`): [`Vector3`](Vector3.md)

Get the euler rotation of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

[`Vector3`](Vector3.md)

The euler rotation

#### Defined in

packages/dev/core/src/Bones/bone.ts:982

___

### getRotationMatrix

▸ **getRotationMatrix**(`space?`, `tNode`): [`Matrix`](Matrix.md)

Get the rotation matrix of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

[`Matrix`](Matrix.md)

The rotation matrix

#### Defined in

packages/dev/core/src/Bones/bone.ts:1052

___

### getRotationMatrixToRef

▸ **getRotationMatrixToRef**(`space?`, `tNode`, `result`): `void`

Copy the rotation matrix of the bone to a matrix.  The rotation can be in either local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to.  This is only used in world space |
| `result` | [`Matrix`](Matrix.md) | `undefined` | The quaternion that the rotation should be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:1066

___

### getRotationQuaternion

▸ **getRotationQuaternion**(`space?`, `tNode?`): [`Quaternion`](Quaternion.md)

Get the quaternion rotation of the bone in either local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

[`Quaternion`](Quaternion.md)

The quaternion rotation

#### Defined in

packages/dev/core/src/Bones/bone.ts:1010

___

### getRotationQuaternionToRef

▸ **getRotationQuaternionToRef**(`space?`, `tNode?`, `result`): `void`

Copy the quaternion rotation of the bone to a quaternion.  The rotation can be in either local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to.  This is only used in world space |
| `result` | [`Quaternion`](Quaternion.md) | `undefined` | The quaternion that the rotation should be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:1024

___

### getRotationToRef

▸ **getRotationToRef**(`space?`, `tNode?`, `result`): `void`

Copy the euler rotation of the bone to a vector3.  The rotation can be in either local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation should be in |
| `tNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | The TransformNode that this bone is attached to.  This is only used in world space |
| `result` | [`Vector3`](Vector3.md) | `undefined` | The vector3 that the rotation should be copied to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:996

___

### getScale

▸ **getScale**(): [`Vector3`](Vector3.md)

Gets the current scaling in local space

#### Returns

[`Vector3`](Vector3.md)

the current scaling vector

#### Defined in

packages/dev/core/src/Bones/bone.ts:619

___

### getScaleToRef

▸ **getScaleToRef**(`result`): `void`

Gets the current scaling in local space and stores it in a target vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:628

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[Node](Node.md).[getScene](Node.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getSkeleton

▸ **getSkeleton**(): [`Skeleton`](Skeleton.md)

Gets the parent skeleton

#### Returns

[`Skeleton`](Skeleton.md)

a skeleton

#### Defined in

packages/dev/core/src/Bones/bone.ts:133

___

### getTransformNode

▸ **getTransformNode**(): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Gets the node used to drive the bone's transformation

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

a transform node or null

#### Defined in

packages/dev/core/src/Bones/bone.ts:317

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets a matrix used to store world matrix (ie. the matrix sent to shaders)

#### Returns

[`Matrix`](Matrix.md)

#### Overrides

[Node](Node.md).[getWorldMatrix](Node.md#getworldmatrix)

#### Defined in

packages/dev/core/src/Bones/bone.ts:253

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

[Node](Node.md).[isDescendantOf](Node.md#isdescendantof)

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

[Node](Node.md).[isDisposed](Node.md#isdisposed)

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

[Node](Node.md).[isEnabled](Node.md#isenabled)

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

[Node](Node.md).[isReady](Node.md#isready)

#### Defined in

packages/dev/core/src/node.ts:548

___

### linkTransformNode

▸ **linkTransformNode**(`transformNode`): `void`

Links with the given transform node.
The local matrix of this bone is copied from the transform node every frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transformNode` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | defines the transform node to link to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:299

___

### markAsDirty

▸ **markAsDirty**(): [`Bone`](Bone.md)

Flag the bone as dirty (Forcing it to update everything)

#### Returns

[`Bone`](Bone.md)

this bone

#### Overrides

[Node](Node.md).[markAsDirty](Node.md#markasdirty)

#### Defined in

packages/dev/core/src/Bones/bone.ts:450

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

[Node](Node.md).[removeBehavior](Node.md#removebehavior)

#### Defined in

packages/dev/core/src/node.ts:393

___

### returnToRest

▸ **returnToRest**(): `void`

Sets the local matrix to rest pose matrix

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:260

___

### rotate

▸ **rotate**(`axis`, `amount`, `space?`, `tNode?`): `void`

Add a rotation to the bone on an axis in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | `undefined` | The axis to rotate the bone on |
| `amount` | `number` | `undefined` | The amount to rotate the bone |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the axis is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:668

___

### scale

▸ **scale**(`x`, `y`, `z`, `scaleChildren?`): `void`

Scale the bone on the x, y and z axes (in local space)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | The amount to scale the bone on the x axis |
| `y` | `number` | `undefined` | The amount to scale the bone on the y axis |
| `z` | `number` | `undefined` | The amount to scale the bone on the z axis |
| `scaleChildren` | `boolean` | `false` | sets this to true if children of the bone should be scaled as well (false by default) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:575

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[Node](Node.md).[serializeAnimationRanges](Node.md#serializeanimationranges)

#### Defined in

packages/dev/core/src/node.ts:847

___

### setAbsolutePosition

▸ **setAbsolutePosition**(`position`, `tNode?`): `void`

Set the absolute position of the bone (world space)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | The position to set the bone |
| `tNode?` | [`TransformNode`](TransformNode.md) | The TransformNode that this bone is attached to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:564

___

### setAxisAngle

▸ **setAxisAngle**(`axis`, `angle`, `space?`, `tNode?`): `void`

Set the rotation of the bone to a particular axis angle in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | `undefined` | The axis to rotate the bone on |
| `angle` | `number` | `undefined` | The angle that the bone should be rotated to |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the axis is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:682

___

### setBindPose

▸ **setBindPose**(`matrix`): `void`

Sets the bind pose matrix

**`Deprecated`**

Please use updateMatrix instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | the local-space bind pose to set for this bone |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:246

___

### setCurrentPoseAsRest

▸ **setCurrentPoseAsRest**(): `void`

Set the current local matrix as the restPose for this bone.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:1175

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

[Node](Node.md).[setEnabled](Node.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### setParent

▸ **setParent**(`parent`, `updateDifferenceMatrix?`): `void`

Sets the parent bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `parent` | [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md) | `undefined` | defines the parent (can be null if the bone is the root) |
| `updateDifferenceMatrix` | `boolean` | `true` | defines if the difference matrix must be updated |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:174

___

### setPosition

▸ **setPosition**(`position`, `space?`, `tNode?`): `void`

Set the position of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | The position to set the bone |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the position is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:522

___

### setRestPose

▸ **setRestPose**(`matrix`): `void`

Sets the rest pose matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | the local-space rest pose to set for this bone |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:228

___

### setRotation

▸ **setRotation**(`rotation`, `space?`, `tNode?`): `void`

Set the euler rotation of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rotation` | [`Vector3`](Vector3.md) | `undefined` | The euler rotation that the bone should be set to |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:709

___

### setRotationMatrix

▸ **setRotationMatrix**(`rotMat`, `space?`, `tNode?`): `void`

Set the rotation matrix of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rotMat` | [`Matrix`](Matrix.md) | `undefined` | The rotation matrix that the bone should be set to |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:748

___

### setRotationQuaternion

▸ **setRotationQuaternion**(`quat`, `space?`, `tNode?`): `void`

Set the quaternion rotation of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `quat` | [`Quaternion`](Quaternion.md) | `undefined` | The quaternion rotation that the bone should be set to |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the rotation is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:719

___

### setScale

▸ **setScale**(`scale`): `void`

Set the bone scaling in local space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | [`Vector3`](Vector3.md) | defines the scaling vector |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:609

___

### setYawPitchRoll

▸ **setYawPitchRoll**(`yaw`, `pitch`, `roll`, `space?`, `tNode?`): `void`

Set the yaw, pitch, and roll of the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `yaw` | `number` | `undefined` | The rotation of the bone on the y axis |
| `pitch` | `number` | `undefined` | The rotation of the bone on the x axis |
| `roll` | `number` | `undefined` | The rotation of the bone on the z axis |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the axes of rotation are in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to.  This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:641

___

### translate

▸ **translate**(`vec`, `space?`, `tNode?`): `void`

Translate the bone in local or world space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `vec` | [`Vector3`](Vector3.md) | `undefined` | The amount to translate the bone |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | The space that the translation is in |
| `tNode?` | [`TransformNode`](TransformNode.md) | `undefined` | The TransformNode that this bone is attached to. This is only used in world space |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:474

___

### updateMatrix

▸ **updateMatrix**(`matrix`, `updateDifferenceMatrix?`, `updateLocalMatrix?`): `void`

Update the base and local matrices

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | `undefined` | defines the new base or local matrix |
| `updateDifferenceMatrix` | `boolean` | `true` | defines if the difference matrix must be updated |
| `updateLocalMatrix` | `boolean` | `true` | defines if the local matrix should be updated |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Bones/bone.ts:405

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

[Node](Node.md).[AddNodeConstructor](Node.md#addnodeconstructor)

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

[Node](Node.md).[Construct](Node.md#construct)

#### Defined in

packages/dev/core/src/node.ts:75

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

[Node](Node.md).[ParseAnimationRanges](Node.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919

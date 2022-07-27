[@dev/core](../README.md) / [Exports](../modules.md) / Skeleton

# Class: Skeleton

Class used to handle skinning animations

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](Skeleton.md#constructor)

### Properties

- [\_absoluteTransformIsDirty](Skeleton.md#_absolutetransformisdirty)
- [\_animatables](Skeleton.md#_animatables)
- [\_animationPropertiesOverride](Skeleton.md#_animationpropertiesoverride)
- [\_canUseTextureForBones](Skeleton.md#_canusetextureforbones)
- [\_identity](Skeleton.md#_identity)
- [\_isDirty](Skeleton.md#_isdirty)
- [\_meshesWithPoseMatrix](Skeleton.md#_mesheswithposematrix)
- [\_ranges](Skeleton.md#_ranges)
- [\_scene](Skeleton.md#_scene)
- [\_synchronizedWithMesh](Skeleton.md#_synchronizedwithmesh)
- [\_transformMatrices](Skeleton.md#_transformmatrices)
- [\_transformMatrixTexture](Skeleton.md#_transformmatrixtexture)
- [\_uniqueId](Skeleton.md#_uniqueid)
- [\_useTextureToStoreBoneMatrices](Skeleton.md#_usetexturetostorebonematrices)
- [animations](Skeleton.md#animations)
- [bones](Skeleton.md#bones)
- [dimensionsAtRest](Skeleton.md#dimensionsatrest)
- [doNotSerialize](Skeleton.md#donotserialize)
- [id](Skeleton.md#id)
- [inspectableCustomProperties](Skeleton.md#inspectablecustomproperties)
- [name](Skeleton.md#name)
- [needInitialSkinMatrix](Skeleton.md#needinitialskinmatrix)
- [onBeforeComputeObservable](Skeleton.md#onbeforecomputeobservable)

### Accessors

- [animationPropertiesOverride](Skeleton.md#animationpropertiesoverride)
- [isUsingTextureForMatrices](Skeleton.md#isusingtextureformatrices)
- [uniqueId](Skeleton.md#uniqueid)
- [useTextureToStoreBoneMatrices](Skeleton.md#usetexturetostorebonematrices)

### Methods

- [\_computeTransformMatrices](Skeleton.md#_computetransformmatrices)
- [\_getHighestAnimationFrame](Skeleton.md#_gethighestanimationframe)
- [\_sortBones](Skeleton.md#_sortbones)
- [beginAnimation](Skeleton.md#beginanimation)
- [clone](Skeleton.md#clone)
- [computeAbsoluteTransforms](Skeleton.md#computeabsolutetransforms)
- [copyAnimationRange](Skeleton.md#copyanimationrange)
- [createAnimationRange](Skeleton.md#createanimationrange)
- [deleteAnimationRange](Skeleton.md#deleteanimationrange)
- [dispose](Skeleton.md#dispose)
- [enableBlending](Skeleton.md#enableblending)
- [getAnimatables](Skeleton.md#getanimatables)
- [getAnimationRange](Skeleton.md#getanimationrange)
- [getAnimationRanges](Skeleton.md#getanimationranges)
- [getBoneIndexByName](Skeleton.md#getboneindexbyname)
- [getChildren](Skeleton.md#getchildren)
- [getClassName](Skeleton.md#getclassname)
- [getPoseMatrix](Skeleton.md#getposematrix)
- [getScene](Skeleton.md#getscene)
- [getTransformMatrices](Skeleton.md#gettransformmatrices)
- [getTransformMatrixTexture](Skeleton.md#gettransformmatrixtexture)
- [prepare](Skeleton.md#prepare)
- [returnToRest](Skeleton.md#returntorest)
- [serialize](Skeleton.md#serialize)
- [setCurrentPoseAsRest](Skeleton.md#setcurrentposeasrest)
- [sortBones](Skeleton.md#sortbones)
- [toString](Skeleton.md#tostring)
- [MakeAnimationAdditive](Skeleton.md#makeanimationadditive)
- [Parse](Skeleton.md#parse)

## Constructors

### constructor

• **new Skeleton**(`name`, `id`, `scene`)

Creates a new skeleton

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the skeleton name |
| `id` | `string` | defines the skeleton Id |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:136

## Properties

### \_absoluteTransformIsDirty

• `Private` **\_absoluteTransformIsDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:54

___

### \_animatables

• `Private` **\_animatables**: [`IAnimatable`](../interfaces/IAnimatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:48

___

### \_animationPropertiesOverride

• `Private` **\_animationPropertiesOverride**: [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:87

___

### \_canUseTextureForBones

• `Private` **\_canUseTextureForBones**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:56

___

### \_identity

• `Private` **\_identity**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:49

___

### \_isDirty

• `Private` **\_isDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:44

___

### \_meshesWithPoseMatrix

• `Private` **\_meshesWithPoseMatrix**: [`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:47

___

### \_ranges

• `Private` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:52

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:43

___

### \_synchronizedWithMesh

• `Private` **\_synchronizedWithMesh**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:50

___

### \_transformMatrices

• `Private` **\_transformMatrices**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:45

___

### \_transformMatrixTexture

• `Private` **\_transformMatrixTexture**: [`Nullable`](../modules.md#nullable)[`RawTexture`](RawTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:46

___

### \_uniqueId

• `Private` **\_uniqueId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:57

___

### \_useTextureToStoreBoneMatrices

• `Private` **\_useTextureToStoreBoneMatrices**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:73

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets the list of animations attached to this skeleton

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:41

___

### bones

• **bones**: [`Bone`](Bone.md)[]

Defines the list of child bones

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:28

___

### dimensionsAtRest

• **dimensionsAtRest**: [`Vector3`](Vector3.md)

Defines an estimate of the dimension of the skeleton at rest

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:32

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the skeleton should be serialized

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:71

___

### id

• **id**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:140

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:107

___

### name

• **name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:138

___

### needInitialSkinMatrix

• **needInitialSkinMatrix**: `boolean` = `false`

Defines a boolean indicating if the root matrix is provided by meshes or by the current skeleton (this is the default value)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:36

___

### onBeforeComputeObservable

• **onBeforeComputeObservable**: [`Observable`](Observable.md)[`Skeleton`](Skeleton.md)

An observable triggered before computing the skeleton's matrices

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:114

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:92

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:99

___

### isUsingTextureForMatrices

• `get` **isUsingTextureForMatrices**(): `boolean`

Gets a boolean indicating that the skeleton effectively stores matrices into a texture

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:119

___

### uniqueId

• `get` **uniqueId**(): `number`

Gets the unique ID of this skeleton

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:126

___

### useTextureToStoreBoneMatrices

• `get` **useTextureToStoreBoneMatrices**(): `boolean`

Gets or sets a boolean indicating that bone matrices should be stored as a texture instead of using shader uniforms (default is true).
Please note that this option is not available if the hardware does not support it

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:78

• `set` **useTextureToStoreBoneMatrices**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:82

## Methods

### \_computeTransformMatrices

▸ `Private` **_computeTransformMatrices**(`targetMatrix`, `initialSkinMatrix`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetMatrix` | `Float32Array` |
| `initialSkinMatrix` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:478

___

### \_getHighestAnimationFrame

▸ `Private` **_getHighestAnimationFrame**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:369

___

### \_sortBones

▸ `Private` **_sortBones**(`index`, `bones`, `visited`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |
| `bones` | [`Bone`](Bone.md)[] |
| `visited` | `boolean`[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:872

___

### beginAnimation

▸ **beginAnimation**(`name`, `loop?`, `speedRatio?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Begin a specific animation range

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the range to start |
| `loop?` | `boolean` | defines if looping must be turned on (false by default) |
| `speedRatio?` | `number` | defines the speed ratio to apply (1 by default) |
| `onAnimationEnd?` | () => `void` | defines a callback which will be called when animation will end |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

a new animatable

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:390

___

### clone

▸ **clone**(`name`, `id?`): [`Skeleton`](Skeleton.md)

Clone the current skeleton

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the new skeleton |
| `id?` | `string` | defines the id of the new skeleton |

#### Returns

[`Skeleton`](Skeleton.md)

the new skeleton

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:631

___

### computeAbsoluteTransforms

▸ **computeAbsoluteTransforms**(`forceUpdate?`): `void`

Compute all node absolute transforms

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `forceUpdate` | `boolean` | `false` | defines if computation must be done even if cache is up to date |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:838

___

### copyAnimationRange

▸ **copyAnimationRange**(`source`, `name`, `rescaleAsRequired?`): `boolean`

Copy animation range from a source skeleton.
This is not for a complete retargeting, only between very similar skeleton's with only possible bone length differences

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | [`Skeleton`](Skeleton.md) | `undefined` | defines the source skeleton |
| `name` | `string` | `undefined` | defines the name of the range to copy |
| `rescaleAsRequired` | `boolean` | `false` | defines if rescaling must be applied if required |

#### Returns

`boolean`

true if operation was successful

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:317

___

### createAnimationRange

▸ **createAnimationRange**(`name`, `from`, `to`): `void`

Create a new animation range

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the range |
| `from` | `number` | defines the start key |
| `to` | `number` | defines the end key |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:261

___

### deleteAnimationRange

▸ **deleteAnimationRange**(`name`, `deleteFrames?`): `void`

Delete a specific animation range

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the range |
| `deleteFrames` | `boolean` | `true` | defines if frames must be removed as well |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:278

___

### dispose

▸ **dispose**(): `void`

Releases all resources associated with the current skeleton

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:689

___

### enableBlending

▸ **enableBlending**(`blendingSpeed?`): `void`

Enable animation blending for this skeleton

**`See`**

https://doc.babylonjs.com/babylon101/animations#animation-blending

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `blendingSpeed` | `number` | `0.01` | defines the blending speed to apply |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:677

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Gets the list of animatables currently running for this skeleton

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

an array of animatables

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:613

___

### getAnimationRange

▸ **getAnimationRange**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

Gets a specific animation range

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the range to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

the requested animation range or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:292

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

Gets the list of all animation ranges defined on this skeleton

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

an array

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:300

___

### getBoneIndexByName

▸ **getBoneIndexByName**(`name`): `number`

Get bone's index searching by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines bone's name to search for |

#### Returns

`number`

the indice of the bone. Returns -1 if not found

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:246

___

### getChildren

▸ **getChildren**(): [`Bone`](Bone.md)[]

Returns an array containing the root bones

#### Returns

[`Bone`](Bone.md)[]

an array containing the root bones

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:169

___

### getClassName

▸ **getClassName**(): `string`

Gets the current object class name.

#### Returns

`string`

the class name

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:161

___

### getPoseMatrix

▸ **getPoseMatrix**(): [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

Gets the root pose matrix

#### Returns

[`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

a matrix

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:849

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the current hosting scene

#### Returns

[`Scene`](Scene.md)

a scene object

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:212

___

### getTransformMatrices

▸ **getTransformMatrices**(`mesh`): `Float32Array`

Gets the list of transform matrices to send to shaders (one matrix per bone)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to use to get the root matrix (if needInitialSkinMatrix === true) |

#### Returns

`Float32Array`

a Float32Array containing matrices data

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:179

___

### getTransformMatrixTexture

▸ **getTransformMatrixTexture**(`mesh`): [`Nullable`](../modules.md#nullable)[`RawTexture`](RawTexture.md)

Gets the list of transform matrices to send to shaders inside a texture (one matrix per bone)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to use to get the root matrix (if needInitialSkinMatrix === true) |

#### Returns

[`Nullable`](../modules.md#nullable)[`RawTexture`](RawTexture.md)

a raw texture containing the data

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:200

___

### prepare

▸ **prepare**(): `void`

Build all resources required to render a skeleton

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:508

___

### returnToRest

▸ **returnToRest**(): `void`

Forces the skeleton to go to rest pose

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:361

___

### serialize

▸ **serialize**(): `any`

Serialize the skeleton in a JSON object

#### Returns

`any`

a JSON object

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:716

___

### setCurrentPoseAsRest

▸ **setCurrentPoseAsRest**(): `void`

Set the current local matrix as the restPose for all bones in the skeleton.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:897

___

### sortBones

▸ **sortBones**(): `void`

Sorts bones per internal index

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:862

___

### toString

▸ **toString**(`fullDetails?`): `string`

Gets a string representing the current skeleton data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | defines a boolean indicating if we want a verbose version |

#### Returns

`string`

a string representing the current skeleton data

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:223

___

### MakeAnimationAdditive

▸ `Static` **MakeAnimationAdditive**(`skeleton`, `referenceFrame?`, `range`): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Convert the keyframes for a range of animation on a skeleton to be relative to a given reference frame.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `skeleton` | [`Skeleton`](Skeleton.md) | `undefined` | defines the Skeleton containing the animation range to convert |
| `referenceFrame` | `number` | `0` | defines the frame that keyframes in the range will be relative to |
| `range` | `string` | `undefined` | defines the name of the AnimationRange belonging to the Skeleton to convert |

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

the original skeleton

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:407

___

### Parse

▸ `Static` **Parse**(`parsedSkeleton`, `scene`): [`Skeleton`](Skeleton.md)

Creates a new skeleton from serialized data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedSkeleton` | `any` | defines the serialized data |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`Skeleton`](Skeleton.md)

a new skeleton

#### Defined in

https://github.com/babylon.js/core/src/Bones/skeleton.ts:782

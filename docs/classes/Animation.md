[@dev/core](../README.md) / [Exports](../modules.md) / Animation

# Class: Animation

Class used to store any kind of animation

## Table of contents

### Constructors

- [constructor](Animation.md#constructor)

### Properties

- [\_easingFunction](Animation.md#_easingfunction)
- [\_events](Animation.md#_events)
- [\_keys](Animation.md#_keys)
- [\_ranges](Animation.md#_ranges)
- [blendingSpeed](Animation.md#blendingspeed)
- [dataType](Animation.md#datatype)
- [enableBlending](Animation.md#enableblending)
- [framePerSecond](Animation.md#framepersecond)
- [loopMode](Animation.md#loopmode)
- [name](Animation.md#name)
- [snippetId](Animation.md#snippetid)
- [targetProperty](Animation.md#targetproperty)
- [targetPropertyPath](Animation.md#targetpropertypath)
- [uniqueId](Animation.md#uniqueid)
- [ANIMATIONLOOPMODE\_CONSTANT](Animation.md#animationloopmode_constant)
- [ANIMATIONLOOPMODE\_CYCLE](Animation.md#animationloopmode_cycle)
- [ANIMATIONLOOPMODE\_RELATIVE](Animation.md#animationloopmode_relative)
- [ANIMATIONTYPE\_COLOR3](Animation.md#animationtype_color3)
- [ANIMATIONTYPE\_COLOR4](Animation.md#animationtype_color4)
- [ANIMATIONTYPE\_FLOAT](Animation.md#animationtype_float)
- [ANIMATIONTYPE\_MATRIX](Animation.md#animationtype_matrix)
- [ANIMATIONTYPE\_QUATERNION](Animation.md#animationtype_quaternion)
- [ANIMATIONTYPE\_SIZE](Animation.md#animationtype_size)
- [ANIMATIONTYPE\_VECTOR2](Animation.md#animationtype_vector2)
- [ANIMATIONTYPE\_VECTOR3](Animation.md#animationtype_vector3)
- [AllowMatricesInterpolation](Animation.md#allowmatricesinterpolation)
- [AllowMatrixDecomposeForInterpolation](Animation.md#allowmatrixdecomposeforinterpolation)
- [CreateFromSnippetAsync](Animation.md#createfromsnippetasync)
- [SnippetUrl](Animation.md#snippeturl)
- [\_UniqueIdGenerator](Animation.md#_uniqueidgenerator)

### Accessors

- [hasRunningRuntimeAnimations](Animation.md#hasrunningruntimeanimations)
- [runtimeAnimations](Animation.md#runtimeanimations)

### Methods

- [addEvent](Animation.md#addevent)
- [clone](Animation.md#clone)
- [color3InterpolateFunction](Animation.md#color3interpolatefunction)
- [color3InterpolateFunctionWithTangents](Animation.md#color3interpolatefunctionwithtangents)
- [color4InterpolateFunction](Animation.md#color4interpolatefunction)
- [color4InterpolateFunctionWithTangents](Animation.md#color4interpolatefunctionwithtangents)
- [createRange](Animation.md#createrange)
- [deleteRange](Animation.md#deleterange)
- [evaluate](Animation.md#evaluate)
- [floatInterpolateFunction](Animation.md#floatinterpolatefunction)
- [floatInterpolateFunctionWithTangents](Animation.md#floatinterpolatefunctionwithtangents)
- [getEasingFunction](Animation.md#geteasingfunction)
- [getEvents](Animation.md#getevents)
- [getHighestFrame](Animation.md#gethighestframe)
- [getKeys](Animation.md#getkeys)
- [getRange](Animation.md#getrange)
- [matrixInterpolateFunction](Animation.md#matrixinterpolatefunction)
- [quaternionInterpolateFunction](Animation.md#quaternioninterpolatefunction)
- [quaternionInterpolateFunctionWithTangents](Animation.md#quaternioninterpolatefunctionwithtangents)
- [removeEvents](Animation.md#removeevents)
- [serialize](Animation.md#serialize)
- [setEasingFunction](Animation.md#seteasingfunction)
- [setKeys](Animation.md#setkeys)
- [sizeInterpolateFunction](Animation.md#sizeinterpolatefunction)
- [toString](Animation.md#tostring)
- [vector2InterpolateFunction](Animation.md#vector2interpolatefunction)
- [vector2InterpolateFunctionWithTangents](Animation.md#vector2interpolatefunctionwithtangents)
- [vector3InterpolateFunction](Animation.md#vector3interpolatefunction)
- [vector3InterpolateFunctionWithTangents](Animation.md#vector3interpolatefunctionwithtangents)
- [AppendSerializedAnimations](Animation.md#appendserializedanimations)
- [CreateAndStartAnimation](Animation.md#createandstartanimation)
- [CreateAndStartHierarchyAnimation](Animation.md#createandstarthierarchyanimation)
- [CreateAnimation](Animation.md#createanimation)
- [CreateMergeAndStartAnimation](Animation.md#createmergeandstartanimation)
- [MakeAnimationAdditive](Animation.md#makeanimationadditive)
- [Parse](Animation.md#parse)
- [ParseFromFileAsync](Animation.md#parsefromfileasync)
- [ParseFromSnippetAsync](Animation.md#parsefromsnippetasync)
- [TransitionTo](Animation.md#transitionto)

## Constructors

### constructor

• **new Animation**(`name`, `targetProperty`, `framePerSecond`, `dataType`, `loopMode?`, `enableBlending?`)

Initializes the animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the animation |
| `targetProperty` | `string` | Property to animate |
| `framePerSecond` | `number` | The frames per second of the animation |
| `dataType` | `number` | The data type of the animation |
| `loopMode?` | `number` | The loop mode of the animation |
| `enableBlending?` | `boolean` | Specifies if blending should be enabled |

#### Defined in

packages/dev/core/src/Animations/animation.ts:577

## Properties

### \_easingFunction

• `Private` **\_easingFunction**: [`Nullable`](../modules.md#nullable)[`IEasingFunction`](../interfaces/IEasingFunction.md) = `null`

Stores the easing function of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:71

___

### \_events

• `Private` **\_events**: [`AnimationEvent`](AnimationEvent.md)[]

The set of event that will be linked to this animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:81

___

### \_keys

• `Private` **\_keys**: [`IAnimationKey`](../interfaces/IAnimationKey.md)[]

Stores the key frames of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:66

___

### \_ranges

• `Private` **\_ranges**: `Object` = `{}`

Stores the animation ranges for the animation

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

#### Defined in

packages/dev/core/src/Animations/animation.ts:96

___

### blendingSpeed

• **blendingSpeed**: `number` = `0.01`

Stores the blending speed of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:91

___

### dataType

• **dataType**: `number`

#### Defined in

packages/dev/core/src/Animations/animation.ts:585

___

### enableBlending

• `Optional` **enableBlending**: `boolean`

#### Defined in

packages/dev/core/src/Animations/animation.ts:589

___

### framePerSecond

• **framePerSecond**: `number`

#### Defined in

packages/dev/core/src/Animations/animation.ts:583

___

### loopMode

• `Optional` **loopMode**: `number`

#### Defined in

packages/dev/core/src/Animations/animation.ts:587

___

### name

• **name**: `string`

#### Defined in

packages/dev/core/src/Animations/animation.ts:579

___

### snippetId

• **snippetId**: `string`

Snippet ID if the animation was created from the snippet server

#### Defined in

packages/dev/core/src/Animations/animation.ts:61

___

### targetProperty

• **targetProperty**: `string`

#### Defined in

packages/dev/core/src/Animations/animation.ts:581

___

### targetPropertyPath

• **targetPropertyPath**: `string`[]

Stores an array of target property paths

#### Defined in

packages/dev/core/src/Animations/animation.ts:86

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the animation (the uniqueness is solely among other animations)

#### Defined in

packages/dev/core/src/Animations/animation.ts:55

___

### ANIMATIONLOOPMODE\_CONSTANT

▪ `Static` `Readonly` **ANIMATIONLOOPMODE\_CONSTANT**: ``2``

Constant Loop Mode

#### Defined in

packages/dev/core/src/Animations/animation.ts:1295

___

### ANIMATIONLOOPMODE\_CYCLE

▪ `Static` `Readonly` **ANIMATIONLOOPMODE\_CYCLE**: ``1``

Cycle Loop Mode

#### Defined in

packages/dev/core/src/Animations/animation.ts:1291

___

### ANIMATIONLOOPMODE\_RELATIVE

▪ `Static` `Readonly` **ANIMATIONLOOPMODE\_RELATIVE**: ``0``

Relative Loop Mode

#### Defined in

packages/dev/core/src/Animations/animation.ts:1287

___

### ANIMATIONTYPE\_COLOR3

▪ `Static` `Readonly` **ANIMATIONTYPE\_COLOR3**: ``4``

Color3 animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1271

___

### ANIMATIONTYPE\_COLOR4

▪ `Static` `Readonly` **ANIMATIONTYPE\_COLOR4**: ``7``

Color3 animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1275

___

### ANIMATIONTYPE\_FLOAT

▪ `Static` `Readonly` **ANIMATIONTYPE\_FLOAT**: ``0``

Float animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1255

___

### ANIMATIONTYPE\_MATRIX

▪ `Static` `Readonly` **ANIMATIONTYPE\_MATRIX**: ``3``

Matrix animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1267

___

### ANIMATIONTYPE\_QUATERNION

▪ `Static` `Readonly` **ANIMATIONTYPE\_QUATERNION**: ``2``

Quaternion animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1263

___

### ANIMATIONTYPE\_SIZE

▪ `Static` `Readonly` **ANIMATIONTYPE\_SIZE**: ``6``

Size animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1283

___

### ANIMATIONTYPE\_VECTOR2

▪ `Static` `Readonly` **ANIMATIONTYPE\_VECTOR2**: ``5``

Vector2 animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1279

___

### ANIMATIONTYPE\_VECTOR3

▪ `Static` `Readonly` **ANIMATIONTYPE\_VECTOR3**: ``1``

Vector3 animation type

#### Defined in

packages/dev/core/src/Animations/animation.ts:1259

___

### AllowMatricesInterpolation

▪ `Static` **AllowMatricesInterpolation**: `boolean` = `false`

Use matrix interpolation instead of using direct key value when animating matrices

#### Defined in

packages/dev/core/src/Animations/animation.ts:45

___

### AllowMatrixDecomposeForInterpolation

▪ `Static` **AllowMatrixDecomposeForInterpolation**: `boolean` = `true`

When matrix interpolation is enabled, this boolean forces the system to use Matrix.DecomposeLerp instead of Matrix.Lerp. Interpolation is more precise but slower

#### Defined in

packages/dev/core/src/Animations/animation.ts:50

___

### CreateFromSnippetAsync

▪ `Static` **CreateFromSnippetAsync**: (`snippetId`: `string`) => `Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[] = `Animation.ParseFromSnippetAsync`

#### Type declaration

▸ (`snippetId`): `Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

Creates an animation or an array of animations from a snippet saved by the Inspector

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snippetId` | `string` | defines the snippet to load |

##### Returns

`Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

a promise that will resolve to the new animation or a new array of animations

#### Defined in

packages/dev/core/src/Animations/animation.ts:1552

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Defined in

packages/dev/core/src/Animations/animation.ts:58

___

### \_UniqueIdGenerator

▪ `Static` `Private` **\_UniqueIdGenerator**: `number` = `0`

#### Defined in

packages/dev/core/src/Animations/animation.ts:40

## Accessors

### hasRunningRuntimeAnimations

• `get` **hasRunningRuntimeAnimations**(): `boolean`

Specifies if any of the runtime animations are currently running

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Animations/animation.ts:558

___

### runtimeAnimations

• `get` **runtimeAnimations**(): [`RuntimeAnimation`](RuntimeAnimation.md)[]

Return the array of runtime animations currently using this animation

#### Returns

[`RuntimeAnimation`](RuntimeAnimation.md)[]

#### Defined in

packages/dev/core/src/Animations/animation.ts:551

## Methods

### addEvent

▸ **addEvent**(`event`): `void`

Add an event to this animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | [`AnimationEvent`](AnimationEvent.md) | Event to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:627

___

### clone

▸ **clone**(): [`Animation`](Animation.md)

Makes a copy of the animation

#### Returns

[`Animation`](Animation.md)

Cloned animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:1126

___

### color3InterpolateFunction

▸ **color3InterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Color3`](Color3.md)

Interpolates a Color3 linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Color3`](Color3.md) | Start value of the animation curve |
| `endValue` | [`Color3`](Color3.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Color3`](Color3.md)

Interpolated Color3 value

#### Defined in

packages/dev/core/src/Animations/animation.ts:852

___

### color3InterpolateFunctionWithTangents

▸ **color3InterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): [`Color3`](Color3.md)

Interpolates a Color3 cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Color3`](Color3.md) | Start value of the animation curve |
| `outTangent` | [`Color3`](Color3.md) | End tangent of the animation |
| `endValue` | [`Color3`](Color3.md) | End value of the animation curve |
| `inTangent` | [`Color3`](Color3.md) | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Color3`](Color3.md)

interpolated value

#### Defined in

packages/dev/core/src/Animations/animation.ts:865

___

### color4InterpolateFunction

▸ **color4InterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Color4`](Color4.md)

Interpolates a Color4 linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Color4`](Color4.md) | Start value of the animation curve |
| `endValue` | [`Color4`](Color4.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Color4`](Color4.md)

Interpolated Color3 value

#### Defined in

packages/dev/core/src/Animations/animation.ts:876

___

### color4InterpolateFunctionWithTangents

▸ **color4InterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): [`Color4`](Color4.md)

Interpolates a Color4 cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Color4`](Color4.md) | Start value of the animation curve |
| `outTangent` | [`Color4`](Color4.md) | End tangent of the animation |
| `endValue` | [`Color4`](Color4.md) | End value of the animation curve |
| `inTangent` | [`Color4`](Color4.md) | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Color4`](Color4.md)

interpolated value

#### Defined in

packages/dev/core/src/Animations/animation.ts:889

___

### createRange

▸ **createRange**(`name`, `from`, `to`): `void`

Creates an animation range

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the animation range |
| `from` | `number` | Starting frame of the animation range |
| `to` | `number` | Ending frame of the animation |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:659

___

### deleteRange

▸ **deleteRange**(`name`, `deleteFrames?`): `void`

Deletes an animation range by name

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Name of the animation range to delete |
| `deleteFrames` | `boolean` | `true` | Specifies if the key frames for the range should also be deleted (true) or not (false) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:671

___

### evaluate

▸ **evaluate**(`currentFrame`): `any`

Evaluate the animation value at a given frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentFrame` | `number` | defines the frame where we want to evaluate the animation |

#### Returns

`any`

the animation value

#### Defined in

packages/dev/core/src/Animations/animation.ts:910

___

### floatInterpolateFunction

▸ **floatInterpolateFunction**(`startValue`, `endValue`, `gradient`): `number`

Interpolates a scalar linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | `number` | Start value of the animation curve |
| `endValue` | `number` | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

`number`

Interpolated scalar value

#### Defined in

packages/dev/core/src/Animations/animation.ts:745

___

### floatInterpolateFunctionWithTangents

▸ **floatInterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): `number`

Interpolates a scalar cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | `number` | Start value of the animation curve |
| `outTangent` | `number` | End tangent of the animation |
| `endValue` | `number` | End value of the animation curve |
| `inTangent` | `number` | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

`number`

Interpolated scalar value

#### Defined in

packages/dev/core/src/Animations/animation.ts:758

___

### getEasingFunction

▸ **getEasingFunction**(): [`Nullable`](../modules.md#nullable)[`IEasingFunction`](../interfaces/IEasingFunction.md)

Gets the easing function of the animation

#### Returns

[`Nullable`](../modules.md#nullable)[`IEasingFunction`](../interfaces/IEasingFunction.md)

Easing function of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:726

___

### getEvents

▸ **getEvents**(): [`AnimationEvent`](AnimationEvent.md)[]

Retrieves all the events from the animation

#### Returns

[`AnimationEvent`](AnimationEvent.md)[]

Events from the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:649

___

### getHighestFrame

▸ **getHighestFrame**(): `number`

Gets the highest frame rate of the animation

#### Returns

`number`

Highest frame rate of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:711

___

### getKeys

▸ **getKeys**(): [`IAnimationKey`](../interfaces/IAnimationKey.md)[]

Gets the key frames from the animation

#### Returns

[`IAnimationKey`](../interfaces/IAnimationKey.md)[]

The key frames of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:703

___

### getRange

▸ **getRange**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

Gets the animation range by name, or null if not defined

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the animation range |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

Nullable animation range

#### Defined in

packages/dev/core/src/Animations/animation.ts:695

___

### matrixInterpolateFunction

▸ **matrixInterpolateFunction**(`startValue`, `endValue`, `gradient`, `result?`): [`Matrix`](Matrix.md)

Defines the function to use to interpolate matrices

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Matrix`](Matrix.md) | defines the start matrix |
| `endValue` | [`Matrix`](Matrix.md) | defines the end matrix |
| `gradient` | `number` | defines the gradient between both matrices |
| `result?` | [`Matrix`](Matrix.md) | defines an optional target matrix where to store the interpolation |

#### Returns

[`Matrix`](Matrix.md)

the interpolated matrix

#### Defined in

packages/dev/core/src/Animations/animation.ts:1106

___

### quaternionInterpolateFunction

▸ **quaternionInterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Quaternion`](Quaternion.md)

Interpolates a quaternion using a spherical linear interpolation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Quaternion`](Quaternion.md) | Start value of the animation curve |
| `endValue` | [`Quaternion`](Quaternion.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Quaternion`](Quaternion.md)

Interpolated quaternion value

#### Defined in

packages/dev/core/src/Animations/animation.ts:769

___

### quaternionInterpolateFunctionWithTangents

▸ **quaternionInterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): [`Quaternion`](Quaternion.md)

Interpolates a quaternion cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Quaternion`](Quaternion.md) | Start value of the animation curve |
| `outTangent` | [`Quaternion`](Quaternion.md) | End tangent of the animation curve |
| `endValue` | [`Quaternion`](Quaternion.md) | End value of the animation curve |
| `inTangent` | [`Quaternion`](Quaternion.md) | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Quaternion`](Quaternion.md)

Interpolated quaternion value

#### Defined in

packages/dev/core/src/Animations/animation.ts:782

___

### removeEvents

▸ **removeEvents**(`frame`): `void`

Remove all events found at the given frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `number` | The frame to remove events from |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:636

___

### serialize

▸ **serialize**(): `any`

Serializes the animation to an object

#### Returns

`any`

Serialized object

#### Defined in

packages/dev/core/src/Animations/animation.ts:1162

___

### setEasingFunction

▸ **setEasingFunction**(`easingFunction`): `void`

Sets the easing function of the animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `easingFunction` | [`Nullable`](../modules.md#nullable)[`IEasingFunction`](../interfaces/IEasingFunction.md) | A custom mathematical formula for animation |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:734

___

### setKeys

▸ **setKeys**(`values`): `void`

Sets the key frames of the animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `values` | [`IAnimationKey`](../interfaces/IAnimationKey.md)[] | The animation key frames to set |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:1154

___

### sizeInterpolateFunction

▸ **sizeInterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Size`](Size.md)

Interpolates a size linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Size`](Size.md) | Start value of the animation curve |
| `endValue` | [`Size`](Size.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate |

#### Returns

[`Size`](Size.md)

Interpolated Size value

#### Defined in

packages/dev/core/src/Animations/animation.ts:841

___

### toString

▸ **toString**(`fullDetails?`): `string`

Converts the animation to a string

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | support for multiple levels of logging within scene loading |

#### Returns

`string`

String form of the animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:603

___

### vector2InterpolateFunction

▸ **vector2InterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Vector2`](Vector2.md)

Interpolates a Vector2 linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Vector2`](Vector2.md) | Start value of the animation curve |
| `endValue` | [`Vector2`](Vector2.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate (value between 0 and 1) |

#### Returns

[`Vector2`](Vector2.md)

Interpolated Vector2 value

#### Defined in

packages/dev/core/src/Animations/animation.ts:817

___

### vector2InterpolateFunctionWithTangents

▸ **vector2InterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): [`Vector2`](Vector2.md)

Interpolates a Vector2 cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Vector2`](Vector2.md) | Start value of the animation curve |
| `outTangent` | [`Vector2`](Vector2.md) | End tangent of the animation |
| `endValue` | [`Vector2`](Vector2.md) | End value of the animation curve |
| `inTangent` | [`Vector2`](Vector2.md) | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate (value between 0 and 1) |

#### Returns

[`Vector2`](Vector2.md)

Interpolated Vector2 value

#### Defined in

packages/dev/core/src/Animations/animation.ts:830

___

### vector3InterpolateFunction

▸ **vector3InterpolateFunction**(`startValue`, `endValue`, `gradient`): [`Vector3`](Vector3.md)

Interpolates a Vector3 linearly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Vector3`](Vector3.md) | Start value of the animation curve |
| `endValue` | [`Vector3`](Vector3.md) | End value of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate (value between 0 and 1) |

#### Returns

[`Vector3`](Vector3.md)

Interpolated scalar value

#### Defined in

packages/dev/core/src/Animations/animation.ts:793

___

### vector3InterpolateFunctionWithTangents

▸ **vector3InterpolateFunctionWithTangents**(`startValue`, `outTangent`, `endValue`, `inTangent`, `gradient`): [`Vector3`](Vector3.md)

Interpolates a Vector3 cubically

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`Vector3`](Vector3.md) | Start value of the animation curve |
| `outTangent` | [`Vector3`](Vector3.md) | End tangent of the animation |
| `endValue` | [`Vector3`](Vector3.md) | End value of the animation curve |
| `inTangent` | [`Vector3`](Vector3.md) | Start tangent of the animation curve |
| `gradient` | `number` | Scalar amount to interpolate (value between 0 and 1) |

#### Returns

[`Vector3`](Vector3.md)

InterpolatedVector3 value

#### Defined in

packages/dev/core/src/Animations/animation.ts:806

___

### AppendSerializedAnimations

▸ `Static` **AppendSerializedAnimations**(`source`, `destination`): `void`

Appends the serialized animations from the source animations

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`IAnimatable`](../interfaces/IAnimatable.md) | Source containing the animations |
| `destination` | `any` | Target to store the animations |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animation.ts:1456

___

### CreateAndStartAnimation

▸ `Static` **CreateAndStartAnimation**(`name`, `target`, `targetProperty`, `framePerSecond`, `totalFrame`, `from`, `to`, `loopMode?`, `easingFunction?`, `onAnimationEnd?`, `scene?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Create and start an animation on a node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the global animation that will be run on all nodes |
| `target` | `any` | defines the target where the animation will take place |
| `targetProperty` | `string` | defines property to animate |
| `framePerSecond` | `number` | defines the number of frame per second yo use |
| `totalFrame` | `number` | defines the number of frames in total |
| `from` | `any` | defines the initial value |
| `to` | `any` | defines the final value |
| `loopMode?` | `number` | defines which loop mode you want to use (off by default) |
| `easingFunction?` | [`EasingFunction`](EasingFunction.md) | defines the easing function to use (linear by default) |
| `onAnimationEnd?` | () => `void` | defines the callback to call when animation end |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

the animatable created for this animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:187

___

### CreateAndStartHierarchyAnimation

▸ `Static` **CreateAndStartHierarchyAnimation**(`name`, `node`, `directDescendantsOnly`, `targetProperty`, `framePerSecond`, `totalFrame`, `from`, `to`, `loopMode?`, `easingFunction?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)[]

Create and start an animation on a node and its descendants

**`Example`**

```ts
https://www.babylonjs-playground.com/#MH0VLI
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the global animation that will be run on all nodes |
| `node` | [`Node`](Node.md) | defines the root node where the animation will take place |
| `directDescendantsOnly` | `boolean` | if true only direct descendants will be used, if false direct and also indirect (children of children, an so on in a recursive manner) descendants will be used |
| `targetProperty` | `string` | defines property to animate |
| `framePerSecond` | `number` | defines the number of frame per second to use |
| `totalFrame` | `number` | defines the number of frames in total |
| `from` | `any` | defines the initial value |
| `to` | `any` | defines the final value |
| `loopMode?` | `number` | defines which loop mode you want to use (off by default) |
| `easingFunction?` | [`EasingFunction`](EasingFunction.md) | defines the easing function to use (linear by default) |
| `onAnimationEnd?` | () => `void` | defines the callback to call when an animation ends (will be called once per node) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)[]

the list of animatables created for all nodes

#### Defined in

packages/dev/core/src/Animations/animation.ts:233

___

### CreateAnimation

▸ `Static` **CreateAnimation**(`property`, `animationType`, `framePerSecond`, `easingFunction`): [`Animation`](Animation.md)

Sets up an animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `string` | The property to animate |
| `animationType` | `number` | The animation type to apply |
| `framePerSecond` | `number` | The frames per second of the animation |
| `easingFunction` | [`EasingFunction`](EasingFunction.md) | The easing function used in the animation |

#### Returns

[`Animation`](Animation.md)

The created animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:164

___

### CreateMergeAndStartAnimation

▸ `Static` **CreateMergeAndStartAnimation**(`name`, `node`, `targetProperty`, `framePerSecond`, `totalFrame`, `from`, `to`, `loopMode?`, `easingFunction?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Creates a new animation, merges it with the existing animations and starts it

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the animation |
| `node` | [`Node`](Node.md) | Node which contains the scene that begins the animations |
| `targetProperty` | `string` | Specifies which property to animate |
| `framePerSecond` | `number` | The frames per second of the animation |
| `totalFrame` | `number` | The total number of frames |
| `from` | `any` | The frame at the beginning of the animation |
| `to` | `any` | The frame at the end of the animation |
| `loopMode?` | `number` | Specifies the loop mode of the animation |
| `easingFunction?` | [`EasingFunction`](EasingFunction.md) | (Optional) The easing function of the animation, which allow custom mathematical formulas for animations |
| `onAnimationEnd?` | () => `void` | Callback to run once the animation is complete |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Nullable animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:270

___

### MakeAnimationAdditive

▸ `Static` **MakeAnimationAdditive**(`sourceAnimation`, `referenceFrame?`, `range?`, `cloneOriginal?`, `clonedName?`): [`Animation`](Animation.md)

Convert the keyframes for all animations belonging to the group to be relative to a given reference frame.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sourceAnimation` | [`Animation`](Animation.md) | `undefined` | defines the Animation containing keyframes to convert |
| `referenceFrame` | `number` | `0` | defines the frame that keyframes in the range will be relative to |
| `range?` | `string` | `undefined` | defines the name of the AnimationRange belonging to the Animation to convert |
| `cloneOriginal` | `boolean` | `false` | defines whether or not to clone the animation and convert the clone or convert the original animation (default is false) |
| `clonedName?` | `string` | `undefined` | defines the name of the resulting cloned Animation if cloneOriginal is true |

#### Returns

[`Animation`](Animation.md)

a new Animation if cloneOriginal is true or the original Animation if cloneOriginal is false

#### Defined in

packages/dev/core/src/Animations/animation.ts:302

___

### Parse

▸ `Static` **Parse**(`parsedAnimation`): [`Animation`](Animation.md)

Parses an animation object and creates an animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedAnimation` | `any` | Parsed animation object |

#### Returns

[`Animation`](Animation.md)

Animation object

#### Defined in

packages/dev/core/src/Animations/animation.ts:1325

___

### ParseFromFileAsync

▸ `Static` **ParseFromFileAsync**(`name`, `url`): `Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

Creates a new animation or an array of animations from a snippet saved in a remote file

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | [`Nullable`](../modules.md#nullable)`string` | defines the name of the animation to create (can be null or empty to use the one from the json data) |
| `url` | `string` | defines the url to load from |

#### Returns

`Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

a promise that will resolve to the new animation or an array of animations

#### Defined in

packages/dev/core/src/Animations/animation.ts:1466

___

### ParseFromSnippetAsync

▸ `Static` **ParseFromSnippetAsync**(`snippetId`): `Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

Creates an animation or an array of animations from a snippet saved by the Inspector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snippetId` | `string` | defines the snippet to load |

#### Returns

`Promise`[`Animation`](Animation.md) \| [`Animation`](Animation.md)[]

a promise that will resolve to the new animation or a new array of animations

#### Defined in

packages/dev/core/src/Animations/animation.ts:1509

___

### TransitionTo

▸ `Static` **TransitionTo**(`property`, `targetValue`, `host`, `scene`, `frameRate`, `transition`, `duration`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Transition property of an host to the target Value

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `property` | `string` | `undefined` | The property to transition |
| `targetValue` | `any` | `undefined` | The target Value of the property |
| `host` | `any` | `undefined` | The object where the property to animate belongs |
| `scene` | [`Scene`](Scene.md) | `undefined` | Scene used to run the animation |
| `frameRate` | `number` | `undefined` | Framerate (in frame/s) to use |
| `transition` | [`Animation`](Animation.md) | `undefined` | The transition type we want to use |
| `duration` | `number` | `undefined` | The duration of the animation, in milliseconds |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback trigger at the end of the animation |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Nullable animation

#### Defined in

packages/dev/core/src/Animations/animation.ts:506

[@dev/core](../README.md) / [Exports](../modules.md) / AnimationGroup

# Class: AnimationGroup

Use this class to create coordinated animations on multiple targets

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](AnimationGroup.md#constructor)

### Properties

- [\_animatables](AnimationGroup.md#_animatables)
- [\_animationLoopCount](AnimationGroup.md#_animationloopcount)
- [\_animationLoopFlags](AnimationGroup.md#_animationloopflags)
- [\_from](AnimationGroup.md#_from)
- [\_isAdditive](AnimationGroup.md#_isadditive)
- [\_isPaused](AnimationGroup.md#_ispaused)
- [\_isStarted](AnimationGroup.md#_isstarted)
- [\_loopAnimation](AnimationGroup.md#_loopanimation)
- [\_scene](AnimationGroup.md#_scene)
- [\_speedRatio](AnimationGroup.md#_speedratio)
- [\_targetedAnimations](AnimationGroup.md#_targetedanimations)
- [\_to](AnimationGroup.md#_to)
- [metadata](AnimationGroup.md#metadata)
- [name](AnimationGroup.md#name)
- [onAnimationEndObservable](AnimationGroup.md#onanimationendobservable)
- [onAnimationGroupEndObservable](AnimationGroup.md#onanimationgroupendobservable)
- [onAnimationGroupLoopObservable](AnimationGroup.md#onanimationgrouploopobservable)
- [onAnimationGroupPauseObservable](AnimationGroup.md#onanimationgrouppauseobservable)
- [onAnimationGroupPlayObservable](AnimationGroup.md#onanimationgroupplayobservable)
- [onAnimationLoopObservable](AnimationGroup.md#onanimationloopobservable)
- [uniqueId](AnimationGroup.md#uniqueid)

### Accessors

- [animatables](AnimationGroup.md#animatables)
- [children](AnimationGroup.md#children)
- [from](AnimationGroup.md#from)
- [isAdditive](AnimationGroup.md#isadditive)
- [isPlaying](AnimationGroup.md#isplaying)
- [isStarted](AnimationGroup.md#isstarted)
- [loopAnimation](AnimationGroup.md#loopanimation)
- [speedRatio](AnimationGroup.md#speedratio)
- [targetedAnimations](AnimationGroup.md#targetedanimations)
- [to](AnimationGroup.md#to)

### Methods

- [\_checkAnimationGroupEnded](AnimationGroup.md#_checkanimationgroupended)
- [\_processLoop](AnimationGroup.md#_processloop)
- [addTargetedAnimation](AnimationGroup.md#addtargetedanimation)
- [clone](AnimationGroup.md#clone)
- [dispose](AnimationGroup.md#dispose)
- [getClassName](AnimationGroup.md#getclassname)
- [goToFrame](AnimationGroup.md#gotoframe)
- [normalize](AnimationGroup.md#normalize)
- [pause](AnimationGroup.md#pause)
- [play](AnimationGroup.md#play)
- [reset](AnimationGroup.md#reset)
- [restart](AnimationGroup.md#restart)
- [serialize](AnimationGroup.md#serialize)
- [setWeightForAllAnimatables](AnimationGroup.md#setweightforallanimatables)
- [start](AnimationGroup.md#start)
- [stop](AnimationGroup.md#stop)
- [syncAllAnimationsWith](AnimationGroup.md#syncallanimationswith)
- [toString](AnimationGroup.md#tostring)
- [MakeAnimationAdditive](AnimationGroup.md#makeanimationadditive)
- [Parse](AnimationGroup.md#parse)

## Constructors

### constructor

• **new AnimationGroup**(`name`, `scene?`)

Instantiates a new Animation Group.
This helps managing several animations at once.

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/groupAnimations

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Defines the name of the group |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `null` | Defines the scene the group belongs to |

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:225

## Properties

### \_animatables

• `Private` **\_animatables**: [`Animatable`](Animatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:54

___

### \_animationLoopCount

• `Private` **\_animationLoopCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:311

___

### \_animationLoopFlags

• `Private` **\_animationLoopFlags**: `boolean`[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:312

___

### \_from

• `Private` **\_from**: `number` = `Number.MAX_VALUE`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:55

___

### \_isAdditive

• `Private` **\_isAdditive**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:61

___

### \_isPaused

• `Private` **\_isPaused**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:58

___

### \_isStarted

• `Private` **\_isStarted**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:57

___

### \_loopAnimation

• `Private` **\_loopAnimation**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:60

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:51

___

### \_speedRatio

• `Private` **\_speedRatio**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:59

___

### \_targetedAnimations

• `Private` **\_targetedAnimations**: [`TargetedAnimation`](TargetedAnimation.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:53

___

### \_to

• `Private` **\_to**: `number` = `-Number.MAX_VALUE`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:56

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:104

___

### name

• **name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:227

___

### onAnimationEndObservable

• **onAnimationEndObservable**: [`Observable`](Observable.md)[`TargetedAnimation`](TargetedAnimation.md)

This observable will notify when one animation have ended

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:74

___

### onAnimationGroupEndObservable

• **onAnimationGroupEndObservable**: [`Observable`](Observable.md)[`AnimationGroup`](AnimationGroup.md)

This observable will notify when all animations have ended.

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:89

___

### onAnimationGroupLoopObservable

• **onAnimationGroupLoopObservable**: [`Observable`](Observable.md)[`AnimationGroup`](AnimationGroup.md)

Observer raised when all animations have looped

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:84

___

### onAnimationGroupPauseObservable

• **onAnimationGroupPauseObservable**: [`Observable`](Observable.md)[`AnimationGroup`](AnimationGroup.md)

This observable will notify when all animations have paused.

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:94

___

### onAnimationGroupPlayObservable

• **onAnimationGroupPlayObservable**: [`Observable`](Observable.md)[`AnimationGroup`](AnimationGroup.md)

This observable will notify when all animations are playing.

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:99

___

### onAnimationLoopObservable

• **onAnimationLoopObservable**: [`Observable`](Observable.md)[`TargetedAnimation`](TargetedAnimation.md)

Observer raised when one animation loops

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:79

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:69

## Accessors

### animatables

• `get` **animatables**(): [`Animatable`](Animatable.md)[]

returning the list of animatables controlled by this animation group.

#### Returns

[`Animatable`](Animatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:207

___

### children

• `get` **children**(): [`TargetedAnimation`](TargetedAnimation.md)[]

Gets the list of target animations

#### Returns

[`TargetedAnimation`](TargetedAnimation.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:214

___

### from

• `get` **from**(): `number`

Gets the first frame

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:109

___

### isAdditive

• `get` **isAdditive**(): `boolean`

Gets or sets if all animations should be evaluated additively

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:180

• `set` **isAdditive**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:184

___

### isPlaying

• `get` **isPlaying**(): `boolean`

Gets a value indicating that the current group is playing

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:130

___

### isStarted

• `get` **isStarted**(): `boolean`

Define if the animations are started

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:123

___

### loopAnimation

• `get` **loopAnimation**(): `boolean`

Gets or sets if all animations should loop or not

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:160

• `set` **loopAnimation**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:164

___

### speedRatio

• `get` **speedRatio**(): `number`

Gets or sets the speed ratio to use for all animations

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:137

• `set` **speedRatio**(`value`): `void`

Gets or sets the speed ratio to use for all animations

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:144

___

### targetedAnimations

• `get` **targetedAnimations**(): [`TargetedAnimation`](TargetedAnimation.md)[]

Gets the targeted animations for this animation group

#### Returns

[`TargetedAnimation`](TargetedAnimation.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:200

___

### to

• `get` **to**(): `number`

Gets the last frame

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:116

## Methods

### \_checkAnimationGroupEnded

▸ `Private` **_checkAnimationGroupEnded**(`animatable`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `animatable` | [`Animatable`](Animatable.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:564

___

### \_processLoop

▸ `Private` **_processLoop**(`animatable`, `targetedAnimation`, `index`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `animatable` | [`Animatable`](Animatable.md) |
| `targetedAnimation` | [`TargetedAnimation`](TargetedAnimation.md) |
| `index` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:314

___

### addTargetedAnimation

▸ **addTargetedAnimation**(`animation`, `target`): [`TargetedAnimation`](TargetedAnimation.md)

Add an animation (with its target) in the group

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `animation` | [`Animation`](Animation.md) | defines the animation we want to add |
| `target` | `any` | defines the target of the animation |

#### Returns

[`TargetedAnimation`](TargetedAnimation.md)

the TargetedAnimation object

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:242

___

### clone

▸ **clone**(`newName`, `targetConverter?`, `cloneAnimations?`): [`AnimationGroup`](AnimationGroup.md)

Clone the current animation group and returns a copy

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newName` | `string` | `undefined` | defines the name of the new group |
| `targetConverter?` | (`oldTarget`: `any`) => `any` | `undefined` | defines an optional function used to convert current animation targets to new ones |
| `cloneAnimations` | `boolean` | `false` | defines if the animations should be cloned or referenced |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the new animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:585

___

### dispose

▸ **dispose**(): `void`

Dispose all associated resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:537

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "AnimationGroup"

#### Returns

`string`

"AnimationGroup"

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:699

___

### goToFrame

▸ **goToFrame**(`frame`): [`AnimationGroup`](AnimationGroup.md)

Goes to a specific frame in this animation group

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `number` | the frame number to go to |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animationGroup

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:521

___

### normalize

▸ **normalize**(`beginFrame?`, `endFrame?`): [`AnimationGroup`](AnimationGroup.md)

This function will normalize every animation in the group to make sure they all go from beginFrame to endFrame
It can add constant keys at begin or end

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `beginFrame` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the new begin frame for all animations or the smallest begin frame of all animations if null (defaults to null) |
| `endFrame` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the new end frame for all animations or the largest end frame of all animations if null (defaults to null) |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:268

___

### pause

▸ **pause**(): [`AnimationGroup`](AnimationGroup.md)

Pause all animations

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:388

___

### play

▸ **play**(`loop?`): [`AnimationGroup`](AnimationGroup.md)

Play all animations to initial state
This function will start() the animations if they were not started or will restart() them if they were paused

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `loop?` | `boolean` | defines if animations must loop |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:411

___

### reset

▸ **reset**(): [`AnimationGroup`](AnimationGroup.md)

Reset all animations to initial state

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:432

___

### restart

▸ **restart**(): [`AnimationGroup`](AnimationGroup.md)

Restart animations from key 0

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:452

___

### serialize

▸ **serialize**(): `any`

Serializes the animationGroup to an object

#### Returns

`any`

Serialized object

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:602

___

### setWeightForAllAnimatables

▸ **setWeightForAllAnimatables**(`weight`): [`AnimationGroup`](AnimationGroup.md)

Set animation weight for all animatables

**`See`**

https://doc.babylonjs.com/babylon101/animations#animation-weights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `weight` | `number` | defines the weight to use |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animationGroup

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:492

___

### start

▸ **start**(`loop?`, `speedRatio?`, `from?`, `to?`, `isAdditive?`): [`AnimationGroup`](AnimationGroup.md)

Start all animations on given targets

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `loop` | `boolean` | `false` | defines if animations must loop |
| `speedRatio` | `number` | `1` | defines the ratio to apply to animation speed (1 by default) |
| `from?` | `number` | `undefined` | defines the from key (optional) |
| `to?` | `number` | `undefined` | defines the to key (optional) |
| `isAdditive?` | `boolean` | `undefined` | defines the additive state for the resulting animatables (optional) |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the current animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:342

___

### stop

▸ **stop**(): [`AnimationGroup`](AnimationGroup.md)

Stop all animations

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animation group

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:471

___

### syncAllAnimationsWith

▸ **syncAllAnimationsWith**(`root`): [`AnimationGroup`](AnimationGroup.md)

Synchronize and normalize all animatables with a source animatable

**`See`**

https://doc.babylonjs.com/babylon101/animations#animation-weights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `root` | [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md) | defines the root animatable to synchronize with (null to stop synchronizing) |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

the animationGroup

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:507

___

### toString

▸ **toString**(`fullDetails?`): `string`

Creates a detailed string about the object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | defines if the output string will support multiple levels of logging within scene loading |

#### Returns

`string`

a string representing the object

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:708

___

### MakeAnimationAdditive

▸ `Static` **MakeAnimationAdditive**(`sourceAnimationGroup`, `referenceFrame?`, `range?`, `cloneOriginal?`, `clonedName?`): [`AnimationGroup`](AnimationGroup.md)

Convert the keyframes for all animations belonging to the group to be relative to a given reference frame.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sourceAnimationGroup` | [`AnimationGroup`](AnimationGroup.md) | `undefined` | defines the AnimationGroup containing animations to convert |
| `referenceFrame` | `number` | `0` | defines the frame that keyframes in the range will be relative to |
| `range?` | `string` | `undefined` | defines the name of the AnimationRange belonging to the animations in the group to convert |
| `cloneOriginal` | `boolean` | `false` | defines whether or not to clone the group and convert the clone or convert the original group (default is false) |
| `clonedName?` | `string` | `undefined` | defines the name of the resulting cloned AnimationGroup if cloneOriginal is true |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

a new AnimationGroup if cloneOriginal is true or the original AnimationGroup if cloneOriginal is false

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:678

___

### Parse

▸ `Static` **Parse**(`parsedAnimationGroup`, `scene`): [`AnimationGroup`](AnimationGroup.md)

Returns a new AnimationGroup object parsed from the source provided.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedAnimationGroup` | `any` | defines the source |
| `scene` | [`Scene`](Scene.md) | defines the scene that will receive the animationGroup |

#### Returns

[`AnimationGroup`](AnimationGroup.md)

a new AnimationGroup

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationGroup.ts:633

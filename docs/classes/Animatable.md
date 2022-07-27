[@dev/core](../README.md) / [Exports](../modules.md) / Animatable

# Class: Animatable

Class used to store an actual running animation

## Table of contents

### Constructors

- [constructor](Animatable.md#constructor)

### Properties

- [\_frameToSyncFromJump](Animatable.md#_frametosyncfromjump)
- [\_localDelayOffset](Animatable.md#_localdelayoffset)
- [\_manualJumpDelay](Animatable.md#_manualjumpdelay)
- [\_paused](Animatable.md#_paused)
- [\_pausedDelay](Animatable.md#_pauseddelay)
- [\_runtimeAnimations](Animatable.md#_runtimeanimations)
- [\_scene](Animatable.md#_scene)
- [\_speedRatio](Animatable.md#_speedratio)
- [\_syncRoot](Animatable.md#_syncroot)
- [\_weight](Animatable.md#_weight)
- [animationStarted](Animatable.md#animationstarted)
- [disposeOnEnd](Animatable.md#disposeonend)
- [fromFrame](Animatable.md#fromframe)
- [isAdditive](Animatable.md#isadditive)
- [loopAnimation](Animatable.md#loopanimation)
- [onAnimationEnd](Animatable.md#onanimationend)
- [onAnimationEndObservable](Animatable.md#onanimationendobservable)
- [onAnimationLoop](Animatable.md#onanimationloop)
- [onAnimationLoopObservable](Animatable.md#onanimationloopobservable)
- [target](Animatable.md#target)
- [toFrame](Animatable.md#toframe)

### Accessors

- [masterFrame](Animatable.md#masterframe)
- [speedRatio](Animatable.md#speedratio)
- [syncRoot](Animatable.md#syncroot)
- [weight](Animatable.md#weight)

### Methods

- [\_raiseOnAnimationEnd](Animatable.md#_raiseonanimationend)
- [appendAnimations](Animatable.md#appendanimations)
- [disableBlending](Animatable.md#disableblending)
- [enableBlending](Animatable.md#enableblending)
- [getAnimationByTargetProperty](Animatable.md#getanimationbytargetproperty)
- [getAnimations](Animatable.md#getanimations)
- [getRuntimeAnimationByTargetProperty](Animatable.md#getruntimeanimationbytargetproperty)
- [goToFrame](Animatable.md#gotoframe)
- [pause](Animatable.md#pause)
- [reset](Animatable.md#reset)
- [restart](Animatable.md#restart)
- [stop](Animatable.md#stop)
- [syncWith](Animatable.md#syncwith)
- [waitAsync](Animatable.md#waitasync)

## Constructors

### constructor

• **new Animatable**(`scene`, `target`, `fromFrame?`, `toFrame?`, `loopAnimation?`, `speedRatio?`, `onAnimationEnd?`, `animations?`, `onAnimationLoop?`, `isAdditive?`)

Creates a new Animatable

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `target` | `any` | `undefined` | defines the target object |
| `fromFrame` | `number` | `0` | defines the starting frame number (default is 0) |
| `toFrame` | `number` | `100` | defines the ending frame number (default is 100) |
| `loopAnimation` | `boolean` | `false` | defines if the animation must loop (default is false) |
| `speedRatio` | `number` | `1.0` | defines the factor to apply to animation speed (default is 1) |
| `onAnimationEnd?` | [`Nullable`](../modules.md#nullable)() => `void` | `undefined` | defines a callback to call when animation ends if it is not looping |
| `animations?` | [`Animation`](Animation.md)[] | `undefined` | defines a group of animation to add to the new Animatable |
| `onAnimationLoop?` | [`Nullable`](../modules.md#nullable)() => `void` | `undefined` | defines a callback to call when animation loops |
| `isAdditive` | `boolean` | `false` | defines whether the animation should be evaluated additively |

#### Defined in

packages/dev/core/src/Animations/animatable.ts:114

## Properties

### \_frameToSyncFromJump

• `Private` **\_frameToSyncFromJump**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:25

___

### \_localDelayOffset

• `Private` **\_localDelayOffset**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:16

___

### \_manualJumpDelay

• `Private` **\_manualJumpDelay**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:18

___

### \_paused

• `Private` **\_paused**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:20

___

### \_pausedDelay

• `Private` **\_pausedDelay**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:17

___

### \_runtimeAnimations

• `Private` **\_runtimeAnimations**: [`RuntimeAnimation`](RuntimeAnimation.md)[]

#### Defined in

packages/dev/core/src/Animations/animatable.ts:19

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Animations/animatable.ts:21

___

### \_speedRatio

• `Private` **\_speedRatio**: `number` = `1`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:22

___

### \_syncRoot

• `Private` **\_syncRoot**: [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md) = `null`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:24

___

### \_weight

• `Private` **\_weight**: `number` = `-1.0`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:23

___

### animationStarted

• **animationStarted**: `boolean` = `false`

Gets a boolean indicating if the animation has started

#### Defined in

packages/dev/core/src/Animations/animatable.ts:36

___

### disposeOnEnd

• **disposeOnEnd**: `boolean` = `true`

Gets or sets a boolean indicating if the animatable must be disposed and removed at the end of the animation.
This will only apply for non looping animation (default is true)

#### Defined in

packages/dev/core/src/Animations/animatable.ts:31

___

### fromFrame

• **fromFrame**: `number` = `0`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:119

___

### isAdditive

• **isAdditive**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:131

___

### loopAnimation

• **loopAnimation**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:123

___

### onAnimationEnd

• `Optional` **onAnimationEnd**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:126

___

### onAnimationEndObservable

• **onAnimationEndObservable**: [`Observable`](Observable.md)[`Animatable`](Animatable.md)

Observer raised when the animation ends

#### Defined in

packages/dev/core/src/Animations/animatable.ts:41

___

### onAnimationLoop

• `Optional` **onAnimationLoop**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:129

___

### onAnimationLoopObservable

• **onAnimationLoopObservable**: [`Observable`](Observable.md)[`Animatable`](Animatable.md)

Observer raised when the animation loops

#### Defined in

packages/dev/core/src/Animations/animatable.ts:46

___

### target

• **target**: `any`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:117

___

### toFrame

• **toFrame**: `number` = `100`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:121

## Accessors

### masterFrame

• `get` **masterFrame**(): `number`

Gets the current frame of the first RuntimeAnimation
Used to synchronize Animatables

#### Returns

`number`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:59

___

### speedRatio

• `get` **speedRatio**(): `number`

Gets or sets the speed ratio to apply to the animatable (1.0 by default)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:88

• `set` **speedRatio**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:92

___

### syncRoot

• `get` **syncRoot**(): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Gets the root Animatable used to synchronize and normalize animations

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

#### Defined in

packages/dev/core/src/Animations/animatable.ts:51

___

### weight

• `get` **weight**(): `number`

Gets or sets the animatable weight (-1.0 by default meaning not weighted)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:70

• `set` **weight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:74

## Methods

### \_raiseOnAnimationEnd

▸ `Private` **_raiseOnAnimationEnd**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:303

___

### appendAnimations

▸ **appendAnimations**(`target`, `animations`): `void`

Adds more animations to the current animatable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target of the animations |
| `animations` | [`Animation`](Animation.md)[] | defines the new animations to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:177

___

### disableBlending

▸ **disableBlending**(): `void`

Disable animation blending

**`See`**

https://doc.babylonjs.com/babylon101/animations#animation-blending

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:259

___

### enableBlending

▸ **enableBlending**(`blendingSpeed`): `void`

Allows the animatable to blend with current running animations

**`See`**

https://doc.babylonjs.com/babylon101/animations#animation-blending

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blendingSpeed` | `number` | defines the blending speed to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:246

___

### getAnimationByTargetProperty

▸ **getAnimationByTargetProperty**(`property`): [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

Gets the source animation for a specific property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `string` | defines the property to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

null or the source animation for the given property

#### Defined in

packages/dev/core/src/Animations/animatable.ts:198

___

### getAnimations

▸ **getAnimations**(): [`RuntimeAnimation`](RuntimeAnimation.md)[]

Gets the list of runtime animations

#### Returns

[`RuntimeAnimation`](RuntimeAnimation.md)[]

an array of RuntimeAnimation

#### Defined in

packages/dev/core/src/Animations/animatable.ts:168

___

### getRuntimeAnimationByTargetProperty

▸ **getRuntimeAnimationByTargetProperty**(`property`): [`Nullable`](../modules.md#nullable)[`RuntimeAnimation`](RuntimeAnimation.md)

Gets the runtime animation for a specific property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `string` | defines the property to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`RuntimeAnimation`](RuntimeAnimation.md)

null or the runtime animation for the given property

#### Defined in

packages/dev/core/src/Animations/animatable.ts:215

___

### goToFrame

▸ **goToFrame**(`frame`): `void`

Jump directly to a given frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `number` | defines the frame to jump to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:271

___

### pause

▸ **pause**(): `void`

Pause the animation

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:289

___

### reset

▸ **reset**(): `void`

Resets the animatable to its original state

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:230

___

### restart

▸ **restart**(): `void`

Restart the animation

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:299

___

### stop

▸ **stop**(`animationName?`, `targetMask?`): `void`

Stop and delete the current animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `animationName?` | `string` | defines a string used to only stop some of the runtime animations instead of all |
| `targetMask?` | (`target`: `any`) => `boolean` | a function that determines if the animation should be stopped based on its target (all animations will be stopped if both this and animationName are empty) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animatable.ts:316

___

### syncWith

▸ **syncWith**(`root`): [`Animatable`](Animatable.md)

Synchronize and normalize current Animatable with a source Animatable
This is useful when using animation weights and when animations are not of the same length

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `root` | [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md) | defines the root Animatable to synchronize with (null to stop synchronizing) |

#### Returns

[`Animatable`](Animatable.md)

the current Animatable

#### Defined in

packages/dev/core/src/Animations/animatable.ts:149

___

### waitAsync

▸ **waitAsync**(): `Promise`[`Animatable`](Animatable.md)

Wait asynchronously for the animation to end

#### Returns

`Promise`[`Animatable`](Animatable.md)

a promise which will be fulfilled when the animation ends

#### Defined in

packages/dev/core/src/Animations/animatable.ts:361

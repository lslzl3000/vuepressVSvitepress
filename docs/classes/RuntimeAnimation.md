[@dev/core](../README.md) / [Exports](../modules.md) / RuntimeAnimation

# Class: RuntimeAnimation

Defines a runtime animation

## Table of contents

### Constructors

- [constructor](RuntimeAnimation.md#constructor)

### Properties

- [\_activeTargets](RuntimeAnimation.md#_activetargets)
- [\_animation](RuntimeAnimation.md#_animation)
- [\_blendingFactor](RuntimeAnimation.md#_blendingfactor)
- [\_currentActiveTarget](RuntimeAnimation.md#_currentactivetarget)
- [\_currentFrame](RuntimeAnimation.md#_currentframe)
- [\_currentValue](RuntimeAnimation.md#_currentvalue)
- [\_directTarget](RuntimeAnimation.md#_directtarget)
- [\_enableBlending](RuntimeAnimation.md#_enableblending)
- [\_events](RuntimeAnimation.md#_events)
- [\_highLimitsCache](RuntimeAnimation.md#_highlimitscache)
- [\_host](RuntimeAnimation.md#_host)
- [\_keys](RuntimeAnimation.md#_keys)
- [\_maxFrame](RuntimeAnimation.md#_maxframe)
- [\_maxValue](RuntimeAnimation.md#_maxvalue)
- [\_minFrame](RuntimeAnimation.md#_minframe)
- [\_minValue](RuntimeAnimation.md#_minvalue)
- [\_offsetsCache](RuntimeAnimation.md#_offsetscache)
- [\_originalBlendValue](RuntimeAnimation.md#_originalblendvalue)
- [\_originalValue](RuntimeAnimation.md#_originalvalue)
- [\_previousDelay](RuntimeAnimation.md#_previousdelay)
- [\_previousRatio](RuntimeAnimation.md#_previousratio)
- [\_ratioOffset](RuntimeAnimation.md#_ratiooffset)
- [\_scene](RuntimeAnimation.md#_scene)
- [\_stopped](RuntimeAnimation.md#_stopped)
- [\_target](RuntimeAnimation.md#_target)
- [\_targetIsArray](RuntimeAnimation.md#_targetisarray)
- [\_targetPath](RuntimeAnimation.md#_targetpath)
- [\_weight](RuntimeAnimation.md#_weight)

### Accessors

- [animation](RuntimeAnimation.md#animation)
- [currentFrame](RuntimeAnimation.md#currentframe)
- [currentValue](RuntimeAnimation.md#currentvalue)
- [isAdditive](RuntimeAnimation.md#isadditive)
- [target](RuntimeAnimation.md#target)
- [targetPath](RuntimeAnimation.md#targetpath)
- [weight](RuntimeAnimation.md#weight)

### Methods

- [\_getCorrectLoopMode](RuntimeAnimation.md#_getcorrectloopmode)
- [\_getOriginalValues](RuntimeAnimation.md#_getoriginalvalues)
- [\_preparePath](RuntimeAnimation.md#_preparepath)
- [\_setValue](RuntimeAnimation.md#_setvalue)
- [animate](RuntimeAnimation.md#animate)
- [dispose](RuntimeAnimation.md#dispose)
- [goToFrame](RuntimeAnimation.md#gotoframe)
- [isStopped](RuntimeAnimation.md#isstopped)
- [reset](RuntimeAnimation.md#reset)
- [setValue](RuntimeAnimation.md#setvalue)

## Constructors

### constructor

• **new RuntimeAnimation**(`target`, `animation`, `scene`, `host`)

Create a new RuntimeAnimation object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target of the animation |
| `animation` | [`Animation`](Animation.md) | defines the source animation object |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `host` | [`Animatable`](Animatable.md) | defines the initiating Animatable |

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:193

## Properties

### \_activeTargets

• `Private` **\_activeTargets**: `any`[]

The active target of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:103

___

### \_animation

• `Private` **\_animation**: [`Animation`](Animation.md)

The animation used by the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:45

___

### \_blendingFactor

• `Private` **\_blendingFactor**: `number` = `0`

The blending factor of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:85

___

### \_currentActiveTarget

• `Private` **\_currentActiveTarget**: `any` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:104

___

### \_currentFrame

• `Private` **\_currentFrame**: `number` = `0`

The current frame of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:40

___

### \_currentValue

• `Private` **\_currentValue**: `any` = `null`

The current value of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:95

___

### \_directTarget

• `Private` **\_directTarget**: `any` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:105

___

### \_enableBlending

• `Private` **\_enableBlending**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:132

___

### \_events

• `Private` **\_events**: [`AnimationEvent`](AnimationEvent.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:35

___

### \_highLimitsCache

• `Private` **\_highLimitsCache**: `Object` = `{}`

The high limits cache of the runtime animation

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:75

___

### \_host

• `Private` **\_host**: [`Animatable`](Animatable.md)

The initiating animatable

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:55

___

### \_keys

• `Private` **\_keys**: [`IAnimationKey`](../interfaces/IAnimationKey.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:134

___

### \_maxFrame

• `Private` **\_maxFrame**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:136

___

### \_maxValue

• `Private` **\_maxValue**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:138

___

### \_minFrame

• `Private` **\_minFrame**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:135

___

### \_minValue

• `Private` **\_minValue**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:137

___

### \_offsetsCache

• `Private` **\_offsetsCache**: `Object` = `{}`

The offsets cache of the runtime animation

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:70

___

### \_originalBlendValue

• `Private` **\_originalBlendValue**: `any` = `null`

The original blend value of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:65

___

### \_originalValue

• `Private` **\_originalValue**: `any`[]

The original value of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:60

___

### \_previousDelay

• `Private` **\_previousDelay**: `number` = `0`

The previous delay of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:125

___

### \_previousRatio

• `Private` **\_previousRatio**: `number` = `0`

The previous ratio of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:130

___

### \_ratioOffset

• `Private` **\_ratioOffset**: `number` = `0`

The ratio offset of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:120

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

The BabylonJS scene

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:90

___

### \_stopped

• `Private` **\_stopped**: `boolean` = `false`

Specifies if the runtime animation has been stopped

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:80

___

### \_target

• `Private` **\_target**: `any`

The target of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:50

___

### \_targetIsArray

• `Private` **\_targetIsArray**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:139

___

### \_targetPath

• `Private` **\_targetPath**: `string` = `""`

The target path of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:110

___

### \_weight

• `Private` **\_weight**: `number` = `1.0`

The weight of the runtime animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:115

## Accessors

### animation

• `get` **animation**(): [`Animation`](Animation.md)

Gets the animation from the runtime animation

#### Returns

[`Animation`](Animation.md)

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:274

___

### currentFrame

• `get` **currentFrame**(): `number`

Gets the current frame of the runtime animation

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:144

___

### currentValue

• `get` **currentValue**(): `any`

Gets the current value of the runtime animation

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:158

___

### isAdditive

• `get` **isAdditive**(): `boolean`

Gets the additive state of the runtime animation

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:179

___

### target

• `get` **target**(): `any`

Gets the actual target of the runtime animation

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:172

___

### targetPath

• `get` **targetPath**(): `string`

Gets or sets the target path of the runtime animation

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:165

___

### weight

• `get` **weight**(): `number`

Gets the weight of the runtime animation

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:151

## Methods

### \_getCorrectLoopMode

▸ `Private` **_getCorrectLoopMode**(): `undefined` \| `number`

Gets the loop pmode of the runtime animation

#### Returns

`undefined` \| `number`

Loop Mode

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:430

___

### \_getOriginalValues

▸ `Private` **_getOriginalValues**(`targetIndex?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `targetIndex` | `number` | `0` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:345

___

### \_preparePath

▸ `Private` **_preparePath**(`target`, `targetIndex?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `target` | `any` | `undefined` |
| `targetIndex` | `number` | `0` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:253

___

### \_setValue

▸ `Private` **_setValue**(`target`, `destination`, `currentValue`, `weight`, `targetIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `destination` | `any` |
| `currentValue` | `any` |
| `weight` | `number` |
| `targetIndex` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:363

___

### animate

▸ **animate**(`delay`, `from`, `to`, `loop`, `speedRatio`, `weight?`): `boolean`

Execute the current animation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `delay` | `number` | `undefined` | defines the delay to add to the current frame |
| `from` | `number` | `undefined` | defines the lower bound of the animation range |
| `to` | `number` | `undefined` | defines the upper bound of the animation range |
| `loop` | `boolean` | `undefined` | defines if the current animation must loop |
| `speedRatio` | `number` | `undefined` | defines the current speed ratio |
| `weight` | `number` | `-1.0` | defines the weight of the animation (default is -1 so no weight) |

#### Returns

`boolean`

a boolean indicating if the animation is running

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:488

___

### dispose

▸ **dispose**(): `void`

Disposes of the runtime animation

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:321

___

### goToFrame

▸ **goToFrame**(`frame`): `void`

Move the current animation to a given frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `number` | defines the frame to move to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:442

___

### isStopped

▸ **isStopped**(): `boolean`

Specifies if the runtime animation is stopped

#### Returns

`boolean`

Boolean specifying if the runtime animation is stopped

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:314

___

### reset

▸ **reset**(`restoreOriginal?`): `void`

Resets the runtime animation to the beginning

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `restoreOriginal` | `boolean` | `false` | defines whether to restore the target property to the original value |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:282

___

### setValue

▸ **setValue**(`currentValue`, `weight`): `void`

Apply the interpolated value to the target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentValue` | `any` | defines the value computed by the animation |
| `weight` | `number` | defines the weight to apply to this value (Defaults to 1.0) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/runtimeAnimation.ts:334

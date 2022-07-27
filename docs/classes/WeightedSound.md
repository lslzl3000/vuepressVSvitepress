[@dev/core](../README.md) / [Exports](../modules.md) / WeightedSound

# Class: WeightedSound

Wraps one or more Sound objects and selects one with random weight for playback.

## Table of contents

### Constructors

- [constructor](WeightedSound.md#constructor)

### Properties

- [\_coneInnerAngle](WeightedSound.md#_coneinnerangle)
- [\_coneOuterAngle](WeightedSound.md#_coneouterangle)
- [\_currentIndex](WeightedSound.md#_currentindex)
- [\_sounds](WeightedSound.md#_sounds)
- [\_volume](WeightedSound.md#_volume)
- [\_weights](WeightedSound.md#_weights)
- [isPaused](WeightedSound.md#ispaused)
- [isPlaying](WeightedSound.md#isplaying)
- [loop](WeightedSound.md#loop)

### Accessors

- [directionalConeInnerAngle](WeightedSound.md#directionalconeinnerangle)
- [directionalConeOuterAngle](WeightedSound.md#directionalconeouterangle)
- [volume](WeightedSound.md#volume)

### Methods

- [\_onended](WeightedSound.md#_onended)
- [pause](WeightedSound.md#pause)
- [play](WeightedSound.md#play)
- [stop](WeightedSound.md#stop)

## Constructors

### constructor

• **new WeightedSound**(`loop`, `sounds`, `weights`)

Creates a new WeightedSound from the list of sounds given.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `loop` | `boolean` | When true a Sound will be selected and played when the current playing Sound completes. |
| `sounds` | [`Sound`](Sound.md)[] | Array of Sounds that will be selected from. |
| `weights` | `number`[] | Array of number values for selection weights; length must equal sounds, values will be normalized to 1 |

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:28

## Properties

### \_coneInnerAngle

• `Private` **\_coneInnerAngle**: `number` = `360`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:10

___

### \_coneOuterAngle

• `Private` **\_coneOuterAngle**: `number` = `360`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:11

___

### \_currentIndex

• `Private` `Optional` **\_currentIndex**: `number`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:20

___

### \_sounds

• `Private` **\_sounds**: [`Sound`](Sound.md)[] = `[]`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:18

___

### \_volume

• `Private` **\_volume**: `number` = `1`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:12

___

### \_weights

• `Private` **\_weights**: `number`[] = `[]`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:19

___

### isPaused

• **isPaused**: `boolean` = `false`

A Sound is currently paused.

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:16

___

### isPlaying

• **isPlaying**: `boolean` = `false`

A Sound is currently playing.

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:14

___

### loop

• **loop**: `boolean` = `false`

When true a Sound will be selected and played when the current playing Sound completes.

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:9

## Accessors

### directionalConeInnerAngle

• `get` **directionalConeInnerAngle**(): `number`

The size of cone in degrees for a directional sound in which there will be no attenuation.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:55

• `set` **directionalConeInnerAngle**(`value`): `void`

The size of cone in degrees for a directional sound in which there will be no attenuation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:62

___

### directionalConeOuterAngle

• `get` **directionalConeOuterAngle**(): `number`

Size of cone in degrees for a directional sound outside of which there will be no sound.
Listener angles between innerAngle and outerAngle will falloff linearly.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:80

• `set` **directionalConeOuterAngle**(`value`): `void`

Size of cone in degrees for a directional sound outside of which there will be no sound.
Listener angles between innerAngle and outerAngle will falloff linearly.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:88

___

### volume

• `get` **volume**(): `number`

Playback volume.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:105

• `set` **volume**(`value`): `void`

Playback volume.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:112

## Methods

### \_onended

▸ `Private` **_onended**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:120

___

### pause

▸ **pause**(): `void`

Suspend playback

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:134

___

### play

▸ **play**(`startOffset?`): `void`

Start playback.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startOffset?` | `number` | Position the clip head at a specific time in seconds. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:155

___

### stop

▸ **stop**(): `void`

Stop playback

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/weightedsound.ts:144

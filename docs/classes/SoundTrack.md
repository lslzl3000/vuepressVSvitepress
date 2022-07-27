[@dev/core](../README.md) / [Exports](../modules.md) / SoundTrack

# Class: SoundTrack

It could be useful to isolate your music & sounds on several tracks to better manage volume on a grouped instance of sounds.
It will be also used in a future release to apply effects on a specific track.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#using-sound-tracks

## Table of contents

### Constructors

- [constructor](SoundTrack.md#constructor)

### Properties

- [\_connectedAnalyser](SoundTrack.md#_connectedanalyser)
- [\_isInitialized](SoundTrack.md#_isinitialized)
- [\_options](SoundTrack.md#_options)
- [\_outputAudioNode](SoundTrack.md#_outputaudionode)
- [\_scene](SoundTrack.md#_scene)
- [id](SoundTrack.md#id)
- [soundCollection](SoundTrack.md#soundcollection)

### Methods

- [\_initializeSoundTrackAudioGraph](SoundTrack.md#_initializesoundtrackaudiograph)
- [addSound](SoundTrack.md#addsound)
- [connectToAnalyser](SoundTrack.md#connecttoanalyser)
- [dispose](SoundTrack.md#dispose)
- [removeSound](SoundTrack.md#removesound)
- [setVolume](SoundTrack.md#setvolume)
- [switchPanningModelToEqualPower](SoundTrack.md#switchpanningmodeltoequalpower)
- [switchPanningModelToHRTF](SoundTrack.md#switchpanningmodeltohrtf)

## Constructors

### constructor

• **new SoundTrack**(`scene?`, `options?`)

Creates a new sound track.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#using-sound-tracks

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | Define the scene the sound track belongs to |
| `options` | [`ISoundTrackOptions`](../interfaces/ISoundTrackOptions.md) |  |

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:49

## Properties

### \_connectedAnalyser

• `Private` **\_connectedAnalyser**: [`Analyser`](Analyser.md)

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:39

___

### \_isInitialized

• `Private` **\_isInitialized**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:41

___

### \_options

• `Private` **\_options**: [`ISoundTrackOptions`](../interfaces/ISoundTrackOptions.md)

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:40

___

### \_outputAudioNode

• `Private` **\_outputAudioNode**: [`Nullable`](../modules.md#nullable)`GainNode`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:37

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:38

___

### id

• **id**: `number` = `-1`

The unique identifier of the sound track in the scene.

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:31

___

### soundCollection

• **soundCollection**: [`Sound`](Sound.md)[]

The list of sounds included in the sound track.

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:35

## Methods

### \_initializeSoundTrackAudioGraph

▸ `Private` **_initializeSoundTrackAudioGraph**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:64

___

### addSound

▸ **addSound**(`sound`): `void`

Adds a sound to this sound track

**`Ignore Naming`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sound` | [`Sound`](Sound.md) | define the sound to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:102

___

### connectToAnalyser

▸ **connectToAnalyser**(`analyser`): `void`

Connect the sound track to an audio analyser allowing some amazing
synchronization between the sounds/music and your visualization (VuMeter for instance).

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#using-the-analyser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `analyser` | [`Analyser`](Analyser.md) | The analyser to connect to the engine |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:175

___

### dispose

▸ **dispose**(): `void`

Release the sound track and its associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:82

___

### removeSound

▸ **removeSound**(`sound`): `void`

Removes a sound to this sound track

**`Ignore Naming`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sound` | [`Sound`](Sound.md) | define the sound to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:126

___

### setVolume

▸ **setVolume**(`newVolume`): `void`

Set a global volume for the full sound track.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newVolume` | `number` | Define the new volume of the sound track |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:137

___

### switchPanningModelToEqualPower

▸ **switchPanningModelToEqualPower**(): `void`

Switch the panning model to Equal Power:
Represents the equal-power panning algorithm, generally regarded as simple and efficient. equalpower is the default value.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:161

___

### switchPanningModelToHRTF

▸ **switchPanningModelToHRTF**(): `void`

Switch the panning model to HRTF:
Renders a stereo output of higher quality than equalpower — it uses a convolution with measured impulse responses from human subjects.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/soundTrack.ts:148

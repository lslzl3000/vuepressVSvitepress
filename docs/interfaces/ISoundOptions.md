[@dev/core](../README.md) / [Exports](../modules.md) / ISoundOptions

# Interface: ISoundOptions

Interface used to define options for Sound class

## Table of contents

### Properties

- [autoplay](ISoundOptions.md#autoplay)
- [distanceModel](ISoundOptions.md#distancemodel)
- [length](ISoundOptions.md#length)
- [loop](ISoundOptions.md#loop)
- [maxDistance](ISoundOptions.md#maxdistance)
- [offset](ISoundOptions.md#offset)
- [playbackRate](ISoundOptions.md#playbackrate)
- [refDistance](ISoundOptions.md#refdistance)
- [rolloffFactor](ISoundOptions.md#rollofffactor)
- [skipCodecCheck](ISoundOptions.md#skipcodeccheck)
- [spatialSound](ISoundOptions.md#spatialsound)
- [streaming](ISoundOptions.md#streaming)
- [useCustomAttenuation](ISoundOptions.md#usecustomattenuation)
- [volume](ISoundOptions.md#volume)

## Properties

### autoplay

• `Optional` **autoplay**: `boolean`

Does the sound autoplay once loaded.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:8

___

### distanceModel

• `Optional` **distanceModel**: `string`

Define the distance attenuation model the sound will follow.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:43

___

### length

• `Optional` **length**: `number`

Defines an optional length (in seconds) inside the sound file

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:55

___

### loop

• `Optional` **loop**: `boolean`

Does the sound loop after it finishes playing once.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:12

___

### maxDistance

• `Optional` **maxDistance**: `number`

Maximum distance to hear that sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:24

___

### offset

• `Optional` **offset**: `number`

Defines an optional offset (in seconds) inside the sound file

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:59

___

### playbackRate

• `Optional` **playbackRate**: `number`

Defines the playback speed (1 by default)

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:47

___

### refDistance

• `Optional` **refDistance**: `number`

Define the reference distance the sound should be heard perfectly.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:38

___

### rolloffFactor

• `Optional` **rolloffFactor**: `number`

Define the roll off factor of spatial sounds.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:33

___

### skipCodecCheck

• `Optional` **skipCodecCheck**: `boolean`

If true, URLs will not be required to state the audio file codec to use.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:63

___

### spatialSound

• `Optional` **spatialSound**: `boolean`

Is it a spatial sound?

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:20

___

### streaming

• `Optional` **streaming**: `boolean`

Defines if the sound is from a streaming source

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:51

___

### useCustomAttenuation

• `Optional` **useCustomAttenuation**: `boolean`

Uses user defined attenuation function

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:28

___

### volume

• `Optional` **volume**: `number`

Sound's volume

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/ISoundOptions.ts:16

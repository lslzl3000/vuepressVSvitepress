[@dev/core](../README.md) / [Exports](../modules.md) / IAudioEngine

# Interface: IAudioEngine

This represents an audio engine and it is responsible
to play, synchronize and analyse sounds throughout the application.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`IAudioEngine`**

## Implemented by

- [`AudioEngine`](../classes/AudioEngine.md)

## Table of contents

### Properties

- [WarnedWebAudioUnsupported](IAudioEngine.md#warnedwebaudiounsupported)
- [audioContext](IAudioEngine.md#audiocontext)
- [canUseWebAudio](IAudioEngine.md#canusewebaudio)
- [isMP3supported](IAudioEngine.md#ismp3supported)
- [isOGGsupported](IAudioEngine.md#isoggsupported)
- [masterGain](IAudioEngine.md#mastergain)
- [onAudioLockedObservable](IAudioEngine.md#onaudiolockedobservable)
- [onAudioUnlockedObservable](IAudioEngine.md#onaudiounlockedobservable)
- [unlocked](IAudioEngine.md#unlocked)
- [useCustomUnlockedButton](IAudioEngine.md#usecustomunlockedbutton)

### Methods

- [connectToAnalyser](IAudioEngine.md#connecttoanalyser)
- [dispose](IAudioEngine.md#dispose)
- [getGlobalVolume](IAudioEngine.md#getglobalvolume)
- [lock](IAudioEngine.md#lock)
- [setGlobalVolume](IAudioEngine.md#setglobalvolume)
- [unlock](IAudioEngine.md#unlock)

## Properties

### WarnedWebAudioUnsupported

• **WarnedWebAudioUnsupported**: `boolean`

Defines if Babylon should emit a warning if WebAudio is not supported.

**`Ignore Naming`**

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:42

___

### audioContext

• `Readonly` **audioContext**: [`Nullable`](../modules.md#nullable)`AudioContext`

Gets the current AudioContext if available.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:20

___

### canUseWebAudio

• `Readonly` **canUseWebAudio**: `boolean`

Gets whether the current host supports Web Audio and thus could create AudioContexts.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:15

___

### isMP3supported

• `Readonly` **isMP3supported**: `boolean`

Gets whether or not mp3 are supported by your browser.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:30

___

### isOGGsupported

• `Readonly` **isOGGsupported**: `boolean`

Gets whether or not ogg are supported by your browser.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:35

___

### masterGain

• `Readonly` **masterGain**: `GainNode`

The master gain node defines the global audio volume of your audio engine.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:25

___

### onAudioLockedObservable

• **onAudioLockedObservable**: [`Observable`](../classes/Observable.md)[`IAudioEngine`](IAudioEngine.md)

Event raised when audio has been locked on the browser.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:63

___

### onAudioUnlockedObservable

• **onAudioUnlockedObservable**: [`Observable`](../classes/Observable.md)[`IAudioEngine`](IAudioEngine.md)

Event raised when audio has been unlocked on the browser.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:58

___

### unlocked

• `Readonly` **unlocked**: `boolean`

Gets whether or not the audio engine is unlocked (require first a user gesture on some browser).

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:53

___

### useCustomUnlockedButton

• **useCustomUnlockedButton**: `boolean`

Defines if the audio engine relies on a custom unlocked button.
In this case, the embedded button will not be displayed.

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:48

## Methods

### connectToAnalyser

▸ **connectToAnalyser**(`analyser`): `void`

Connect the audio engine to an audio analyser allowing some amazing
synchronization between the sounds/music and your visualization (VuMeter for instance).

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#using-the-analyser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `analyser` | [`Analyser`](../classes/Analyser.md) | The analyser to connect to the engine |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:95

___

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Inherited from

[IDisposable](IDisposable.md).[dispose](IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:103

___

### getGlobalVolume

▸ **getGlobalVolume**(): `number`

Gets the global volume sets on the master gain.

#### Returns

`number`

the global volume if set or -1 otherwise

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:81

___

### lock

▸ **lock**(): `void`

Flags the audio engine in Locked state.
This happens due to new browser policies preventing audio to autoplay.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:69

___

### setGlobalVolume

▸ **setGlobalVolume**(`newVolume`): `void`

Sets the global volume of your experience (sets on the master gain).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newVolume` | `number` | Defines the new global volume of the application |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:87

___

### unlock

▸ **unlock**(): `void`

Unlocks the audio engine once a user action has been done on the dom.
This is helpful to resume play once browser policies have been satisfied.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/Interfaces/IAudioEngine.ts:75

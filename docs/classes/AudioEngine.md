[@dev/core](../README.md) / [Exports](../modules.md) / AudioEngine

# Class: AudioEngine

This represents the default audio engine used in babylon.
It is responsible to play, synchronize and analyse sounds throughout the  application.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

## Implements

- [`IAudioEngine`](../interfaces/IAudioEngine.md)

## Table of contents

### Constructors

- [constructor](AudioEngine.md#constructor)

### Properties

- [WarnedWebAudioUnsupported](AudioEngine.md#warnedwebaudiounsupported)
- [\_audioContext](AudioEngine.md#_audiocontext)
- [\_audioContextInitialized](AudioEngine.md#_audiocontextinitialized)
- [\_audioDestination](AudioEngine.md#_audiodestination)
- [\_connectedAnalyser](AudioEngine.md#_connectedanalyser)
- [\_hostElement](AudioEngine.md#_hostelement)
- [\_muteButton](AudioEngine.md#_mutebutton)
- [\_tryToRun](AudioEngine.md#_trytorun)
- [canUseWebAudio](AudioEngine.md#canusewebaudio)
- [isMP3supported](AudioEngine.md#ismp3supported)
- [isOGGsupported](AudioEngine.md#isoggsupported)
- [masterGain](AudioEngine.md#mastergain)
- [onAudioLockedObservable](AudioEngine.md#onaudiolockedobservable)
- [onAudioUnlockedObservable](AudioEngine.md#onaudiounlockedobservable)
- [unlocked](AudioEngine.md#unlocked)
- [useCustomUnlockedButton](AudioEngine.md#usecustomunlockedbutton)

### Accessors

- [audioContext](AudioEngine.md#audiocontext)

### Methods

- [\_displayMuteButton](AudioEngine.md#_displaymutebutton)
- [\_hideMuteButton](AudioEngine.md#_hidemutebutton)
- [\_initializeAudioContext](AudioEngine.md#_initializeaudiocontext)
- [\_moveButtonToTopLeft](AudioEngine.md#_movebuttontotopleft)
- [\_onResize](AudioEngine.md#_onresize)
- [\_resumeAudioContext](AudioEngine.md#_resumeaudiocontext)
- [\_triggerRunningState](AudioEngine.md#_triggerrunningstate)
- [\_triggerSuspendedState](AudioEngine.md#_triggersuspendedstate)
- [connectToAnalyser](AudioEngine.md#connecttoanalyser)
- [dispose](AudioEngine.md#dispose)
- [getGlobalVolume](AudioEngine.md#getglobalvolume)
- [lock](AudioEngine.md#lock)
- [setGlobalVolume](AudioEngine.md#setglobalvolume)
- [unlock](AudioEngine.md#unlock)

## Constructors

### constructor

• **new AudioEngine**(`hostElement?`, `audioContext?`, `audioDestination?`)

Instantiates a new audio engine.

There should be only one per page as some browsers restrict the number
of audio contexts you can create.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `hostElement` | [`Nullable`](../modules.md#nullable)`HTMLElement` | `null` | defines the host element where to display the mute icon if necessary |
| `audioContext` | [`Nullable`](../modules.md#nullable)`AudioContext` | `null` | defines the audio context to be used by the audio engine |
| `audioDestination` | [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode` | `null` | defines the audio destination node to be used by audio engine |

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:106

## Properties

### WarnedWebAudioUnsupported

• **WarnedWebAudioUnsupported**: `boolean` = `false`

Defines if Babylon should emit a warning if WebAudio is not supported.

**`Ignore Naming`**

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[WarnedWebAudioUnsupported](../interfaces/IAudioEngine.md#warnedwebaudiounsupported)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:46

___

### \_audioContext

• `Private` **\_audioContext**: [`Nullable`](../modules.md#nullable)`AudioContext` = `null`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:25

___

### \_audioContextInitialized

• `Private` **\_audioContextInitialized**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:26

___

### \_audioDestination

• `Private` **\_audioDestination**: [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode` = `null`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:29

___

### \_connectedAnalyser

• `Private` **\_connectedAnalyser**: [`Nullable`](../modules.md#nullable)[`Analyser`](Analyser.md)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:95

___

### \_hostElement

• `Private` **\_hostElement**: [`Nullable`](../modules.md#nullable)`HTMLElement`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:28

___

### \_muteButton

• `Private` **\_muteButton**: [`Nullable`](../modules.md#nullable)`HTMLButtonElement` = `null`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:27

___

### \_tryToRun

• `Private` **\_tryToRun**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:194

___

### canUseWebAudio

• **canUseWebAudio**: `boolean` = `false`

Gets whether the current host supports Web Audio and thus could create AudioContexts.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[canUseWebAudio](../interfaces/IAudioEngine.md#canusewebaudio)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:34

___

### isMP3supported

• **isMP3supported**: `boolean` = `false`

Gets whether or not mp3 are supported by your browser.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[isMP3supported](../interfaces/IAudioEngine.md#ismp3supported)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:51

___

### isOGGsupported

• **isOGGsupported**: `boolean` = `false`

Gets whether or not ogg are supported by your browser.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[isOGGsupported](../interfaces/IAudioEngine.md#isoggsupported)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:56

___

### masterGain

• **masterGain**: `GainNode`

The master gain node defines the global audio volume of your audio engine.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[masterGain](../interfaces/IAudioEngine.md#mastergain)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:39

___

### onAudioLockedObservable

• **onAudioLockedObservable**: [`Observable`](Observable.md)[`IAudioEngine`](../interfaces/IAudioEngine.md)

Event raised when audio has been locked on the browser.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[onAudioLockedObservable](../interfaces/IAudioEngine.md#onaudiolockedobservable)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:79

___

### onAudioUnlockedObservable

• **onAudioUnlockedObservable**: [`Observable`](Observable.md)[`IAudioEngine`](../interfaces/IAudioEngine.md)

Event raised when audio has been unlocked on the browser.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[onAudioUnlockedObservable](../interfaces/IAudioEngine.md#onaudiounlockedobservable)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:74

___

### unlocked

• **unlocked**: `boolean` = `true`

Gets whether audio has been unlocked on the device.
Some Browsers have strong restrictions about Audio and won t autoplay unless
a user interaction has happened.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[unlocked](../interfaces/IAudioEngine.md#unlocked)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:63

___

### useCustomUnlockedButton

• **useCustomUnlockedButton**: `boolean` = `false`

Defines if the audio engine relies on a custom unlocked button.
In this case, the embedded button will not be displayed.

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[useCustomUnlockedButton](../interfaces/IAudioEngine.md#usecustomunlockedbutton)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:69

## Accessors

### audioContext

• `get` **audioContext**(): [`Nullable`](../modules.md#nullable)`AudioContext`

Gets the current AudioContext if available.

#### Returns

[`Nullable`](../modules.md#nullable)`AudioContext`

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[audioContext](../interfaces/IAudioEngine.md#audiocontext)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:84

## Methods

### \_displayMuteButton

▸ `Private` **_displayMuteButton**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:223

___

### \_hideMuteButton

▸ `Private` **_hideMuteButton**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:278

___

### \_initializeAudioContext

▸ `Private` **_initializeAudioContext**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:169

___

### \_moveButtonToTopLeft

▸ `Private` **_moveButtonToTopLeft**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:267

___

### \_onResize

▸ `Private` **_onResize**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:274

___

### \_resumeAudioContext

▸ `Private` **_resumeAudioContext**(): `Promise``void`

#### Returns

`Promise``void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:161

___

### \_triggerRunningState

▸ `Private` **_triggerRunningState**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:195

___

### \_triggerSuspendedState

▸ `Private` **_triggerSuspendedState**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:217

___

### connectToAnalyser

▸ **connectToAnalyser**(`analyser`): `void`

Connect the audio engine to an audio analyser allowing some amazing
synchronization between the sounds/music and your visualization (VuMeter for instance).

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#using-the-analyser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `analyser` | [`Analyser`](Analyser.md) | The analyser to connect to the engine |

#### Returns

`void`

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[connectToAnalyser](../interfaces/IAudioEngine.md#connecttoanalyser)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:335

___

### dispose

▸ **dispose**(): `void`

Destroy and release the resources associated with the audio context.

#### Returns

`void`

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[dispose](../interfaces/IAudioEngine.md#dispose)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:288

___

### getGlobalVolume

▸ **getGlobalVolume**(): `number`

Gets the global volume sets on the master gain.

#### Returns

`number`

the global volume if set or -1 otherwise

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[getGlobalVolume](../interfaces/IAudioEngine.md#getglobalvolume)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:311

___

### lock

▸ **lock**(): `void`

Flags the audio engine in Locked state.
This happens due to new browser policies preventing audio to autoplay.

#### Returns

`void`

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[lock](../interfaces/IAudioEngine.md#lock)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:149

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

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[setGlobalVolume](../interfaces/IAudioEngine.md#setglobalvolume)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:323

___

### unlock

▸ **unlock**(): `void`

Unlocks the audio engine once a user action has been done on the dom.
This is helpful to resume play once browser policies have been satisfied.

#### Returns

`void`

#### Implementation of

[IAudioEngine](../interfaces/IAudioEngine.md).[unlock](../interfaces/IAudioEngine.md#unlock)

#### Defined in

packages/dev/core/src/Audio/audioEngine.ts:157

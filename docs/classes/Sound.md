[@dev/core](../README.md) / [Exports](../modules.md) / Sound

# Class: Sound

Defines a sound that can be played in the application.
The sound can either be an ambient track or a simple sound played in reaction to a user action.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

## Table of contents

### Constructors

- [constructor](Sound.md#constructor)

### Properties

- [\_audioBuffer](Sound.md#_audiobuffer)
- [\_coneInnerAngle](Sound.md#_coneinnerangle)
- [\_coneOuterAngle](Sound.md#_coneouterangle)
- [\_coneOuterGain](Sound.md#_coneoutergain)
- [\_connectedTransformNode](Sound.md#_connectedtransformnode)
- [\_customAttenuationFunction](Sound.md#_customattenuationfunction)
- [\_htmlAudioElement](Sound.md#_htmlaudioelement)
- [\_inputAudioNode](Sound.md#_inputaudionode)
- [\_isDirectional](Sound.md#_isdirectional)
- [\_isOutputConnected](Sound.md#_isoutputconnected)
- [\_isReadyToPlay](Sound.md#_isreadytoplay)
- [\_length](Sound.md#_length)
- [\_localDirection](Sound.md#_localdirection)
- [\_loop](Sound.md#_loop)
- [\_offset](Sound.md#_offset)
- [\_outputAudioNode](Sound.md#_outputaudionode)
- [\_panningModel](Sound.md#_panningmodel)
- [\_playbackRate](Sound.md#_playbackrate)
- [\_position](Sound.md#_position)
- [\_readyToPlayCallback](Sound.md#_readytoplaycallback)
- [\_registerFunc](Sound.md#_registerfunc)
- [\_scene](Sound.md#_scene)
- [\_soundGain](Sound.md#_soundgain)
- [\_soundPanner](Sound.md#_soundpanner)
- [\_soundSource](Sound.md#_soundsource)
- [\_spatialSound](Sound.md#_spatialsound)
- [\_startOffset](Sound.md#_startoffset)
- [\_startTime](Sound.md#_starttime)
- [\_streaming](Sound.md#_streaming)
- [\_streamingSource](Sound.md#_streamingsource)
- [\_urlType](Sound.md#_urltype)
- [\_volume](Sound.md#_volume)
- [autoplay](Sound.md#autoplay)
- [distanceModel](Sound.md#distancemodel)
- [isPaused](Sound.md#ispaused)
- [isPlaying](Sound.md#isplaying)
- [maxDistance](Sound.md#maxdistance)
- [metadata](Sound.md#metadata)
- [name](Sound.md#name)
- [onEndedObservable](Sound.md#onendedobservable)
- [refDistance](Sound.md#refdistance)
- [rolloffFactor](Sound.md#rollofffactor)
- [soundTrackId](Sound.md#soundtrackid)
- [useCustomAttenuation](Sound.md#usecustomattenuation)

### Accessors

- [currentTime](Sound.md#currenttime)
- [directionalConeInnerAngle](Sound.md#directionalconeinnerangle)
- [directionalConeOuterAngle](Sound.md#directionalconeouterangle)
- [loop](Sound.md#loop)
- [spatialSound](Sound.md#spatialsound)

### Methods

- [\_createSpatialParameters](Sound.md#_createspatialparameters)
- [\_onRegisterAfterWorldMatrixUpdate](Sound.md#_onregisterafterworldmatrixupdate)
- [\_onended](Sound.md#_onended)
- [\_soundLoaded](Sound.md#_soundloaded)
- [\_switchPanningModel](Sound.md#_switchpanningmodel)
- [\_updateDirection](Sound.md#_updatedirection)
- [\_updateSpatialParameters](Sound.md#_updatespatialparameters)
- [attachToMesh](Sound.md#attachtomesh)
- [clone](Sound.md#clone)
- [connectToSoundTrackAudioNode](Sound.md#connecttosoundtrackaudionode)
- [detachFromMesh](Sound.md#detachfrommesh)
- [dispose](Sound.md#dispose)
- [getAudioBuffer](Sound.md#getaudiobuffer)
- [getClassName](Sound.md#getclassname)
- [getSoundGain](Sound.md#getsoundgain)
- [getSoundSource](Sound.md#getsoundsource)
- [getVolume](Sound.md#getvolume)
- [isReady](Sound.md#isready)
- [pause](Sound.md#pause)
- [play](Sound.md#play)
- [serialize](Sound.md#serialize)
- [setAttenuationFunction](Sound.md#setattenuationfunction)
- [setAudioBuffer](Sound.md#setaudiobuffer)
- [setDirectionalCone](Sound.md#setdirectionalcone)
- [setLocalDirectionToMesh](Sound.md#setlocaldirectiontomesh)
- [setPlaybackRate](Sound.md#setplaybackrate)
- [setPosition](Sound.md#setposition)
- [setVolume](Sound.md#setvolume)
- [stop](Sound.md#stop)
- [switchPanningModelToEqualPower](Sound.md#switchpanningmodeltoequalpower)
- [switchPanningModelToHRTF](Sound.md#switchpanningmodeltohrtf)
- [updateOptions](Sound.md#updateoptions)
- [Parse](Sound.md#parse)

## Constructors

### constructor

• **new Sound**(`name`, `urlOrArrayBuffer`, `scene?`, `readyToPlayCallback?`, `options?`)

Create a sound and attach it to a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Name of your sound |
| `urlOrArrayBuffer` | `any` | `undefined` | Url to the sound to load async or ArrayBuffer, it also works with MediaStreams |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `undefined` | defines the scene the sound belongs to |
| `readyToPlayCallback` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Provide a callback function if you'd like to load your code once the sound is ready to be played |
| `options?` | [`ISoundOptions`](../interfaces/ISoundOptions.md) | `undefined` | Objects to provide with the current available options: autoplay, loop, volume, spatialSound, maxDistance, rolloffFactor, refDistance, distanceModel, panningModel, streaming |

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:181

## Properties

### \_audioBuffer

• `Private` **\_audioBuffer**: [`Nullable`](../modules.md#nullable)`AudioBuffer`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:143

___

### \_coneInnerAngle

• `Private` **\_coneInnerAngle**: `number` = `360`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:152

___

### \_coneOuterAngle

• `Private` **\_coneOuterAngle**: `number` = `360`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:153

___

### \_coneOuterGain

• `Private` **\_coneOuterGain**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:154

___

### \_connectedTransformNode

• `Private` **\_connectedTransformNode**: [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:156

___

### \_customAttenuationFunction

• `Private` **\_customAttenuationFunction**: (`currentVolume`: `number`, `currentDistance`: `number`, `maxDistance`: `number`, `refDistance`: `number`, `rolloffFactor`: `number`) => `number`

#### Type declaration

▸ (`currentVolume`, `currentDistance`, `maxDistance`, `refDistance`, `rolloffFactor`): `number`

##### Parameters

| Name | Type |
| :------ | :------ |
| `currentVolume` | `number` |
| `currentDistance` | `number` |
| `maxDistance` | `number` |
| `refDistance` | `number` |
| `rolloffFactor` | `number` |

##### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:157

___

### \_htmlAudioElement

• `Private` **\_htmlAudioElement**: `HTMLAudioElement`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:160

___

### \_inputAudioNode

• `Private` **\_inputAudioNode**: [`Nullable`](../modules.md#nullable)`AudioNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:148

___

### \_isDirectional

• `Private` **\_isDirectional**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:141

___

### \_isOutputConnected

• `Private` **\_isOutputConnected**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:159

___

### \_isReadyToPlay

• `Private` **\_isReadyToPlay**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:140

___

### \_length

• `Private` `Optional` **\_length**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:162

___

### \_localDirection

• `Private` **\_localDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:138

___

### \_loop

• `Private` **\_loop**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:29

___

### \_offset

• `Private` `Optional` **\_offset**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:163

___

### \_outputAudioNode

• `Private` **\_outputAudioNode**: [`Nullable`](../modules.md#nullable)`AudioNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:149

___

### \_panningModel

• `Private` **\_panningModel**: `string` = `"equalpower"`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:132

___

### \_playbackRate

• `Private` **\_playbackRate**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:133

___

### \_position

• `Private` **\_position**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:137

___

### \_readyToPlayCallback

• `Private` **\_readyToPlayCallback**: [`Nullable`](../modules.md#nullable)() => `any`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:142

___

### \_registerFunc

• `Private` **\_registerFunc**: [`Nullable`](../modules.md#nullable)(`connectedMesh`: [`TransformNode`](TransformNode.md)) => `void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:158

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:155

___

### \_soundGain

• `Private` **\_soundGain**: [`Nullable`](../modules.md#nullable)`GainNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:147

___

### \_soundPanner

• `Private` **\_soundPanner**: [`Nullable`](../modules.md#nullable)`PannerNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:146

___

### \_soundSource

• `Private` **\_soundSource**: [`Nullable`](../modules.md#nullable)`AudioBufferSourceNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:144

___

### \_spatialSound

• `Private` **\_spatialSound**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:131

___

### \_startOffset

• `Private` **\_startOffset**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:136

___

### \_startTime

• `Private` **\_startTime**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:135

___

### \_streaming

• `Private` **\_streaming**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:134

___

### \_streamingSource

• `Private` **\_streamingSource**: `AudioNode`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:145

___

### \_urlType

• `Private` **\_urlType**: ``"Unknown"`` \| ``"String"`` \| ``"Array"`` \| ``"ArrayBuffer"`` \| ``"MediaStream"`` \| ``"MediaElement"`` = `"Unknown"`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:161

___

### \_volume

• `Private` **\_volume**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:139

___

### autoplay

• **autoplay**: `boolean` = `false`

Does the sound autoplay once loaded.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:27

___

### distanceModel

• **distanceModel**: `string` = `"linear"`

Define the distance attenuation model the sound will follow.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:83

___

### isPaused

• **isPaused**: `boolean` = `false`

Is this sound currently paused.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:63

___

### isPlaying

• **isPlaying**: `boolean` = `false`

Is this sound currently played.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:59

___

### maxDistance

• **maxDistance**: `number` = `100`

Define the max distance the sound should be heard (intensity just became 0 at this point).

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:78

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the sound.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:92

___

### name

• **name**: `string`

The name of the sound in the scene.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:23

___

### onEndedObservable

• **onEndedObservable**: [`Observable`](Observable.md)[`Sound`](Sound.md)

Observable event when the current playing sound finishes.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:97

___

### refDistance

• **refDistance**: `number` = `1`

Define the reference distance the sound should be heard perfectly.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:68

___

### rolloffFactor

• **rolloffFactor**: `number` = `1`

Define the roll off factor of spatial sounds.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:73

___

### soundTrackId

• **soundTrackId**: `number`

The sound track id this sound belongs to.

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:55

___

### useCustomAttenuation

• **useCustomAttenuation**: `boolean` = `false`

Does the sound use a custom attenuation curve to simulate the falloff
happening when the source gets further away from the camera.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-your-own-custom-attenuation-function

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:51

## Accessors

### currentTime

• `get` **currentTime**(): `number`

Gets the current time for the sound.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:102

___

### directionalConeInnerAngle

• `get` **directionalConeInnerAngle**(): `number`

Gets or sets the inner angle for the directional cone.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:618

• `set` **directionalConeInnerAngle**(`value`): `void`

Gets or sets the inner angle for the directional cone.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:625

___

### directionalConeOuterAngle

• `get` **directionalConeOuterAngle**(): `number`

Gets or sets the outer angle for the directional cone.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:642

• `set` **directionalConeOuterAngle**(`value`): `void`

Gets or sets the outer angle for the directional cone.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:649

___

### loop

• `get` **loop**(): `boolean`

Does the sound loop after it finishes playing once.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:33

• `set` **loop**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:37

___

### spatialSound

• `get` **spatialSound**(): `boolean`

Does this sound enables spatial sound.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:118

• `set` **spatialSound**(`newValue`): `void`

Does this sound enables spatial sound.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-a-spatial-3d-sound

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:125

## Methods

### \_createSpatialParameters

▸ `Private` **_createSpatialParameters**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:520

___

### \_onRegisterAfterWorldMatrixUpdate

▸ `Private` **_onRegisterAfterWorldMatrixUpdate**(`node`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`TransformNode`](TransformNode.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1004

___

### \_onended

▸ `Private` **_onended**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:863

___

### \_soundLoaded

▸ `Private` **_soundLoaded**(`audioData`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `audioData` | `ArrayBuffer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:446

___

### \_switchPanningModel

▸ `Private` **_switchPanningModel**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:573

___

### \_updateDirection

▸ `Private` **_updateDirection**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:692

___

### \_updateSpatialParameters

▸ `Private` **_updateSpatialParameters**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:534

___

### attachToMesh

▸ **attachToMesh**(`transformNode`): `void`

Attach the sound to a dedicated mesh

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#attaching-a-sound-to-a-mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transformNode` | [`TransformNode`](TransformNode.md) | The transform node to connect the sound with |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:973

___

### clone

▸ **clone**(): [`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)

Clone the current sound in the scene.

#### Returns

[`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)

the new sound clone

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1021

___

### connectToSoundTrackAudioNode

▸ **connectToSoundTrackAudioNode**(`soundTrackAudioNode`): `void`

Connect this sound to a sound track audio node like gain...

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `soundTrackAudioNode` | `AudioNode` | the sound track audio node to connect to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:583

___

### detachFromMesh

▸ **detachFromMesh**(): `void`

Detach the sound from the previously attached mesh

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#attaching-a-sound-to-a-mesh

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:996

___

### dispose

▸ **dispose**(): `void`

Release the sound and its associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:388

___

### getAudioBuffer

▸ **getAudioBuffer**(): [`Nullable`](../modules.md#nullable)`AudioBuffer`

Gets the current underlying audio buffer containing the data

#### Returns

[`Nullable`](../modules.md#nullable)`AudioBuffer`

the audio buffer

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1067

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name.

#### Returns

`string`

current class name

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:442

___

### getSoundGain

▸ **getSoundGain**(): [`Nullable`](../modules.md#nullable)`GainNode`

Gets the WebAudio GainNode, gives you precise control over the gain of instances of this Sound.

#### Returns

[`Nullable`](../modules.md#nullable)`GainNode`

the gain node

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1083

___

### getSoundSource

▸ **getSoundSource**(): [`Nullable`](../modules.md#nullable)`AudioBufferSourceNode`

Gets the WebAudio AudioBufferSourceNode, lets you keep track of and stop instances of this Sound.

#### Returns

[`Nullable`](../modules.md#nullable)`AudioBufferSourceNode`

the source node

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1075

___

### getVolume

▸ **getVolume**(): `number`

Gets the volume of the sound.

#### Returns

`number`

the volume of the sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:964

___

### isReady

▸ **isReady**(): `boolean`

Gets if the sounds is ready to be played or not.

#### Returns

`boolean`

true if ready, otherwise false

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:434

___

### pause

▸ **pause**(): `void`

Put the sound in pause

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:910

___

### play

▸ **play**(`time?`, `offset?`, `length?`): `void`

Play the sound

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `time?` | `number` | (optional) Start the sound after X seconds. Start immediately (0) by default. |
| `offset?` | `number` | (optional) Start the sound at a specific time in seconds |
| `length?` | `number` | (optional) Sound duration (in seconds) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:728

___

### serialize

▸ **serialize**(): `any`

Serializes the Sound in a JSON representation

#### Returns

`any`

the JSON representation of the sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1091

___

### setAttenuationFunction

▸ **setAttenuationFunction**(`callback`): `void`

Sets a new custom attenuation function for the sound.

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music#creating-your-own-custom-attenuation-function

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`currentVolume`: `number`, `currentDistance`: `number`, `maxDistance`: `number`, `refDistance`: `number`, `rolloffFactor`: `number`) => `number` | Defines the function used for the attenuation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:718

___

### setAudioBuffer

▸ **setAudioBuffer**(`audioBuffer`): `void`

Sets the data of the sound from an audiobuffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `audioBuffer` | `AudioBuffer` | The audioBuffer containing the data |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:472

___

### setDirectionalCone

▸ **setDirectionalCone**(`coneInnerAngle`, `coneOuterAngle`, `coneOuterGain`): `void`

Transform this sound into a directional source

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `coneInnerAngle` | `number` | Size of the inner cone in degree |
| `coneOuterAngle` | `number` | Size of the outer cone in degree |
| `coneOuterGain` | `number` | Volume of the sound outside the outer cone (between 0.0 and 1.0) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:599

___

### setLocalDirectionToMesh

▸ **setLocalDirectionToMesh**(`newLocalDirection`): `void`

Sets the local direction of the emitter if spatial sound is enabled

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newLocalDirection` | [`Vector3`](Vector3.md) | Defines the new local direction |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:684

___

### setPlaybackRate

▸ **setPlaybackRate**(`newPlaybackRate`): `void`

Set the sound play back rate

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newPlaybackRate` | `number` | Define the playback rate the sound should be played at |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:949

___

### setPosition

▸ **setPosition**(`newPosition`): `void`

Sets the position of the emitter if spatial sound is enabled

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) | Defines the new position |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:667

___

### setVolume

▸ **setVolume**(`newVolume`, `time?`): `void`

Sets a dedicated volume for this sounds

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newVolume` | `number` | Define the new volume of the sound |
| `time?` | `number` | Define time for gradual change to new volume |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:932

___

### stop

▸ **stop**(`time?`): `void`

Stop the sound

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `time?` | `number` | (optional) Stop the sound after X seconds. Stop immediately (0) by default. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:876

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

https://github.com/babylon.js/core/src/Audio/sound.ts:568

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

https://github.com/babylon.js/core/src/Audio/sound.ts:558

___

### updateOptions

▸ **updateOptions**(`options`): `void`

Updates the current sounds options such as maxdistance, loop...

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ISoundOptions`](../interfaces/ISoundOptions.md) | A JSON object containing values named as the object properties |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:483

___

### Parse

▸ `Static` **Parse**(`parsedSound`, `scene`, `rootUrl`, `sourceSound?`): [`Sound`](Sound.md)

Parse a JSON representation of a sound to instantiate in a given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedSound` | `any` | Define the JSON representation of the sound (usually coming from the serialize method) |
| `scene` | [`Scene`](Scene.md) | Define the scene the new parsed sound should be created in |
| `rootUrl` | `string` | Define the rooturl of the load in case we need to fetch relative dependencies |
| `sourceSound?` | [`Sound`](Sound.md) | Define a sound place holder if do not need to instantiate a new one |

#### Returns

[`Sound`](Sound.md)

the newly parsed sound

#### Defined in

https://github.com/babylon.js/core/src/Audio/sound.ts:1136

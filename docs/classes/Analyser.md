[@dev/core](../README.md) / [Exports](../modules.md) / Analyser

# Class: Analyser

Class used to work with sound analyzer using fast fourier transform (FFT)

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

## Table of contents

### Constructors

- [constructor](Analyser.md#constructor)

### Properties

- [BARGRAPHAMPLITUDE](Analyser.md#bargraphamplitude)
- [DEBUGCANVASPOS](Analyser.md#debugcanvaspos)
- [DEBUGCANVASSIZE](Analyser.md#debugcanvassize)
- [FFT\_SIZE](Analyser.md#fft_size)
- [SMOOTHING](Analyser.md#smoothing)
- [\_audioEngine](Analyser.md#_audioengine)
- [\_byteFreqs](Analyser.md#_bytefreqs)
- [\_byteTime](Analyser.md#_bytetime)
- [\_debugCanvas](Analyser.md#_debugcanvas)
- [\_debugCanvasContext](Analyser.md#_debugcanvascontext)
- [\_floatFreqs](Analyser.md#_floatfreqs)
- [\_registerFunc](Analyser.md#_registerfunc)
- [\_scene](Analyser.md#_scene)
- [\_webAudioAnalyser](Analyser.md#_webaudioanalyser)

### Methods

- [connectAudioNodes](Analyser.md#connectaudionodes)
- [dispose](Analyser.md#dispose)
- [drawDebugCanvas](Analyser.md#drawdebugcanvas)
- [getByteFrequencyData](Analyser.md#getbytefrequencydata)
- [getByteTimeDomainData](Analyser.md#getbytetimedomaindata)
- [getFloatFrequencyData](Analyser.md#getfloatfrequencydata)
- [getFrequencyBinCount](Analyser.md#getfrequencybincount)
- [stopDebugCanvas](Analyser.md#stopdebugcanvas)

## Constructors

### constructor

• **new Analyser**(`scene?`)

Creates a new analyser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines hosting scene |

#### Defined in

packages/dev/core/src/Audio/analyser.ts:54

## Properties

### BARGRAPHAMPLITUDE

• **BARGRAPHAMPLITUDE**: `number` = `256`

Gets or sets the bar graph amplitude

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Audio/analyser.ts:28

___

### DEBUGCANVASPOS

• **DEBUGCANVASPOS**: `Object`

Gets or sets the position of the debug canvas

**`Ignorenaming`**

#### Type declaration

| Name | Type |
| :------ | :------ |
| `x` | `number` |
| `y` | `number` |

#### Defined in

packages/dev/core/src/Audio/analyser.ts:33

___

### DEBUGCANVASSIZE

• **DEBUGCANVASSIZE**: `Object`

Gets or sets the debug canvas size

**`Ignorenaming`**

#### Type declaration

| Name | Type |
| :------ | :------ |
| `height` | `number` |
| `width` | `number` |

#### Defined in

packages/dev/core/src/Audio/analyser.ts:38

___

### FFT\_SIZE

• **FFT\_SIZE**: `number` = `512`

Gets or sets the FFT table size

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Audio/analyser.ts:23

___

### SMOOTHING

• **SMOOTHING**: `number` = `0.75`

Gets or sets the smoothing

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Audio/analyser.ts:18

___

### \_audioEngine

• `Private` **\_audioEngine**: [`IAudioEngine`](../interfaces/IAudioEngine.md)

#### Defined in

packages/dev/core/src/Audio/analyser.ts:48

___

### \_byteFreqs

• `Private` **\_byteFreqs**: `Uint8Array`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:40

___

### \_byteTime

• `Private` **\_byteTime**: `Uint8Array`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:41

___

### \_debugCanvas

• `Private` **\_debugCanvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:44

___

### \_debugCanvasContext

• `Private` **\_debugCanvasContext**: [`Nullable`](../modules.md#nullable)`CanvasRenderingContext2D`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:45

___

### \_floatFreqs

• `Private` **\_floatFreqs**: `Float32Array`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:42

___

### \_registerFunc

• `Private` **\_registerFunc**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:47

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Audio/analyser.ts:46

___

### \_webAudioAnalyser

• `Private` **\_webAudioAnalyser**: `AnalyserNode`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:43

## Methods

### connectAudioNodes

▸ **connectAudioNodes**(`inputAudioNode`, `outputAudioNode`): `void`

Connects two audio nodes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `inputAudioNode` | `AudioNode` | defines first node to connect |
| `outputAudioNode` | `AudioNode` | defines second node to connect |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:190

___

### dispose

▸ **dispose**(): `void`

Releases all associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:200

___

### drawDebugCanvas

▸ **drawDebugCanvas**(): `void`

Renders the debug canvas

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:133

___

### getByteFrequencyData

▸ **getByteFrequencyData**(): `Uint8Array`

Gets the current frequency data as a byte array

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/AnalyserNode/getByteFrequencyData

#### Returns

`Uint8Array`

a Uint8Array

#### Defined in

packages/dev/core/src/Audio/analyser.ts:93

___

### getByteTimeDomainData

▸ **getByteTimeDomainData**(): `Uint8Array`

Gets the current waveform as a byte array

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/AnalyserNode/getByteTimeDomainData

#### Returns

`Uint8Array`

a Uint8Array

#### Defined in

packages/dev/core/src/Audio/analyser.ts:107

___

### getFloatFrequencyData

▸ **getFloatFrequencyData**(): `Float32Array`

Gets the current frequency data as a float array

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/AnalyserNode/getByteFrequencyData

#### Returns

`Float32Array`

a Float32Array

#### Defined in

packages/dev/core/src/Audio/analyser.ts:121

___

### getFrequencyBinCount

▸ **getFrequencyBinCount**(): `number`

Get the number of data values you will have to play with for the visualization

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/AnalyserNode/frequencyBinCount

#### Returns

`number`

a number

#### Defined in

packages/dev/core/src/Audio/analyser.ts:80

___

### stopDebugCanvas

▸ **stopDebugCanvas**(): `void`

Stops rendering the debug canvas and removes it

#### Returns

`void`

#### Defined in

packages/dev/core/src/Audio/analyser.ts:173

[@dev/core](../README.md) / [Exports](../modules.md) / VideoRecorder

# Class: VideoRecorder

This can help with recording videos from BabylonJS.
This is based on the available WebRTC functionalities of the browser.

**`See`**

https://doc.babylonjs.com/how_to/render_scene_on_a_video

## Table of contents

### Constructors

- [constructor](VideoRecorder.md#constructor)

### Properties

- [\_canvas](VideoRecorder.md#_canvas)
- [\_fileName](VideoRecorder.md#_filename)
- [\_mediaRecorder](VideoRecorder.md#_mediarecorder)
- [\_options](VideoRecorder.md#_options)
- [\_recordedChunks](VideoRecorder.md#_recordedchunks)
- [\_reject](VideoRecorder.md#_reject)
- [\_resolve](VideoRecorder.md#_resolve)
- [\_DefaultOptions](VideoRecorder.md#_defaultoptions)

### Accessors

- [isRecording](VideoRecorder.md#isrecording)

### Methods

- [\_handleDataAvailable](VideoRecorder.md#_handledataavailable)
- [\_handleError](VideoRecorder.md#_handleerror)
- [\_handleStop](VideoRecorder.md#_handlestop)
- [dispose](VideoRecorder.md#dispose)
- [startRecording](VideoRecorder.md#startrecording)
- [stopRecording](VideoRecorder.md#stoprecording)
- [IsSupported](VideoRecorder.md#issupported)

## Constructors

### constructor

• **new VideoRecorder**(`engine`, `options?`)

Create a new VideoCapture object which can help converting what you see in Babylon to a video file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | Defines the BabylonJS Engine you wish to record. |
| `options` | `Partial`[`VideoRecorderOptions`](../interfaces/VideoRecorderOptions.md) | Defines options that can be used to customize the capture. |

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:110

## Properties

### \_canvas

• `Private` **\_canvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:90

___

### \_fileName

• `Private` **\_fileName**: [`Nullable`](../modules.md#nullable)`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:94

___

### \_mediaRecorder

• `Private` **\_mediaRecorder**: [`Nullable`](../modules.md#nullable)`MediaRecorder`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:91

___

### \_options

• `Private` `Readonly` **\_options**: [`VideoRecorderOptions`](../interfaces/VideoRecorderOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:89

___

### \_recordedChunks

• `Private` **\_recordedChunks**: `any`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:93

___

### \_reject

• `Private` **\_reject**: [`Nullable`](../modules.md#nullable)(`error`: `any`) => `void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:96

___

### \_resolve

• `Private` **\_resolve**: [`Nullable`](../modules.md#nullable)(`blob`: `Blob`) => `void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:95

___

### \_DefaultOptions

▪ `Static` `Private` `Readonly` **\_DefaultOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fps` | `number` |
| `mimeType` | `string` |
| `recordChunckSize` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:73

## Accessors

### isRecording

• `get` **isRecording**(): `boolean`

True when a recording is already in progress.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:101

## Methods

### \_handleDataAvailable

▸ `Private` **_handleDataAvailable**(`event`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:207

___

### \_handleError

▸ `Private` **_handleError**(`event`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `ErrorEvent` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:213

___

### \_handleStop

▸ `Private` **_handleStop**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:223

___

### dispose

▸ **dispose**(): `void`

Releases internal resources used during the recording.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:197

___

### startRecording

▸ **startRecording**(`fileName?`, `maxDuration?`): `Promise``Blob`

Starts recording the canvas for a max duration specified in parameters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fileName` | [`Nullable`](../modules.md#nullable)`string` | `"babylonjs.webm"` | Defines the name of the file to be downloaded when the recording stop.  If null no automatic download will start and you can rely on the promise to get the data back. |
| `maxDuration` | `number` | `7` | Defines the maximum recording time in seconds.  It defaults to 7 seconds. A value of zero will not stop automatically, you would need to call stopRecording manually. |

#### Returns

`Promise``Blob`

A promise callback at the end of the recording with the video data in Blob.

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:165

___

### stopRecording

▸ **stopRecording**(): `void`

Stops the current recording before the default capture timeout passed in the startRecording function.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:144

___

### IsSupported

▸ `Static` **IsSupported**(`engine`): `boolean`

Returns whether or not the VideoRecorder is available in your browser.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | Defines the Babylon Engine. |

#### Returns

`boolean`

true if supported otherwise false.

#### Defined in

https://github.com/babylon.js/core/src/Misc/videoRecorder.ts:84

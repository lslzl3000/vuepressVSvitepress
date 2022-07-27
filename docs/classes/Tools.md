[@dev/core](../README.md) / [Exports](../modules.md) / Tools

# Class: Tools

Class containing a set of static utilities functions

## Table of contents

### Constructors

- [constructor](Tools.md#constructor)

### Properties

- [AllLogLevel](Tools.md#allloglevel)
- [CustomRequestHeaders](Tools.md#customrequestheaders)
- [EndPerformanceCounter](Tools.md#endperformancecounter)
- [ErrorLogLevel](Tools.md#errorloglevel)
- [GetAbsoluteUrl](Tools.md#getabsoluteurl)
- [GetDOMTextContent](Tools.md#getdomtextcontent)
- [IsWindowObjectExist](Tools.md#iswindowobjectexist)
- [MessageLogLevel](Tools.md#messageloglevel)
- [NoneLogLevel](Tools.md#noneloglevel)
- [OnNewCacheEntry](Tools.md#onnewcacheentry)
- [PerformanceConsoleLogLevel](Tools.md#performanceconsoleloglevel)
- [PerformanceNoneLogLevel](Tools.md#performancenoneloglevel)
- [PerformanceUserMarkLogLevel](Tools.md#performanceusermarkloglevel)
- [StartPerformanceCounter](Tools.md#startperformancecounter)
- [UseCustomRequestHeaders](Tools.md#usecustomrequestheaders)
- [WarningLogLevel](Tools.md#warningloglevel)
- [\_Performance](Tools.md#_performance)
- [\_TmpFloatArray](Tools.md#_tmpfloatarray)

### Accessors

- [BaseUrl](Tools.md#baseurl)
- [CorsBehavior](Tools.md#corsbehavior)
- [DefaultRetryStrategy](Tools.md#defaultretrystrategy)
- [LogCache](Tools.md#logcache)
- [LogLevels](Tools.md#loglevels)
- [Now](Tools.md#now)
- [PerformanceLogLevel](Tools.md#performanceloglevel)
- [PreprocessUrl](Tools.md#preprocessurl)
- [RegisteredExternalClasses](Tools.md#registeredexternalclasses)
- [UseFallbackTexture](Tools.md#usefallbacktexture)
- [errorsCount](Tools.md#errorscount)
- [fallbackTexture](Tools.md#fallbacktexture)

### Methods

- [BackCompatCameraNoPreventDefault](Tools.md#backcompatcameranopreventdefault)
- [CleanUrl](Tools.md#cleanurl)
- [ClearLogCache](Tools.md#clearlogcache)
- [CreateScreenshot](Tools.md#createscreenshot)
- [CreateScreenshotAsync](Tools.md#createscreenshotasync)
- [CreateScreenshotUsingRenderTarget](Tools.md#createscreenshotusingrendertarget)
- [CreateScreenshotUsingRenderTargetAsync](Tools.md#createscreenshotusingrendertargetasync)
- [DecodeBase64](Tools.md#decodebase64)
- [DeepCopy](Tools.md#deepcopy)
- [DelayAsync](Tools.md#delayasync)
- [Download](Tools.md#download)
- [DownloadBlob](Tools.md#downloadblob)
- [DumpData](Tools.md#dumpdata)
- [DumpDataAsync](Tools.md#dumpdataasync)
- [DumpFramebuffer](Tools.md#dumpframebuffer)
- [EncodeScreenshotCanvasData](Tools.md#encodescreenshotcanvasdata)
- [Error](Tools.md#error)
- [FetchToRef](Tools.md#fetchtoref)
- [FileAsURL](Tools.md#fileasurl)
- [First](Tools.md#first)
- [FloatRound](Tools.md#floatround)
- [Format](Tools.md#format)
- [GetClassName](Tools.md#getclassname)
- [GetFilename](Tools.md#getfilename)
- [GetFolderPath](Tools.md#getfolderpath)
- [GetPointerPrefix](Tools.md#getpointerprefix)
- [Instantiate](Tools.md#instantiate)
- [IsBase64](Tools.md#isbase64)
- [IsEmpty](Tools.md#isempty)
- [IsExponentOfTwo](Tools.md#isexponentoftwo)
- [IsSafari](Tools.md#issafari)
- [LoadFile](Tools.md#loadfile)
- [LoadFileAsync](Tools.md#loadfileasync)
- [LoadImage](Tools.md#loadimage)
- [LoadScript](Tools.md#loadscript)
- [LoadScriptAsync](Tools.md#loadscriptasync)
- [Log](Tools.md#log)
- [MakeArray](Tools.md#makearray)
- [Mix](Tools.md#mix)
- [RandomId](Tools.md#randomid)
- [ReadFile](Tools.md#readfile)
- [ReadFileAsDataURL](Tools.md#readfileasdataurl)
- [RegisterTopRootEvents](Tools.md#registertoprootevents)
- [SetCorsBehavior](Tools.md#setcorsbehavior)
- [SetImmediate](Tools.md#setimmediate)
- [SetReferrerPolicyBehavior](Tools.md#setreferrerpolicybehavior)
- [ToBlob](Tools.md#toblob)
- [ToDegrees](Tools.md#todegrees)
- [ToRadians](Tools.md#toradians)
- [UnregisterTopRootEvents](Tools.md#unregistertoprootevents)
- [Warn](Tools.md#warn)
- [\_EndPerformanceConsole](Tools.md#_endperformanceconsole)
- [\_EndPerformanceCounterDisabled](Tools.md#_endperformancecounterdisabled)
- [\_EndUserMark](Tools.md#_endusermark)
- [\_StartPerformanceConsole](Tools.md#_startperformanceconsole)
- [\_StartPerformanceCounterDisabled](Tools.md#_startperformancecounterdisabled)
- [\_StartUserMark](Tools.md#_startusermark)
- [getFullClassName](Tools.md#getfullclassname)

## Constructors

### constructor

• **new Tools**()

## Properties

### AllLogLevel

▪ `Static` `Readonly` **AllLogLevel**: ``7``

All logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1064

___

### CustomRequestHeaders

▪ `Static` **CustomRequestHeaders**: `Object` = `WebRequest.CustomRequestHeaders`

Custom HTTP Request Headers to be sent with XMLHttpRequests
i.e. when loading files, where the server/service expects an Authorization header

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:64

___

### EndPerformanceCounter

▪ `Static` **EndPerformanceCounter**: (`counterName`: `string`, `condition?`: `boolean`) => `void` = `Tools._EndPerformanceCounterDisabled`

#### Type declaration

▸ (`counterName`, `condition?`): `void`

Ends a specific performance counter

##### Parameters

| Name | Type |
| :------ | :------ |
| `counterName` | `string` |
| `condition?` | `boolean` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1226

___

### ErrorLogLevel

▪ `Static` `Readonly` **ErrorLogLevel**: ``4``

Only error logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1060

___

### GetAbsoluteUrl

▪ `Static` **GetAbsoluteUrl**: (`url`: `string`) => `string`

#### Type declaration

▸ (`url`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

##### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1031

___

### GetDOMTextContent

▪ `Static` **GetDOMTextContent**: (`element`: `HTMLElement`) => `string` = `GetDOMTextContent`

#### Type declaration

▸ (`element`): `string`

Extracts text content from a DOM element hierarchy

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `HTMLElement` | defines the root element |

##### Returns

`string`

a string

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:243

___

### IsWindowObjectExist

▪ `Static` **IsWindowObjectExist**: () => `boolean` = `IsWindowObjectExist`

#### Type declaration

▸ (): `boolean`

Checks if the window object exists

##### Returns

`boolean`

true if the window object exists

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1129

___

### MessageLogLevel

▪ `Static` `Readonly` **MessageLogLevel**: ``1``

Only message logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1052

___

### NoneLogLevel

▪ `Static` `Readonly` **NoneLogLevel**: ``0``

No log

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1048

___

### OnNewCacheEntry

▪ `Static` **OnNewCacheEntry**: (`entry`: `string`) => `void`

#### Type declaration

▸ (`entry`): `void`

Callback called when a new log is added

##### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | `string` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1078

___

### PerformanceConsoleLogLevel

▪ `Static` `Readonly` **PerformanceConsoleLogLevel**: ``2``

Log performance to the console

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1144

___

### PerformanceNoneLogLevel

▪ `Static` `Readonly` **PerformanceNoneLogLevel**: ``0``

No performance log

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1136

___

### PerformanceUserMarkLogLevel

▪ `Static` `Readonly` **PerformanceUserMarkLogLevel**: ``1``

Use user marks to log performance

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1140

___

### StartPerformanceCounter

▪ `Static` **StartPerformanceCounter**: (`counterName`: `string`, `condition?`: `boolean`) => `void` = `Tools._StartPerformanceCounterDisabled`

#### Type declaration

▸ (`counterName`, `condition?`): `void`

Starts a performance counter

##### Parameters

| Name | Type |
| :------ | :------ |
| `counterName` | `string` |
| `condition?` | `boolean` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1221

___

### UseCustomRequestHeaders

▪ `Static` **UseCustomRequestHeaders**: `boolean` = `false`

Enable/Disable Custom HTTP Request Headers globally.
default = false

**`See`**

CustomRequestHeaders

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:58

___

### WarningLogLevel

▪ `Static` `Readonly` **WarningLogLevel**: ``2``

Only warning logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1056

___

### \_Performance

▪ `Static` `Private` **\_Performance**: `Performance`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1146

___

### \_TmpFloatArray

▪ `Static` `Private` **\_TmpFloatArray**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:191

## Accessors

### BaseUrl

• `Static` `get` **BaseUrl**(): `string`

Gets or sets the base URL to use to load assets

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:45

• `Static` `set` **BaseUrl**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:49

___

### CorsBehavior

• `Static` `get` **CorsBehavior**(): `string` \| (`url`: `string` \| `string`[]) => `string`

Default behaviour for cors in the application.
It can be a string if the expected behavior is identical in the entire app.
Or a callback to be able to set it per url or on a group of them (in case of Video source for instance)

#### Returns

`string` \| (`url`: `string` \| `string`[]) => `string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:82

• `Static` `set` **CorsBehavior**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` \| (`url`: `string` \| `string`[]) => `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:86

___

### DefaultRetryStrategy

• `Static` `get` **DefaultRetryStrategy**(): (`url`: `string`, `request`: [`WebRequest`](WebRequest.md), `retryIndex`: `number`) => `number`

Gets or sets the retry strategy to apply when an error happens while loading an asset

#### Returns

`fn`

▸ (`url`, `request`, `retryIndex`): `number`

##### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `request` | [`WebRequest`](WebRequest.md) |
| `retryIndex` | `number` |

##### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:69

• `Static` `set` **DefaultRetryStrategy**(`strategy`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `strategy` | (`url`: `string`, `request`: [`WebRequest`](WebRequest.md), `retryIndex`: `number`) => `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:73

___

### LogCache

• `Static` `get` **LogCache**(): `string`

Gets current log cache (list of logs)

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1107

___

### LogLevels

• `Static` `set` **LogLevels**(`level`): `void`

Sets the current log level (MessageLogLevel / WarningLogLevel / ErrorLogLevel)

#### Parameters

| Name | Type |
| :------ | :------ |
| `level` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1121

___

### Now

• `Static` `get` **Now**(): `number`

Gets either window.performance.now() if supported or Date.now() else

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1231

___

### PerformanceLogLevel

• `Static` `set` **PerformanceLogLevel**(`level`): `void`

Sets the current performance log level

#### Parameters

| Name | Type |
| :------ | :------ |
| `level` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1151

___

### PreprocessUrl

• `Static` `get` **PreprocessUrl**(): (`url`: `string`) => `string`

Gets or sets a function used to pre-process url before using them to load assets

#### Returns

`fn`

▸ (`url`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

##### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:338

• `Static` `set` **PreprocessUrl**(`processor`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `processor` | (`url`: `string`) => `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:342

___

### RegisteredExternalClasses

• `Static` `get` **RegisteredExternalClasses**(): `Object`

Use this object to register external classes like custom textures or material
to allow the loaders to instantiate them

#### Returns

`Object`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:106

• `Static` `set` **RegisteredExternalClasses**(`classes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `classes` | `Object` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:110

___

### UseFallbackTexture

• `Static` `get` **UseFallbackTexture**(): `boolean`

Gets or sets a global variable indicating if fallback texture must be used when a texture cannot be loaded

**`Ignorenaming`**

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:94

• `Static` `set` **UseFallbackTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:98

___

### errorsCount

• `Static` `get` **errorsCount**(): `number`

Gets a value indicating the number of loading errors

**`Ignorenaming`**

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1071

___

### fallbackTexture

• `Static` `get` **fallbackTexture**(): `string`

Texture content used if a texture cannot loaded

**`Ignorenaming`**

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:119

• `Static` `set` **fallbackTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:124

## Methods

### BackCompatCameraNoPreventDefault

▸ `Static` **BackCompatCameraNoPreventDefault**(`args`): `boolean`

Will return the right value of the noPreventDefault variable
Needed to keep backwards compatibility to the old API.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `args` | `IArguments` | arguments passed to the attachControl function |

#### Returns

`boolean`

the correct value for noPreventDefault

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:885

___

### CleanUrl

▸ `Static` **CleanUrl**(`url`): `string`

Removes unwanted characters from an url

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the url to clean |

#### Returns

`string`

the cleaned url

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:330

___

### ClearLogCache

▸ `Static` **ClearLogCache**(): `void`

Clears the log cache

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1114

___

### CreateScreenshot

▸ `Static` **CreateScreenshot**(`engine`, `camera`, `size`, `successCallback?`, `mimeType?`): `void`

Captures a screenshot of the current rendering

**`See`**

https://doc.babylonjs.com/how_to/render_scene_on_a_png

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | `undefined` | defines the rendering engine |
| `camera` | [`Camera`](Camera.md) | `undefined` | defines the source camera |
| `size` | `number` \| [`IScreenshotSize`](../interfaces/IScreenshotSize.md) | `undefined` | This parameter can be set to a single number or to an object with the  following (optional) properties: precision, width, height. If a single number is passed,  it will be used for both width and height. If an object is passed, the screenshot size  will be derived from the parameters. The precision property is a multiplier allowing  rendering at a higher or lower resolution |
| `successCallback?` | (`data`: `string`) => `void` | `undefined` | defines the callback receives a single parameter which contains the  screenshot as a string of base64-encoded characters. This string can be assigned to the  src parameter of an  to display it |
| `mimeType` | `string` | `"image/png"` | defines the MIME type of the screenshot image (default: image/png).  Check your browser for supported MIME types |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:913

___

### CreateScreenshotAsync

▸ `Static` **CreateScreenshotAsync**(`engine`, `camera`, `size`, `mimeType?`): `Promise``string`

Captures a screenshot of the current rendering

**`See`**

https://doc.babylonjs.com/how_to/render_scene_on_a_png

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | `undefined` | defines the rendering engine |
| `camera` | [`Camera`](Camera.md) | `undefined` | defines the source camera |
| `size` | `number` \| [`IScreenshotSize`](../interfaces/IScreenshotSize.md) | `undefined` | This parameter can be set to a single number or to an object with the  following (optional) properties: precision, width, height. If a single number is passed,  it will be used for both width and height. If an object is passed, the screenshot size  will be derived from the parameters. The precision property is a multiplier allowing  rendering at a higher or lower resolution |
| `mimeType` | `string` | `"image/png"` | defines the MIME type of the screenshot image (default: image/png).  Check your browser for supported MIME types |

#### Returns

`Promise``string`

screenshot as a string of base64-encoded characters. This string can be assigned
to the src parameter of an  to display it

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:933

___

### CreateScreenshotUsingRenderTarget

▸ `Static` **CreateScreenshotUsingRenderTarget**(`engine`, `camera`, `size`, `successCallback?`, `mimeType?`, `samples?`, `antialiasing?`, `fileName?`): `void`

Generates an image screenshot from the specified camera.

**`See`**

https://doc.babylonjs.com/how_to/render_scene_on_a_png

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | `undefined` | The engine to use for rendering |
| `camera` | [`Camera`](Camera.md) | `undefined` | The camera to use for rendering |
| `size` | `number` \| [`IScreenshotSize`](../interfaces/IScreenshotSize.md) | `undefined` | This parameter can be set to a single number or to an object with the  following (optional) properties: precision, width, height. If a single number is passed,  it will be used for both width and height. If an object is passed, the screenshot size  will be derived from the parameters. The precision property is a multiplier allowing  rendering at a higher or lower resolution |
| `successCallback?` | (`data`: `string`) => `void` | `undefined` | The callback receives a single parameter which contains the  screenshot as a string of base64-encoded characters. This string can be assigned to the  src parameter of an  to display it |
| `mimeType` | `string` | `"image/png"` | The MIME type of the screenshot image (default: image/png).  Check your browser for supported MIME types |
| `samples` | `number` | `1` | Texture samples (default: 1) |
| `antialiasing` | `boolean` | `false` | Whether antialiasing should be turned on or not (default: false) |
| `fileName?` | `string` | `undefined` | A name for for the downloaded file. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:957

___

### CreateScreenshotUsingRenderTargetAsync

▸ `Static` **CreateScreenshotUsingRenderTargetAsync**(`engine`, `camera`, `size`, `mimeType?`, `samples?`, `antialiasing?`, `fileName?`): `Promise``string`

Generates an image screenshot from the specified camera.

**`See`**

https://doc.babylonjs.com/how_to/render_scene_on_a_png

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | `undefined` | The engine to use for rendering |
| `camera` | [`Camera`](Camera.md) | `undefined` | The camera to use for rendering |
| `size` | `number` \| [`IScreenshotSize`](../interfaces/IScreenshotSize.md) | `undefined` | This parameter can be set to a single number or to an object with the  following (optional) properties: precision, width, height. If a single number is passed,  it will be used for both width and height. If an object is passed, the screenshot size  will be derived from the parameters. The precision property is a multiplier allowing  rendering at a higher or lower resolution |
| `mimeType` | `string` | `"image/png"` | The MIME type of the screenshot image (default: image/png).  Check your browser for supported MIME types |
| `samples` | `number` | `1` | Texture samples (default: 1) |
| `antialiasing` | `boolean` | `false` | Whether antialiasing should be turned on or not (default: false) |
| `fileName?` | `string` | `undefined` | A name for for the downloaded file. |

#### Returns

`Promise``string`

screenshot as a string of base64-encoded characters. This string can be assigned
to the src parameter of an  to display it

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:989

___

### DecodeBase64

▸ `Static` **DecodeBase64**(`uri`): `ArrayBuffer`

Decode the given base64 uri.

**`Deprecated`**

Please use FileTools.DecodeBase64UrlToBinary instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | `string` | The uri to decode |

#### Returns

`ArrayBuffer`

The decoded base64 data.

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1027

___

### DeepCopy

▸ `Static` **DeepCopy**(`source`, `destination`, `doNotCopyList?`, `mustCopyList?`): `void`

Tries to copy an object by duplicating every property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | defines the source object |
| `destination` | `any` | defines the target object |
| `doNotCopyList?` | `string`[] | defines a list of properties to avoid |
| `mustCopyList?` | `string`[] | defines a list of properties to copy (even if they start with _) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:545

___

### DelayAsync

▸ `Static` **DelayAsync**(`delay`): `Promise``void`

Returns a promise that resolves after the given amount of time.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `delay` | `number` | Number of milliseconds to delay |

#### Returns

`Promise``void`

Promise that resolves after the given amount of time

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1313

___

### Download

▸ `Static` **Download**(`blob`, `fileName`): `void`

Downloads a blob in the browser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blob` | `Blob` | defines the blob to download |
| `fileName` | `string` | defines the name of the downloaded file |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:857

___

### DownloadBlob

▸ `Static` **DownloadBlob**(`blob`, `fileName?`): `void`

Download a Blob object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blob` | `Blob` | the Blob object |
| `fileName?` | `string` | the file name to download |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:791

___

### DumpData

▸ `Static` **DumpData**(`width`, `height`, `data`, `successCallback?`, `mimeType?`, `fileName?`, `invertY?`, `toArrayBuffer?`, `quality?`): `void`

Dumps an array buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the rendering width |
| `height` | `number` | `undefined` | defines the rendering height |
| `data` | `ArrayBufferView` | `undefined` | the data array |
| `successCallback?` | (`data`: `string` \| `ArrayBuffer`) => `void` | `undefined` | defines the callback triggered once the data are available |
| `mimeType` | `string` | `"image/png"` | defines the mime type of the result |
| `fileName?` | `string` | `undefined` | defines the filename to download. If present, the result will automatically be downloaded |
| `invertY` | `boolean` | `false` | true to invert the picture in the Y dimension |
| `toArrayBuffer` | `boolean` | `false` | true to convert the data to an ArrayBuffer (encoded as `mimeType`) instead of a base64 string |
| `quality?` | `number` | `undefined` | defines the quality of the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:646

___

### DumpDataAsync

▸ `Static` **DumpDataAsync**(`width`, `height`, `data`, `mimeType?`, `fileName?`, `invertY?`, `toArrayBuffer?`, `quality?`): `Promise``string` \| `ArrayBuffer`

Dumps an array buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the rendering width |
| `height` | `number` | `undefined` | defines the rendering height |
| `data` | `ArrayBufferView` | `undefined` | the data array |
| `mimeType` | `string` | `"image/png"` | defines the mime type of the result |
| `fileName?` | `string` | `undefined` | defines the filename to download. If present, the result will automatically be downloaded |
| `invertY` | `boolean` | `false` | true to invert the picture in the Y dimension |
| `toArrayBuffer` | `boolean` | `false` | true to convert the data to an ArrayBuffer (encoded as `mimeType`) instead of a base64 string |
| `quality?` | `number` | `undefined` | defines the quality of the result |

#### Returns

`Promise``string` \| `ArrayBuffer`

a promise that resolve to the final data

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:736

___

### DumpFramebuffer

▸ `Static` **DumpFramebuffer**(`width`, `height`, `engine`, `successCallback?`, `mimeType?`, `fileName?`): `Promise``void`

Dumps the current bound framebuffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the rendering width |
| `height` | `number` | `undefined` | defines the rendering height |
| `engine` | [`Engine`](Engine.md) | `undefined` | defines the hosting engine |
| `successCallback?` | (`data`: `string`) => `void` | `undefined` | defines the callback triggered once the data are available |
| `mimeType` | `string` | `"image/png"` | defines the mime type of the result |
| `fileName?` | `string` | `undefined` | defines the filename to download. If present, the result will automatically be downloaded |

#### Returns

`Promise``void`

a void promise

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:618

___

### EncodeScreenshotCanvasData

▸ `Static` **EncodeScreenshotCanvasData**(`successCallback?`, `mimeType?`, `fileName?`, `canvas?`, `quality?`): `void`

Encodes the canvas data to base 64 or automatically download the result if filename is defined

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `successCallback?` | (`data`: `string`) => `void` | `undefined` | defines the callback triggered once the data are available |
| `mimeType` | `string` | `"image/png"` | defines the mime type of the result |
| `fileName?` | `string` | `undefined` | defines he filename to download. If present, the result will automatically be downloaded |
| `canvas?` | `HTMLCanvasElement` | `undefined` | canvas to get the data from. If not provided, use the default screenshot canvas |
| `quality?` | `number` | `undefined` | defines the quality of the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:828

___

### Error

▸ `Static` **Error**(`message`): `void`

Write an error message to the console

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | defines the message to log |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1100

___

### FetchToRef

▸ `Static` **FetchToRef**(`u`, `v`, `width`, `height`, `pixels`, `color`): `void`

Read the content of a byte array at a specified coordinates (taking in account wrapping)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `u` | `number` | defines the coordinate on X axis |
| `v` | `number` | defines the coordinate on Y axis |
| `width` | `number` | defines the width of the source data |
| `height` | `number` | defines the height of the source data |
| `pixels` | `Uint8Array` | defines the source byte array |
| `color` | `IColor4Like` | defines the output color |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:137

___

### FileAsURL

▸ `Static` **FileAsURL**(`content`): `string`

Creates a data url from a given string content

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `content` | `string` | defines the content to convert |

#### Returns

`string`

the new data url link

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:521

___

### First

▸ `Static` **First**`T`(`array`, `predicate`): [`Nullable`](../modules.md#nullable)`T`

Gets the first element of an array satisfying a given predicate

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | `T`[] | defines the array to browse |
| `predicate` | (`item`: `T`) => `boolean` | defines the predicate to use |

#### Returns

[`Nullable`](../modules.md#nullable)`T`

null if not found or the element

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1265

___

### FloatRound

▸ `Static` **FloatRound**(`value`): `number`

Returns the nearest 32-bit single precision float representation of a Number

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | A Number.  If the parameter is of a different type, it will get converted  to a number or to NaN if it cannot be converted |

#### Returns

`number`

number

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:199

___

### Format

▸ `Static` **Format**(`value`, `decimals?`): `string`

Format the given number to a specific decimal format

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `value` | `number` | `undefined` | defines the number to format |
| `decimals` | `number` | `2` | defines the number of decimals to use |

#### Returns

`string`

the formatted string

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:534

___

### GetClassName

▸ `Static` **GetClassName**(`object`, `isType?`): `string`

This method will return the name of the class used to create the instance of the given object.
It will works only on Javascript basic data types (number, string, ...) and instance of class declared with the

**`Class Name`**

decorator.

**`Class Name`**

decorator

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `object` | `any` | `undefined` | the object to get the class name from |
| `isType` | `boolean` | `false` | defines if the object is actually a type |

#### Returns

`string`

the name of the class, will be "object" for a custom data type not using the

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1242

___

### GetFilename

▸ `Static` **GetFilename**(`path`): `string`

Extracts the filename from a path

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | defines the path to use |

#### Returns

`string`

the filename

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:212

___

### GetFolderPath

▸ `Static` **GetFolderPath**(`uri`, `returnUnchangedIfNoSlash?`): `string`

Extracts the "folder" part of a path (everything before the filename).

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `uri` | `string` | `undefined` | The URI to extract the info from |
| `returnUnchangedIfNoSlash` | `boolean` | `false` | Do not touch the URI if no slashes are present |

#### Returns

`string`

The "folder" part of the path

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:227

___

### GetPointerPrefix

▸ `Static` **GetPointerPrefix**(`engine`): `string`

Gets the pointer prefix to use

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | defines the engine we are finding the prefix for |

#### Returns

`string`

"pointer" if touch is enabled. Else returns "mouse"

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:282

___

### Instantiate

▸ `Static` **Instantiate**(`className`): `any`

Tries to instantiate a new object from a given class name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `className` | `string` | defines the class name to instantiate |

#### Returns

`any`

the new object or null if the system was not able to do the instantiation

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:164

___

### IsBase64

▸ `Static` **IsBase64**(`uri`): `boolean`

Test if the given uri is a base64 string

**`Deprecated`**

Please use FileTools.IsBase64DataUrl instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | `string` | The uri to test |

#### Returns

`boolean`

True if the uri is a base64 string or false otherwise

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1017

___

### IsEmpty

▸ `Static` **IsEmpty**(`obj`): `boolean`

Gets a boolean indicating if the given object has no own property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to test |

#### Returns

`boolean`

true if object has no own property

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:554

___

### IsExponentOfTwo

▸ `Static` **IsExponentOfTwo**(`value`): `boolean`

Function indicating if a number is an exponent of 2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | defines the value to test |

#### Returns

`boolean`

true if the value is an exponent of 2

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:181

___

### IsSafari

▸ `Static` **IsSafari**(): `boolean`

Utility function to detect if the current user agent is Safari

#### Returns

`boolean`

whether or not the current user agent is safari

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1325

___

### LoadFile

▸ `Static` **LoadFile**(`url`, `onSuccess`, `onProgress?`, `offlineProvider?`, `useArrayBuffer?`, `onError?`): [`IFileRequest`](../interfaces/IFileRequest.md)

Loads a file from a url

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | url string, ArrayBuffer, or Blob to load |
| `onSuccess` | (`data`: `string` \| `ArrayBuffer`, `responseURL?`: `string`) => `void` | callback called when the file successfully loads |
| `onProgress?` | (`data`: `any`) => `void` | callback called while file is loading (if the server supports this mode) |
| `offlineProvider?` | [`IOfflineProvider`](../interfaces/IOfflineProvider.md) | defines the offline provider for caching |
| `useArrayBuffer?` | `boolean` | defines a boolean indicating that date must be returned as ArrayBuffer |
| `onError?` | (`request?`: [`WebRequest`](WebRequest.md), `exception?`: `any`) => `void` | callback called when the file fails to load |

#### Returns

[`IFileRequest`](../interfaces/IFileRequest.md)

a file request object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:377

___

### LoadFileAsync

▸ `Static` **LoadFileAsync**(`url`, `useArrayBuffer?`): `Promise``string` \| `ArrayBuffer`

Loads a file from a url

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | the file url to load |
| `useArrayBuffer` | `boolean` | `true` | defines a boolean indicating that date must be returned as ArrayBuffer |

#### Returns

`Promise``string` \| `ArrayBuffer`

a promise containing an ArrayBuffer corresponding to the loaded file

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:394

___

### LoadImage

▸ `Static` **LoadImage**(`input`, `onLoad`, `onError`, `offlineProvider`, `mimeType?`, `imageBitmapOptions?`): [`Nullable`](../modules.md#nullable)`HTMLImageElement`

Loads an image as an HTMLImageElement.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | `string` \| `ArrayBuffer` \| `Blob` | url string, ArrayBuffer, or Blob to load |
| `onLoad` | (`img`: `HTMLImageElement` \| `ImageBitmap`) => `void` | callback called when the image successfully loads |
| `onError` | (`message?`: `string`, `exception?`: `any`) => `void` | callback called when the image fails to load |
| `offlineProvider` | [`Nullable`](../modules.md#nullable)[`IOfflineProvider`](../interfaces/IOfflineProvider.md) | offline provider for caching |
| `mimeType?` | `string` | optional mime type |
| `imageBitmapOptions?` | `ImageBitmapOptions` | optional the options to use when creating an ImageBitmap |

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLImageElement`

the HTMLImageElement of the loaded image

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:356

___

### LoadScript

▸ `Static` **LoadScript**(`scriptUrl`, `onSuccess`, `onError?`, `scriptId?`): `void`

Load a script (identified by an url). When the url returns, the
content of this file is added into a new script element, attached to the DOM (body element)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scriptUrl` | `string` | defines the url of the script to laod |
| `onSuccess` | () => `void` | defines the callback called when the script is loaded |
| `onError?` | (`message?`: `string`, `exception?`: `any`) => `void` | defines the callback to call if an error occurs |
| `scriptId?` | `string` | defines the id of the script element |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:419

___

### LoadScriptAsync

▸ `Static` **LoadScriptAsync**(`scriptUrl`): `Promise``void`

Load an asynchronous script (identified by an url). When the url returns, the
content of this file is added into a new script element, attached to the DOM (body element)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scriptUrl` | `string` | defines the url of the script to laod |

#### Returns

`Promise``void`

a promise request object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:452

___

### Log

▸ `Static` **Log**(`message`): `void`

Log a message to the console

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | defines the message to log |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1084

___

### MakeArray

▸ `Static` **MakeArray**(`obj`, `allowsNullUndefined?`): [`Nullable`](../modules.md#nullable)`any`[]

Returns an array if obj is not an array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to evaluate as an array |
| `allowsNullUndefined?` | `boolean` | defines a boolean indicating if obj is allowed to be null or undefined |

#### Returns

[`Nullable`](../modules.md#nullable)`any`[]

either obj directly if obj is an array or a new array containing obj

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:269

___

### Mix

▸ `Static` **Mix**(`a`, `b`, `alpha`): `number`

Interpolates between a and b via alpha

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | `number` | The lower value (returned when alpha = 0) |
| `b` | `number` | The upper value (returned when alpha = 1) |
| `alpha` | `number` | The interpolation-factor |

#### Returns

`number`

The mixed value

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:155

___

### RandomId

▸ `Static` **RandomId**(): `string`

Implementation from http://stackoverflow.com/questions/105034/how-to-create-a-guid-uuid-in-javascript/2117523#answer-2117523
Be aware Math.random() could cause collisions, but:
"All but 6 of the 128 bits of the ID are randomly generated, which means that for any two ids, there's a 1 in 2^^122 (or 5.3x10^^36) chance they'll collide"

#### Returns

`string`

a pseudo random id

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1007

___

### ReadFile

▸ `Static` **ReadFile**(`file`, `onSuccess`, `onProgress?`, `useArrayBuffer?`, `onError?`): [`IFileRequest`](../interfaces/IFileRequest.md)

Reads a file from a File object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `File` | defines the file to load |
| `onSuccess` | (`data`: `any`) => `void` | defines the callback to call when data is loaded |
| `onProgress?` | (`ev`: `ProgressEvent``EventTarget`) => `any` | defines the callback to call during loading process |
| `useArrayBuffer?` | `boolean` | defines a boolean indicating that data must be returned as an ArrayBuffer |
| `onError?` | (`error`: `ReadFileError`) => `void` | defines the callback to call when an error occurs |

#### Returns

[`IFileRequest`](../interfaces/IFileRequest.md)

a file request object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:506

___

### ReadFileAsDataURL

▸ `Static` **ReadFileAsDataURL**(`fileToLoad`, `callback`, `progressCallback`): [`IFileRequest`](../interfaces/IFileRequest.md)

Loads a file from a blob

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fileToLoad` | `Blob` | defines the blob to use |
| `callback` | (`data`: `any`) => `void` | defines the callback to call when data is loaded |
| `progressCallback` | (`ev`: `ProgressEvent``EventTarget`) => `any` | defines the callback to call during loading process |

#### Returns

[`IFileRequest`](../interfaces/IFileRequest.md)

a file request object

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:473

___

### RegisterTopRootEvents

▸ `Static` **RegisterTopRootEvents**(`windowElement`, `events`): `void`

Function used to register events at window level

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `windowElement` | `Window` | defines the Window object to use |
| `events` | { `handler`: [`Nullable`](../modules.md#nullable)(`e`: `FocusEvent`) => `any` ; `name`: `string`  }[] | defines the events to register |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:568

___

### SetCorsBehavior

▸ `Static` **SetCorsBehavior**(`url`, `element`): `void`

Sets the cors behavior on a dom element. This will add the required Tools.CorsBehavior to the element.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` \| `string`[] | define the url we are trying |
| `element` | `Object` | define the dom element where to configure the cors policy |
| `element.crossOrigin` | ``null`` \| `string` |  |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:309

___

### SetImmediate

▸ `Static` **SetImmediate**(`action`): `void`

Polyfill for setImmediate

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | () => `void` | defines the action to execute after the current execution block |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:172

___

### SetReferrerPolicyBehavior

▸ `Static` **SetReferrerPolicyBehavior**(`referrerPolicy`, `element`): `void`

Sets the referrerPolicy behavior on a dom element.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `referrerPolicy` | [`Nullable`](../modules.md#nullable)`ReferrerPolicy` | define the referrer policy to use |
| `element` | `Object` | define the dom element where to configure the referrer policy |
| `element.referrerPolicy` | ``null`` \| `string` |  |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:319

___

### ToBlob

▸ `Static` **ToBlob**(`canvas`, `successCallback`, `mimeType?`, `quality?`): `void`

Converts the canvas data to blob.
This acts as a polyfill for browsers not supporting the to blob function.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | `undefined` | Defines the canvas to extract the data from |
| `successCallback` | (`blob`: [`Nullable`](../modules.md#nullable)`Blob`) => `void` | `undefined` | Defines the callback triggered once the data are available |
| `mimeType` | `string` | `"image/png"` | Defines the mime type of the result |
| `quality?` | `number` | `undefined` | defines the quality of the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:759

___

### ToDegrees

▸ `Static` **ToDegrees**(`angle`): `number`

Convert an angle in radians to degrees

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle to convert |

#### Returns

`number`

the angle in degrees

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:250

___

### ToRadians

▸ `Static` **ToRadians**(`angle`): `number`

Convert an angle in degrees to radians

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle to convert |

#### Returns

`number`

the angle in radians

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:259

___

### UnregisterTopRootEvents

▸ `Static` **UnregisterTopRootEvents**(`windowElement`, `events`): `void`

Function used to unregister events from window level

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `windowElement` | `Window` | defines the Window object to use |
| `events` | { `handler`: [`Nullable`](../modules.md#nullable)(`e`: `FocusEvent`) => `any` ; `name`: `string`  }[] | defines the events to unregister |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:588

___

### Warn

▸ `Static` **Warn**(`message`): `void`

Write a warning message to the console

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | defines the message to log |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1092

___

### \_EndPerformanceConsole

▸ `Static` `Private` **_EndPerformanceConsole**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `counterName` | `string` | `undefined` |
| `condition` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1208

___

### \_EndPerformanceCounterDisabled

▸ `Static` `Private` **_EndPerformanceCounterDisabled**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `counterName` | `string` |
| `condition?` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1172

___

### \_EndUserMark

▸ `Static` `Private` **_EndUserMark**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `counterName` | `string` | `undefined` |
| `condition` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1188

___

### \_StartPerformanceConsole

▸ `Static` `Private` **_StartPerformanceConsole**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `counterName` | `string` | `undefined` |
| `condition` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1196

___

### \_StartPerformanceCounterDisabled

▸ `Static` `Private` **_StartPerformanceCounterDisabled**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `counterName` | `string` |
| `condition?` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1169

___

### \_StartUserMark

▸ `Static` `Private` **_StartUserMark**(`counterName`, `condition?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `counterName` | `string` | `undefined` |
| `condition` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1174

___

### getFullClassName

▸ `Static` **getFullClassName**(`object`, `isType?`): [`Nullable`](../modules.md#nullable)`string`

This method will return the name of the full name of the class, including its owning module (if any).
It will works only on Javascript basic data types (number, string, ...) and instance of class declared with the

**`Class Name`**

decorator or implementing a method getClassName():string (in which case the module won't be specified).

**`Ignorenaming`**

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `object` | `any` | `undefined` | the object to get the class name from |
| `isType` | `boolean` | `false` | defines if the object is actually a type |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

a string that can have two forms: "moduleName.className" if module was specified when the class' Name was registered or "className" if there was not module specified.

#### Defined in

https://github.com/babylon.js/core/src/Misc/tools.ts:1284

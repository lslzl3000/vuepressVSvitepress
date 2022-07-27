[@dev/core](../README.md) / [Exports](../modules.md) / WebXRSessionManager

# Class: WebXRSessionManager

Manages an XRSession to work with Babylon's engine

**`See`**

https://doc.babylonjs.com/how_to/webxr_session_manager

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- `IWebXRRenderTargetTextureProvider`

## Table of contents

### Constructors

- [constructor](WebXRSessionManager.md#constructor)

### Properties

- [\_baseLayerRTTProvider](WebXRSessionManager.md#_baselayerrttprovider)
- [\_baseLayerWrapper](WebXRSessionManager.md#_baselayerwrapper)
- [\_engine](WebXRSessionManager.md#_engine)
- [\_onEngineDisposedObserver](WebXRSessionManager.md#_onenginedisposedobserver)
- [\_referenceSpace](WebXRSessionManager.md#_referencespace)
- [\_sessionMode](WebXRSessionManager.md#_sessionmode)
- [\_xrNavigator](WebXRSessionManager.md#_xrnavigator)
- [baseReferenceSpace](WebXRSessionManager.md#basereferencespace)
- [currentFrame](WebXRSessionManager.md#currentframe)
- [currentTimestamp](WebXRSessionManager.md#currenttimestamp)
- [defaultHeightCompensation](WebXRSessionManager.md#defaultheightcompensation)
- [inXRFrameLoop](WebXRSessionManager.md#inxrframeloop)
- [inXRSession](WebXRSessionManager.md#inxrsession)
- [onXRFrameObservable](WebXRSessionManager.md#onxrframeobservable)
- [onXRReferenceSpaceChanged](WebXRSessionManager.md#onxrreferencespacechanged)
- [onXRSessionEnded](WebXRSessionManager.md#onxrsessionended)
- [onXRSessionInit](WebXRSessionManager.md#onxrsessioninit)
- [scene](WebXRSessionManager.md#scene)
- [session](WebXRSessionManager.md#session)
- [viewerReferenceSpace](WebXRSessionManager.md#viewerreferencespace)

### Accessors

- [currentFrameRate](WebXRSessionManager.md#currentframerate)
- [fixedFoveation](WebXRSessionManager.md#fixedfoveation)
- [isFixedFoveationSupported](WebXRSessionManager.md#isfixedfoveationsupported)
- [isNative](WebXRSessionManager.md#isnative)
- [referenceSpace](WebXRSessionManager.md#referencespace)
- [sessionMode](WebXRSessionManager.md#sessionmode)
- [supportedFrameRates](WebXRSessionManager.md#supportedframerates)

### Methods

- [dispose](WebXRSessionManager.md#dispose)
- [exitXRAsync](WebXRSessionManager.md#exitxrasync)
- [getRenderTargetTextureForEye](WebXRSessionManager.md#getrendertargettextureforeye)
- [getRenderTargetTextureForView](WebXRSessionManager.md#getrendertargettextureforview)
- [getWebXRRenderTarget](WebXRSessionManager.md#getwebxrrendertarget)
- [initializeAsync](WebXRSessionManager.md#initializeasync)
- [initializeSessionAsync](WebXRSessionManager.md#initializesessionasync)
- [isSessionSupportedAsync](WebXRSessionManager.md#issessionsupportedasync)
- [resetReferenceSpace](WebXRSessionManager.md#resetreferencespace)
- [runInXRFrame](WebXRSessionManager.md#runinxrframe)
- [runXRRenderLoop](WebXRSessionManager.md#runxrrenderloop)
- [setReferenceSpaceTypeAsync](WebXRSessionManager.md#setreferencespacetypeasync)
- [trySetViewportForView](WebXRSessionManager.md#trysetviewportforview)
- [updateRenderState](WebXRSessionManager.md#updaterenderstate)
- [updateRenderStateAsync](WebXRSessionManager.md#updaterenderstateasync)
- [updateTargetFrameRate](WebXRSessionManager.md#updatetargetframerate)
- [IsSessionSupportedAsync](WebXRSessionManager.md#issessionsupportedasync-1)

## Constructors

### constructor

• **new WebXRSessionManager**(`scene`)

Constructs a WebXRSessionManager, this must be initialized within a user action before usage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene which the session should be created for |

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:84

## Properties

### \_baseLayerRTTProvider

• `Private` **\_baseLayerRTTProvider**: [`Nullable`](../modules.md#nullable)`WebXRLayerRenderTargetTextureProvider`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:25

___

### \_baseLayerWrapper

• `Private` **\_baseLayerWrapper**: [`Nullable`](../modules.md#nullable)`WebXRLayerWrapper`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:24

___

### \_engine

• `Private` **\_engine**: [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:22

___

### \_onEngineDisposedObserver

• `Private` **\_onEngineDisposedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:28

___

### \_referenceSpace

• `Private` **\_referenceSpace**: `XRReferenceSpace`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:23

___

### \_sessionMode

• `Private` **\_sessionMode**: `XRSessionMode`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:27

___

### \_xrNavigator

• `Private` **\_xrNavigator**: `any`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:26

___

### baseReferenceSpace

• **baseReferenceSpace**: `XRReferenceSpace`

The base reference space from which the session started. good if you want to reset your
reference space

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:34

___

### currentFrame

• **currentFrame**: [`Nullable`](../modules.md#nullable)`XRFrame`

Current XR frame

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:38

___

### currentTimestamp

• **currentTimestamp**: `number` = `-1`

WebXR timestamp updated every frame

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:40

___

### defaultHeightCompensation

• **defaultHeightCompensation**: `number` = `1.7`

Used just in case of a failure to initialize an immersive session.
The viewer reference space is compensated using this height, creating a kind of "viewer-floor" reference space

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:45

___

### inXRFrameLoop

• **inXRFrameLoop**: `boolean` = `false`

Are we currently in the XR loop?

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:74

___

### inXRSession

• **inXRSession**: `boolean` = `false`

Are we in an XR session?

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:78

___

### onXRFrameObservable

• **onXRFrameObservable**: [`Observable`](Observable.md)`XRFrame`

Fires every time a new xrFrame arrives which can be used to update the camera

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:49

___

### onXRReferenceSpaceChanged

• **onXRReferenceSpaceChanged**: [`Observable`](Observable.md)`XRReferenceSpace`

Fires when the reference space changed

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:53

___

### onXRSessionEnded

• **onXRSessionEnded**: [`Observable`](Observable.md)`any`

Fires when the xr session is ended either by the device or manually done

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:57

___

### onXRSessionInit

• **onXRSessionInit**: [`Observable`](Observable.md)`XRSession`

Fires when the xr session is initialized: right after requestSession was called and returned with a successful result

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:61

___

### scene

• **scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:86

___

### session

• **session**: `XRSession`

Underlying xr session

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:65

___

### viewerReferenceSpace

• **viewerReferenceSpace**: `XRReferenceSpace`

The viewer (head position) reference space. This can be used to get the XR world coordinates
or get the offset the player is currently at.

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:70

## Accessors

### currentFrameRate

• `get` **currentFrameRate**(): `undefined` \| `number`

The current frame rate as reported by the device

#### Returns

`undefined` \| `number`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:428

___

### fixedFoveation

• `get` **fixedFoveation**(): [`Nullable`](../modules.md#nullable)`number`

Get the fixed foveation currently set, as specified by the webxr specs
If this returns null, then fixed foveation is not supported

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:472

• `set` **fixedFoveation**(`value`): `void`

Set the fixed foveation to the specified value, as specified by the webxr specs
This value will be normalized to be between 0 and 1, 1 being max foveation, 0 being no foveation

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:480

___

### isFixedFoveationSupported

• `get` **isFixedFoveationSupported**(): `boolean`

Check if fixed foveation is supported on this device

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:464

___

### isNative

• `get` **isNative**(): `boolean`

Returns true if Babylon.js is using the BabylonNative backend, otherwise false

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:421

___

### referenceSpace

• `get` **referenceSpace**(): `XRReferenceSpace`

The current reference space used in this session. This reference space can constantly change!
It is mainly used to offset the camera's position.

#### Returns

`XRReferenceSpace`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:101

• `set` **referenceSpace**(`newReferenceSpace`): `void`

Set a new reference space and triggers the observable

#### Parameters

| Name | Type |
| :------ | :------ |
| `newReferenceSpace` | `XRReferenceSpace` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:108

___

### sessionMode

• `get` **sessionMode**(): `XRSessionMode`

The mode for the managed XR session

#### Returns

`XRSessionMode`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:116

___

### supportedFrameRates

• `get` **supportedFrameRates**(): `undefined` \| `Float32Array`

A list of supported frame rates (only available in-session!

#### Returns

`undefined` \| `Float32Array`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:435

## Methods

### dispose

▸ **dispose**(): `void`

Disposes of the session manager
This should be called explicitly by the dev, if required.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:124

___

### exitXRAsync

▸ **exitXRAsync**(): `Promise``void`

Stops the xrSession and restores the render loop

#### Returns

`Promise``void`

Promise which resolves after it exits XR

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:141

___

### getRenderTargetTextureForEye

▸ **getRenderTargetTextureForEye**(`eye`): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the correct render target texture to be rendered this frame for this eye

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eye` | `XREye` | the eye for which to get the render target |

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

the render target for the specified eye or null if not available

#### Implementation of

IWebXRRenderTargetTextureProvider.getRenderTargetTextureForEye

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:167

___

### getRenderTargetTextureForView

▸ **getRenderTargetTextureForView**(`view`): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the correct render target texture to be rendered this frame for this view

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `view` | `XRView` | the view for which to get the render target |

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

the render target for the specified view or null if not available

#### Implementation of

IWebXRRenderTargetTextureProvider.getRenderTargetTextureForView

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:176

___

### getWebXRRenderTarget

▸ **getWebXRRenderTarget**(`options?`): [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

Creates a WebXRRenderTarget object for the XR session

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`WebXRManagedOutputCanvasOptions`](WebXRManagedOutputCanvasOptions.md) | optional options to provide when creating a new render target |

#### Returns

[`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

a WebXR render target to which the session can render

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:185

___

### initializeAsync

▸ **initializeAsync**(): `Promise``void`

Initializes the manager
After initialization enterXR can be called to start an XR session

#### Returns

`Promise``void`

Promise which resolves after it is initialized

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:201

___

### initializeSessionAsync

▸ **initializeSessionAsync**(`xrSessionMode?`, `xrSessionInit?`): `Promise``XRSession`

Initializes an xr session

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `xrSessionMode` | `XRSessionMode` | `"immersive-vr"` | mode to initialize |
| `xrSessionInit` | `XRSessionInit` | `{}` | defines optional and required values to pass to the session builder |

#### Returns

`Promise``XRSession`

a promise which will resolve once the session has been initialized

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:216

___

### isSessionSupportedAsync

▸ **isSessionSupportedAsync**(`sessionMode`): `Promise``boolean`

Checks if a session would be supported for the creation options specified

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionMode` | `XRSessionMode` | session mode to check if supported eg. immersive-vr |

#### Returns

`Promise``boolean`

A Promise that resolves to true if supported and false if not

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:264

___

### resetReferenceSpace

▸ **resetReferenceSpace**(): `void`

Resets the reference space to the one started the session

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:271

___

### runInXRFrame

▸ **runInXRFrame**(`callback`, `ignoreIfNotInSession?`): `void`

Run a callback in the xr render loop

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `callback` | () => `void` | `undefined` | the callback to call when in XR Frame |
| `ignoreIfNotInSession` | `boolean` | `true` | if no session is currently running, run it first thing on the next session |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:453

___

### runXRRenderLoop

▸ **runXRRenderLoop**(): `void`

Starts rendering to the xr layer

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:278

___

### setReferenceSpaceTypeAsync

▸ **setReferenceSpaceTypeAsync**(`referenceSpaceType?`): `Promise``XRReferenceSpace`

Sets the reference space on the xr session

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `referenceSpaceType` | `XRReferenceSpaceType` | `"local-floor"` | space to set |

#### Returns

`Promise``XRReferenceSpace`

a promise that will resolve once the reference space has been set

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:318

___

### trySetViewportForView

▸ **trySetViewportForView**(`viewport`, `view`): `boolean`

Attempts to set the framebuffer-size-normalized viewport to be rendered this frame for this view.
In the event of a failure, the supplied viewport is not updated.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewport` | [`Viewport`](Viewport.md) | the viewport to which the view will be rendered |
| `view` | `XRView` | the view for which to set the viewport |

#### Returns

`boolean`

whether the operation was successful

#### Implementation of

IWebXRRenderTargetTextureProvider.trySetViewportForView

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:158

___

### updateRenderState

▸ **updateRenderState**(`state`): `void`

Updates the render state of the session

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `XRRenderStateInit` | state to set |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:383

___

### updateRenderStateAsync

▸ **updateRenderStateAsync**(`state`): `Promise``void`

Updates the render state of the session.
Note that this is deprecated in favor of WebXRSessionManager.updateRenderState().

**`Deprecated`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | `XRRenderState` | state to set |

#### Returns

`Promise``void`

a promise that resolves once the render state has been updated

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:363

___

### updateTargetFrameRate

▸ **updateTargetFrameRate**(`rate`): `Promise``void`

Set the framerate of the session.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rate` | `number` | the new framerate. This value needs to be in the supportedFrameRates array |

#### Returns

`Promise``void`

a promise that resolves once the framerate has been set

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:444

___

### IsSessionSupportedAsync

▸ `Static` **IsSessionSupportedAsync**(`sessionMode`): `Promise``boolean`

Returns a promise that resolves with a boolean indicating if the provided session mode is supported by this browser

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionMode` | `XRSessionMode` | defines the session to test |

#### Returns

`Promise``boolean`

a promise with boolean as final value

#### Defined in

packages/dev/core/src/XR/webXRSessionManager.ts:396

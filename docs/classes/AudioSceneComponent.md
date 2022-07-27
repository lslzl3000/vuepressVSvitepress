[@dev/core](../README.md) / [Exports](../modules.md) / AudioSceneComponent

# Class: AudioSceneComponent

Defines the sound scene component responsible to manage any sounds
in a given scene.

## Implements

- [`ISceneSerializableComponent`](../interfaces/ISceneSerializableComponent.md)

## Table of contents

### Constructors

- [constructor](AudioSceneComponent.md#constructor)

### Properties

- [\_audioEnabled](AudioSceneComponent.md#_audioenabled)
- [\_audioListenerPositionProvider](AudioSceneComponent.md#_audiolistenerpositionprovider)
- [\_cachedCameraDirection](AudioSceneComponent.md#_cachedcameradirection)
- [\_cachedCameraPosition](AudioSceneComponent.md#_cachedcameraposition)
- [\_cameraDirectionTemp](AudioSceneComponent.md#_cameradirectiontemp)
- [\_headphone](AudioSceneComponent.md#_headphone)
- [\_invertMatrixTemp](AudioSceneComponent.md#_invertmatrixtemp)
- [\_lastCheck](AudioSceneComponent.md#_lastcheck)
- [audioPositioningRefreshRate](AudioSceneComponent.md#audiopositioningrefreshrate)
- [name](AudioSceneComponent.md#name)
- [scene](AudioSceneComponent.md#scene)
- [\_CameraDirection](AudioSceneComponent.md#_cameradirection)

### Accessors

- [audioEnabled](AudioSceneComponent.md#audioenabled)
- [audioListenerPositionProvider](AudioSceneComponent.md#audiolistenerpositionprovider)
- [headphone](AudioSceneComponent.md#headphone)

### Methods

- [\_afterRender](AudioSceneComponent.md#_afterrender)
- [addFromContainer](AudioSceneComponent.md#addfromcontainer)
- [disableAudio](AudioSceneComponent.md#disableaudio)
- [dispose](AudioSceneComponent.md#dispose)
- [enableAudio](AudioSceneComponent.md#enableaudio)
- [rebuild](AudioSceneComponent.md#rebuild)
- [register](AudioSceneComponent.md#register)
- [removeFromContainer](AudioSceneComponent.md#removefromcontainer)
- [serialize](AudioSceneComponent.md#serialize)
- [switchAudioModeForHeadphones](AudioSceneComponent.md#switchaudiomodeforheadphones)
- [switchAudioModeForNormalSpeakers](AudioSceneComponent.md#switchaudiomodefornormalspeakers)

## Constructors

### constructor

• **new AudioSceneComponent**(`scene?`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:307

## Properties

### \_audioEnabled

• `Private` **\_audioEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:265

___

### \_audioListenerPositionProvider

• `Private` **\_audioListenerPositionProvider**: [`Nullable`](../modules.md#nullable)() => [`Vector3`](Vector3.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:288

___

### \_cachedCameraDirection

• `Private` **\_cachedCameraDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:484

___

### \_cachedCameraPosition

• `Private` **\_cachedCameraPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:485

___

### \_cameraDirectionTemp

• `Private` **\_cameraDirectionTemp**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:488

___

### \_headphone

• `Private` **\_headphone**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:274

___

### \_invertMatrixTemp

• `Private` **\_invertMatrixTemp**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:487

___

### \_lastCheck

• `Private` **\_lastCheck**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:486

___

### audioPositioningRefreshRate

• **audioPositioningRefreshRate**: `number` = `500`

Gets or sets a refresh rate when using 3D audio positioning

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:286

___

### name

• `Readonly` **name**: ``"Audio"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[name](../interfaces/ISceneSerializableComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:258

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[scene](../interfaces/ISceneSerializableComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:263

___

### \_CameraDirection

▪ `Static` `Private` **\_CameraDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:253

## Accessors

### audioEnabled

• `get` **audioEnabled**(): `boolean`

Gets whether audio is enabled or not.
Please use related enable/disable method to switch state.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:270

___

### audioListenerPositionProvider

• `get` **audioListenerPositionProvider**(): [`Nullable`](../modules.md#nullable)() => [`Vector3`](Vector3.md)

Gets the current audio listener position provider

#### Returns

[`Nullable`](../modules.md#nullable)() => [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:292

• `set` **audioListenerPositionProvider**(`value`): `void`

Sets a custom listener position for all sounds in the scene
By default, this is the position of the first active camera

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)() => [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:299

___

### headphone

• `get` **headphone**(): `boolean`

Gets whether audio is outputting to headphone or not.
Please use the according Switch methods to change output.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:279

## Methods

### \_afterRender

▸ `Private` **_afterRender**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:490

___

### addFromContainer

▸ **addFromContainer**(`container`): `void`

Adds all the elements from the container to the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | the container holding the elements |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[addFromContainer](../interfaces/ISceneSerializableComponent.md#addfromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:355

___

### disableAudio

▸ **disableAudio**(): `void`

Disables audio in the associated scene.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:404

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[dispose](../interfaces/ISceneSerializableComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:388

___

### enableAudio

▸ **enableAudio**(): `void`

Enables audio in the associated scene.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:428

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[rebuild](../interfaces/ISceneSerializableComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:329

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[register](../interfaces/ISceneSerializableComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:321

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | `undefined` | contains the elements to remove |
| `dispose` | `boolean` | `false` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[removeFromContainer](../interfaces/ISceneSerializableComponent.md#removefromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:371

___

### serialize

▸ **serialize**(`serializationObject`): `void`

Serializes the component data to the specified json object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | The object to serialize to |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[serialize](../interfaces/ISceneSerializableComponent.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:337

___

### switchAudioModeForHeadphones

▸ **switchAudioModeForHeadphones**(): `void`

Switch audio to headphone output.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:456

___

### switchAudioModeForNormalSpeakers

▸ **switchAudioModeForNormalSpeakers**(): `void`

Switch audio to normal speakers.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:471

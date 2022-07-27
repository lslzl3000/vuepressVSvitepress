[@dev/core](../README.md) / [Exports](../modules.md) / LensFlareSystem

# Class: LensFlareSystem

This represents a Lens Flare System or the shiny effect created by the light reflection on the  camera lenses.
It is usually composed of several `lensFlare`.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

## Table of contents

### Constructors

- [constructor](LensFlareSystem.md#constructor)

### Properties

- [\_emitter](LensFlareSystem.md#_emitter)
- [\_indexBuffer](LensFlareSystem.md#_indexbuffer)
- [\_isEnabled](LensFlareSystem.md#_isenabled)
- [\_positionX](LensFlareSystem.md#_positionx)
- [\_positionY](LensFlareSystem.md#_positiony)
- [\_scene](LensFlareSystem.md#_scene)
- [\_vertexBuffers](LensFlareSystem.md#_vertexbuffers)
- [borderLimit](LensFlareSystem.md#borderlimit)
- [id](LensFlareSystem.md#id)
- [layerMask](LensFlareSystem.md#layermask)
- [lensFlares](LensFlareSystem.md#lensflares)
- [meshesSelectionPredicate](LensFlareSystem.md#meshesselectionpredicate)
- [name](LensFlareSystem.md#name)
- [viewportBorder](LensFlareSystem.md#viewportborder)

### Accessors

- [isEnabled](LensFlareSystem.md#isenabled)
- [scene](LensFlareSystem.md#scene)

### Methods

- [\_createIndexBuffer](LensFlareSystem.md#_createindexbuffer)
- [dispose](LensFlareSystem.md#dispose)
- [getEmitter](LensFlareSystem.md#getemitter)
- [getEmitterPosition](LensFlareSystem.md#getemitterposition)
- [getScene](LensFlareSystem.md#getscene)
- [rebuild](LensFlareSystem.md#rebuild)
- [serialize](LensFlareSystem.md#serialize)
- [setEmitter](LensFlareSystem.md#setemitter)
- [Parse](LensFlareSystem.md#parse)

## Constructors

### constructor

• **new LensFlareSystem**(`name`, `emitter`, `scene`)

Instantiates a lens flare system.
This represents a Lens Flare System or the shiny effect created by the light reflection on the  camera lenses.
It is usually composed of several `lensFlare`.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the lens flare system in the scene |
| `emitter` | `any` | Define the source (the emitter) of the lens flares (it can be a camera, a light or a mesh). |
| `scene` | [`Scene`](Scene.md) | Define the scene the lens flare system belongs to |

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:88

## Properties

### \_emitter

• `Private` **\_emitter**: `any`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:64

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:66

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:69

___

### \_positionX

• `Private` **\_positionX**: `number`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:67

___

### \_positionY

• `Private` **\_positionY**: `number`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:68

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:63

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:65

___

### borderLimit

• **borderLimit**: `number` = `300`

Define a limit from the border the lens flare can be visible.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:35

___

### id

• **id**: `string`

Define the id of the lens flare system in the scene.
(equal to name by default)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:61

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Restricts the rendering of the effect to only the camera rendering this layer mask.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:50

___

### lensFlares

• **lensFlares**: [`LensFlare`](LensFlare.md)[]

List of lens flares used in this system.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:30

___

### meshesSelectionPredicate

• **meshesSelectionPredicate**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

Define a predicate which could limit the list of meshes able to occlude the effect.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:45

___

### name

• **name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:92

___

### viewportBorder

• **viewportBorder**: `number` = `0`

Define a viewport border we do not want to see the lens flare in.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:40

## Accessors

### isEnabled

• `get` **isEnabled**(): `boolean`

Define if the lens flare system is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:137

• `set` **isEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:141

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets the scene

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:53

## Methods

### \_createIndexBuffer

▸ `Private` **_createIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:121

___

### dispose

▸ **dispose**(): `void`

Dispose and release the lens flare with its associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:369

___

### getEmitter

▸ **getEmitter**(): `any`

Get the emitter of the lens flare system.
It defines the source of the lens flares (it can be a camera, a light or a mesh).

#### Returns

`any`

the emitter of the lens flare system

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:158

___

### getEmitterPosition

▸ **getEmitterPosition**(): [`Vector3`](Vector3.md)

Get the lens flare system emitter position.
The emitter defines the source of the lens flares (it can be a camera, a light or a mesh).

#### Returns

[`Vector3`](Vector3.md)

the position

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:176

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Get the scene the effects belongs to.

#### Returns

[`Scene`](Scene.md)

the scene holding the lens flare system

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:149

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the lens flare system

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:358

___

### serialize

▸ **serialize**(): `any`

Serialize the current Lens Flare System into a JSON representation.

#### Returns

`any`

the serialized JSON

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:425

___

### setEmitter

▸ **setEmitter**(`newEmitter`): `void`

Set the emitter of the lens flare system.
It defines the source of the lens flares (it can be a camera, a light or a mesh).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newEmitter` | `any` | Define the new emitter of the system |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:167

___

### Parse

▸ `Static` **Parse**(`parsedLensFlareSystem`, `scene`, `rootUrl`): [`LensFlareSystem`](LensFlareSystem.md)

Parse a lens flare system from a JSON representation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedLensFlareSystem` | `any` | Define the JSON to parse |
| `scene` | [`Scene`](Scene.md) | Define the scene the parsed system should be instantiated in |
| `rootUrl` | `string` | Define the rootUrl of the load sequence to easily find a load relative dependencies such as textures |

#### Returns

[`LensFlareSystem`](LensFlareSystem.md)

the parsed system

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystem.ts:397

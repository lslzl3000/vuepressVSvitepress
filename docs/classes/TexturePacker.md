[@dev/core](../README.md) / [Exports](../modules.md) / TexturePacker

# Class: TexturePacker

This is a support class that generates a series of packed texture sets.

**`See`**

https://doc.babylonjs.com/babylon101/materials

## Table of contents

### Constructors

- [constructor](TexturePacker.md#constructor)

### Properties

- [\_expecting](TexturePacker.md#_expecting)
- [\_paddingValue](TexturePacker.md#_paddingvalue)
- [frames](TexturePacker.md#frames)
- [meshes](TexturePacker.md#meshes)
- [name](TexturePacker.md#name)
- [options](TexturePacker.md#options)
- [promise](TexturePacker.md#promise)
- [scene](TexturePacker.md#scene)
- [sets](TexturePacker.md#sets)
- [LAYOUT\_COLNUM](TexturePacker.md#layout_colnum)
- [LAYOUT\_POWER2](TexturePacker.md#layout_power2)
- [LAYOUT\_STRIP](TexturePacker.md#layout_strip)
- [SUBUV\_COLOR](TexturePacker.md#subuv_color)
- [SUBUV\_EXTEND](TexturePacker.md#subuv_extend)
- [SUBUV\_WRAP](TexturePacker.md#subuv_wrap)

### Methods

- [\_calculateMeshUVFrames](TexturePacker.md#_calculatemeshuvframes)
- [\_calculateSize](TexturePacker.md#_calculatesize)
- [\_createFrames](TexturePacker.md#_createframes)
- [\_getFrameOffset](TexturePacker.md#_getframeoffset)
- [\_updateMeshUV](TexturePacker.md#_updatemeshuv)
- [\_updateTextureReferences](TexturePacker.md#_updatetexturereferences)
- [dispose](TexturePacker.md#dispose)
- [download](TexturePacker.md#download)
- [processAsync](TexturePacker.md#processasync)
- [setMeshToFrame](TexturePacker.md#setmeshtoframe)
- [updateFromJSON](TexturePacker.md#updatefromjson)

## Constructors

### constructor

• **new TexturePacker**(`name`, `meshes`, `options`, `scene`)

Initializes a texture package series from an array of meshes or a single mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the package |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | The target meshes to compose the package from |
| `options` | [`ITexturePackerOptions`](../interfaces/ITexturePackerOptions.md) | The arguments that texture packer should follow while building. |
| `scene` | [`Scene`](Scene.md) | The scene which the textures are scoped to. |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:164

## Properties

### \_expecting

• `Private` **\_expecting**: `number`

The expected number of textures the system is parsing.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:151

___

### \_paddingValue

• `Private` **\_paddingValue**: `number`

The padding value from Math.ceil(frameSize * paddingRatio)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:154

___

### frames

• **frames**: [`TexturePackerFrame`](TexturePackerFrame.md)[]

The Container array for the frames that are generated

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:148

___

### meshes

• **meshes**: [`AbstractMesh`](AbstractMesh.md)[]

The Meshes to target

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:136

___

### name

• **name**: `string`

The Name of the Texture Package

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:130

___

### options

• **options**: [`ITexturePackerOptions`](../interfaces/ITexturePackerOptions.md)

Arguments passed with the Constructor

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:139

___

### promise

• **promise**: [`Nullable`](../modules.md#nullable)`Promise``string` \| [`TexturePacker`](TexturePacker.md)

The promise that is started upon initialization

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:142

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene scope of the TexturePacker

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:133

___

### sets

• **sets**: `object`

The Container object for the channel sets that are generated

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:145

___

### LAYOUT\_COLNUM

▪ `Static` `Readonly` **LAYOUT\_COLNUM**: ``2``

Packer Layout Constant 2

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:120

___

### LAYOUT\_POWER2

▪ `Static` `Readonly` **LAYOUT\_POWER2**: ``1``

Packer Layout Constant 1

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:118

___

### LAYOUT\_STRIP

▪ `Static` `Readonly` **LAYOUT\_STRIP**: ``0``

Packer Layout Constant 0

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:116

___

### SUBUV\_COLOR

▪ `Static` `Readonly` **SUBUV\_COLOR**: ``2``

Packer Layout Constant 2

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:127

___

### SUBUV\_EXTEND

▪ `Static` `Readonly` **SUBUV\_EXTEND**: ``1``

Packer Layout Constant 1

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:125

___

### SUBUV\_WRAP

▪ `Static` `Readonly` **SUBUV\_WRAP**: ``0``

Packer Layout Constant 0

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:123

## Methods

### \_calculateMeshUVFrames

▸ `Private` **_calculateMeshUVFrames**(`baseSize`, `padding`, `dtSize`, `dtUnits`, `update`): `void`

Calculates the UV data for the frames.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseSize` | `number` | the base frameSize |
| `padding` | `number` | the base frame padding |
| `dtSize` | [`Vector2`](Vector2.md) | size of the Dynamic Texture for that channel |
| `dtUnits` | [`Vector2`](Vector2.md) | is 1/dtSize |
| `update` | `boolean` | flag to update the input meshes |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:418

___

### \_calculateSize

▸ `Private` **_calculateSize**(): [`Vector2`](Vector2.md)

Calculates the Size of the Channel Sets

#### Returns

[`Vector2`](Vector2.md)

Vector2

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:383

___

### \_createFrames

▸ `Private` **_createFrames**(`resolve`): `void`

Starts the package process

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resolve` | () => `void` | The promises resolution function |

#### Returns

`void`

TexturePacker

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:230

___

### \_getFrameOffset

▸ `Private` **_getFrameOffset**(`index`): [`Vector2`](Vector2.md)

Calculates the frames Offset.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | of the frame |

#### Returns

[`Vector2`](Vector2.md)

Vector2

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:447

___

### \_updateMeshUV

▸ `Private` **_updateMeshUV**(`mesh`, `frameID`): `void`

Updates a Mesh to the frame data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | that is the target |
| `frameID` | `number` | or the frame index |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:484

___

### \_updateTextureReferences

▸ `Private` **_updateTextureReferences**(`m`, `force?`): `void`

Updates a Meshes materials to use the texture packer channels

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `m` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | is the mesh to target |
| `force` | `boolean` | `false` | all channels on the packer to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:506

___

### dispose

▸ **dispose**(): `void`

Disposes all textures associated with this packer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:609

___

### download

▸ **download**(`imageType?`, `quality?`): `void`

Starts the download process for all the channels converting them to base64 data and embedding it all in a JSON file.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `imageType` | `string` | `"png"` | is the image type to use. |
| `quality` | `number` | `1` | of the image if downloading as jpeg, Ranges from >0 to 1. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:622

___

### processAsync

▸ **processAsync**(): `Promise``void`

Starts the async promise to compile the texture packer.

#### Returns

`Promise``void`

Promise

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:552

___

### setMeshToFrame

▸ **setMeshToFrame**(`m`, `frameID`, `updateMaterial?`): `void`

Public method to set a Mesh to a frame

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `m` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | that is the target |
| `frameID` | `number` | `undefined` | or the frame index |
| `updateMaterial` | `boolean` | `false` | trigger for if the Meshes attached Material be updated? |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:541

___

### updateFromJSON

▸ **updateFromJSON**(`data`): `void`

Public method to load a texturePacker JSON file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | of the JSON file in string format. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:666

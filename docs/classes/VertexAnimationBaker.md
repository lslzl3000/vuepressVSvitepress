[@dev/core](../README.md) / [Exports](../modules.md) / VertexAnimationBaker

# Class: VertexAnimationBaker

Class to bake vertex animation textures.

**`Since`**

5.0

## Table of contents

### Constructors

- [constructor](VertexAnimationBaker.md#constructor)

### Properties

- [\_mesh](VertexAnimationBaker.md#_mesh)
- [\_scene](VertexAnimationBaker.md#_scene)

### Methods

- [\_executeAnimationFrame](VertexAnimationBaker.md#_executeanimationframe)
- [bakeVertexData](VertexAnimationBaker.md#bakevertexdata)
- [loadBakedVertexDataFromJSON](VertexAnimationBaker.md#loadbakedvertexdatafromjson)
- [loadBakedVertexDataFromObject](VertexAnimationBaker.md#loadbakedvertexdatafromobject)
- [serializeBakedVertexDataToJSON](VertexAnimationBaker.md#serializebakedvertexdatatojson)
- [serializeBakedVertexDataToObject](VertexAnimationBaker.md#serializebakedvertexdatatoobject)
- [textureFromBakedVertexData](VertexAnimationBaker.md#texturefrombakedvertexdata)

## Constructors

### constructor

• **new VertexAnimationBaker**(`scene`, `mesh`)

Create a new VertexAnimationBaker object which can help baking animations into a texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene the VAT belongs to |
| `mesh` | [`Mesh`](Mesh.md) | Defines the mesh the VAT belongs to |

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:22

## Properties

### \_mesh

• `Private` **\_mesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:15

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:14

## Methods

### \_executeAnimationFrame

▸ `Private` **_executeAnimationFrame**(`vertexData`, `frameIndex`, `textureIndex`): `Promise``void`

Runs an animation frame and stores its vertex data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexData` | `Float32Array` | The array to save data to. |
| `frameIndex` | `number` | Current frame in the skeleton animation to render. |
| `textureIndex` | `number` | Current index of the texture data. |

#### Returns

`Promise``void`

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:70

___

### bakeVertexData

▸ **bakeVertexData**(`ranges`): `Promise``Float32Array`

Bakes the animation into the texture. This should be called once, when the
scene starts, so the VAT is generated and associated to the mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ranges` | [`AnimationRange`](AnimationRange.md)[] | Defines the ranges in the animation that will be baked. |

#### Returns

`Promise``Float32Array`

The array of matrix transforms for each vertex (columns) and frame (rows), as a Float32Array.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:33

___

### loadBakedVertexDataFromJSON

▸ **loadBakedVertexDataFromJSON**(`json`): `Float32Array`

Loads previously baked data in string format.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `json` | `string` | The json string as serialized by serializeBakedVertexDataToJSON(). |

#### Returns

`Float32Array`

The array of matrix transforms for each vertex (columns) and frame (rows), as a Float32Array.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:149

___

### loadBakedVertexDataFromObject

▸ **loadBakedVertexDataFromObject**(`data`): `Float32Array`

Loads previously baked data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Record``string`, `any` | The object as serialized by serializeBakedVertexDataToObject() |

#### Returns

`Float32Array`

The array of matrix transforms for each vertex (columns) and frame (rows), as a Float32Array.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:132

___

### serializeBakedVertexDataToJSON

▸ **serializeBakedVertexDataToJSON**(`vertexData`): `string`

Serializes our vertexData to a JSON string, with a nice string for the vertexData.
Should be called right after bakeVertexData().

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexData` | `Float32Array` | The vertex array data. |

#### Returns

`string`

This object serialized to a safe string.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:141

___

### serializeBakedVertexDataToObject

▸ **serializeBakedVertexDataToObject**(`vertexData`): `Record``string`, `any`

Serializes our vertexData to an object, with a nice string for the vertexData.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexData` | `Float32Array` | The vertex array data. |

#### Returns

`Record``string`, `any`

This object serialized to a JS dict.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:110

___

### textureFromBakedVertexData

▸ **textureFromBakedVertexData**(`vertexData`): [`RawTexture`](RawTexture.md)

Builds a vertex animation texture given the vertexData in an array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexData` | `Float32Array` | The vertex animation data. You can generate it with bakeVertexData(). |

#### Returns

[`RawTexture`](RawTexture.md)

The vertex animation texture to be used with BakedVertexAnimationManager.

#### Defined in

https://github.com/babylon.js/core/src/BakedVertexAnimation/vertexAnimationBaker.ts:86

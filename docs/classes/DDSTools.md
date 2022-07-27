[@dev/core](../README.md) / [Exports](../modules.md) / DDSTools

# Class: DDSTools

Class used to provide DDS decompression tools

## Table of contents

### Constructors

- [constructor](DDSTools.md#constructor)

### Properties

- [StoreLODInAlphaChannel](DDSTools.md#storelodinalphachannel)

### Methods

- [GetDDSInfo](DDSTools.md#getddsinfo)
- [\_ExtractLongWordOrder](DDSTools.md#_extractlongwordorder)
- [\_GetFloatAsHalfFloatRGBAArrayBuffer](DDSTools.md#_getfloatashalffloatrgbaarraybuffer)
- [\_GetFloatAsUIntRGBAArrayBuffer](DDSTools.md#_getfloatasuintrgbaarraybuffer)
- [\_GetFloatRGBAArrayBuffer](DDSTools.md#_getfloatrgbaarraybuffer)
- [\_GetHalfFloatAsFloatRGBAArrayBuffer](DDSTools.md#_gethalffloatasfloatrgbaarraybuffer)
- [\_GetHalfFloatAsUIntRGBAArrayBuffer](DDSTools.md#_gethalffloatasuintrgbaarraybuffer)
- [\_GetHalfFloatRGBAArrayBuffer](DDSTools.md#_gethalffloatrgbaarraybuffer)
- [\_GetLuminanceArrayBuffer](DDSTools.md#_getluminancearraybuffer)
- [\_GetRGBAArrayBuffer](DDSTools.md#_getrgbaarraybuffer)
- [\_GetRGBArrayBuffer](DDSTools.md#_getrgbarraybuffer)

## Constructors

### constructor

• **new DDSTools**()

## Properties

### StoreLODInAlphaChannel

▪ `Static` **StoreLODInAlphaChannel**: `boolean` = `false`

Gets or sets a boolean indicating that LOD info is stored in alpha channel (false by default)

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:156

## Methods

### GetDDSInfo

▸ `Static` **GetDDSInfo**(`data`): [`DDSInfo`](../interfaces/DDSInfo.md)

Gets DDS information from an array buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | defines the array buffer view to read data from |

#### Returns

[`DDSInfo`](../interfaces/DDSInfo.md)

the DDS information

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:163

___

### \_ExtractLongWordOrder

▸ `Static` `Private` **_ExtractLongWordOrder**(`value`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:367

___

### \_GetFloatAsHalfFloatRGBAArrayBuffer

▸ `Static` `Private` **_GetFloatAsHalfFloatRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Uint16Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Uint16Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:273

___

### \_GetFloatAsUIntRGBAArrayBuffer

▸ `Static` `Private` **_GetFloatAsUIntRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Uint8Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Uint8Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:294

___

### \_GetFloatRGBAArrayBuffer

▸ `Static` `Private` **_GetFloatRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:252

___

### \_GetHalfFloatAsFloatRGBAArrayBuffer

▸ `Static` `Private` **_GetHalfFloatAsFloatRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:208

___

### \_GetHalfFloatAsUIntRGBAArrayBuffer

▸ `Static` `Private` **_GetHalfFloatAsUIntRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Uint8Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Uint8Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:316

___

### \_GetHalfFloatRGBAArrayBuffer

▸ `Static` `Private` **_GetHalfFloatRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `lod`): `Uint16Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `lod` | `number` |

#### Returns

`Uint16Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:230

___

### \_GetLuminanceArrayBuffer

▸ `Static` `Private` **_GetLuminanceArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`): `Uint8Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |

#### Returns

`Uint8Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:402

___

### \_GetRGBAArrayBuffer

▸ `Static` `Private` **_GetRGBAArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `rOffset`, `gOffset`, `bOffset`, `aOffset`): `Uint8Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `rOffset` | `number` |
| `gOffset` | `number` |
| `bOffset` | `number` |
| `aOffset` | `number` |

#### Returns

`Uint8Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:338

___

### \_GetRGBArrayBuffer

▸ `Static` `Private` **_GetRGBArrayBuffer**(`width`, `height`, `dataOffset`, `dataLength`, `arrayBuffer`, `rOffset`, `gOffset`, `bOffset`): `Uint8Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `dataOffset` | `number` |
| `dataLength` | `number` |
| `arrayBuffer` | `ArrayBuffer` |
| `rOffset` | `number` |
| `gOffset` | `number` |
| `bOffset` | `number` |

#### Returns

`Uint8Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:375

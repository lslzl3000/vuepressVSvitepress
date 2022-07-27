[@dev/core](../README.md) / [Exports](../modules.md) / MaterialDefines

# Class: MaterialDefines

Manages the defines for the Material

## Indexable

▪ [id: `string`]: `any`

## Table of contents

### Constructors

- [constructor](MaterialDefines.md#constructor)

### Properties

- [\_externalProperties](MaterialDefines.md#_externalproperties)
- [\_isDirty](MaterialDefines.md#_isdirty)

### Accessors

- [isDirty](MaterialDefines.md#isdirty)

### Methods

- [\_setDefaultValue](MaterialDefines.md#_setdefaultvalue)
- [cloneTo](MaterialDefines.md#cloneto)
- [isEqual](MaterialDefines.md#isequal)
- [markAllAsDirty](MaterialDefines.md#markallasdirty)
- [markAsAttributesDirty](MaterialDefines.md#markasattributesdirty)
- [markAsFresnelDirty](MaterialDefines.md#markasfresneldirty)
- [markAsImageProcessingDirty](MaterialDefines.md#markasimageprocessingdirty)
- [markAsLightDirty](MaterialDefines.md#markaslightdirty)
- [markAsMiscDirty](MaterialDefines.md#markasmiscdirty)
- [markAsPrePassDirty](MaterialDefines.md#markasprepassdirty)
- [markAsProcessed](MaterialDefines.md#markasprocessed)
- [markAsTexturesDirty](MaterialDefines.md#markastexturesdirty)
- [markAsUnprocessed](MaterialDefines.md#markasunprocessed)
- [rebuild](MaterialDefines.md#rebuild)
- [reset](MaterialDefines.md#reset)
- [toString](MaterialDefines.md#tostring)

## Constructors

### constructor

• **new MaterialDefines**(`externalProperties?`)

Creates a new instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `externalProperties?` | `Object` | list of external properties to inject into the object |

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:46

## Properties

### \_externalProperties

• `Protected` `Optional` **\_externalProperties**: `Object`

#### Index signature

▪ [name: `string`]: { `default`: `any` ; `type`: `string`  }

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:38

___

### \_isDirty

• `Private` **\_isDirty**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:7

## Accessors

### isDirty

• `get` **isDirty**(): `boolean`

Specifies if the material needs to be re-calculated

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:62

## Methods

### \_setDefaultValue

▸ `Private` **_setDefaultValue**(`prop`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prop` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:226

___

### cloneTo

▸ **cloneTo**(`other`): `void`

Clones this instance's defines to another instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`MaterialDefines`](MaterialDefines.md) | material defines to clone values to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:207

___

### isEqual

▸ **isEqual**(`other`): `boolean`

Specifies if two material defines are equal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`MaterialDefines`](MaterialDefines.md) | A material define instance to compare to |

#### Returns

`boolean`

- Boolean indicating if the material defines are equal (true) or not (false)

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:187

___

### markAllAsDirty

▸ **markAllAsDirty**(): `void`

Marks the material to indicate all of its defines need to be re-calculated

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:91

___

### markAsAttributesDirty

▸ **markAsAttributesDirty**(): `void`

Marks the attribute state as changed

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:122

___

### markAsFresnelDirty

▸ **markAsFresnelDirty**(): `void`

Marks the fresnel state as changed

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:138

___

### markAsImageProcessingDirty

▸ **markAsImageProcessingDirty**(): `void`

Marks the material to indicate that image processing needs to be re-calculated

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:104

___

### markAsLightDirty

▸ **markAsLightDirty**(`disposed?`): `void`

Marks the material to indicate the lights need to be re-calculated

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposed` | `boolean` | `false` | Defines whether the light is dirty due to dispose or not |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:113

___

### markAsMiscDirty

▸ **markAsMiscDirty**(): `void`

Marks the misc state as changed

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:146

___

### markAsPrePassDirty

▸ **markAsPrePassDirty**(): `void`

Marks the prepass state as changed

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:154

___

### markAsProcessed

▸ **markAsProcessed**(): `void`

Marks the material to indicate that it has been re-calculated

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:69

___

### markAsTexturesDirty

▸ **markAsTexturesDirty**(): `void`

Marks the texture state as changed

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:130

___

### markAsUnprocessed

▸ **markAsUnprocessed**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:84

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the material defines

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:162

___

### reset

▸ **reset**(): `void`

Resets the material define values

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:222

___

### toString

▸ **toString**(): `string`

Converts the material define values to a string

#### Returns

`string`

- String of material define information

#### Defined in

packages/dev/core/src/Materials/materialDefines.ts:247

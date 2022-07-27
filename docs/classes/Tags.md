[@dev/core](../README.md) / [Exports](../modules.md) / Tags

# Class: Tags

Class used to store custom tags

## Table of contents

### Constructors

- [constructor](Tags.md#constructor)

### Methods

- [AddTagsTo](Tags.md#addtagsto)
- [DisableFor](Tags.md#disablefor)
- [EnableFor](Tags.md#enablefor)
- [GetTags](Tags.md#gettags)
- [HasTags](Tags.md#hastags)
- [MatchesQuery](Tags.md#matchesquery)
- [RemoveTagsFrom](Tags.md#removetagsfrom)

## Constructors

### constructor

• **new Tags**()

## Methods

### AddTagsTo

▸ `Static` **AddTagsTo**(`obj`, `tagsString`): `void`

Adds tags to an object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |
| `tagsString` | `string` | defines the tag string. The tags 'true' and 'false' are reserved and cannot be used as tags.  A tag cannot start with '\|\|', '&&', and '!'. It cannot contain whitespaces |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:91

___

### DisableFor

▸ `Static` **DisableFor**(`obj`): `void`

Removes tags support

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:35

___

### EnableFor

▸ `Static` **EnableFor**(`obj`): `void`

Adds support for tags on the given object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:11

___

### GetTags

▸ `Static` **GetTags**(`obj`, `asString?`): `any`

Gets the tags available on a given object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `obj` | `any` | `undefined` | defines the object to use |
| `asString` | `boolean` | `true` | defines if the tags must be returned as a string instead of an array of strings |

#### Returns

`any`

the tags

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:68

___

### HasTags

▸ `Static` **HasTags**(`obj`): `boolean`

Gets a boolean indicating if the given object has tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |

#### Returns

`boolean`

a boolean

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:48

___

### MatchesQuery

▸ `Static` **MatchesQuery**(`obj`, `tagsQuery`): `boolean`

Defines if tags hosted on an object match a given query

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |
| `tagsQuery` | `string` | defines the tag query |

#### Returns

`boolean`

a boolean

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:156

___

### RemoveTagsFrom

▸ `Static` **RemoveTagsFrom**(`obj`, `tagsString`): `void`

Removes specific tags from a specific object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `any` | defines the object to use |
| `tagsString` | `string` | defines the tags to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/tags.ts:131

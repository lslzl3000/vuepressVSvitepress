[@dev/core](../README.md) / [Exports](../modules.md) / MorphTarget

# Class: MorphTarget

Defines a target to use with MorphTargetManager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](MorphTarget.md#constructor)

### Properties

- [\_animationPropertiesOverride](MorphTarget.md#_animationpropertiesoverride)
- [\_influence](MorphTarget.md#_influence)
- [\_normals](MorphTarget.md#_normals)
- [\_positions](MorphTarget.md#_positions)
- [\_scene](MorphTarget.md#_scene)
- [\_tangents](MorphTarget.md#_tangents)
- [\_uniqueId](MorphTarget.md#_uniqueid)
- [\_uvs](MorphTarget.md#_uvs)
- [animations](MorphTarget.md#animations)
- [id](MorphTarget.md#id)
- [name](MorphTarget.md#name)
- [onInfluenceChanged](MorphTarget.md#oninfluencechanged)

### Accessors

- [animationPropertiesOverride](MorphTarget.md#animationpropertiesoverride)
- [hasNormals](MorphTarget.md#hasnormals)
- [hasPositions](MorphTarget.md#haspositions)
- [hasTangents](MorphTarget.md#hastangents)
- [hasUVs](MorphTarget.md#hasuvs)
- [influence](MorphTarget.md#influence)
- [uniqueId](MorphTarget.md#uniqueid)

### Methods

- [clone](MorphTarget.md#clone)
- [getClassName](MorphTarget.md#getclassname)
- [getNormals](MorphTarget.md#getnormals)
- [getPositions](MorphTarget.md#getpositions)
- [getTangents](MorphTarget.md#gettangents)
- [getUVs](MorphTarget.md#getuvs)
- [serialize](MorphTarget.md#serialize)
- [setNormals](MorphTarget.md#setnormals)
- [setPositions](MorphTarget.md#setpositions)
- [setTangents](MorphTarget.md#settangents)
- [setUVs](MorphTarget.md#setuvs)
- [FromMesh](MorphTarget.md#frommesh)
- [Parse](MorphTarget.md#parse)

## Constructors

### constructor

• **new MorphTarget**(`name`, `influence?`, `scene?`)

Creates a new MorphTarget

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the target |
| `influence` | `number` | `0` | defines the influence to use |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `null` | defines the scene the morphtarget belongs to |

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:88

## Properties

### \_animationPropertiesOverride

• `Private` **\_animationPropertiesOverride**: [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) = `null`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:66

___

### \_influence

• `Private` **\_influence**: `number`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:29

___

### \_normals

• `Private` **\_normals**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:26

___

### \_positions

• `Private` **\_positions**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:25

___

### \_scene

• `Private` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:24

___

### \_tangents

• `Private` **\_tangents**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:27

___

### \_uniqueId

• `Private` **\_uniqueId**: `number` = `0`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:30

___

### \_uvs

• `Private` **\_uvs**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:28

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets or sets the list of animations

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:22

___

### id

• **id**: `string`

Gets or sets the id of the morph Target

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:64

___

### name

• **name**: `string`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:90

___

### onInfluenceChanged

• **onInfluenceChanged**: [`Observable`](Observable.md)`boolean`

Observable raised when the influence changes

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:35

## Accessors

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:71

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:78

___

### hasNormals

• `get` **hasNormals**(): `boolean`

Gets a boolean defining if the target contains normal data

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:119

___

### hasPositions

• `get` **hasPositions**(): `boolean`

Gets a boolean defining if the target contains position data

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:112

___

### hasTangents

• `get` **hasTangents**(): `boolean`

Gets a boolean defining if the target contains tangent data

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:126

___

### hasUVs

• `get` **hasUVs**(): `boolean`

Gets a boolean defining if the target contains texture coordinates data

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:133

___

### influence

• `get` **influence**(): `number`

Gets or sets the influence of this target (ie. its weight in the overall morphing)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:43

• `set` **influence**(`influence`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `influence` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:47

___

### uniqueId

• `get` **uniqueId**(): `number`

Gets the unique ID of this manager

#### Returns

`number`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:105

## Methods

### clone

▸ **clone**(): [`MorphTarget`](MorphTarget.md)

Clone the current target

#### Returns

[`MorphTarget`](MorphTarget.md)

a new MorphTarget

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:229

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "MorphTarget"

#### Returns

`string`

"MorphTarget"

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:274

___

### getNormals

▸ **getNormals**(): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets the normal data stored in this target

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a FloatArray containing the normal data (or null if not present)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:177

___

### getPositions

▸ **getPositions**(): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets the position data stored in this target

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a FloatArray containing the position data (or null if not present)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:155

___

### getTangents

▸ **getTangents**(): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets the tangent data stored in this target

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a FloatArray containing the tangent data (or null if not present)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:199

___

### getUVs

▸ **getUVs**(): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets the texture coordinates data stored in this target

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a FloatArray containing the texture coordinates data (or null if not present)

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:221

___

### serialize

▸ **serialize**(): `any`

Serializes the current target into a Serialization object

#### Returns

`any`

the serialized object

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:244

___

### setNormals

▸ **setNormals**(`data`): `void`

Affects normal data to this target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | defines the normal data to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:163

___

### setPositions

▸ **setPositions**(`data`): `void`

Affects position data to this target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | defines the position data to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:141

___

### setTangents

▸ **setTangents**(`data`): `void`

Affects tangent data to this target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | defines the tangent data to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:185

___

### setUVs

▸ **setUVs**(`data`): `void`

Affects texture coordinates data to this target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | defines the texture coordinates data to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:207

___

### FromMesh

▸ `Static` **FromMesh**(`mesh`, `name?`, `influence?`): [`MorphTarget`](MorphTarget.md)

Creates a MorphTarget from mesh data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the source mesh |
| `name?` | `string` | defines the name to use for the new target |
| `influence?` | `number` | defines the influence to attach to the target |

#### Returns

[`MorphTarget`](MorphTarget.md)

a new MorphTarget

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:335

___

### Parse

▸ `Static` **Parse**(`serializationObject`, `scene?`): [`MorphTarget`](MorphTarget.md)

Creates a new target from serialized data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the serialized data to use |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`MorphTarget`](MorphTarget.md)

a new MorphTarget

#### Defined in

packages/dev/core/src/Morph/morphTarget.ts:286

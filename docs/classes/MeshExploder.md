[@dev/core](../README.md) / [Exports](../modules.md) / MeshExploder

# Class: MeshExploder

Class used to explode meshes (ie. to have a center and move them away from that center to better see the overall organization)

## Table of contents

### Constructors

- [constructor](MeshExploder.md#constructor)

### Properties

- [\_centerMesh](MeshExploder.md#_centermesh)
- [\_centerPosition](MeshExploder.md#_centerposition)
- [\_meshes](MeshExploder.md#_meshes)
- [\_meshesOrigins](MeshExploder.md#_meshesorigins)
- [\_newPosition](MeshExploder.md#_newposition)
- [\_scaledDirection](MeshExploder.md#_scaleddirection)
- [\_toCenterVectors](MeshExploder.md#_tocentervectors)

### Methods

- [\_setCenterMesh](MeshExploder.md#_setcentermesh)
- [explode](MeshExploder.md#explode)
- [getClassName](MeshExploder.md#getclassname)
- [getMeshes](MeshExploder.md#getmeshes)

## Constructors

### constructor

• **new MeshExploder**(`meshes`, `centerMesh?`)

Explodes meshes from a center mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`Mesh`](Mesh.md)[] | The meshes to explode. |
| `centerMesh?` | [`Mesh`](Mesh.md) | The mesh to be center of explosion. |

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:21

## Properties

### \_centerMesh

• `Private` **\_centerMesh**: [`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:8

___

### \_centerPosition

• `Private` **\_centerPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:14

___

### \_meshes

• `Private` **\_meshes**: [`Mesh`](Mesh.md)[]

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:9

___

### \_meshesOrigins

• `Private` **\_meshesOrigins**: [`Vector3`](Vector3.md)[] = `[]`

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:10

___

### \_newPosition

• `Private` **\_newPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:13

___

### \_scaledDirection

• `Private` **\_scaledDirection**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:12

___

### \_toCenterVectors

• `Private` **\_toCenterVectors**: [`Vector3`](Vector3.md)[] = `[]`

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:11

## Methods

### \_setCenterMesh

▸ `Private` **_setCenterMesh**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:46

___

### explode

▸ **explode**(`direction?`): `void`

Explodes meshes giving a specific direction

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `direction` | `number` | `1.0` | Number to multiply distance of each mesh's origin from center. Use a negative number to implode, or zero to reset. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:97

___

### getClassName

▸ **getClassName**(): `string`

Get class name

#### Returns

`string`

"MeshExploder"

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:79

___

### getMeshes

▸ **getMeshes**(): [`Mesh`](Mesh.md)[]

"Exploded meshes"

#### Returns

[`Mesh`](Mesh.md)[]

Array of meshes with the centerMesh at index 0.

#### Defined in

packages/dev/core/src/Misc/meshExploder.ts:87

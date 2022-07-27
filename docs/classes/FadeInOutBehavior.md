[@dev/core](../README.md) / [Exports](../modules.md) / FadeInOutBehavior

# Class: FadeInOutBehavior

A behavior that when attached to a mesh will allow the mesh to fade in and out

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`Mesh`](Mesh.md)

## Table of contents

### Constructors

- [constructor](FadeInOutBehavior.md#constructor)

### Properties

- [\_hoverValue](FadeInOutBehavior.md#_hovervalue)
- [\_hovered](FadeInOutBehavior.md#_hovered)
- [\_millisecondsPerFrame](FadeInOutBehavior.md#_millisecondsperframe)
- [\_ownerNode](FadeInOutBehavior.md#_ownernode)
- [delay](FadeInOutBehavior.md#delay)
- [fadeInTime](FadeInOutBehavior.md#fadeintime)

### Accessors

- [name](FadeInOutBehavior.md#name)

### Methods

- [\_setAllVisibility](FadeInOutBehavior.md#_setallvisibility)
- [\_update](FadeInOutBehavior.md#_update)
- [attach](FadeInOutBehavior.md#attach)
- [detach](FadeInOutBehavior.md#detach)
- [fadeIn](FadeInOutBehavior.md#fadein)
- [init](FadeInOutBehavior.md#init)

## Constructors

### constructor

• **new FadeInOutBehavior**()

Instantiates the FadeInOutBehavior

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:27

## Properties

### \_hoverValue

• `Private` **\_hoverValue**: `number` = `0`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:21

___

### \_hovered

• `Private` **\_hovered**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:20

___

### \_millisecondsPerFrame

• `Private` **\_millisecondsPerFrame**: `number`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:19

___

### \_ownerNode

• `Private` **\_ownerNode**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) = `null`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:22

___

### delay

• **delay**: `number` = `0`

Time in milliseconds to delay before fading in (Default: 0)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:13

___

### fadeInTime

• **fadeInTime**: `number` = `300`

Time in milliseconds for the mesh to fade in (Default: 300)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:17

## Accessors

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:32

## Methods

### \_setAllVisibility

▸ `Private` **_setAllVisibility**(`mesh`, `value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:86

___

### \_update

▸ `Private` **_update**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:65

___

### attach

▸ **attach**(`ownerNode`): `void`

Attaches the fade behavior on the passed in mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`Mesh`](Mesh.md) | The mesh that will be faded in/out once attached |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:45

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:52

___

### fadeIn

▸ **fadeIn**(`value`): `void`

Triggers the mesh to begin fading in or out

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | if the object should fade in or out (true to fade in) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:60

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/fadeInOutBehavior.ts:39

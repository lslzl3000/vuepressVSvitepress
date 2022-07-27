[@dev/core](../README.md) / [Exports](../modules.md) / Reflector

# Class: Reflector

Class used to connect with the reflector zone of the sandbox via the reflector bridge

**`Since`**

5.0.0

## Table of contents

### Constructors

- [constructor](Reflector.md#constructor)

### Properties

- [\_scene](Reflector.md#_scene)
- [\_webSocket](Reflector.md#_websocket)
- [\_SERVER\_PREFIX](Reflector.md#_server_prefix)

### Methods

- [\_handleClientMessage](Reflector.md#_handleclientmessage)
- [\_handleServerMessage](Reflector.md#_handleservermessage)
- [close](Reflector.md#close)

## Constructors

### constructor

• **new Reflector**(`scene`, `hostname`, `port`)

Constructs a reflector object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene to use |
| `hostname` | `string` | The hostname of the reflector bridge |
| `port` | `number` | The port of the reflector bridge |

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:21

## Properties

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:12

___

### \_webSocket

• `Private` **\_webSocket**: `WebSocket`

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:13

___

### \_SERVER\_PREFIX

▪ `Static` `Private` `Readonly` **\_SERVER\_PREFIX**: ``"$$"``

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:10

## Methods

### \_handleClientMessage

▸ `Private` **_handleClientMessage**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:63

___

### \_handleServerMessage

▸ `Private` **_handleServerMessage**(`message`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:52

___

### close

▸ **close**(): `void`

Closes the reflector connection

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/reflector.ts:48

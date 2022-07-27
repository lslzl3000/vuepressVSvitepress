[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsViewer

# Class: PhysicsViewer

Used to show the physics impostor around the specific mesh

## Table of contents

### Constructors

- [constructor](PhysicsViewer.md#constructor)

### Properties

- [\_debugBoxMesh](PhysicsViewer.md#_debugboxmesh)
- [\_debugCapsuleMesh](PhysicsViewer.md#_debugcapsulemesh)
- [\_debugCylinderMesh](PhysicsViewer.md#_debugcylindermesh)
- [\_debugMaterial](PhysicsViewer.md#_debugmaterial)
- [\_debugMeshMeshes](PhysicsViewer.md#_debugmeshmeshes)
- [\_debugSphereMesh](PhysicsViewer.md#_debugspheremesh)
- [\_renderFunction](PhysicsViewer.md#_renderfunction)
- [\_utilityLayer](PhysicsViewer.md#_utilitylayer)

### Methods

- [\_getDebugBoxMesh](PhysicsViewer.md#_getdebugboxmesh)
- [\_getDebugCapsuleMesh](PhysicsViewer.md#_getdebugcapsulemesh)
- [\_getDebugCylinderMesh](PhysicsViewer.md#_getdebugcylindermesh)
- [\_getDebugMaterial](PhysicsViewer.md#_getdebugmaterial)
- [\_getDebugMesh](PhysicsViewer.md#_getdebugmesh)
- [\_getDebugMeshMesh](PhysicsViewer.md#_getdebugmeshmesh)
- [\_getDebugSphereMesh](PhysicsViewer.md#_getdebugspheremesh)
- [dispose](PhysicsViewer.md#dispose)
- [hideImpostor](PhysicsViewer.md#hideimpostor)
- [showImpostor](PhysicsViewer.md#showimpostor)

## Constructors

### constructor

• **new PhysicsViewer**(`scene?`)

Creates a new PhysicsViewer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:48

## Properties

### \_debugBoxMesh

• `Private` **\_debugBoxMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:37

___

### \_debugCapsuleMesh

• `Private` **\_debugCapsuleMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:39

___

### \_debugCylinderMesh

• `Private` **\_debugCylinderMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:40

___

### \_debugMaterial

• `Private` **\_debugMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:41

___

### \_debugMeshMeshes

• `Private` **\_debugMeshMeshes**: [`Mesh`](Mesh.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:42

___

### \_debugSphereMesh

• `Private` **\_debugSphereMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:38

___

### \_renderFunction

• `Private` **\_renderFunction**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:34

___

### \_utilityLayer

• `Private` **\_utilityLayer**: [`Nullable`](../modules.md#nullable)[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:35

## Methods

### \_getDebugBoxMesh

▸ `Private` **_getDebugBoxMesh**(`scene`): [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:183

___

### \_getDebugCapsuleMesh

▸ `Private` **_getDebugCapsuleMesh**(`scene`): [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:205

___

### \_getDebugCylinderMesh

▸ `Private` **_getDebugCylinderMesh**(`scene`): [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:216

___

### \_getDebugMaterial

▸ `Private` **_getDebugMaterial**(`scene`): [`Material`](Material.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:172

___

### \_getDebugMesh

▸ `Private` **_getDebugMesh**(`impostor`, `targetMesh?`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) |
| `targetMesh?` | [`Mesh`](Mesh.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:238

___

### \_getDebugMeshMesh

▸ `Private` **_getDebugMeshMesh**(`mesh`, `scene`): [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:227

___

### \_getDebugSphereMesh

▸ `Private` **_getDebugSphereMesh**(`scene`): [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:194

___

### dispose

▸ **dispose**(): `void`

Releases all resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:334

___

### hideImpostor

▸ **hideImpostor**(`impostor`): `void`

Hides a specified physic impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md) | defines the impostor to hide |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:128

___

### showImpostor

▸ **showImpostor**(`impostor`, `targetMesh?`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Renders a specified physic impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `impostor` | [`PhysicsImpostor`](PhysicsImpostor.md) | defines the impostor to render |
| `targetMesh?` | [`Mesh`](Mesh.md) | defines the mesh represented by the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the new debug mesh used to render the impostor

#### Defined in

https://github.com/babylon.js/core/src/Debug/physicsViewer.ts:96

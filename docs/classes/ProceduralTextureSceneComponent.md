[@dev/core](../README.md) / [Exports](../modules.md) / ProceduralTextureSceneComponent

# Class: ProceduralTextureSceneComponent

Defines the Procedural Texture scene component responsible to manage any Procedural Texture
in a given scene.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](ProceduralTextureSceneComponent.md#constructor)

### Properties

- [name](ProceduralTextureSceneComponent.md#name)
- [scene](ProceduralTextureSceneComponent.md#scene)

### Methods

- [\_beforeClear](ProceduralTextureSceneComponent.md#_beforeclear)
- [dispose](ProceduralTextureSceneComponent.md#dispose)
- [rebuild](ProceduralTextureSceneComponent.md#rebuild)
- [register](ProceduralTextureSceneComponent.md#register)

## Constructors

### constructor

• **new ProceduralTextureSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:36

## Properties

### name

• `Readonly` **name**: ``"ProceduralTexture"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:25

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:30

## Methods

### \_beforeClear

▸ `Private` **_beforeClear**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:63

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:59

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:52

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:44

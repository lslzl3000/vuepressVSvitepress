[@dev/core](../README.md) / [Exports](../modules.md) / EngineStore

# Class: EngineStore

The engine store class is responsible to hold all the instances of Engine and Scene created
during the life time of the application.

## Table of contents

### Constructors

- [constructor](EngineStore.md#constructor)

### Properties

- [FallbackTexture](EngineStore.md#fallbacktexture)
- [Instances](EngineStore.md#instances)
- [UseFallbackTexture](EngineStore.md#usefallbacktexture)

### Accessors

- [LastCreatedEngine](EngineStore.md#lastcreatedengine)
- [LastCreatedScene](EngineStore.md#lastcreatedscene)

## Constructors

### constructor

• **new EngineStore**()

## Properties

### FallbackTexture

▪ `Static` **FallbackTexture**: `string` = `""`

Texture content used if a texture cannot loaded

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Engines/engineStore.ts:45

___

### Instances

▪ `Static` **Instances**: [`Engine`](Engine.md)[]

Gets the list of created engines

#### Defined in

packages/dev/core/src/Engines/engineStore.ts:12

___

### UseFallbackTexture

▪ `Static` **UseFallbackTexture**: `boolean` = `true`

Gets or sets a global variable indicating if fallback texture must be used when a texture cannot be loaded

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Engines/engineStore.ts:39

## Accessors

### LastCreatedEngine

• `Static` `get` **LastCreatedEngine**(): [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

Gets the latest created engine

#### Returns

[`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Engines/engineStore.ts:20

___

### LastCreatedScene

• `Static` `get` **LastCreatedScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Gets the latest created scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Engines/engineStore.ts:31

[@dev/core](../README.md) / [Exports](../modules.md) / EffectWrapper

# Class: EffectWrapper

Wraps an effect to be used for rendering

## Table of contents

### Constructors

- [constructor](EffectWrapper.md#constructor)

### Properties

- [\_onContextRestoredObserver](EffectWrapper.md#_oncontextrestoredobserver)
- [onApplyObservable](EffectWrapper.md#onapplyobservable)

### Accessors

- [effect](EffectWrapper.md#effect)

### Methods

- [dispose](EffectWrapper.md#dispose)

## Constructors

### constructor

• **new EffectWrapper**(`creationOptions`)

Creates an effect to be renderer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `creationOptions` | `EffectWrapperCreationOptions` | options to create the effect |

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:253

## Properties

### \_onContextRestoredObserver

• `Private` **\_onContextRestoredObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:247

___

### onApplyObservable

• **onApplyObservable**: [`Observable`](Observable.md){}

Event that is fired right before the effect is drawn (should be used to update uniforms)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:232

## Accessors

### effect

• `get` **effect**(): [`Effect`](Effect.md)

The underlying effect

#### Returns

[`Effect`](Effect.md)

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:236

• `set` **effect**(`effect`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `effect` | [`Effect`](Effect.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:240

## Methods

### dispose

▸ **dispose**(): `void`

Disposes of the effect wrapper

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effectRenderer.ts:330

[@dev/core](../README.md) / [Exports](../modules.md) / ParticleHelper

# Class: ParticleHelper

This class is made for on one-liner static method to help creating particle system set.

## Table of contents

### Constructors

- [constructor](ParticleHelper.md#constructor)

### Properties

- [BaseAssetsUrl](ParticleHelper.md#baseassetsurl)
- [CreateFromSnippetAsync](ParticleHelper.md#createfromsnippetasync)
- [SnippetUrl](ParticleHelper.md#snippeturl)

### Methods

- [CreateAsync](ParticleHelper.md#createasync)
- [CreateDefault](ParticleHelper.md#createdefault)
- [ExportSet](ParticleHelper.md#exportset)
- [ParseFromFileAsync](ParticleHelper.md#parsefromfileasync)
- [ParseFromSnippetAsync](ParticleHelper.md#parsefromsnippetasync)

## Constructors

### constructor

• **new ParticleHelper**()

## Properties

### BaseAssetsUrl

▪ `Static` **BaseAssetsUrl**: `string` = `ParticleSystemSet.BaseAssetsUrl`

Gets or sets base Assets URL

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:22

___

### CreateFromSnippetAsync

▪ `Static` **CreateFromSnippetAsync**: (`snippetId`: `string`, `scene`: [`Scene`](Scene.md), `gpu`: `boolean`, `rootUrl`: `string`, `capacity?`: `number`) => `Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md) = `ParticleHelper.ParseFromSnippetAsync`

#### Type declaration

▸ (`snippetId`, `scene`, `gpu?`, `rootUrl?`, `capacity?`): `Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

Creates a particle system from a snippet saved by the particle system editor

##### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load (can be set to _BLANK to create a default one) |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `gpu` | `boolean` | `false` | If the system will use gpu |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

##### Returns

`Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

a promise that will resolve to the new particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:221

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:25

## Methods

### CreateAsync

▸ `Static` **CreateAsync**(`type`, `scene`, `gpu?`, `capacity?`): `Promise`[`ParticleSystemSet`](ParticleSystemSet.md)

This is the main static method (one-liner) of this helper to create different particle systems

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `type` | `string` | `undefined` | This string represents the type to the particle system to create |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `undefined` | The scene where the particle system should live |
| `gpu` | `boolean` | `false` | If the system will use gpu |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

`Promise`[`ParticleSystemSet`](ParticleSystemSet.md)

the ParticleSystemSet created

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:77

___

### CreateDefault

▸ `Static` **CreateDefault**(`emitter`, `capacity?`, `scene?`, `useGPU?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Create a default particle system that you can tweak

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `emitter` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md) | `undefined` | defines the emitter to use |
| `capacity` | `number` | `500` | defines the system capacity (default is 500 particles) |
| `scene?` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `useGPU` | `boolean` | `false` | defines if a GPUParticleSystem must be created (default is false) |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the new Particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:35

___

### ExportSet

▸ `Static` **ExportSet**(`systems`): [`ParticleSystemSet`](ParticleSystemSet.md)

Static function used to export a particle system to a ParticleSystemSet variable.
Please note that the emitter shape is not exported

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `systems` | [`IParticleSystem`](../interfaces/IParticleSystem.md)[] | defines the particle systems to export |

#### Returns

[`ParticleSystemSet`](ParticleSystemSet.md)

the created particle system set

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:116

___

### ParseFromFileAsync

▸ `Static` **ParseFromFileAsync**(`name`, `url`, `scene`, `gpu?`, `rootUrl?`, `capacity?`): `Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

Creates a particle system from a snippet saved in a remote file

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines the name of the particle system to create (can be null or empty to use the one from the json data) |
| `url` | `string` | `undefined` | defines the url to load from |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `gpu` | `boolean` | `false` | If the system will use gpu |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

`Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

a promise that will resolve to the new particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:136

___

### ParseFromSnippetAsync

▸ `Static` **ParseFromSnippetAsync**(`snippetId`, `scene`, `gpu?`, `rootUrl?`, `capacity?`): `Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

Creates a particle system from a snippet saved by the particle system editor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load (can be set to _BLANK to create a default one) |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `gpu` | `boolean` | `false` | If the system will use gpu |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

`Promise`[`IParticleSystem`](../interfaces/IParticleSystem.md)

a promise that will resolve to the new particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleHelper.ts:176

[@dev/core](../README.md) / [Exports](../modules.md) / ReflectionProbe

# Class: ReflectionProbe

Class used to generate realtime reflection / refraction cube textures

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_reflection_probes

## Table of contents

### Constructors

- [constructor](ReflectionProbe.md#constructor)

### Properties

- [\_add](ReflectionProbe.md#_add)
- [\_attachedMesh](ReflectionProbe.md#_attachedmesh)
- [\_currentSceneUBO](ReflectionProbe.md#_currentsceneubo)
- [\_invertYAxis](ReflectionProbe.md#_invertyaxis)
- [\_projectionMatrix](ReflectionProbe.md#_projectionmatrix)
- [\_renderTargetTexture](ReflectionProbe.md#_rendertargettexture)
- [\_scene](ReflectionProbe.md#_scene)
- [\_sceneUBOs](ReflectionProbe.md#_sceneubos)
- [\_target](ReflectionProbe.md#_target)
- [\_viewMatrix](ReflectionProbe.md#_viewmatrix)
- [name](ReflectionProbe.md#name)
- [position](ReflectionProbe.md#position)

### Accessors

- [cubeTexture](ReflectionProbe.md#cubetexture)
- [refreshRate](ReflectionProbe.md#refreshrate)
- [renderList](ReflectionProbe.md#renderlist)
- [samples](ReflectionProbe.md#samples)

### Methods

- [attachToMesh](ReflectionProbe.md#attachtomesh)
- [dispose](ReflectionProbe.md#dispose)
- [getClassName](ReflectionProbe.md#getclassname)
- [getScene](ReflectionProbe.md#getscene)
- [serialize](ReflectionProbe.md#serialize)
- [setRenderingAutoClearDepthStencil](ReflectionProbe.md#setrenderingautocleardepthstencil)
- [toString](ReflectionProbe.md#tostring)
- [Parse](ReflectionProbe.md#parse)

## Constructors

### constructor

• **new ReflectionProbe**(`name`, `size`, `scene`, `generateMipMaps?`, `useFloat?`, `linearSpace?`)

Creates a new reflection probe

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the probe |
| `size` | `number` | `undefined` | defines the texture resolution (for each face) |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `generateMipMaps` | `boolean` | `true` | defines if mip maps should be generated automatically (true by default) |
| `useFloat` | `boolean` | `false` | defines if HDR data (float data) should be used to store colors (false by default) |
| `linearSpace` | `boolean` | `false` | defines if the probe should be generated in linear space or not (false by default) |

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:89

## Properties

### \_add

• `Private` **\_add**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:65

___

### \_attachedMesh

• `Private` **\_attachedMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:67

___

### \_currentSceneUBO

• `Private` **\_currentSceneUBO**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:71

___

### \_invertYAxis

• `Private` **\_invertYAxis**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:69

___

### \_projectionMatrix

• `Private` **\_projectionMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:62

___

### \_renderTargetTexture

• `Private` **\_renderTargetTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:61

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:60

___

### \_sceneUBOs

• `Private` **\_sceneUBOs**: [`UniformBuffer`](UniformBuffer.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:70

___

### \_target

• `Private` **\_target**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:64

___

### \_viewMatrix

• `Private` **\_viewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:63

___

### name

• **name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:91

___

### position

• **position**: [`Vector3`](Vector3.md)

Gets or sets probe position (center of the cube map)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:75

## Accessors

### cubeTexture

• `get` **cubeTexture**(): [`RenderTargetTexture`](RenderTargetTexture.md)

Gets the internal CubeTexture used to render to

#### Returns

[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:229

___

### refreshRate

• `get` **refreshRate**(): `number`

Gets or sets the refresh rate to use (on every frame by default)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:212

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:216

___

### renderList

• `get` **renderList**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Gets the list of meshes to render

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:234

___

### samples

• `get` **samples**(): `number`

Gets or sets the number of samples to use for multi-sampling (0 by default). Required WebGL2

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:203

• `set` **samples**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:207

## Methods

### attachToMesh

▸ **attachToMesh**(`mesh`): `void`

Attach the probe to a specific mesh (Rendering will be done from attached mesh's position)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | defines the mesh to attach to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:242

___

### dispose

▸ **dispose**(): `void`

Clean all associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:258

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the refection probe.

#### Returns

`string`

"ReflectionProbe"

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:310

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the hosting scene

#### Returns

[`Scene`](Scene.md)

a Scene

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:224

___

### serialize

▸ **serialize**(): `any`

Serialize the reflection probe to a JSON representation we can easily use in the respective Parse function.

#### Returns

`any`

The JSON representation of the texture

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:318

___

### setRenderingAutoClearDepthStencil

▸ **setRenderingAutoClearDepthStencil**(`renderingGroupId`, `autoClearDepthStencil`): `void`

Specifies whether or not the stencil and depth buffer are cleared between two rendering groups

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderingGroupId` | `number` | The rendering group id corresponding to its index |
| `autoClearDepthStencil` | `boolean` | Automatically clears depth and stencil between groups if true. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:251

___

### toString

▸ **toString**(`fullDetails?`): `string`

Converts the reflection probe information to a readable string for debug purpose.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | Supports for multiple levels of logging within scene loading |

#### Returns

`string`

the human readable reflection probe info

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:292

___

### Parse

▸ `Static` **Parse**(`parsedReflectionProbe`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`ReflectionProbe`](ReflectionProbe.md)

Parse the JSON representation of a reflection probe in order to recreate the reflection probe in the given scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedReflectionProbe` | `any` | Define the JSON representation of the reflection probe |
| `scene` | [`Scene`](Scene.md) | Define the scene the parsed reflection probe should be instantiated in |
| `rootUrl` | `string` | Define the root url of the parsing sequence in the case of relative dependencies |

#### Returns

[`Nullable`](../modules.md#nullable)[`ReflectionProbe`](ReflectionProbe.md)

The parsed reflection probe if successful

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:332

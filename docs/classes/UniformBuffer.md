[@dev/core](../README.md) / [Exports](../modules.md) / UniformBuffer

# Class: UniformBuffer

Uniform buffer objects.

Handles blocks of uniform on the GPU.

If WebGL 2 is not available, this class falls back on traditional setUniformXXX calls.

For more information, please refer to :
https://www.khronos.org/opengl/wiki/Uniform_Buffer_Object

## Table of contents

### Constructors

- [constructor](UniformBuffer.md#constructor)

### Properties

- [\_buffer](UniformBuffer.md#_buffer)
- [\_bufferData](UniformBuffer.md#_bufferdata)
- [\_bufferIndex](UniformBuffer.md#_bufferindex)
- [\_buffers](UniformBuffer.md#_buffers)
- [\_createBufferOnWrite](UniformBuffer.md#_createbufferonwrite)
- [\_currentEffect](UniformBuffer.md#_currenteffect)
- [\_currentEffectName](UniformBuffer.md#_currenteffectname)
- [\_currentFrameId](UniformBuffer.md#_currentframeid)
- [\_data](UniformBuffer.md#_data)
- [\_dynamic](UniformBuffer.md#_dynamic)
- [\_engine](UniformBuffer.md#_engine)
- [\_name](UniformBuffer.md#_name)
- [\_needSync](UniformBuffer.md#_needsync)
- [\_noUBO](UniformBuffer.md#_noubo)
- [\_uniformArraySizes](UniformBuffer.md#_uniformarraysizes)
- [\_uniformLocationPointer](UniformBuffer.md#_uniformlocationpointer)
- [\_uniformLocations](UniformBuffer.md#_uniformlocations)
- [\_uniformSizes](UniformBuffer.md#_uniformsizes)
- [\_valueCache](UniformBuffer.md#_valuecache)
- [updateArray](UniformBuffer.md#updatearray)
- [updateColor3](UniformBuffer.md#updatecolor3)
- [updateColor4](UniformBuffer.md#updatecolor4)
- [updateDirectColor4](UniformBuffer.md#updatedirectcolor4)
- [updateFloat](UniformBuffer.md#updatefloat)
- [updateFloat2](UniformBuffer.md#updatefloat2)
- [updateFloat3](UniformBuffer.md#updatefloat3)
- [updateFloat4](UniformBuffer.md#updatefloat4)
- [updateFloatArray](UniformBuffer.md#updatefloatarray)
- [updateInt](UniformBuffer.md#updateint)
- [updateInt2](UniformBuffer.md#updateint2)
- [updateInt3](UniformBuffer.md#updateint3)
- [updateInt4](UniformBuffer.md#updateint4)
- [updateIntArray](UniformBuffer.md#updateintarray)
- [updateMatrices](UniformBuffer.md#updatematrices)
- [updateMatrix](UniformBuffer.md#updatematrix)
- [updateMatrix2x2](UniformBuffer.md#updatematrix2x2)
- [updateMatrix3x3](UniformBuffer.md#updatematrix3x3)
- [updateVector3](UniformBuffer.md#updatevector3)
- [updateVector4](UniformBuffer.md#updatevector4)
- [\_MAX\_UNIFORM\_SIZE](UniformBuffer.md#_max_uniform_size)
- [\_TempBuffer](UniformBuffer.md#_tempbuffer)
- [\_TempBufferInt32View](UniformBuffer.md#_tempbufferint32view)

### Accessors

- [isSync](UniformBuffer.md#issync)
- [name](UniformBuffer.md#name)
- [useUbo](UniformBuffer.md#useubo)

### Methods

- [\_buffersEqual](UniformBuffer.md#_buffersequal)
- [\_cacheMatrix](UniformBuffer.md#_cachematrix)
- [\_checkNewFrame](UniformBuffer.md#_checknewframe)
- [\_copyBuffer](UniformBuffer.md#_copybuffer)
- [\_createNewBuffer](UniformBuffer.md#_createnewbuffer)
- [\_fillAlignment](UniformBuffer.md#_fillalignment)
- [\_updateArrayForEffect](UniformBuffer.md#_updatearrayforeffect)
- [\_updateArrayForUniform](UniformBuffer.md#_updatearrayforuniform)
- [\_updateColor3ForEffect](UniformBuffer.md#_updatecolor3foreffect)
- [\_updateColor3ForUniform](UniformBuffer.md#_updatecolor3foruniform)
- [\_updateColor4ForEffect](UniformBuffer.md#_updatecolor4foreffect)
- [\_updateColor4ForUniform](UniformBuffer.md#_updatecolor4foruniform)
- [\_updateDirectColor4ForEffect](UniformBuffer.md#_updatedirectcolor4foreffect)
- [\_updateDirectColor4ForUniform](UniformBuffer.md#_updatedirectcolor4foruniform)
- [\_updateFloat2ForEffect](UniformBuffer.md#_updatefloat2foreffect)
- [\_updateFloat2ForUniform](UniformBuffer.md#_updatefloat2foruniform)
- [\_updateFloat3ForEffect](UniformBuffer.md#_updatefloat3foreffect)
- [\_updateFloat3ForUniform](UniformBuffer.md#_updatefloat3foruniform)
- [\_updateFloat4ForEffect](UniformBuffer.md#_updatefloat4foreffect)
- [\_updateFloat4ForUniform](UniformBuffer.md#_updatefloat4foruniform)
- [\_updateFloatArrayForEffect](UniformBuffer.md#_updatefloatarrayforeffect)
- [\_updateFloatArrayForUniform](UniformBuffer.md#_updatefloatarrayforuniform)
- [\_updateFloatForEffect](UniformBuffer.md#_updatefloatforeffect)
- [\_updateFloatForUniform](UniformBuffer.md#_updatefloatforuniform)
- [\_updateInt2ForEffect](UniformBuffer.md#_updateint2foreffect)
- [\_updateInt2ForUniform](UniformBuffer.md#_updateint2foruniform)
- [\_updateInt3ForEffect](UniformBuffer.md#_updateint3foreffect)
- [\_updateInt3ForUniform](UniformBuffer.md#_updateint3foruniform)
- [\_updateInt4ForEffect](UniformBuffer.md#_updateint4foreffect)
- [\_updateInt4ForUniform](UniformBuffer.md#_updateint4foruniform)
- [\_updateIntArrayForEffect](UniformBuffer.md#_updateintarrayforeffect)
- [\_updateIntArrayForUniform](UniformBuffer.md#_updateintarrayforuniform)
- [\_updateIntForEffect](UniformBuffer.md#_updateintforeffect)
- [\_updateIntForUniform](UniformBuffer.md#_updateintforuniform)
- [\_updateMatricesForEffect](UniformBuffer.md#_updatematricesforeffect)
- [\_updateMatricesForUniform](UniformBuffer.md#_updatematricesforuniform)
- [\_updateMatrix2x2ForEffect](UniformBuffer.md#_updatematrix2x2foreffect)
- [\_updateMatrix2x2ForUniform](UniformBuffer.md#_updatematrix2x2foruniform)
- [\_updateMatrix3x3ForEffect](UniformBuffer.md#_updatematrix3x3foreffect)
- [\_updateMatrix3x3ForUniform](UniformBuffer.md#_updatematrix3x3foruniform)
- [\_updateMatrixForEffect](UniformBuffer.md#_updatematrixforeffect)
- [\_updateMatrixForUniform](UniformBuffer.md#_updatematrixforuniform)
- [\_updateVector3ForEffect](UniformBuffer.md#_updatevector3foreffect)
- [\_updateVector3ForUniform](UniformBuffer.md#_updatevector3foruniform)
- [\_updateVector4ForEffect](UniformBuffer.md#_updatevector4foreffect)
- [\_updateVector4ForUniform](UniformBuffer.md#_updatevector4foruniform)
- [addColor3](UniformBuffer.md#addcolor3)
- [addColor4](UniformBuffer.md#addcolor4)
- [addFloat2](UniformBuffer.md#addfloat2)
- [addFloat3](UniformBuffer.md#addfloat3)
- [addMatrix](UniformBuffer.md#addmatrix)
- [addMatrix2x2](UniformBuffer.md#addmatrix2x2)
- [addMatrix3x3](UniformBuffer.md#addmatrix3x3)
- [addUniform](UniformBuffer.md#adduniform)
- [addVector3](UniformBuffer.md#addvector3)
- [bindToEffect](UniformBuffer.md#bindtoeffect)
- [bindUniformBuffer](UniformBuffer.md#binduniformbuffer)
- [create](UniformBuffer.md#create)
- [dispose](UniformBuffer.md#dispose)
- [getBuffer](UniformBuffer.md#getbuffer)
- [getData](UniformBuffer.md#getdata)
- [isDynamic](UniformBuffer.md#isdynamic)
- [setDataBuffer](UniformBuffer.md#setdatabuffer)
- [setTexture](UniformBuffer.md#settexture)
- [unbindEffect](UniformBuffer.md#unbindeffect)
- [update](UniformBuffer.md#update)
- [updateUniform](UniformBuffer.md#updateuniform)
- [updateUniformArray](UniformBuffer.md#updateuniformarray)
- [updateUniformDirectly](UniformBuffer.md#updateuniformdirectly)

## Constructors

### constructor

• **new UniformBuffer**(`engine`, `data?`, `dynamic?`, `name?`, `forceNoUniformBuffer?`)

Instantiates a new Uniform buffer objects.

Handles blocks of uniform on the GPU.

If WebGL 2 is not available, this class falls back on traditional setUniformXXX calls.

For more information, please refer to :

**`See`**

https://www.khronos.org/opengl/wiki/Uniform_Buffer_Object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | `undefined` | Define the engine the buffer is associated with |
| `data?` | `number`[] | `undefined` | Define the data contained in the buffer |
| `dynamic?` | `boolean` | `undefined` | Define if the buffer is updatable |
| `name?` | `string` | `undefined` | to assign to the buffer (debugging purpose) |
| `forceNoUniformBuffer` | `boolean` | `false` | define that this object must not rely on UBO objects |

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:205

## Properties

### \_buffer

• `Private` **\_buffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:27

___

### \_bufferData

• `Private` **\_bufferData**: `Float32Array`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:32

___

### \_bufferIndex

• `Private` **\_bufferIndex**: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:29

___

### \_buffers

• `Private` **\_buffers**: [[`DataBuffer`](DataBuffer.md), `undefined` \| `Float32Array`][]

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:28

___

### \_createBufferOnWrite

• `Private` **\_createBufferOnWrite**: `boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:30

___

### \_currentEffect

• `Private` **\_currentEffect**: [`Effect`](Effect.md)

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:40

___

### \_currentEffectName

• `Private` **\_currentEffectName**: `string`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:41

___

### \_currentFrameId

• `Private` **\_currentFrameId**: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:43

___

### \_data

• `Private` **\_data**: `number`[]

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:31

___

### \_dynamic

• `Private` `Optional` **\_dynamic**: `boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:33

___

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:26

___

### \_name

• `Private` **\_name**: `string`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:42

___

### \_needSync

• `Private` **\_needSync**: `boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:38

___

### \_noUBO

• `Private` **\_noUBO**: `boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:39

___

### \_uniformArraySizes

• `Private` **\_uniformArraySizes**: `Object`

#### Index signature

▪ [key: `string`]: { `arraySize`: `number` ; `strideSize`: `number`  }

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:36

___

### \_uniformLocationPointer

• `Private` **\_uniformLocationPointer**: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:37

___

### \_uniformLocations

• `Private` **\_uniformLocations**: `Object`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:34

___

### \_uniformSizes

• `Private` **\_uniformSizes**: `Object`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:35

___

### \_valueCache

• `Private` **\_valueCache**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:736

___

### updateArray

• **updateArray**: (`name`: `string`, `array`: `number`[]) => `void`

#### Type declaration

▸ (`name`, `array`): `void`

Lambda to Update an array of number in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `number`[] |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:104

___

### updateColor3

• **updateColor3**: (`name`: `string`, `color`: `IColor3Like`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `color`, `suffix?`): `void`

Lambda to Update vec3 of float from a Color in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor3Like` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:146

___

### updateColor4

• **updateColor4**: (`name`: `string`, `color`: `IColor3Like`, `alpha`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `color`, `alpha`, `suffix?`): `void`

Lambda to Update vec4 of float from a Color in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor3Like` |
| `alpha` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:153

___

### updateDirectColor4

• **updateDirectColor4**: (`name`: `string`, `color`: `IColor4Like`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `color`, `suffix?`): `void`

Lambda to Update vec4 of float from a Color in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor4Like` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:160

___

### updateFloat

• **updateFloat**: (`name`: `string`, `x`: `number`) => `void`

#### Type declaration

▸ (`name`, `x`): `void`

Lambda to Update a single float in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:69

___

### updateFloat2

• **updateFloat2**: (`name`: `string`, `x`: `number`, `y`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `suffix?`): `void`

Lambda to Update a vec2 of float in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:76

___

### updateFloat3

• **updateFloat3**: (`name`: `string`, `x`: `number`, `y`: `number`, `z`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `z`, `suffix?`): `void`

Lambda to Update a vec3 of float in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:83

___

### updateFloat4

• **updateFloat4**: (`name`: `string`, `x`: `number`, `y`: `number`, `z`: `number`, `w`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `z`, `w`, `suffix?`): `void`

Lambda to Update a vec4 of float in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `w` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:90

___

### updateFloatArray

• **updateFloatArray**: (`name`: `string`, `array`: `Float32Array`) => `void`

#### Type declaration

▸ (`name`, `array`): `void`

Lambda to Update an array of float in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Float32Array` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:97

___

### updateInt

• **updateInt**: (`name`: `string`, `x`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `suffix?`): `void`

Lambda to Update a int a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:167

___

### updateInt2

• **updateInt2**: (`name`: `string`, `x`: `number`, `y`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `suffix?`): `void`

Lambda to Update a vec2 of int in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:174

___

### updateInt3

• **updateInt3**: (`name`: `string`, `x`: `number`, `y`: `number`, `z`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `z`, `suffix?`): `void`

Lambda to Update a vec3 of int in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:181

___

### updateInt4

• **updateInt4**: (`name`: `string`, `x`: `number`, `y`: `number`, `z`: `number`, `w`: `number`, `suffix?`: `string`) => `void`

#### Type declaration

▸ (`name`, `x`, `y`, `z`, `w`, `suffix?`): `void`

Lambda to Update a vec4 of int in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `w` | `number` |
| `suffix?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:188

___

### updateIntArray

• **updateIntArray**: (`name`: `string`, `array`: `Int32Array`) => `void`

#### Type declaration

▸ (`name`, `array`): `void`

Lambda to Update an array of number in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Int32Array` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:111

___

### updateMatrices

• **updateMatrices**: (`name`: `string`, `mat`: `Float32Array`) => `void`

#### Type declaration

▸ (`name`, `mat`): `void`

Lambda to Update an array of 4x4 Matrix in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `Float32Array` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:125

___

### updateMatrix

• **updateMatrix**: (`name`: `string`, `mat`: `IMatrixLike`) => `void`

#### Type declaration

▸ (`name`, `mat`): `void`

Lambda to Update a 4x4 Matrix in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `IMatrixLike` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:118

___

### updateMatrix2x2

• **updateMatrix2x2**: (`name`: `string`, `matrix`: `Float32Array`) => `void`

#### Type declaration

▸ (`name`, `matrix`): `void`

Lambda to Update a 2x2 Matrix in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:62

___

### updateMatrix3x3

• **updateMatrix3x3**: (`name`: `string`, `matrix`: `Float32Array`) => `void`

#### Type declaration

▸ (`name`, `matrix`): `void`

Lambda to Update a 3x3 Matrix in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:55

___

### updateVector3

• **updateVector3**: (`name`: `string`, `vector`: `IVector3Like`) => `void`

#### Type declaration

▸ (`name`, `vector`): `void`

Lambda to Update vec3 of float from a Vector in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector3Like` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:132

___

### updateVector4

• **updateVector4**: (`name`: `string`, `vector`: `IVector4Like`) => `void`

#### Type declaration

▸ (`name`, `vector`): `void`

Lambda to Update vec4 of float from a Vector in a uniform buffer.
This is dynamic to allow compat with webgl 1 and 2.
You will need to pass the name of the uniform as well as the value.

##### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector4Like` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:139

___

### \_MAX\_UNIFORM\_SIZE

▪ `Static` `Private` **\_MAX\_UNIFORM\_SIZE**: `number` = `256`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:46

___

### \_TempBuffer

▪ `Static` `Private` **\_TempBuffer**: `Float32Array`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:47

___

### \_TempBufferInt32View

▪ `Static` `Private` **\_TempBufferInt32View**: `Uint32Array`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:48

## Accessors

### isSync

• `get` **isSync**(): `boolean`

Indicates if the WebGL underlying uniform buffer is in sync
with the javascript cache data.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:285

___

### name

• `get` **name**(): `string`

Gets the name of this buffer

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:544

___

### useUbo

• `get` **useUbo**(): `boolean`

Indicates if the buffer is using the WebGL2 UBO implementation,
or just falling back on setUniformXXX calls.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:277

## Methods

### \_buffersEqual

▸ `Private` **_buffersEqual**(`buf1`, `buf2`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buf1` | `Float32Array` |
| `buf2` | `Float32Array` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:548

___

### \_cacheMatrix

▸ `Private` **_cacheMatrix**(`name`, `matrix`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `IMatrixLike` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:737

___

### \_checkNewFrame

▸ `Private` **_checkNewFrame**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:619

___

### \_copyBuffer

▸ `Private` **_copyBuffer**(`src`, `dst`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `src` | `Float32Array` |
| `dst` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:557

___

### \_createNewBuffer

▸ `Private` **_createNewBuffer**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:608

___

### \_fillAlignment

▸ `Private` **_fillAlignment**(`size`): `void`

std140 layout specifies how to align data within an UBO structure.
See https://khronos.org/registry/OpenGL/specs/gl/glspec45.core.pdf#page=159
for specs.

#### Parameters

| Name | Type |
| :------ | :------ |
| `size` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:321

___

### \_updateArrayForEffect

▸ `Private` **_updateArrayForEffect**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:834

___

### \_updateArrayForUniform

▸ `Private` **_updateArrayForUniform**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:838

___

### \_updateColor3ForEffect

▸ `Private` **_updateColor3ForEffect**(`name`, `color`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `color` | `IColor3Like` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:892

___

### \_updateColor3ForUniform

▸ `Private` **_updateColor3ForUniform**(`name`, `color`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor3Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:896

___

### \_updateColor4ForEffect

▸ `Private` **_updateColor4ForEffect**(`name`, `color`, `alpha`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `color` | `IColor3Like` | `undefined` |
| `alpha` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:903

___

### \_updateColor4ForUniform

▸ `Private` **_updateColor4ForUniform**(`name`, `color`, `alpha`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor3Like` |
| `alpha` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:911

___

### \_updateDirectColor4ForEffect

▸ `Private` **_updateDirectColor4ForEffect**(`name`, `color`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `color` | `IColor4Like` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:907

___

### \_updateDirectColor4ForUniform

▸ `Private` **_updateDirectColor4ForUniform**(`name`, `color`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `color` | `IColor4Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:919

___

### \_updateFloat2ForEffect

▸ `Private` **_updateFloat2ForEffect**(`name`, `x`, `y`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:793

___

### \_updateFloat2ForUniform

▸ `Private` **_updateFloat2ForUniform**(`name`, `x`, `y`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:797

___

### \_updateFloat3ForEffect

▸ `Private` **_updateFloat3ForEffect**(`name`, `x`, `y`, `z`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `z` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:803

___

### \_updateFloat3ForUniform

▸ `Private` **_updateFloat3ForUniform**(`name`, `x`, `y`, `z`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:807

___

### \_updateFloat4ForEffect

▸ `Private` **_updateFloat4ForEffect**(`name`, `x`, `y`, `z`, `w`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `z` | `number` | `undefined` |
| `w` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:814

___

### \_updateFloat4ForUniform

▸ `Private` **_updateFloat4ForUniform**(`name`, `x`, `y`, `z`, `w`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `w` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:818

___

### \_updateFloatArrayForEffect

▸ `Private` **_updateFloatArrayForEffect**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:826

___

### \_updateFloatArrayForUniform

▸ `Private` **_updateFloatArrayForUniform**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:830

___

### \_updateFloatForEffect

▸ `Private` **_updateFloatForEffect**(`name`, `x`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:784

___

### \_updateFloatForUniform

▸ `Private` **_updateFloatForUniform**(`name`, `x`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:788

___

### \_updateInt2ForEffect

▸ `Private` **_updateInt2ForEffect**(`name`, `x`, `y`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:936

___

### \_updateInt2ForUniform

▸ `Private` **_updateInt2ForUniform**(`name`, `x`, `y`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:940

___

### \_updateInt3ForEffect

▸ `Private` **_updateInt3ForEffect**(`name`, `x`, `y`, `z`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `z` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:946

___

### \_updateInt3ForUniform

▸ `Private` **_updateInt3ForUniform**(`name`, `x`, `y`, `z`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:950

___

### \_updateInt4ForEffect

▸ `Private` **_updateInt4ForEffect**(`name`, `x`, `y`, `z`, `w`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `y` | `number` | `undefined` |
| `z` | `number` | `undefined` |
| `w` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:957

___

### \_updateInt4ForUniform

▸ `Private` **_updateInt4ForUniform**(`name`, `x`, `y`, `z`, `w`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |
| `w` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:961

___

### \_updateIntArrayForEffect

▸ `Private` **_updateIntArrayForEffect**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Int32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:842

___

### \_updateIntArrayForUniform

▸ `Private` **_updateIntArrayForUniform**(`name`, `array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `array` | `Int32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:846

___

### \_updateIntForEffect

▸ `Private` **_updateIntForEffect**(`name`, `x`, `suffix?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `x` | `number` | `undefined` |
| `suffix` | `string` | `""` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:927

___

### \_updateIntForUniform

▸ `Private` **_updateIntForUniform**(`name`, `x`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `x` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:931

___

### \_updateMatricesForEffect

▸ `Private` **_updateMatricesForEffect**(`name`, `mat`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:861

___

### \_updateMatricesForUniform

▸ `Private` **_updateMatricesForUniform**(`name`, `mat`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:865

___

### \_updateMatrix2x2ForEffect

▸ `Private` **_updateMatrix2x2ForEffect**(`name`, `matrix`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:768

___

### \_updateMatrix2x2ForUniform

▸ `Private` **_updateMatrix2x2ForUniform**(`name`, `matrix`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:772

___

### \_updateMatrix3x3ForEffect

▸ `Private` **_updateMatrix3x3ForEffect**(`name`, `matrix`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:764

___

### \_updateMatrix3x3ForUniform

▸ `Private` **_updateMatrix3x3ForUniform**(`name`, `matrix`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `matrix` | `Float32Array` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:752

___

### \_updateMatrixForEffect

▸ `Private` **_updateMatrixForEffect**(`name`, `mat`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `IMatrixLike` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:851

___

### \_updateMatrixForUniform

▸ `Private` **_updateMatrixForUniform**(`name`, `mat`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `mat` | `IMatrixLike` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:855

___

### \_updateVector3ForEffect

▸ `Private` **_updateVector3ForEffect**(`name`, `vector`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector3Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:869

___

### \_updateVector3ForUniform

▸ `Private` **_updateVector3ForUniform**(`name`, `vector`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector3Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:873

___

### \_updateVector4ForEffect

▸ `Private` **_updateVector4ForEffect**(`name`, `vector`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector4Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:880

___

### \_updateVector4ForUniform

▸ `Private` **_updateVector4ForUniform**(`name`, `vector`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `vector` | `IVector4Like` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:884

___

### addColor3

▸ **addColor3**(`name`, `color`): `void`

Adds a vec3 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `color` | `IColor3Like` | Define the vec3 from a Color |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:452

___

### addColor4

▸ **addColor4**(`name`, `color`, `alpha`): `void`

Adds a vec4 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `color` | `IColor3Like` | Define the rgb components from a Color |
| `alpha` | `number` | Define the a component of the vec4 |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:463

___

### addFloat2

▸ **addFloat2**(`name`, `x`, `y`): `void`

Adds a vec2 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `x` | `number` | Define the x component value of the vec2 |
| `y` | `number` | Define the y component value of the vec2 |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:430

___

### addFloat3

▸ **addFloat3**(`name`, `x`, `y`, `z`): `void`

Adds a vec3 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `x` | `number` | Define the x component value of the vec3 |
| `y` | `number` | Define the y component value of the vec3 |
| `z` | `number` | Define the z component value of the vec3 |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:442

___

### addMatrix

▸ **addMatrix**(`name`, `mat`): `void`

Adds a Matrix 4x4 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `mat` | `IMatrixLike` | A 4x4 matrix. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:420

___

### addMatrix2x2

▸ **addMatrix2x2**(`name`): `void`

Adds a Matrix 2x2 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:490

___

### addMatrix3x3

▸ **addMatrix3x3**(`name`): `void`

Adds a Matrix 3x3 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:482

___

### addUniform

▸ **addUniform**(`name`, `size`, `arraySize?`): `void`

Adds an uniform in the buffer.
Warning : the subsequents calls of this function must be in the same order as declared in the shader
for the layout to be correct ! The addUniform function only handles types like float, vec2, vec3, vec4, mat4,
meaning size=1,2,3,4 or 16. It does not handle struct types.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Name of the uniform, as used in the uniform block in the shader. |
| `size` | `number` \| `number`[] | `undefined` | Data size, or data directly. |
| `arraySize` | `number` | `0` | The number of elements in the array, 0 if not an array. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:353

___

### addVector3

▸ **addVector3**(`name`, `vector`): `void`

Adds a vec3 to the uniform buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the uniform, as used in the uniform block in the shader. |
| `vector` | `IVector3Like` | Define the vec3 components from a Vector |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:473

___

### bindToEffect

▸ **bindToEffect**(`effect`, `name`): `void`

Associates an effect to this uniform buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | Define the effect to associate the buffer to |
| `name` | `string` | Name of the uniform block in the shader. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:994

___

### bindUniformBuffer

▸ **bindUniformBuffer**(): `void`

Binds the current (GPU) buffer to the effect

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:1002

___

### create

▸ **create**(): `void`

Effectively creates the WebGL Uniform Buffer, once layout is completed with `addUniform`.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:497

___

### dispose

▸ **dispose**(): `void`

Disposes the uniform buffer.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:1044

___

### getBuffer

▸ **getBuffer**(): [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

The underlying WebGL Uniform buffer.

#### Returns

[`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

the webgl buffer

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:311

___

### getData

▸ **getData**(): `Float32Array`

The data cache on JS side.

#### Returns

`Float32Array`

the underlying data as a float array

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:303

___

### isDynamic

▸ **isDynamic**(): `boolean`

Indicates if the WebGL underlying uniform buffer is dynamic.
Also, a dynamic UniformBuffer will disable cache verification and always
update the underlying WebGL uniform buffer to the GPU.

#### Returns

`boolean`

if Dynamic, otherwise false

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:295

___

### setDataBuffer

▸ **setDataBuffer**(`dataBuffer`): `boolean`

Sets the current state of the class (_bufferIndex, _buffer) to point to the data buffer passed in parameter if this buffer is one of the buffers handled by the class (meaning if it can be found in the _buffers array)
This method is meant to be able to update a buffer at any time: just call setDataBuffer to set the class in the right state, call some updateXXX methods and then call udpate() => that will update the GPU buffer on the graphic card

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataBuffer` | [`DataBuffer`](DataBuffer.md) | buffer to look for |

#### Returns

`boolean`

true if the buffer has been found and the class internal state points to it, else false

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:1022

___

### setTexture

▸ **setTexture**(`name`, `texture`): `void`

Sets a sampler uniform on the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the sampler. |
| `texture` | [`Nullable`](../modules.md#nullable)[`ThinTexture`](ThinTexture.md) | Define the texture to set in the sampler |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:974

___

### unbindEffect

▸ **unbindEffect**(): `void`

Dissociates the current effect from this uniform buffer

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:1011

___

### update

▸ **update**(): `void`

Updates the WebGL Uniform Buffer on the GPU.
If the `dynamic` flag is set to true, no cache comparison is done.
Otherwise, the buffer will be updated only if the cache differs.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:568

___

### updateUniform

▸ **updateUniform**(`uniformName`, `data`, `size`): `void`

Updates the value of an uniform. The `update` method must be called afterwards to make it effective in the GPU.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Define the name of the uniform, as used in the uniform block in the shader. |
| `data` | [`FloatArray`](../modules.md#floatarray) | Define the flattened data |
| `size` | `number` | Define the size of the data. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:639

___

### updateUniformArray

▸ **updateUniformArray**(`uniformName`, `data`, `size`): `void`

Updates the value of an uniform. The `update` method must be called afterwards to make it effective in the GPU.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Define the name of the uniform, as used in the uniform block in the shader. |
| `data` | [`FloatArray`](../modules.md#floatarray) | Define the flattened data |
| `size` | `number` | Define the size of the data. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:688

___

### updateUniformDirectly

▸ **updateUniformDirectly**(`uniformName`, `data`): `void`

Directly updates the value of the uniform in the cache AND on the GPU.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Define the name of the uniform, as used in the uniform block in the shader. |
| `data` | [`FloatArray`](../modules.md#floatarray) | Define the flattened data |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/uniformBuffer.ts:983

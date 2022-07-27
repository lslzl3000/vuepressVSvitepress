[@dev/core](../README.md) / [Exports](../modules.md) / IPipelineContext

# Interface: IPipelineContext

Class used to store and describe the pipeline context associated with an effect

## Table of contents

### Properties

- [isAsync](IPipelineContext.md#isasync)
- [isReady](IPipelineContext.md#isready)

### Methods

- [dispose](IPipelineContext.md#dispose)
- [setArray](IPipelineContext.md#setarray)
- [setArray2](IPipelineContext.md#setarray2)
- [setArray3](IPipelineContext.md#setarray3)
- [setArray4](IPipelineContext.md#setarray4)
- [setColor3](IPipelineContext.md#setcolor3)
- [setColor4](IPipelineContext.md#setcolor4)
- [setDirectColor4](IPipelineContext.md#setdirectcolor4)
- [setFloat](IPipelineContext.md#setfloat)
- [setFloat2](IPipelineContext.md#setfloat2)
- [setFloat3](IPipelineContext.md#setfloat3)
- [setFloat4](IPipelineContext.md#setfloat4)
- [setInt](IPipelineContext.md#setint)
- [setInt2](IPipelineContext.md#setint2)
- [setInt3](IPipelineContext.md#setint3)
- [setInt4](IPipelineContext.md#setint4)
- [setIntArray](IPipelineContext.md#setintarray)
- [setIntArray2](IPipelineContext.md#setintarray2)
- [setIntArray3](IPipelineContext.md#setintarray3)
- [setIntArray4](IPipelineContext.md#setintarray4)
- [setMatrices](IPipelineContext.md#setmatrices)
- [setMatrix](IPipelineContext.md#setmatrix)
- [setMatrix2x2](IPipelineContext.md#setmatrix2x2)
- [setMatrix3x3](IPipelineContext.md#setmatrix3x3)
- [setQuaternion](IPipelineContext.md#setquaternion)
- [setVector2](IPipelineContext.md#setvector2)
- [setVector3](IPipelineContext.md#setvector3)
- [setVector4](IPipelineContext.md#setvector4)

## Properties

### isAsync

• **isAsync**: `boolean`

Gets a boolean indicating that this pipeline context is supporting asynchronous creating

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:12

___

### isReady

• **isReady**: `boolean`

Gets a boolean indicating that the context is ready to be used (like shaders / pipelines are compiled and ready for instance)

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:16

## Methods

### dispose

▸ **dispose**(): `void`

Releases the resources associated with the pipeline.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:43

___

### setArray

▸ **setArray**(`uniformName`, `array`): `void`

Sets an array on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] \| `Float32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:112

___

### setArray2

▸ **setArray2**(`uniformName`, `array`): `void`

Sets an array 2 on a uniform variable. (Array is specified as single array eg. [1,2,3,4] will result in [[1,2],[3,4]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] \| `Float32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:119

___

### setArray3

▸ **setArray3**(`uniformName`, `array`): `void`

Sets an array 3 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6] will result in [[1,2,3],[4,5,6]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] \| `Float32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:126

___

### setArray4

▸ **setArray4**(`uniformName`, `array`): `void`

Sets an array 4 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6,7,8] will result in [[1,2,3,4],[5,6,7,8]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] \| `Float32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:133

___

### setColor3

▸ **setColor3**(`uniformName`, `color3`): `void`

Sets a Color3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `color3` | `IColor3Like` | Value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:230

___

### setColor4

▸ **setColor4**(`uniformName`, `color3`, `alpha`): `void`

Sets a Color4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `color3` | `IColor3Like` | Value to be set. |
| `alpha` | `number` | Alpha value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:238

___

### setDirectColor4

▸ **setDirectColor4**(`uniformName`, `color4`): `void`

Sets a Color4 on a uniform variable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | defines the name of the variable |
| `color4` | `IColor4Like` | defines the value to be set |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:245

___

### setFloat

▸ **setFloat**(`uniformName`, `value`): `void`

Sets a float on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `value` | `number` | value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:168

___

### setFloat2

▸ **setFloat2**(`uniformName`, `x`, `y`): `void`

Sets a float2 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float2. |
| `y` | `number` | Second float in float2. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:183

___

### setFloat3

▸ **setFloat3**(`uniformName`, `x`, `y`, `z`): `void`

Sets a float3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float3. |
| `y` | `number` | Second float in float3. |
| `z` | `number` | Third float in float3. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:199

___

### setFloat4

▸ **setFloat4**(`uniformName`, `x`, `y`, `z`, `w`): `void`

Sets a float4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float4. |
| `y` | `number` | Second float in float4. |
| `z` | `number` | Third float in float4. |
| `w` | `number` | Fourth float in float4. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:223

___

### setInt

▸ **setInt**(`uniformName`, `value`): `void`

Sets an integer value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `value` | `number` | Value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:50

___

### setInt2

▸ **setInt2**(`uniformName`, `x`, `y`): `void`

Sets an int2 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int2. |
| `y` | `number` | Second int in int2. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:58

___

### setInt3

▸ **setInt3**(`uniformName`, `x`, `y`, `z`): `void`

Sets an int3 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int3. |
| `y` | `number` | Second int in int3. |
| `z` | `number` | Third int in int3. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:67

___

### setInt4

▸ **setInt4**(`uniformName`, `x`, `y`, `z`, `w`): `void`

Sets an int4 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int4. |
| `y` | `number` | Second int in int4. |
| `z` | `number` | Third int in int4. |
| `w` | `number` | Fourth int in int4. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:77

___

### setIntArray

▸ **setIntArray**(`uniformName`, `array`): `void`

Sets an int array on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:84

___

### setIntArray2

▸ **setIntArray2**(`uniformName`, `array`): `void`

Sets an int array 2 on a uniform variable. (Array is specified as single array eg. [1,2,3,4] will result in [[1,2],[3,4]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:91

___

### setIntArray3

▸ **setIntArray3**(`uniformName`, `array`): `void`

Sets an int array 3 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6] will result in [[1,2,3],[4,5,6]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:98

___

### setIntArray4

▸ **setIntArray4**(`uniformName`, `array`): `void`

Sets an int array 4 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6,7,8] will result in [[1,2,3,4],[5,6,7,8]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:105

___

### setMatrices

▸ **setMatrices**(`uniformName`, `matrices`): `void`

Sets matrices on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrices` | `Float32Array` | matrices to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:140

___

### setMatrix

▸ **setMatrix**(`uniformName`, `matrix`): `void`

Sets matrix on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `IMatrixLike` | matrix to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:147

___

### setMatrix2x2

▸ **setMatrix2x2**(`uniformName`, `matrix`): `void`

Sets a 2x2 matrix on a uniform variable. (Specified as [1,2,3,4] will result in [1,2][3,4] matrix)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `Float32Array` | matrix to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:161

___

### setMatrix3x3

▸ **setMatrix3x3**(`uniformName`, `matrix`): `void`

Sets a 3x3 matrix on a uniform variable. (Specified as [1,2,3,4,5,6,7,8,9] will result in [1,2,3][4,5,6][7,8,9] matrix)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `Float32Array` | matrix to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:154

___

### setQuaternion

▸ **setQuaternion**(`uniformName`, `quaternion`): `void`

Sets a Quaternion on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `quaternion` | `IQuaternionLike` | Value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:213

___

### setVector2

▸ **setVector2**(`uniformName`, `vector2`): `void`

Sets a Vector2 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector2` | `IVector2Like` | vector2 to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:175

___

### setVector3

▸ **setVector3**(`uniformName`, `vector3`): `void`

Sets a Vector3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector3` | `IVector3Like` | Value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:190

___

### setVector4

▸ **setVector4**(`uniformName`, `vector4`): `void`

Sets a Vector4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector4` | `IVector4Like` | Value to be set. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/IPipelineContext.ts:206

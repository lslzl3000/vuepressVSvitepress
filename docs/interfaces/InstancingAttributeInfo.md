[@dev/core](../README.md) / [Exports](../modules.md) / InstancingAttributeInfo

# Interface: InstancingAttributeInfo

Interface for attribute information associated with buffer instantiation

## Table of contents

### Properties

- [attributeName](InstancingAttributeInfo.md#attributename)
- [attributeSize](InstancingAttributeInfo.md#attributesize)
- [attributeType](InstancingAttributeInfo.md#attributetype)
- [divisor](InstancingAttributeInfo.md#divisor)
- [index](InstancingAttributeInfo.md#index)
- [normalized](InstancingAttributeInfo.md#normalized)
- [offset](InstancingAttributeInfo.md#offset)

## Properties

### attributeName

• **attributeName**: `string`

Name of the GLSL attribute
if attribute index is not specified, this is used to retrieve the index from the effect

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:9

___

### attributeSize

• **attributeSize**: `number`

size of the attribute, 1, 2, 3 or 4

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:20

___

### attributeType

• `Optional` **attributeType**: `number`

type of the attribute, gl.BYTE, gl.UNSIGNED_BYTE, gl.SHORT, gl.UNSIGNED_SHORT, gl.FIXED, gl.FLOAT.
default is FLOAT

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:37

___

### divisor

• `Optional` **divisor**: `number`

Modifies the rate at which generic vertex attributes advance when rendering multiple instances
default to 1

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:31

___

### index

• `Optional` **index**: `number`

Index/offset of the attribute in the vertex shader
if not specified, this will be computes from the name.

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:15

___

### normalized

• `Optional` **normalized**: `boolean`

normalization of fixed-point data. behavior unclear, use FALSE, default is FALSE

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:42

___

### offset

• **offset**: `number`

Offset of the data in the Vertex Buffer acting as the instancing buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/instancingAttributeInfo.ts:25

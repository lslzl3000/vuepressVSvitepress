[@dev/core](../README.md) / [Exports](../modules.md) / IIOptionShadowDepthMaterial

# Interface: IIOptionShadowDepthMaterial

Options to be used when creating a shadow depth material

## Table of contents

### Properties

- [remappedVariables](IIOptionShadowDepthMaterial.md#remappedvariables)
- [standalone](IIOptionShadowDepthMaterial.md#standalone)

## Properties

### remappedVariables

• `Optional` **remappedVariables**: `string`[]

Variables in the vertex shader code that need to have their names remapped.
The format is: ["var_name", "var_remapped_name", "var_name", "var_remapped_name", ...]
"var_name" should be either: worldPos or vNormalW
So, if the variable holding the world position in your vertex shader is not named worldPos, you must tell the system
the name to use instead by using: ["worldPos", "myWorldPosVar"] assuming the variable is named myWorldPosVar in your code.
If the normal must also be remapped: ["worldPos", "myWorldPosVar", "vNormalW", "myWorldNormal"]

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:26

___

### standalone

• `Optional` **standalone**: `boolean`

Set standalone to true if the base material wrapped by ShadowDepthMaterial is not used for a regular object but for depth shadow generation only

#### Defined in

https://github.com/babylon.js/core/src/Materials/shadowDepthWrapper.ts:29

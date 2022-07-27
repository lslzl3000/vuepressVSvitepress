[@dev/core](../README.md) / [Exports](../modules.md) / FresnelParameters

# Class: FresnelParameters

This represents all the required information to add a fresnel effect on a material:

**`See`**

https://doc.babylonjs.com/divingDeeper/materials/using/fresnelParameters

## Table of contents

### Constructors

- [constructor](FresnelParameters.md#constructor)

### Properties

- [\_isEnabled](FresnelParameters.md#_isenabled)
- [bias](FresnelParameters.md#bias)
- [leftColor](FresnelParameters.md#leftcolor)
- [power](FresnelParameters.md#power)
- [rightColor](FresnelParameters.md#rightcolor)

### Accessors

- [isEnabled](FresnelParameters.md#isenabled)

### Methods

- [clone](FresnelParameters.md#clone)
- [equals](FresnelParameters.md#equals)
- [serialize](FresnelParameters.md#serialize)
- [Parse](FresnelParameters.md#parse)

## Constructors

### constructor

• **new FresnelParameters**(`options?`)

Creates a new FresnelParameters object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IFresnelParametersCreationOptions`](../modules.md#ifresnelparameterscreationoptions) | provide your own settings to optionally to override defaults |

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:114

## Properties

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:73

___

### bias

• **bias**: `number`

Define bias applied to computed fresnel term

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:102

___

### leftColor

• **leftColor**: [`Color3`](Color3.md)

Define the color used on edges (grazing angle)

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:92

___

### power

• **power**: `number`

Defined the power exponent applied to fresnel term

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:107

___

### rightColor

• **rightColor**: [`Color3`](Color3.md)

Define the color used on center

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:97

## Accessors

### isEnabled

• `get` **isEnabled**(): `boolean`

Define if the fresnel effect is enable or not.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:77

• `set` **isEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:80

## Methods

### clone

▸ **clone**(): [`FresnelParameters`](FresnelParameters.md)

Clones the current fresnel and its values

#### Returns

[`FresnelParameters`](FresnelParameters.md)

a clone fresnel configuration

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:128

___

### equals

▸ **equals**(`otherFresnelParameters`): `boolean`

Determines equality between FresnelParameters objects

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherFresnelParameters` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`FresnelParameters`](FresnelParameters.md) | defines the second operand |

#### Returns

`boolean`

true if the power, bias, leftColor, rightColor and isEnabled values are equal to the given ones

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:141

___

### serialize

▸ **serialize**(): [`IFresnelParametersSerialized`](../modules.md#ifresnelparametersserialized)

Serializes the current fresnel parameters to a JSON representation.

#### Returns

[`IFresnelParametersSerialized`](../modules.md#ifresnelparametersserialized)

the JSON serialization

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:156

___

### Parse

▸ `Static` **Parse**(`parsedFresnelParameters`): [`FresnelParameters`](FresnelParameters.md)

Parse a JSON object and deserialize it to a new Fresnel parameter object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedFresnelParameters` | [`IFresnelParametersSerialized`](../modules.md#ifresnelparametersserialized) | Define the JSON representation |

#### Returns

[`FresnelParameters`](FresnelParameters.md)

the parsed parameters

#### Defined in

https://github.com/babylon.js/core/src/Materials/fresnelParameters.ts:171

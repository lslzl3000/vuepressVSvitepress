[@dev/core](../README.md) / [Exports](../modules.md) / SphericalPolynomial

# Class: SphericalPolynomial

Class representing spherical polynomial coefficients to the 3rd degree

## Table of contents

### Constructors

- [constructor](SphericalPolynomial.md#constructor)

### Properties

- [\_harmonics](SphericalPolynomial.md#_harmonics)
- [x](SphericalPolynomial.md#x)
- [xx](SphericalPolynomial.md#xx)
- [xy](SphericalPolynomial.md#xy)
- [y](SphericalPolynomial.md#y)
- [yy](SphericalPolynomial.md#yy)
- [yz](SphericalPolynomial.md#yz)
- [z](SphericalPolynomial.md#z)
- [zx](SphericalPolynomial.md#zx)
- [zz](SphericalPolynomial.md#zz)

### Accessors

- [preScaledHarmonics](SphericalPolynomial.md#prescaledharmonics)

### Methods

- [addAmbient](SphericalPolynomial.md#addambient)
- [scaleInPlace](SphericalPolynomial.md#scaleinplace)
- [updateFromHarmonics](SphericalPolynomial.md#updatefromharmonics)
- [FromArray](SphericalPolynomial.md#fromarray)
- [FromHarmonics](SphericalPolynomial.md#fromharmonics)

## Constructors

### constructor

• **new SphericalPolynomial**()

## Properties

### \_harmonics

• `Private` **\_harmonics**: [`Nullable`](../modules.md#nullable)[`SphericalHarmonics`](SphericalHarmonics.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:335

___

### x

• **x**: [`Vector3`](Vector3.md)

The x coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:353

___

### xx

• **xx**: [`Vector3`](Vector3.md)

The xx coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:368

___

### xy

• **xy**: [`Vector3`](Vector3.md)

The xy coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:383

___

### y

• **y**: [`Vector3`](Vector3.md)

The y coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:358

___

### yy

• **yy**: [`Vector3`](Vector3.md)

The yy coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:373

___

### yz

• **yz**: [`Vector3`](Vector3.md)

The yz coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:388

___

### z

• **z**: [`Vector3`](Vector3.md)

The z coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:363

___

### zx

• **zx**: [`Vector3`](Vector3.md)

The zx coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:393

___

### zz

• **zz**: [`Vector3`](Vector3.md)

The zz coefficients of the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:378

## Accessors

### preScaledHarmonics

• `get` **preScaledHarmonics**(): [`SphericalHarmonics`](SphericalHarmonics.md)

The spherical harmonics used to create the polynomials.

#### Returns

[`SphericalHarmonics`](SphericalHarmonics.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:340

## Methods

### addAmbient

▸ **addAmbient**(`color`): `void`

Adds an ambient color to the spherical polynomial

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | the color to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:399

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): `void`

Scales the spherical polynomial by the given amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | the amount to scale |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:411

___

### updateFromHarmonics

▸ **updateFromHarmonics**(`harmonics`): [`SphericalPolynomial`](SphericalPolynomial.md)

Updates the spherical polynomial from harmonics

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `harmonics` | [`SphericalHarmonics`](SphericalHarmonics.md) | the spherical harmonics |

#### Returns

[`SphericalPolynomial`](SphericalPolynomial.md)

the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:428

___

### FromArray

▸ `Static` **FromArray**(`data`): [`SphericalPolynomial`](SphericalPolynomial.md)

Constructs a spherical polynomial from an array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayLike``ArrayLike``number` | defines the 9x3 coefficients (x, y, z, xx, yy, zz, yz, zx, xy) |

#### Returns

[`SphericalPolynomial`](SphericalPolynomial.md)

the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:475

___

### FromHarmonics

▸ `Static` **FromHarmonics**(`harmonics`): [`SphericalPolynomial`](SphericalPolynomial.md)

Gets the spherical polynomial from harmonics

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `harmonics` | [`SphericalHarmonics`](SphericalHarmonics.md) | the spherical harmonics |

#### Returns

[`SphericalPolynomial`](SphericalPolynomial.md)

the spherical polynomial

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:465

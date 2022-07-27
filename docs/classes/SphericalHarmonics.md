[@dev/core](../README.md) / [Exports](../modules.md) / SphericalHarmonics

# Class: SphericalHarmonics

Class representing spherical harmonics coefficients to the 3rd degree

## Table of contents

### Constructors

- [constructor](SphericalHarmonics.md#constructor)

### Properties

- [l00](SphericalHarmonics.md#l00)
- [l10](SphericalHarmonics.md#l10)
- [l11](SphericalHarmonics.md#l11)
- [l1\_1](SphericalHarmonics.md#l1_1)
- [l20](SphericalHarmonics.md#l20)
- [l21](SphericalHarmonics.md#l21)
- [l22](SphericalHarmonics.md#l22)
- [l2\_1](SphericalHarmonics.md#l2_1)
- [l2\_2](SphericalHarmonics.md#l2_2)
- [preScaled](SphericalHarmonics.md#prescaled)

### Methods

- [addLight](SphericalHarmonics.md#addlight)
- [convertIncidentRadianceToIrradiance](SphericalHarmonics.md#convertincidentradiancetoirradiance)
- [convertIrradianceToLambertianRadiance](SphericalHarmonics.md#convertirradiancetolambertianradiance)
- [preScaleForRendering](SphericalHarmonics.md#prescaleforrendering)
- [scaleInPlace](SphericalHarmonics.md#scaleinplace)
- [updateFromArray](SphericalHarmonics.md#updatefromarray)
- [updateFromFloatsArray](SphericalHarmonics.md#updatefromfloatsarray)
- [FromArray](SphericalHarmonics.md#fromarray)
- [FromPolynomial](SphericalHarmonics.md#frompolynomial)

## Constructors

### constructor

• **new SphericalHarmonics**()

## Properties

### l00

• **l00**: [`Vector3`](Vector3.md)

The l0,0 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:96

___

### l10

• **l10**: [`Vector3`](Vector3.md)

The l1,0 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:106

___

### l11

• **l11**: [`Vector3`](Vector3.md)

The l1,1 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:111

___

### l1\_1

• **l1\_1**: [`Vector3`](Vector3.md)

The l1,-1 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:101

___

### l20

• **l20**: [`Vector3`](Vector3.md)

The l2,0 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:126

___

### l21

• **l21**: [`Vector3`](Vector3.md)

The l2,1 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:131

___

### l22

• **l22**: [`Vector3`](Vector3.md)

The l2,2 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:136

___

### l2\_1

• **l2\_1**: [`Vector3`](Vector3.md)

The l2,-1 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:121

___

### l2\_2

• **l2\_2**: [`Vector3`](Vector3.md)

The l2,-2 coefficients of the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:116

___

### preScaled

• **preScaled**: `boolean` = `false`

Defines whether or not the harmonics have been prescaled for rendering.

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:91

## Methods

### addLight

▸ **addLight**(`direction`, `color`, `deltaSolidAngle`): `void`

Adds a light to the spherical harmonics

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction` | [`Vector3`](Vector3.md) | the direction of the light |
| `color` | [`Color3`](Color3.md) | the color of the light |
| `deltaSolidAngle` | `number` | the delta solid angle of the light |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:144

___

### convertIncidentRadianceToIrradiance

▸ **convertIncidentRadianceToIrradiance**(): `void`

Convert from incident radiance (Li) to irradiance (E) by applying convolution with the cosine-weighted hemisphere.

```
E_lm = A_l * L_lm
```

In spherical harmonics this convolution amounts to scaling factors for each frequency band.
This corresponds to equation 5 in "An Efficient Representation for Irradiance Environment Maps", where
the scaling factors are given in equation 9.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:199

___

### convertIrradianceToLambertianRadiance

▸ **convertIrradianceToLambertianRadiance**(): `void`

Convert from irradiance to outgoing radiance for Lambertian BDRF, suitable for efficient shader evaluation.

```
L = (1/pi) * E * rho
```

This is done by an additional scale by 1/pi, so is a fairly trivial operation but important conceptually.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:225

___

### preScaleForRendering

▸ **preScaleForRendering**(): `void`

Integrates the reconstruction coefficients directly in to the SH preventing further
required operations at run time.

This is simply done by scaling back the SH with Ylm constants parameter.
The trigonometric part being applied by the shader at run time.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:239

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): `void`

Scales the spherical harmonics by the given amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | the amount to scale |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:176

___

### updateFromArray

▸ **updateFromArray**(`data`): [`SphericalHarmonics`](SphericalHarmonics.md)

update the spherical harmonics coefficients from the given array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayLike``ArrayLike``number` | defines the 9x3 coefficients (l00, l1-1, l10, l11, l2-2, l2-1, l20, l21, l22) |

#### Returns

[`SphericalHarmonics`](SphericalHarmonics.md)

the spherical harmonics (this)

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:260

___

### updateFromFloatsArray

▸ **updateFromFloatsArray**(`data`): [`SphericalHarmonics`](SphericalHarmonics.md)

update the spherical harmonics coefficients from the given floats array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayLike``number` | defines the 9x3 coefficients (l00, l1-1, l10, l11, l2-2, l2-1, l20, l21, l22) |

#### Returns

[`SphericalHarmonics`](SphericalHarmonics.md)

the spherical harmonics (this)

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:278

___

### FromArray

▸ `Static` **FromArray**(`data`): [`SphericalHarmonics`](SphericalHarmonics.md)

Constructs a spherical harmonics from an array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayLike``ArrayLike``number` | defines the 9x3 coefficients (l00, l1-1, l10, l11, l2-2, l2-1, l20, l21, l22) |

#### Returns

[`SphericalHarmonics`](SphericalHarmonics.md)

the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:296

___

### FromPolynomial

▸ `Static` **FromPolynomial**(`polynomial`): [`SphericalHarmonics`](SphericalHarmonics.md)

Gets the spherical harmonics from polynomial

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `polynomial` | [`SphericalPolynomial`](SphericalPolynomial.md) | the spherical polynomial |

#### Returns

[`SphericalHarmonics`](SphericalHarmonics.md)

the spherical harmonics

#### Defined in

https://github.com/babylon.js/core/src/Maths/sphericalPolynomial.ts:307

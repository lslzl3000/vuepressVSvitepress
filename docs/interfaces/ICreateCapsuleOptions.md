[@dev/core](../README.md) / [Exports](../modules.md) / ICreateCapsuleOptions

# Interface: ICreateCapsuleOptions

The options Interface for creating a Capsule Mesh

## Table of contents

### Properties

- [bottomCapSubdivisions](ICreateCapsuleOptions.md#bottomcapsubdivisions)
- [capSubdivisions](ICreateCapsuleOptions.md#capsubdivisions)
- [height](ICreateCapsuleOptions.md#height)
- [orientation](ICreateCapsuleOptions.md#orientation)
- [radius](ICreateCapsuleOptions.md#radius)
- [radiusBottom](ICreateCapsuleOptions.md#radiusbottom)
- [radiusTop](ICreateCapsuleOptions.md#radiustop)
- [subdivisions](ICreateCapsuleOptions.md#subdivisions)
- [tessellation](ICreateCapsuleOptions.md#tessellation)
- [topCapSubdivisions](ICreateCapsuleOptions.md#topcapsubdivisions)
- [updatable](ICreateCapsuleOptions.md#updatable)

## Properties

### bottomCapSubdivisions

• `Optional` **bottomCapSubdivisions**: `number`

Overwrite for the bottom capSubdivisions.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:250

___

### capSubdivisions

• `Optional` **capSubdivisions**: `number`

Number of sub segments on the cap sections of the capsule running parallel to orientation.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:238

___

### height

• `Optional` **height**: `number`

Height or Length of the capsule.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:232

___

### orientation

• `Optional` **orientation**: [`Vector3`](../classes/Vector3.md)

The Orientation of the capsule.  Default : Vector3.Up()

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:223

___

### radius

• `Optional` **radius**: `number`

Radius of the capsule.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:235

___

### radiusBottom

• `Optional` **radiusBottom**: `number`

Overwrite for the bottom radius.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:244

___

### radiusTop

• `Optional` **radiusTop**: `number`

Overwrite for the top radius.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:241

___

### subdivisions

• `Optional` **subdivisions**: `number`

Number of sub segments on the tube section of the capsule running parallel to orientation.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:226

___

### tessellation

• `Optional` **tessellation**: `number`

Number of cylindrical segments on the capsule.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:229

___

### topCapSubdivisions

• `Optional` **topCapSubdivisions**: `number`

Overwrite for the top capSubdivisions.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:247

___

### updatable

• `Optional` **updatable**: `boolean`

Internal geometry is supposed to change once created.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/Builders/capsuleBuilder.ts:253

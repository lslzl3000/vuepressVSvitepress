[@dev/core](../README.md) / [Exports](../modules.md) / Frustum

# Class: Frustum

Represents a camera frustum

## Table of contents

### Constructors

- [constructor](Frustum.md#constructor)

### Methods

- [GetBottomPlaneToRef](Frustum.md#getbottomplanetoref)
- [GetFarPlaneToRef](Frustum.md#getfarplanetoref)
- [GetLeftPlaneToRef](Frustum.md#getleftplanetoref)
- [GetNearPlaneToRef](Frustum.md#getnearplanetoref)
- [GetPlanes](Frustum.md#getplanes)
- [GetPlanesToRef](Frustum.md#getplanestoref)
- [GetRightPlaneToRef](Frustum.md#getrightplanetoref)
- [GetTopPlaneToRef](Frustum.md#gettopplanetoref)

## Constructors

### constructor

• **new Frustum**()

## Methods

### GetBottomPlaneToRef

▸ `Static` **GetBottomPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the bottom frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:98

___

### GetFarPlaneToRef

▸ `Static` **GetFarPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the far frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:42

___

### GetLeftPlaneToRef

▸ `Static` **GetLeftPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the left frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:56

___

### GetNearPlaneToRef

▸ `Static` **GetNearPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the near frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:28

___

### GetPlanes

▸ `Static` **GetPlanes**(`transform`): [`Plane`](Plane.md)[]

Gets the planes representing the frustum

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | matrix to be applied to the returned planes |

#### Returns

[`Plane`](Plane.md)[]

a new array of 6 Frustum planes computed by the given transformation matrix.

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:14

___

### GetPlanesToRef

▸ `Static` **GetPlanesToRef**(`transform`, `frustumPlanes`): `void`

Sets the given array "frustumPlanes" with the 6 Frustum planes computed by the given transformation matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum planes |
| `frustumPlanes` | [`Plane`](Plane.md)[] | the resulting frustum planes |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:112

___

### GetRightPlaneToRef

▸ `Static` **GetRightPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the right frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:70

___

### GetTopPlaneToRef

▸ `Static` **GetTopPlaneToRef**(`transform`, `frustumPlane`): `void`

Gets the top frustum plane transformed by the transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | transformation matrix to be applied to the resulting frustum plane |
| `frustumPlane` | [`Plane`](Plane.md) | the resulting frustum plane |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.frustum.ts:84

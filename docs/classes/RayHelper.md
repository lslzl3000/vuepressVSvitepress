[@dev/core](../README.md) / [Exports](../modules.md) / RayHelper

# Class: RayHelper

As raycast might be hard to debug, the RayHelper can help rendering the different rays
in order to better appreciate the issue one might have.

**`See`**

https://doc.babylonjs.com/babylon101/raycasts#debugging

## Table of contents

### Constructors

- [constructor](RayHelper.md#constructor)

### Properties

- [\_attachedToMesh](RayHelper.md#_attachedtomesh)
- [\_meshSpaceDirection](RayHelper.md#_meshspacedirection)
- [\_meshSpaceOrigin](RayHelper.md#_meshspaceorigin)
- [\_onAfterRenderObserver](RayHelper.md#_onafterrenderobserver)
- [\_onAfterStepObserver](RayHelper.md#_onafterstepobserver)
- [\_renderFunction](RayHelper.md#_renderfunction)
- [\_renderLine](RayHelper.md#_renderline)
- [\_renderPoints](RayHelper.md#_renderpoints)
- [\_scene](RayHelper.md#_scene)
- [ray](RayHelper.md#ray)

### Methods

- [\_render](RayHelper.md#_render)
- [\_updateToMesh](RayHelper.md#_updatetomesh)
- [attachToMesh](RayHelper.md#attachtomesh)
- [detachFromMesh](RayHelper.md#detachfrommesh)
- [dispose](RayHelper.md#dispose)
- [hide](RayHelper.md#hide)
- [show](RayHelper.md#show)
- [CreateAndShow](RayHelper.md#createandshow)

## Constructors

### constructor

• **new RayHelper**(`ray`)

Instantiate a new ray helper.
As raycast might be hard to debug, the RayHelper can help rendering the different rays
in order to better appreciate the issue one might have.

**`See`**

https://doc.babylonjs.com/babylon101/raycasts#debugging

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | Defines the ray we are currently tryin to visualize |

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:56

## Properties

### \_attachedToMesh

• `Private` **\_attachedToMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:30

___

### \_meshSpaceDirection

• `Private` **\_meshSpaceDirection**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:31

___

### \_meshSpaceOrigin

• `Private` **\_meshSpaceOrigin**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:32

___

### \_onAfterRenderObserver

• `Private` **\_onAfterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:28

___

### \_onAfterStepObserver

• `Private` **\_onAfterStepObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:29

___

### \_renderFunction

• `Private` **\_renderFunction**: [`Nullable`](../modules.md#nullable)() => `void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:25

___

### \_renderLine

• `Private` **\_renderLine**: [`Nullable`](../modules.md#nullable)[`LinesMesh`](LinesMesh.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:24

___

### \_renderPoints

• `Private` **\_renderPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:23

___

### \_scene

• `Private` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:26

___

### ray

• **ray**: [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md)

Defines the ray we are currently tryin to visualize.

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:21

## Methods

### \_render

▸ `Private` **_render**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:102

___

### \_updateToMesh

▸ `Private` **_updateToMesh**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:199

___

### attachToMesh

▸ **attachToMesh**(`mesh`, `meshSpaceDirection?`, `meshSpaceOrigin?`, `length?`): `void`

Attach a ray helper to a mesh so that we can easily see its orientation for instance or information like its normals.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | Defines the mesh we want the helper attached to |
| `meshSpaceDirection?` | [`Vector3`](Vector3.md) | Defines the direction of the Ray in mesh space (local space of the mesh node) |
| `meshSpaceOrigin?` | [`Vector3`](Vector3.md) | Defines the origin of the Ray in mesh space (local space of the mesh node) |
| `length?` | `number` | Defines the length of the ray |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:130

___

### detachFromMesh

▸ **detachFromMesh**(): `void`

Detach the ray helper from the mesh it has previously been attached to.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:186

___

### dispose

▸ **dispose**(): `void`

Dispose the helper and release its associated resources.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:218

___

### hide

▸ **hide**(): `void`

Hides the ray we are debugging.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:88

___

### show

▸ **show**(`scene`, `color?`): `void`

Shows the ray we are willing to debug.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene the ray needs to be rendered in |
| `color?` | [`Color3`](Color3.md) | Defines the color the ray needs to be rendered in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:65

___

### CreateAndShow

▸ `Static` **CreateAndShow**(`ray`, `scene`, `color`): [`RayHelper`](RayHelper.md)

Helper function to create a colored helper in a scene in one line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | Defines the ray we are currently tryin to visualize |
| `scene` | [`Scene`](Scene.md) | Defines the scene the ray is used in |
| `color` | [`Color3`](Color3.md) | Defines the color we want to see the ray in |

#### Returns

[`RayHelper`](RayHelper.md)

The newly created ray helper.

#### Defined in

packages/dev/core/src/Debug/rayHelper.ts:41

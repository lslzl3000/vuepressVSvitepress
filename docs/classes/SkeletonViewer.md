[@dev/core](../README.md) / [Exports](../modules.md) / SkeletonViewer

# Class: SkeletonViewer

Class used to render a debug view of a given skeleton

**`See`**

http://www.babylonjs-playground.com/#1BZJVJ#8

## Table of contents

### Constructors

- [constructor](SkeletonViewer.md#constructor)

### Properties

- [\_boneIndices](SkeletonViewer.md#_boneindices)
- [\_debugLines](SkeletonViewer.md#_debuglines)
- [\_debugMesh](SkeletonViewer.md#_debugmesh)
- [\_isEnabled](SkeletonViewer.md#_isenabled)
- [\_localAxes](SkeletonViewer.md#_localaxes)
- [\_obs](SkeletonViewer.md#_obs)
- [\_ready](SkeletonViewer.md#_ready)
- [\_scene](SkeletonViewer.md#_scene)
- [\_utilityLayer](SkeletonViewer.md#_utilitylayer)
- [autoUpdateBonesMatrices](SkeletonViewer.md#autoupdatebonesmatrices)
- [color](SkeletonViewer.md#color)
- [mesh](SkeletonViewer.md#mesh)
- [options](SkeletonViewer.md#options)
- [renderingGroupId](SkeletonViewer.md#renderinggroupid)
- [skeleton](SkeletonViewer.md#skeleton)
- [DISPLAY\_LINES](SkeletonViewer.md#display_lines)
- [DISPLAY\_SPHERES](SkeletonViewer.md#display_spheres)
- [DISPLAY\_SPHERE\_AND\_SPURS](SkeletonViewer.md#display_sphere_and_spurs)

### Accessors

- [debugMesh](SkeletonViewer.md#debugmesh)
- [displayMode](SkeletonViewer.md#displaymode)
- [isEnabled](SkeletonViewer.md#isenabled)
- [isReady](SkeletonViewer.md#isready)
- [ready](SkeletonViewer.md#ready)
- [scene](SkeletonViewer.md#scene)
- [utilityLayer](SkeletonViewer.md#utilitylayer)

### Methods

- [\_bindObs](SkeletonViewer.md#_bindobs)
- [\_buildLocalAxes](SkeletonViewer.md#_buildlocalaxes)
- [\_buildSpheresAndSpurs](SkeletonViewer.md#_buildspheresandspurs)
- [\_displayLinesUpdate](SkeletonViewer.md#_displaylinesupdate)
- [\_getAbsoluteBindPoseToRef](SkeletonViewer.md#_getabsolutebindposetoref)
- [\_getBonePosition](SkeletonViewer.md#_getboneposition)
- [\_getLinesForBonesNoLength](SkeletonViewer.md#_getlinesforbonesnolength)
- [\_getLinesForBonesWithLength](SkeletonViewer.md#_getlinesforboneswithlength)
- [\_revert](SkeletonViewer.md#_revert)
- [changeDisplayMode](SkeletonViewer.md#changedisplaymode)
- [changeDisplayOptions](SkeletonViewer.md#changedisplayoptions)
- [dispose](SkeletonViewer.md#dispose)
- [update](SkeletonViewer.md#update)
- [CreateBoneWeightShader](SkeletonViewer.md#createboneweightshader)
- [CreateSkeletonMapShader](SkeletonViewer.md#createskeletonmapshader)
- [\_CreateBoneMapColorBuffer](SkeletonViewer.md#_createbonemapcolorbuffer)

## Constructors

### constructor

• **new SkeletonViewer**(`skeleton`, `mesh`, `scene`, `autoUpdateBonesMatrices?`, `renderingGroupId?`, `options?`)

Creates a new SkeletonViewer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `skeleton` | [`Skeleton`](Skeleton.md) | `undefined` | defines the skeleton to render |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh attached to the skeleton |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `autoUpdateBonesMatrices` | `boolean` | `true` | defines a boolean indicating if bones matrices must be forced to update before rendering (true by default) |
| `renderingGroupId` | `number` | `3` | defines the rendering group id to use with the viewer |
| `options` | `Partial`[`ISkeletonViewerOptions`](../interfaces/ISkeletonViewerOptions.md) | `{}` | All of the extra constructor options for the SkeletonViewer |

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:387

## Properties

### \_boneIndices

• `Private` **\_boneIndices**: `Set``number`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:341

___

### \_debugLines

• `Private` **\_debugLines**: [`Vector3`](Vector3.md)[][]

Array of the points of the skeleton fo the line view.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:321

___

### \_debugMesh

• `Private` **\_debugMesh**: [`Nullable`](../modules.md#nullable)[`LinesMesh`](LinesMesh.md)

The SkeletonViewers Mesh.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:324

___

### \_isEnabled

• `Private` **\_isEnabled**: `boolean` = `true`

If SkeletonViewer is enabled.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:330

___

### \_localAxes

• `Private` **\_localAxes**: [`Nullable`](../modules.md#nullable)[`LinesMesh`](LinesMesh.md) = `null`

The local axes Meshes.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:327

___

### \_obs

• `Private` **\_obs**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

SkeletonViewer render observable.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:336

___

### \_ready

• `Private` **\_ready**: `boolean`

If SkeletonViewer is ready.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:333

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

If SkeletonViewer scene scope.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:315

___

### \_utilityLayer

• `Private` **\_utilityLayer**: [`Nullable`](../modules.md#nullable)[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

The Utility Layer to render the gizmos in.

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:339

___

### autoUpdateBonesMatrices

• **autoUpdateBonesMatrices**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:395

___

### color

• **color**: [`Color3`](Color3.md)

Gets or sets the color used to render the skeleton

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:318

___

### mesh

• **mesh**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:391

___

### options

• **options**: `Partial`[`ISkeletonViewerOptions`](../interfaces/ISkeletonViewerOptions.md) = `{}`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:399

___

### renderingGroupId

• **renderingGroupId**: `number` = `3`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:397

___

### skeleton

• **skeleton**: [`Skeleton`](Skeleton.md)

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:389

___

### DISPLAY\_LINES

▪ `Static` `Readonly` **DISPLAY\_LINES**: ``0``

public Display constants BABYLON.SkeletonViewer.DISPLAY_LINES

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:30

___

### DISPLAY\_SPHERES

▪ `Static` `Readonly` **DISPLAY\_SPHERES**: ``1``

public Display constants BABYLON.SkeletonViewer.DISPLAY_SPHERES

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:32

___

### DISPLAY\_SPHERE\_AND\_SPURS

▪ `Static` `Readonly` **DISPLAY\_SPHERE\_AND\_SPURS**: ``2``

public Display constants BABYLON.SkeletonViewer.DISPLAY_SPHERE_AND_SPURS

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:34

## Accessors

### debugMesh

• `get` **debugMesh**(): ``null`` \| [`AbstractMesh`](AbstractMesh.md) \| [`LinesMesh`](LinesMesh.md)

Gets the debugMesh

#### Returns

``null`` \| [`AbstractMesh`](AbstractMesh.md) \| [`LinesMesh`](LinesMesh.md)

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:360

• `set` **debugMesh**(`value`): `void`

Sets the debugMesh

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | ``null`` \| [`AbstractMesh`](AbstractMesh.md) \| [`LinesMesh`](LinesMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:364

___

### displayMode

• `get` **displayMode**(): `number`

Gets the displayMode

#### Returns

`number`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:368

• `set` **displayMode**(`value`): `void`

Sets the displayMode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:372

___

### isEnabled

• `get` **isEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:503

• `set` **isEnabled**(`value`): `void`

Gets or sets a boolean indicating if the viewer is enabled

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:484

___

### isReady

• `get` **isReady**(): `Boolean`

Checks Ready Status.

#### Returns

`Boolean`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:352

___

### ready

• `set` **ready**(`value`): `void`

Sets Ready Status.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:356

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets the Scene.

#### Returns

[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:344

___

### utilityLayer

• `get` **utilityLayer**(): [`Nullable`](../modules.md#nullable)[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

Gets the utilityLayer.

#### Returns

[`Nullable`](../modules.md#nullable)[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:348

## Methods

### \_bindObs

▸ `Private` **_bindObs**(): `void`

The Dynamic bindings for the update functions

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:452

___

### \_buildLocalAxes

▸ `Private` **_buildLocalAxes**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:794

___

### \_buildSpheresAndSpurs

▸ `Private` **_buildSpheresAndSpurs**(`spheresOnly?`): `void`

function to build and bind sphere joint points and spur bone representations.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `spheresOnly` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:611

___

### \_displayLinesUpdate

▸ `Private` **_displayLinesUpdate**(): `void`

Update the viewer to sync with current skeleton state, only used for the line display.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:869

___

### \_getAbsoluteBindPoseToRef

▸ `Private` **_getAbsoluteBindPoseToRef**(`bone`, `matrix`): `void`

function to get the absolute bind pose of a bone by accumulating transformations up the bone hierarchy.

#### Parameters

| Name | Type |
| :------ | :------ |
| `bone` | [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md) |
| `matrix` | [`Matrix`](Matrix.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:596

___

### \_getBonePosition

▸ `Private` **_getBonePosition**(`position`, `bone`, `meshMat`, `x?`, `y?`, `z?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` |
| `bone` | [`Bone`](Bone.md) | `undefined` |
| `meshMat` | [`Matrix`](Matrix.md) | `undefined` |
| `x` | `number` | `0` |
| `y` | `number` | `0` |
| `z` | `number` | `0` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:507

___

### \_getLinesForBonesNoLength

▸ `Private` **_getLinesForBonesNoLength**(`bones`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `bones` | [`Bone`](Bone.md)[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:555

___

### \_getLinesForBonesWithLength

▸ `Private` **_getLinesForBonesWithLength**(`bones`, `meshMat`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `bones` | [`Bone`](Bone.md)[] |
| `meshMat` | [`Matrix`](Matrix.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:530

___

### \_revert

▸ `Private` **_revert**(`animationState`): `void`

function to revert the mesh and scene back to the initial state.

#### Parameters

| Name | Type |
| :------ | :------ |
| `animationState` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:584

___

### changeDisplayMode

▸ **changeDisplayMode**(`mode`): `void`

Changes the displayMode of the skeleton viewer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mode` | `number` | The displayMode numerical value |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:900

___

### changeDisplayOptions

▸ **changeDisplayOptions**(`option`, `value`): `void`

Sets a display option of the skeleton viewer

| Option           | Type    | Default | Description |
| ---------------- | ------- | ------- | ----------- |
| midStep          | float   | 0.235   | A percentage between a bone and its child that determines the widest part of a spur. Only used when `displayMode` is set to `DISPLAY_SPHERE_AND_SPURS`. |
| midStepFactor    | float   | 0.15    | Mid step width expressed as a factor of the length. A value of 0.5 makes the spur width half of the spur length. Only used when `displayMode` is set to `DISPLAY_SPHERE_AND_SPURS`. |
| sphereBaseSize   | float   | 2       | Sphere base size. Only used when `displayMode` is set to `DISPLAY_SPHERE_AND_SPURS`. |
| sphereScaleUnit  | float   | 0.865   | Sphere scale factor used to scale spheres in relation to the longest bone. Only used when `displayMode` is set to `DISPLAY_SPHERE_AND_SPURS`. |
| spurFollowsChild | boolean | false   | Whether a spur should attach its far end to the child bone. |
| showLocalAxes    | boolean | false   | Displays local axes on all bones. |
| localAxesSize    | float   | 0.075   | Determines the length of each local axis. |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `option` | `string` | String of the option name |
| `value` | `number` | The numerical option value |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:932

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:947

___

### update

▸ **update**(): `void`

Update the viewer to sync with current skeleton state, only used to manually update.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:464

___

### CreateBoneWeightShader

▸ `Static` **CreateBoneWeightShader**(`options`, `scene`): [`ShaderMaterial`](ShaderMaterial.md)

public static method to create a BoneWeight Shader

**`See`**

http://www.babylonjs-playground.com/#1BZJVJ#395

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IBoneWeightShaderOptions`](../interfaces/IBoneWeightShaderOptions.md) | The constructor options |
| `scene` | [`Scene`](Scene.md) | The scene that the shader is scoped to |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

The created ShaderMaterial

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:42

___

### CreateSkeletonMapShader

▸ `Static` **CreateSkeletonMapShader**(`options`, `scene`): [`ShaderMaterial`](ShaderMaterial.md)

public static method to create a BoneWeight Shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ISkeletonMapShaderOptions`](../interfaces/ISkeletonMapShaderOptions.md) | The constructor options |
| `scene` | [`Scene`](Scene.md) | The scene that the shader is scoped to |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

The created ShaderMaterial

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:169

___

### \_CreateBoneMapColorBuffer

▸ `Static` `Private` **_CreateBoneMapColorBuffer**(`size`, `colorMap`, `scene`): `number`[]

private static method to create a BoneWeight Shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | The size of the buffer to create (usually the bone count) |
| `colorMap` | [`ISkeletonMapShaderColorMapKnot`](../interfaces/ISkeletonMapShaderColorMapKnot.md)[] | The gradient data to generate |
| `scene` | [`Scene`](Scene.md) | The scene that the shader is scoped to |

#### Returns

`number`[]

an Array of floats from the color gradient values

#### Defined in

packages/dev/core/src/Debug/skeletonViewer.ts:292

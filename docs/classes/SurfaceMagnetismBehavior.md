[@dev/core](../README.md) / [Exports](../modules.md) / SurfaceMagnetismBehavior

# Class: SurfaceMagnetismBehavior

A behavior that allows a transform node to stick to a surface position/orientation

**`Since`**

5.0.0

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`Mesh`](Mesh.md)

## Table of contents

### Constructors

- [constructor](SurfaceMagnetismBehavior.md#constructor)

### Properties

- [\_attachPointLocalOffset](SurfaceMagnetismBehavior.md#_attachpointlocaloffset)
- [\_attachedMesh](SurfaceMagnetismBehavior.md#_attachedmesh)
- [\_hit](SurfaceMagnetismBehavior.md#_hit)
- [\_lastTick](SurfaceMagnetismBehavior.md#_lasttick)
- [\_onBeforeRender](SurfaceMagnetismBehavior.md#_onbeforerender)
- [\_pointerObserver](SurfaceMagnetismBehavior.md#_pointerobserver)
- [\_scene](SurfaceMagnetismBehavior.md#_scene)
- [\_workingPosition](SurfaceMagnetismBehavior.md#_workingposition)
- [\_workingQuaternion](SurfaceMagnetismBehavior.md#_workingquaternion)
- [enabled](SurfaceMagnetismBehavior.md#enabled)
- [hitNormalOffset](SurfaceMagnetismBehavior.md#hitnormaloffset)
- [interpolatePose](SurfaceMagnetismBehavior.md#interpolatepose)
- [keepOrientationVertical](SurfaceMagnetismBehavior.md#keeporientationvertical)
- [lerpTime](SurfaceMagnetismBehavior.md#lerptime)
- [maxStickingDistance](SurfaceMagnetismBehavior.md#maxstickingdistance)
- [meshes](SurfaceMagnetismBehavior.md#meshes)

### Accessors

- [name](SurfaceMagnetismBehavior.md#name)

### Methods

- [\_addObservables](SurfaceMagnetismBehavior.md#_addobservables)
- [\_getAttachPointOffsetToRef](SurfaceMagnetismBehavior.md#_getattachpointoffsettoref)
- [\_getTargetPose](SurfaceMagnetismBehavior.md#_gettargetpose)
- [\_removeObservables](SurfaceMagnetismBehavior.md#_removeobservables)
- [\_updateTransformToGoal](SurfaceMagnetismBehavior.md#_updatetransformtogoal)
- [attach](SurfaceMagnetismBehavior.md#attach)
- [detach](SurfaceMagnetismBehavior.md#detach)
- [findAndUpdateTarget](SurfaceMagnetismBehavior.md#findandupdatetarget)
- [init](SurfaceMagnetismBehavior.md#init)
- [updateAttachPoint](SurfaceMagnetismBehavior.md#updateattachpoint)

## Constructors

### constructor

• **new SurfaceMagnetismBehavior**()

## Properties

### \_attachPointLocalOffset

• `Private` **\_attachPointLocalOffset**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:19

___

### \_attachedMesh

• `Private` **\_attachedMesh**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:18

___

### \_hit

• `Private` **\_hit**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:25

___

### \_lastTick

• `Private` **\_lastTick**: `number` = `-1`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:23

___

### \_onBeforeRender

• `Private` **\_onBeforeRender**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:24

___

### \_pointerObserver

• `Private` **\_pointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:20

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:17

___

### \_workingPosition

• `Private` **\_workingPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:21

___

### \_workingQuaternion

• `Private` **\_workingQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:22

___

### enabled

• **enabled**: `boolean` = `true`

Is this behavior reacting to pointer events

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:68

___

### hitNormalOffset

• **hitNormalOffset**: `number` = `0.05`

Distance offset from the hit point to place the target at, along the hit normal.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:30

___

### interpolatePose

• **interpolatePose**: `boolean` = `true`

Set to false if the node should strictly follow the camera without any interpolation time

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:52

___

### keepOrientationVertical

• **keepOrientationVertical**: `boolean` = `true`

If true, pitch and roll are omitted.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:63

___

### lerpTime

• **lerpTime**: `number` = `250`

Rate of interpolation of position and rotation of the attached node.
Higher values will give a slower interpolation.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:58

___

### maxStickingDistance

• **maxStickingDistance**: `number` = `0.8`

Maximum distance for the node to stick to the surface

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:73

___

### meshes

• **meshes**: [`AbstractMesh`](AbstractMesh.md)[] = `[]`

Spatial mapping meshes to collide with

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:42

## Accessors

### name

• `get` **name**(): `string`

Name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:35

## Methods

### \_addObservables

▸ `Private` **_addObservables**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:224

___

### \_getAttachPointOffsetToRef

▸ `Private` **_getAttachPointOffsetToRef**(`ref`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ref` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:172

___

### \_getTargetPose

▸ `Private` **_getTargetPose**(`pickingInfo`): [`Nullable`](../modules.md#nullable){ `position`: [`Vector3`](Vector3.md) ; `quaternion`: [`Quaternion`](Quaternion.md)  }

#### Parameters

| Name | Type |
| :------ | :------ |
| `pickingInfo` | [`PickingInfo`](PickingInfo.md) |

#### Returns

[`Nullable`](../modules.md#nullable){ `position`: [`Vector3`](Vector3.md) ; `quaternion`: [`Quaternion`](Quaternion.md)  }

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:101

___

### \_removeObservables

▸ `Private` **_removeObservables**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:239

___

### \_updateTransformToGoal

▸ `Private` **_updateTransformToGoal**(`elapsed`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `elapsed` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:194

___

### attach

▸ **attach**(`target`, `scene?`): `void`

Attaches the behavior to a transform node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Mesh`](Mesh.md) | defines the target where the behavior is attached to |
| `scene?` | [`Scene`](Scene.md) | the scene |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:80

___

### detach

▸ **detach**(): `void`

Detaches the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:96

___

### findAndUpdateTarget

▸ **findAndUpdateTarget**(`pickInfo`): `boolean`

Finds the intersection point of the given ray onto the meshes and updates the target.
Transformation will be interpolated according to `interpolatePose` and `lerpTime` properties.
If no mesh of `meshes` are hit, this does nothing.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) | The input pickingInfo that will be used to intersect the meshes |

#### Returns

`boolean`

a boolean indicating if we found a hit to stick to

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:152

___

### init

▸ **init**(): `void`

Function called when the behavior needs to be initialized (after attaching it to a target)

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:47

___

### updateAttachPoint

▸ **updateAttachPoint**(): `void`

Updates the attach point with the current geometry extents of the attached mesh

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/surfaceMagnetismBehavior.ts:141

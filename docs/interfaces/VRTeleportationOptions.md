[@dev/core](../README.md) / [Exports](../modules.md) / VRTeleportationOptions

# Interface: VRTeleportationOptions

Options to modify the vr teleportation behavior.

## Table of contents

### Properties

- [easingFunction](VRTeleportationOptions.md#easingfunction)
- [floorMeshName](VRTeleportationOptions.md#floormeshname)
- [floorMeshes](VRTeleportationOptions.md#floormeshes)
- [teleportationMode](VRTeleportationOptions.md#teleportationmode)
- [teleportationSpeed](VRTeleportationOptions.md#teleportationspeed)
- [teleportationTime](VRTeleportationOptions.md#teleportationtime)

## Properties

### easingFunction

• `Optional` **easingFunction**: [`EasingFunction`](../classes/EasingFunction.md)

The easing function used in the animation or null for Linear. (default CircleEase)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:73

___

### floorMeshName

• `Optional` **floorMeshName**: `string`

The name of the mesh which should be used as the teleportation floor. (default: null)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:53

___

### floorMeshes

• `Optional` **floorMeshes**: [`Mesh`](../classes/Mesh.md)[]

A list of meshes to be used as the teleportation floor. (default: empty)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:57

___

### teleportationMode

• `Optional` **teleportationMode**: `number`

The teleportation mode. (default: TELEPORTATIONMODE_CONSTANTTIME)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:61

___

### teleportationSpeed

• `Optional` **teleportationSpeed**: `number`

The speed of the animation in distance/sec, apply when animationMode is TELEPORTATIONMODE_CONSTANTSPEED. (default 20 units / sec)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:69

___

### teleportationTime

• `Optional` **teleportationTime**: `number`

The duration of the animation in ms, apply when animationMode is TELEPORTATIONMODE_CONSTANTTIME. (default 122ms)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:65

[@dev/core](../README.md) / [Exports](../modules.md) / IEnvironmentHelperOptions

# Interface: IEnvironmentHelperOptions

Represents the different options available during the creation of
a Environment helper.

This can control the default ground, skybox and image processing setup of your scene.

## Table of contents

### Properties

- [backgroundYRotation](IEnvironmentHelperOptions.md#backgroundyrotation)
- [cameraContrast](IEnvironmentHelperOptions.md#cameracontrast)
- [cameraExposure](IEnvironmentHelperOptions.md#cameraexposure)
- [createGround](IEnvironmentHelperOptions.md#createground)
- [createSkybox](IEnvironmentHelperOptions.md#createskybox)
- [enableGroundMirror](IEnvironmentHelperOptions.md#enablegroundmirror)
- [enableGroundShadow](IEnvironmentHelperOptions.md#enablegroundshadow)
- [environmentTexture](IEnvironmentHelperOptions.md#environmenttexture)
- [groundColor](IEnvironmentHelperOptions.md#groundcolor)
- [groundMirrorAmount](IEnvironmentHelperOptions.md#groundmirroramount)
- [groundMirrorBlurKernel](IEnvironmentHelperOptions.md#groundmirrorblurkernel)
- [groundMirrorFallOffDistance](IEnvironmentHelperOptions.md#groundmirrorfalloffdistance)
- [groundMirrorFresnelWeight](IEnvironmentHelperOptions.md#groundmirrorfresnelweight)
- [groundMirrorSizeRatio](IEnvironmentHelperOptions.md#groundmirrorsizeratio)
- [groundMirrorTextureType](IEnvironmentHelperOptions.md#groundmirrortexturetype)
- [groundOpacity](IEnvironmentHelperOptions.md#groundopacity)
- [groundShadowLevel](IEnvironmentHelperOptions.md#groundshadowlevel)
- [groundSize](IEnvironmentHelperOptions.md#groundsize)
- [groundTexture](IEnvironmentHelperOptions.md#groundtexture)
- [groundYBias](IEnvironmentHelperOptions.md#groundybias)
- [rootPosition](IEnvironmentHelperOptions.md#rootposition)
- [setupImageProcessing](IEnvironmentHelperOptions.md#setupimageprocessing)
- [sizeAuto](IEnvironmentHelperOptions.md#sizeauto)
- [skyboxColor](IEnvironmentHelperOptions.md#skyboxcolor)
- [skyboxSize](IEnvironmentHelperOptions.md#skyboxsize)
- [skyboxTexture](IEnvironmentHelperOptions.md#skyboxtexture)
- [toneMappingEnabled](IEnvironmentHelperOptions.md#tonemappingenabled)

## Properties

### backgroundYRotation

• **backgroundYRotation**: `number`

The background rotation around the Y axis of the scene.
This helps aligning the key lights of your scene with the background.
0 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:136

___

### cameraContrast

• **cameraContrast**: `number`

The value of the contrast to apply to the scene.
1.6 by default if setupImageProcessing is true.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:172

___

### cameraExposure

• **cameraExposure**: `number`

The value of the exposure to apply to the scene.
0.6 by default if setupImageProcessing is true.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:166

___

### createGround

• **createGround**: `boolean`

Specifies whether or not to create a ground.
True by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:31

___

### createSkybox

• **createSkybox**: `boolean`

Specifies whether or not to create a skybox.
True by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:112

___

### enableGroundMirror

• **enableGroundMirror**: `boolean`

Creates a mirror texture attach to the ground.
false by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:68

___

### enableGroundShadow

• **enableGroundShadow**: `boolean`

Enables the ground to receive shadows.
True by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:58

___

### environmentTexture

• **environmentTexture**: `string` \| [`BaseTexture`](../classes/BaseTexture.md)

The texture used as your environment texture in the scene.
Comes from the BabylonJS CDN by default and in use if setupImageProcessing is true.

Remarks: Can be either a texture or a url.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:160

___

### groundColor

• **groundColor**: [`Color3`](../classes/Color3.md)

The color mixed in the ground texture by default.
BabylonJS clearColor by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:48

___

### groundMirrorAmount

• **groundMirrorAmount**: `number`

Specifies the ground mirror visibility amount.
1 by default

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:83

___

### groundMirrorBlurKernel

• **groundMirrorBlurKernel**: `number`

Specifies the ground mirror blur kernel size.
64 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:78

___

### groundMirrorFallOffDistance

• **groundMirrorFallOffDistance**: `number`

Specifies the ground mirror Falloff distance.
This can helps reducing the size of the reflection.
0 by Default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:96

___

### groundMirrorFresnelWeight

• **groundMirrorFresnelWeight**: `number`

Specifies the ground mirror reflectance weight.
This uses the standard weight of the background material to setup the fresnel effect
of the mirror.
1 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:90

___

### groundMirrorSizeRatio

• **groundMirrorSizeRatio**: `number`

Specifies the ground mirror size ratio.
0.3 by default as the default kernel is 64.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:73

___

### groundMirrorTextureType

• **groundMirrorTextureType**: `number`

Specifies the ground mirror texture type.
Unsigned Int by Default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:101

___

### groundOpacity

• **groundOpacity**: `number`

Specifies the ground opacity.
1 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:53

___

### groundShadowLevel

• **groundShadowLevel**: `number`

Helps preventing the shadow to be fully black on the ground.
0.5 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:63

___

### groundSize

• **groundSize**: `number`

Specifies the ground size.
15 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:36

___

### groundTexture

• **groundTexture**: `string` \| [`BaseTexture`](../classes/BaseTexture.md)

The texture used on the ground for the main color.
Comes from the BabylonJS CDN by default.

Remarks: Can be either a texture or a url.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:43

___

### groundYBias

• **groundYBias**: `number`

Specifies a bias applied to the ground vertical position to prevent z-fighting with
the shown objects.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:106

___

### rootPosition

• **rootPosition**: [`Vector3`](../classes/Vector3.md)

Default position of the rootMesh if autoSize is not true.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:146

___

### setupImageProcessing

• **setupImageProcessing**: `boolean`

Sets up the image processing in the scene.
true by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:152

___

### sizeAuto

• **sizeAuto**: `boolean`

Compute automatically the size of the elements to best fit with the scene.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:141

___

### skyboxColor

• **skyboxColor**: [`Color3`](../classes/Color3.md)

The color mixed in the skybox texture by default.
BabylonJS clearColor by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:129

___

### skyboxSize

• **skyboxSize**: `number`

Specifies the skybox size.
20 by default.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:117

___

### skyboxTexture

• **skyboxTexture**: `string` \| [`BaseTexture`](../classes/BaseTexture.md)

The texture used on the skybox for the main color.
Comes from the BabylonJS CDN by default.

Remarks: Can be either a texture or a url.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:124

___

### toneMappingEnabled

• **toneMappingEnabled**: `boolean`

Specifies whether or not tonemapping should be enabled in the scene.
true by default if setupImageProcessing is true.

#### Defined in

https://github.com/babylon.js/core/src/Helpers/environmentHelper.ts:178

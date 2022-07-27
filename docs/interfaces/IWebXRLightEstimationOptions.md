[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRLightEstimationOptions

# Interface: IWebXRLightEstimationOptions

Options for Light Estimation feature

## Table of contents

### Properties

- [createDirectionalLightSource](IWebXRLightEstimationOptions.md#createdirectionallightsource)
- [cubeMapPollInterval](IWebXRLightEstimationOptions.md#cubemappollinterval)
- [disableCubeMapReflection](IWebXRLightEstimationOptions.md#disablecubemapreflection)
- [disableSphericalPolynomial](IWebXRLightEstimationOptions.md#disablesphericalpolynomial)
- [disableVectorReuse](IWebXRLightEstimationOptions.md#disablevectorreuse)
- [lightEstimationPollInterval](IWebXRLightEstimationOptions.md#lightestimationpollinterval)
- [reflectionFormat](IWebXRLightEstimationOptions.md#reflectionformat)
- [setSceneEnvironmentTexture](IWebXRLightEstimationOptions.md#setsceneenvironmenttexture)

## Properties

### createDirectionalLightSource

• `Optional` **createDirectionalLightSource**: `boolean`

Should a directional light source be created.
If created, this light source will be updated whenever the light estimation values change

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:44

___

### cubeMapPollInterval

• `Optional` **cubeMapPollInterval**: `number`

How often should the cubemap update in ms.
If not set the cubemap will be updated every time the underlying system updates the environment texture.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:34

___

### disableCubeMapReflection

• `Optional` **disableCubeMapReflection**: `boolean`

Disable the cube map reflection feature. In this case only light direction and color will be updated

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:24

___

### disableSphericalPolynomial

• `Optional` **disableSphericalPolynomial**: `boolean`

disable applying the spherical polynomial to the cube map texture

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:58

___

### disableVectorReuse

• `Optional` **disableVectorReuse**: `boolean`

Should the light estimation's needed vectors be constructed on each frame.
Use this when you use those vectors and don't want their values to change outside of the light estimation feature

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:53

___

### lightEstimationPollInterval

• `Optional` **lightEstimationPollInterval**: `number`

How often should the light estimation properties update in ms.
If not set the light estimation properties will be updated on every frame (depending on the underlying system)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:39

___

### reflectionFormat

• `Optional` **reflectionFormat**: `XRReflectionFormat`

Define the format to be used for the light estimation texture.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:48

___

### setSceneEnvironmentTexture

• `Optional` **setSceneEnvironmentTexture**: `boolean`

Should the scene's env texture be set to the cube map reflection texture
Note that this doesn't work is disableCubeMapReflection if set to false

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:29

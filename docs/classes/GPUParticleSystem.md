[@dev/core](../README.md) / [Exports](../modules.md) / GPUParticleSystem

# Class: GPUParticleSystem

This represents a GPU particle system in Babylon
This is the fastest particle system in Babylon as it uses the GPU to update the individual particle data

**`See`**

https://www.babylonjs-playground.com/#PU4WYI#4

## Hierarchy

- [`BaseParticleSystem`](BaseParticleSystem.md)

  ↳ **`GPUParticleSystem`**

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- [`IParticleSystem`](../interfaces/IParticleSystem.md)
- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](GPUParticleSystem.md#constructor)

### Properties

- [\_accumulatedCount](GPUParticleSystem.md#_accumulatedcount)
- [\_activeCount](GPUParticleSystem.md#_activecount)
- [\_actualFrame](GPUParticleSystem.md#_actualframe)
- [\_alphaRemapGradients](GPUParticleSystem.md#_alpharemapgradients)
- [\_angularSpeedGradients](GPUParticleSystem.md#_angularspeedgradients)
- [\_attributesStrideSize](GPUParticleSystem.md#_attributesstridesize)
- [\_buffer0](GPUParticleSystem.md#_buffer0)
- [\_buffer1](GPUParticleSystem.md#_buffer1)
- [\_cachedUpdateDefines](GPUParticleSystem.md#_cachedupdatedefines)
- [\_capacity](GPUParticleSystem.md#_capacity)
- [\_colorGradients](GPUParticleSystem.md#_colorgradients)
- [\_colorRemapGradients](GPUParticleSystem.md#_colorremapgradients)
- [\_currentActiveCount](GPUParticleSystem.md#_currentactivecount)
- [\_currentRenderId](GPUParticleSystem.md#_currentrenderid)
- [\_currentRenderingCameraUniqueId](GPUParticleSystem.md#_currentrenderingcamerauniqueid)
- [\_customWrappers](GPUParticleSystem.md#_customwrappers)
- [\_dragGradients](GPUParticleSystem.md#_draggradients)
- [\_drawWrappers](GPUParticleSystem.md#_drawwrappers)
- [\_emitRateGradients](GPUParticleSystem.md#_emitrategradients)
- [\_engine](GPUParticleSystem.md#_engine)
- [\_imageProcessingConfiguration](GPUParticleSystem.md#_imageprocessingconfiguration)
- [\_imageProcessingConfigurationDefines](GPUParticleSystem.md#_imageprocessingconfigurationdefines)
- [\_lifeTimeGradients](GPUParticleSystem.md#_lifetimegradients)
- [\_limitVelocityGradients](GPUParticleSystem.md#_limitvelocitygradients)
- [\_platform](GPUParticleSystem.md#_platform)
- [\_preWarmDone](GPUParticleSystem.md#_prewarmdone)
- [\_rampGradients](GPUParticleSystem.md#_rampgradients)
- [\_randomTextureSize](GPUParticleSystem.md#_randomtexturesize)
- [\_rawTextureWidth](GPUParticleSystem.md#_rawtexturewidth)
- [\_rootUrl](GPUParticleSystem.md#_rooturl)
- [\_scene](GPUParticleSystem.md#_scene)
- [\_sizeGradients](GPUParticleSystem.md#_sizegradients)
- [\_sourceBuffer](GPUParticleSystem.md#_sourcebuffer)
- [\_spriteBuffer](GPUParticleSystem.md#_spritebuffer)
- [\_startSizeGradients](GPUParticleSystem.md#_startsizegradients)
- [\_started](GPUParticleSystem.md#_started)
- [\_stopped](GPUParticleSystem.md#_stopped)
- [\_targetBuffer](GPUParticleSystem.md#_targetbuffer)
- [\_targetIndex](GPUParticleSystem.md#_targetindex)
- [\_timeDelta](GPUParticleSystem.md#_timedelta)
- [\_updateBuffer](GPUParticleSystem.md#_updatebuffer)
- [\_velocityGradients](GPUParticleSystem.md#_velocitygradients)
- [animations](GPUParticleSystem.md#animations)
- [beginAnimationFrom](GPUParticleSystem.md#beginanimationfrom)
- [beginAnimationLoop](GPUParticleSystem.md#beginanimationloop)
- [beginAnimationOnStart](GPUParticleSystem.md#beginanimationonstart)
- [beginAnimationTo](GPUParticleSystem.md#beginanimationto)
- [blendMode](GPUParticleSystem.md#blendmode)
- [color1](GPUParticleSystem.md#color1)
- [color2](GPUParticleSystem.md#color2)
- [colorDead](GPUParticleSystem.md#colordead)
- [customShader](GPUParticleSystem.md#customshader)
- [defaultProjectionMatrix](GPUParticleSystem.md#defaultprojectionmatrix)
- [disposeOnStop](GPUParticleSystem.md#disposeonstop)
- [emitRate](GPUParticleSystem.md#emitrate)
- [emitter](GPUParticleSystem.md#emitter)
- [endSpriteCellID](GPUParticleSystem.md#endspritecellid)
- [forceDepthWrite](GPUParticleSystem.md#forcedepthwrite)
- [gravity](GPUParticleSystem.md#gravity)
- [id](GPUParticleSystem.md#id)
- [isLocal](GPUParticleSystem.md#islocal)
- [layerMask](GPUParticleSystem.md#layermask)
- [limitVelocityDamping](GPUParticleSystem.md#limitvelocitydamping)
- [manualEmitCount](GPUParticleSystem.md#manualemitcount)
- [maxAngularSpeed](GPUParticleSystem.md#maxangularspeed)
- [maxEmitPower](GPUParticleSystem.md#maxemitpower)
- [maxInitialRotation](GPUParticleSystem.md#maxinitialrotation)
- [maxLifeTime](GPUParticleSystem.md#maxlifetime)
- [maxScaleX](GPUParticleSystem.md#maxscalex)
- [maxScaleY](GPUParticleSystem.md#maxscaley)
- [maxSize](GPUParticleSystem.md#maxsize)
- [minAngularSpeed](GPUParticleSystem.md#minangularspeed)
- [minEmitPower](GPUParticleSystem.md#minemitpower)
- [minInitialRotation](GPUParticleSystem.md#mininitialrotation)
- [minLifeTime](GPUParticleSystem.md#minlifetime)
- [minScaleX](GPUParticleSystem.md#minscalex)
- [minScaleY](GPUParticleSystem.md#minscaley)
- [minSize](GPUParticleSystem.md#minsize)
- [name](GPUParticleSystem.md#name)
- [noiseStrength](GPUParticleSystem.md#noisestrength)
- [onAnimationEnd](GPUParticleSystem.md#onanimationend)
- [onDisposeObservable](GPUParticleSystem.md#ondisposeobservable)
- [onStoppedObservable](GPUParticleSystem.md#onstoppedobservable)
- [particleEmitterType](GPUParticleSystem.md#particleemittertype)
- [particleTexture](GPUParticleSystem.md#particletexture)
- [preWarmCycles](GPUParticleSystem.md#prewarmcycles)
- [preWarmStepOffset](GPUParticleSystem.md#prewarmstepoffset)
- [preventAutoStart](GPUParticleSystem.md#preventautostart)
- [renderingGroupId](GPUParticleSystem.md#renderinggroupid)
- [snippetId](GPUParticleSystem.md#snippetid)
- [spriteCellChangeSpeed](GPUParticleSystem.md#spritecellchangespeed)
- [spriteCellHeight](GPUParticleSystem.md#spritecellheight)
- [spriteCellLoop](GPUParticleSystem.md#spritecellloop)
- [spriteCellWidth](GPUParticleSystem.md#spritecellwidth)
- [spriteRandomStartCell](GPUParticleSystem.md#spriterandomstartcell)
- [startDelay](GPUParticleSystem.md#startdelay)
- [startSpriteCellID](GPUParticleSystem.md#startspritecellid)
- [targetStopDuration](GPUParticleSystem.md#targetstopduration)
- [textureMask](GPUParticleSystem.md#texturemask)
- [translationPivot](GPUParticleSystem.md#translationpivot)
- [uniqueId](GPUParticleSystem.md#uniqueid)
- [updateSpeed](GPUParticleSystem.md#updatespeed)
- [worldOffset](GPUParticleSystem.md#worldoffset)
- [BLENDMODE\_ADD](GPUParticleSystem.md#blendmode_add)
- [BLENDMODE\_MULTIPLY](GPUParticleSystem.md#blendmode_multiply)
- [BLENDMODE\_MULTIPLYADD](GPUParticleSystem.md#blendmode_multiplyadd)
- [BLENDMODE\_ONEONE](GPUParticleSystem.md#blendmode_oneone)
- [BLENDMODE\_STANDARD](GPUParticleSystem.md#blendmode_standard)

### Accessors

- [activeParticleCount](GPUParticleSystem.md#activeparticlecount)
- [billboardMode](GPUParticleSystem.md#billboardmode)
- [direction1](GPUParticleSystem.md#direction1)
- [direction2](GPUParticleSystem.md#direction2)
- [imageProcessingConfiguration](GPUParticleSystem.md#imageprocessingconfiguration)
- [isAnimationSheetEnabled](GPUParticleSystem.md#isanimationsheetenabled)
- [isBillboardBased](GPUParticleSystem.md#isbillboardbased)
- [maxEmitBox](GPUParticleSystem.md#maxemitbox)
- [minEmitBox](GPUParticleSystem.md#minemitbox)
- [noiseTexture](GPUParticleSystem.md#noisetexture)
- [onBeforeDrawParticlesObservable](GPUParticleSystem.md#onbeforedrawparticlesobservable)
- [useRampGradients](GPUParticleSystem.md#userampgradients)
- [vertexShaderName](GPUParticleSystem.md#vertexshadername)
- [IsSupported](GPUParticleSystem.md#issupported)

### Methods

- [\_addFactorGradient](GPUParticleSystem.md#_addfactorgradient)
- [\_attachImageProcessingConfiguration](GPUParticleSystem.md#_attachimageprocessingconfiguration)
- [\_createAngularSpeedGradientTexture](GPUParticleSystem.md#_createangularspeedgradienttexture)
- [\_createColorGradientTexture](GPUParticleSystem.md#_createcolorgradienttexture)
- [\_createDragGradientTexture](GPUParticleSystem.md#_createdraggradienttexture)
- [\_createFactorGradientTexture](GPUParticleSystem.md#_createfactorgradienttexture)
- [\_createLimitVelocityGradientTexture](GPUParticleSystem.md#_createlimitvelocitygradienttexture)
- [\_createSizeGradientTexture](GPUParticleSystem.md#_createsizegradienttexture)
- [\_createVelocityGradientTexture](GPUParticleSystem.md#_createvelocitygradienttexture)
- [\_createVertexBuffers](GPUParticleSystem.md#_createvertexbuffers)
- [\_getCustomDrawWrapper](GPUParticleSystem.md#_getcustomdrawwrapper)
- [\_hasTargetStopDurationDependantGradient](GPUParticleSystem.md#_hastargetstopdurationdependantgradient)
- [\_initialize](GPUParticleSystem.md#_initialize)
- [\_refreshColorGradient](GPUParticleSystem.md#_refreshcolorgradient)
- [\_refreshFactorGradient](GPUParticleSystem.md#_refreshfactorgradient)
- [\_releaseBuffers](GPUParticleSystem.md#_releasebuffers)
- [\_removeGradientAndTexture](GPUParticleSystem.md#_removegradientandtexture)
- [\_render](GPUParticleSystem.md#_render)
- [\_reset](GPUParticleSystem.md#_reset)
- [addAlphaRemapGradient](GPUParticleSystem.md#addalpharemapgradient)
- [addAngularSpeedGradient](GPUParticleSystem.md#addangularspeedgradient)
- [addColorGradient](GPUParticleSystem.md#addcolorgradient)
- [addColorRemapGradient](GPUParticleSystem.md#addcolorremapgradient)
- [addDragGradient](GPUParticleSystem.md#adddraggradient)
- [addEmitRateGradient](GPUParticleSystem.md#addemitrategradient)
- [addLifeTimeGradient](GPUParticleSystem.md#addlifetimegradient)
- [addLimitVelocityGradient](GPUParticleSystem.md#addlimitvelocitygradient)
- [addRampGradient](GPUParticleSystem.md#addrampgradient)
- [addSizeGradient](GPUParticleSystem.md#addsizegradient)
- [addStartSizeGradient](GPUParticleSystem.md#addstartsizegradient)
- [addVelocityGradient](GPUParticleSystem.md#addvelocitygradient)
- [animate](GPUParticleSystem.md#animate)
- [clone](GPUParticleSystem.md#clone)
- [createBoxEmitter](GPUParticleSystem.md#createboxemitter)
- [createConeEmitter](GPUParticleSystem.md#createconeemitter)
- [createCylinderEmitter](GPUParticleSystem.md#createcylinderemitter)
- [createDirectedCylinderEmitter](GPUParticleSystem.md#createdirectedcylinderemitter)
- [createDirectedSphereEmitter](GPUParticleSystem.md#createdirectedsphereemitter)
- [createHemisphericEmitter](GPUParticleSystem.md#createhemisphericemitter)
- [createPointEmitter](GPUParticleSystem.md#createpointemitter)
- [createSphereEmitter](GPUParticleSystem.md#createsphereemitter)
- [dispose](GPUParticleSystem.md#dispose)
- [fillDefines](GPUParticleSystem.md#filldefines)
- [fillUniformsAttributesAndSamplerNames](GPUParticleSystem.md#filluniformsattributesandsamplernames)
- [forceRefreshGradients](GPUParticleSystem.md#forcerefreshgradients)
- [getActiveCount](GPUParticleSystem.md#getactivecount)
- [getAlphaRemapGradients](GPUParticleSystem.md#getalpharemapgradients)
- [getAngularSpeedGradients](GPUParticleSystem.md#getangularspeedgradients)
- [getCapacity](GPUParticleSystem.md#getcapacity)
- [getClassName](GPUParticleSystem.md#getclassname)
- [getColorGradients](GPUParticleSystem.md#getcolorgradients)
- [getColorRemapGradients](GPUParticleSystem.md#getcolorremapgradients)
- [getCustomEffect](GPUParticleSystem.md#getcustomeffect)
- [getDragGradients](GPUParticleSystem.md#getdraggradients)
- [getEmitRateGradients](GPUParticleSystem.md#getemitrategradients)
- [getLifeTimeGradients](GPUParticleSystem.md#getlifetimegradients)
- [getLimitVelocityGradients](GPUParticleSystem.md#getlimitvelocitygradients)
- [getRampGradients](GPUParticleSystem.md#getrampgradients)
- [getScene](GPUParticleSystem.md#getscene)
- [getSizeGradients](GPUParticleSystem.md#getsizegradients)
- [getStartSizeGradients](GPUParticleSystem.md#getstartsizegradients)
- [getVelocityGradients](GPUParticleSystem.md#getvelocitygradients)
- [isReady](GPUParticleSystem.md#isready)
- [isStarted](GPUParticleSystem.md#isstarted)
- [isStopped](GPUParticleSystem.md#isstopped)
- [isStopping](GPUParticleSystem.md#isstopping)
- [rebuild](GPUParticleSystem.md#rebuild)
- [removeAlphaRemapGradient](GPUParticleSystem.md#removealpharemapgradient)
- [removeAngularSpeedGradient](GPUParticleSystem.md#removeangularspeedgradient)
- [removeColorGradient](GPUParticleSystem.md#removecolorgradient)
- [removeColorRemapGradient](GPUParticleSystem.md#removecolorremapgradient)
- [removeDragGradient](GPUParticleSystem.md#removedraggradient)
- [removeEmitRateGradient](GPUParticleSystem.md#removeemitrategradient)
- [removeLifeTimeGradient](GPUParticleSystem.md#removelifetimegradient)
- [removeLimitVelocityGradient](GPUParticleSystem.md#removelimitvelocitygradient)
- [removeRampGradient](GPUParticleSystem.md#removerampgradient)
- [removeSizeGradient](GPUParticleSystem.md#removesizegradient)
- [removeStartSizeGradient](GPUParticleSystem.md#removestartsizegradient)
- [removeVelocityGradient](GPUParticleSystem.md#removevelocitygradient)
- [render](GPUParticleSystem.md#render)
- [reset](GPUParticleSystem.md#reset)
- [resetDrawCache](GPUParticleSystem.md#resetdrawcache)
- [serialize](GPUParticleSystem.md#serialize)
- [setCustomEffect](GPUParticleSystem.md#setcustomeffect)
- [start](GPUParticleSystem.md#start)
- [stop](GPUParticleSystem.md#stop)
- [Parse](GPUParticleSystem.md#parse)

## Constructors

### constructor

• **new GPUParticleSystem**(`name`, `options`, `sceneOrEngine`, `customEffect?`, `isAnimationSheetEnabled?`)

Instantiates a GPU particle system.
Particles are often small sprites used to simulate hard-to-reproduce phenomena like fire, smoke, water, or abstract visual effects like magic glitter and faery dust.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the particle system |
| `options` | `Partial`{ `capacity`: `number` ; `randomTextureSize`: `number`  } | `undefined` | The options used to create the system |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene the particle system belongs to or the engine to use if no scene |
| `customEffect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `null` | a custom effect used to change the way particles are rendered by default |
| `isAnimationSheetEnabled` | `boolean` | `false` | Must be true if using a spritesheet to animate the particles texture |

#### Overrides

[BaseParticleSystem](BaseParticleSystem.md).[constructor](BaseParticleSystem.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:733

## Properties

### \_accumulatedCount

• `Private` **\_accumulatedCount**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:53

___

### \_activeCount

• `Private` **\_activeCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:51

___

### \_actualFrame

• `Private` **\_actualFrame**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:80

___

### \_alphaRemapGradients

• `Protected` **\_alphaRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_alphaRemapGradients](BaseParticleSystem.md#_alpharemapgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:350

___

### \_angularSpeedGradients

• `Protected` **\_angularSpeedGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_angularSpeedGradients](BaseParticleSystem.md#_angularspeedgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:342

___

### \_attributesStrideSize

• `Private` **\_attributesStrideSize**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:76

___

### \_buffer0

• `Private` **\_buffer0**: [`Buffer`](Buffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:56

___

### \_buffer1

• `Private` **\_buffer1**: [`Buffer`](Buffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:57

___

### \_cachedUpdateDefines

• `Private` **\_cachedUpdateDefines**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:77

___

### \_capacity

• `Private` **\_capacity**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:50

___

### \_colorGradients

• `Protected` **\_colorGradients**: [`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_colorGradients](BaseParticleSystem.md#_colorgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:339

___

### \_colorRemapGradients

• `Protected` **\_colorRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_colorRemapGradients](BaseParticleSystem.md#_colorremapgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:349

___

### \_currentActiveCount

• `Private` **\_currentActiveCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:52

___

### \_currentRenderId

• `Private` **\_currentRenderId**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:64

___

### \_currentRenderingCameraUniqueId

• `Private` **\_currentRenderingCameraUniqueId**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:65

___

### \_customWrappers

• `Private` **\_customWrappers**: `Object`

#### Index signature

▪ [blendMode: `number`]: [`Nullable`](../modules.md#nullable)`DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:82

___

### \_dragGradients

• `Protected` **\_dragGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_dragGradients](BaseParticleSystem.md#_draggradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:345

___

### \_drawWrappers

• `Private` **\_drawWrappers**: `Object`

#### Index signature

▪ [blendMode: `number`]: `DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:81

___

### \_emitRateGradients

• `Protected` **\_emitRateGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_emitRateGradients](BaseParticleSystem.md#_emitrategradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:346

___

### \_engine

• `Protected` **\_engine**: [`ThinEngine`](ThinEngine.md)

The engine the particle system belongs to.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_engine](BaseParticleSystem.md#_engine)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:611

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the standard Material.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_imageProcessingConfiguration](BaseParticleSystem.md#_imageprocessingconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:621

___

### \_imageProcessingConfigurationDefines

• `Protected` **\_imageProcessingConfigurationDefines**: `ImageProcessingConfigurationDefines`

Local cache of defines for image processing.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_imageProcessingConfigurationDefines](BaseParticleSystem.md#_imageprocessingconfigurationdefines)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:616

___

### \_lifeTimeGradients

• `Protected` **\_lifeTimeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_lifeTimeGradients](BaseParticleSystem.md#_lifetimegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:341

___

### \_limitVelocityGradients

• `Protected` **\_limitVelocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_limitVelocityGradients](BaseParticleSystem.md#_limitvelocitygradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:344

___

### \_platform

• `Private` **\_platform**: `IGPUParticleSystemPlatform`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:86

___

### \_preWarmDone

• `Private` **\_preWarmDone**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:134

___

### \_rampGradients

• `Protected` **\_rampGradients**: [`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_rampGradients](BaseParticleSystem.md#_rampgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:348

___

### \_randomTextureSize

• `Private` **\_randomTextureSize**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:79

___

### \_rawTextureWidth

• `Private` `Readonly` **\_rawTextureWidth**: ``256``

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:84

___

### \_rootUrl

• `Protected` **\_rootUrl**: `string` = `""`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_rootUrl](BaseParticleSystem.md#_rooturl)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:205

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

The scene the particle system belongs to.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_scene](BaseParticleSystem.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:606

___

### \_sizeGradients

• `Protected` **\_sizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_sizeGradients](BaseParticleSystem.md#_sizegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:340

___

### \_sourceBuffer

• `Private` **\_sourceBuffer**: [`Buffer`](Buffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:61

___

### \_spriteBuffer

• `Private` **\_spriteBuffer**: [`Buffer`](Buffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:58

___

### \_startSizeGradients

• `Protected` **\_startSizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_startSizeGradients](BaseParticleSystem.md#_startsizegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:347

___

### \_started

• `Private` **\_started**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:66

___

### \_stopped

• `Private` **\_stopped**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:67

___

### \_targetBuffer

• `Private` **\_targetBuffer**: [`Buffer`](Buffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:62

___

### \_targetIndex

• `Private` **\_targetIndex**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:60

___

### \_timeDelta

• `Private` **\_timeDelta**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:69

___

### \_updateBuffer

• `Private` **\_updateBuffer**: `UniformBufferEffectCommonAccessor`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:54

___

### \_velocityGradients

• `Protected` **\_velocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_velocityGradients](BaseParticleSystem.md#_velocitygradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:343

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

List of animations used by the particle system.

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[animations](BaseParticleSystem.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:63

___

### beginAnimationFrom

• **beginAnimationFrom**: `number` = `0`

Gets or sets the frame to start the animation from when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationFrom](../interfaces/IParticleSystem.md#beginanimationfrom)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationFrom](BaseParticleSystem.md#beginanimationfrom)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:292

___

### beginAnimationLoop

• **beginAnimationLoop**: `boolean` = `false`

Gets or sets a boolean indicating if animations must loop when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationLoop](../interfaces/IParticleSystem.md#beginanimationloop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationLoop](BaseParticleSystem.md#beginanimationloop)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:302

___

### beginAnimationOnStart

• **beginAnimationOnStart**: `boolean` = `false`

Gets or sets a boolean indicating that hosted animations (in the system.animations array) must be started when system.start() is called

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationOnStart](../interfaces/IParticleSystem.md#beginanimationonstart)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationOnStart](BaseParticleSystem.md#beginanimationonstart)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:287

___

### beginAnimationTo

• **beginAnimationTo**: `number` = `60`

Gets or sets the frame to end the animation on when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationTo](../interfaces/IParticleSystem.md#beginanimationto)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationTo](BaseParticleSystem.md#beginanimationto)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:297

___

### blendMode

• **blendMode**: `number` = `BaseParticleSystem.BLENDMODE_ONEONE`

Blend mode use to render the particle, it can be either ParticleSystem.BLENDMODE_ONEONE or ParticleSystem.BLENDMODE_STANDARD.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[blendMode](../interfaces/IParticleSystem.md#blendmode)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[blendMode](BaseParticleSystem.md#blendmode)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:235

___

### color1

• **color1**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[color1](../interfaces/IParticleSystem.md#color1)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[color1](BaseParticleSystem.md#color1)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:542

___

### color2

• **color2**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[color2](../interfaces/IParticleSystem.md#color2)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[color2](BaseParticleSystem.md#color2)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:546

___

### colorDead

• **colorDead**: [`Color4`](Color4.md)

Color the particle will have at the end of its lifetime

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[colorDead](../interfaces/IParticleSystem.md#colordead)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[colorDead](BaseParticleSystem.md#colordead)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:550

___

### customShader

• **customShader**: `any` = `null`

This can help using your own shader to render the particle system.
The according effect will be created

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[customShader](BaseParticleSystem.md#customshader)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:197

___

### defaultProjectionMatrix

• **defaultProjectionMatrix**: [`Matrix`](Matrix.md)

Gets or sets a matrix to use to compute projection

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[defaultProjectionMatrix](../interfaces/IParticleSystem.md#defaultprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:142

___

### disposeOnStop

• **disposeOnStop**: `boolean` = `false`

Specifies whether the particle system will be disposed once it reaches the end of the animation.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[disposeOnStop](../interfaces/IParticleSystem.md#disposeonstop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[disposeOnStop](BaseParticleSystem.md#disposeonstop)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:118

___

### emitRate

• **emitRate**: `number` = `10`

The maximum number of particles to emit per frame

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[emitRate](../interfaces/IParticleSystem.md#emitrate)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[emitRate](BaseParticleSystem.md#emitrate)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:98

___

### emitter

• **emitter**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

The emitter represents the Mesh or position we are attaching the particle system to.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[emitter](../interfaces/IParticleSystem.md#emitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[emitter](BaseParticleSystem.md#emitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:93

___

### endSpriteCellID

• **endSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the last sprite cell to display

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[endSpriteCellID](../interfaces/IParticleSystem.md#endspritecellid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[endSpriteCellID](BaseParticleSystem.md#endspritecellid)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:260

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Forces the particle to write their depth information to the depth buffer. This can help preventing other draw calls
to override the particles.

#### Overrides

[BaseParticleSystem](BaseParticleSystem.md).[forceDepthWrite](BaseParticleSystem.md#forcedepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:121

___

### gravity

• **gravity**: [`Vector3`](Vector3.md)

You can use gravity if you want to give an orientation to your particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[gravity](../interfaces/IParticleSystem.md#gravity)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[gravity](BaseParticleSystem.md#gravity)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:337

___

### id

• **id**: `string`

The id of the Particle system.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[id](../interfaces/IParticleSystem.md#id)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[id](BaseParticleSystem.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:73

___

### isLocal

• **isLocal**: `boolean` = `false`

Specifies if the particles are updated in emitter local space or world space.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isLocal](../interfaces/IParticleSystem.md#islocal)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:139

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

The layer mask we are rendering the particles through.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[layerMask](../interfaces/IParticleSystem.md#layermask)

#### Overrides

[BaseParticleSystem](BaseParticleSystem.md).[layerMask](BaseParticleSystem.md#layermask)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:48

___

### limitVelocityDamping

• **limitVelocityDamping**: `number` = `0.4`

Gets or sets a value indicating the damping to apply if the limit velocity factor is reached

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[limitVelocityDamping](../interfaces/IParticleSystem.md#limitvelocitydamping)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[limitVelocityDamping](BaseParticleSystem.md#limitvelocitydamping)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:375

___

### manualEmitCount

• **manualEmitCount**: `number` = `-1`

If you want to launch only a few particles at once, that can be done, as well.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[manualEmitCount](../interfaces/IParticleSystem.md#manualemitcount)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[manualEmitCount](BaseParticleSystem.md#manualemitcount)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:103

___

### maxAngularSpeed

• **maxAngularSpeed**: `number` = `0`

Maximum angular speed of emitting particles (Z-axis rotation for each particle).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxAngularSpeed](../interfaces/IParticleSystem.md#maxangularspeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxAngularSpeed](BaseParticleSystem.md#maxangularspeed)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:181

___

### maxEmitPower

• **maxEmitPower**: `number` = `1`

Maximum power of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxEmitPower](../interfaces/IParticleSystem.md#maxemitpower)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxEmitPower](BaseParticleSystem.md#maxemitpower)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:127

___

### maxInitialRotation

• **maxInitialRotation**: `number` = `0`

Gets or sets the maximal initial rotation in radians.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxInitialRotation](../interfaces/IParticleSystem.md#maxinitialrotation)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxInitialRotation](BaseParticleSystem.md#maxinitialrotation)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:172

___

### maxLifeTime

• **maxLifeTime**: `number` = `1`

Maximum life time of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxLifeTime](../interfaces/IParticleSystem.md#maxlifetime)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxLifeTime](BaseParticleSystem.md#maxlifetime)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:136

___

### maxScaleX

• **maxScaleX**: `number` = `1`

Maximum scale of emitting particles on X axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxScaleX](../interfaces/IParticleSystem.md#maxscalex)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxScaleX](BaseParticleSystem.md#maxscalex)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:154

___

### maxScaleY

• **maxScaleY**: `number` = `1`

Maximum scale of emitting particles on Y axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxScaleY](../interfaces/IParticleSystem.md#maxscaley)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxScaleY](BaseParticleSystem.md#maxscaley)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:163

___

### maxSize

• **maxSize**: `number` = `1`

Maximum Size of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxSize](../interfaces/IParticleSystem.md#maxsize)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxSize](BaseParticleSystem.md#maxsize)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:145

___

### minAngularSpeed

• **minAngularSpeed**: `number` = `0`

Minimum angular speed of emitting particles (Z-axis rotation for each particle).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minAngularSpeed](../interfaces/IParticleSystem.md#minangularspeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minAngularSpeed](BaseParticleSystem.md#minangularspeed)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:177

___

### minEmitPower

• **minEmitPower**: `number` = `1`

Minimum power of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minEmitPower](../interfaces/IParticleSystem.md#minemitpower)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minEmitPower](BaseParticleSystem.md#minemitpower)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:123

___

### minInitialRotation

• **minInitialRotation**: `number` = `0`

Gets or sets the minimal initial rotation in radians.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minInitialRotation](../interfaces/IParticleSystem.md#mininitialrotation)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minInitialRotation](BaseParticleSystem.md#mininitialrotation)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:168

___

### minLifeTime

• **minLifeTime**: `number` = `1`

Minimum life time of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minLifeTime](../interfaces/IParticleSystem.md#minlifetime)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minLifeTime](BaseParticleSystem.md#minlifetime)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:132

___

### minScaleX

• **minScaleX**: `number` = `1`

Minimum scale of emitting particles on X axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minScaleX](../interfaces/IParticleSystem.md#minscalex)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minScaleX](BaseParticleSystem.md#minscalex)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:150

___

### minScaleY

• **minScaleY**: `number` = `1`

Minimum scale of emitting particles on Y axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minScaleY](../interfaces/IParticleSystem.md#minscaley)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minScaleY](BaseParticleSystem.md#minscaley)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:159

___

### minSize

• **minSize**: `number` = `1`

Minimum Size of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minSize](../interfaces/IParticleSystem.md#minsize)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minSize](BaseParticleSystem.md#minsize)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:141

___

### name

• **name**: `string`

The friendly name of the Particle system.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[name](../interfaces/IParticleSystem.md#name)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[name](BaseParticleSystem.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:78

___

### noiseStrength

• **noiseStrength**: [`Vector3`](Vector3.md)

Gets or sets the strength to apply to the noise value (default is (10, 10, 10))

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[noiseStrength](../interfaces/IParticleSystem.md#noisestrength)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[noiseStrength](BaseParticleSystem.md#noisestrength)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:225

___

### onAnimationEnd

• **onAnimationEnd**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

Callback triggered when the particle animation is ending.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[onAnimationEnd](BaseParticleSystem.md#onanimationend)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:230

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`IParticleSystem`](../interfaces/IParticleSystem.md)

An event triggered when the system is disposed.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onDisposeObservable](../interfaces/IParticleSystem.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:103

___

### onStoppedObservable

• **onStoppedObservable**: [`Observable`](Observable.md)[`IParticleSystem`](../interfaces/IParticleSystem.md)

An event triggered when the system is stopped

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onStoppedObservable](../interfaces/IParticleSystem.md#onstoppedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:107

___

### particleEmitterType

• **particleEmitterType**: [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

The particle emitter type defines the emitter used by the particle system.
It can be for example box, sphere, or cone...

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[particleEmitterType](../interfaces/IParticleSystem.md#particleemittertype)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[particleEmitterType](BaseParticleSystem.md#particleemittertype)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:561

___

### particleTexture

• **particleTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The texture used to render each particle. (this can be a spritesheet)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[particleTexture](../interfaces/IParticleSystem.md#particletexture)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[particleTexture](BaseParticleSystem.md#particletexture)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:186

___

### preWarmCycles

• **preWarmCycles**: `number` = `0`

Gets or sets a value indicating how many cycles (or frames) must be executed before first rendering (this value has to be set before starting the system). Default is 0

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[preWarmCycles](../interfaces/IParticleSystem.md#prewarmcycles)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preWarmCycles](BaseParticleSystem.md#prewarmcycles)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:244

___

### preWarmStepOffset

• **preWarmStepOffset**: `number` = `1`

Gets or sets a value indicating the time step multiplier to use in pre-warm mode (default is 1)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[preWarmStepOffset](../interfaces/IParticleSystem.md#prewarmstepoffset)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preWarmStepOffset](BaseParticleSystem.md#prewarmstepoffset)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:247

___

### preventAutoStart

• **preventAutoStart**: `boolean` = `false`

By default particle system starts as soon as they are created. This prevents the
automatic start to happen and let you decide when to start emitting particles.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preventAutoStart](BaseParticleSystem.md#preventautostart)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:203

___

### renderingGroupId

• **renderingGroupId**: `number` = `0`

The rendering group used by the Particle system to chose when to render.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[renderingGroupId](../interfaces/IParticleSystem.md#renderinggroupid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[renderingGroupId](BaseParticleSystem.md#renderinggroupid)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:88

___

### snippetId

• **snippetId**: `string`

Snippet ID if the particle system was created from the snippet server

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[snippetId](../interfaces/IParticleSystem.md#snippetid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[snippetId](BaseParticleSystem.md#snippetid)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:83

___

### spriteCellChangeSpeed

• **spriteCellChangeSpeed**: `number` = `1`

If using a spritesheet (isAnimationSheetEnabled) defines the speed of the sprite loop (default is 1 meaning the animation will play once during the entire particle lifetime)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellChangeSpeed](../interfaces/IParticleSystem.md#spritecellchangespeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellChangeSpeed](BaseParticleSystem.md#spritecellchangespeed)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:252

___

### spriteCellHeight

• **spriteCellHeight**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell height to use

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellHeight](../interfaces/IParticleSystem.md#spritecellheight)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellHeight](BaseParticleSystem.md#spritecellheight)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:268

___

### spriteCellLoop

• **spriteCellLoop**: `boolean` = `true`

If using a spritesheet (isAnimationSheetEnabled), defines wether the sprite animation is looping

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellLoop](../interfaces/IParticleSystem.md#spritecellloop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellLoop](BaseParticleSystem.md#spritecellloop)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:272

___

### spriteCellWidth

• **spriteCellWidth**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell width to use

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellWidth](../interfaces/IParticleSystem.md#spritecellwidth)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellWidth](BaseParticleSystem.md#spritecellwidth)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:264

___

### spriteRandomStartCell

• **spriteRandomStartCell**: `boolean` = `false`

This allows the system to random pick the start cell ID between startSpriteCellID and endSpriteCellID

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteRandomStartCell](../interfaces/IParticleSystem.md#spriterandomstartcell)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteRandomStartCell](BaseParticleSystem.md#spriterandomstartcell)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:276

___

### startDelay

• **startDelay**: `number` = `0`

Defines the delay in milliseconds before starting the system (0 by default)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[startDelay](../interfaces/IParticleSystem.md#startdelay)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[startDelay](BaseParticleSystem.md#startdelay)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:363

___

### startSpriteCellID

• **startSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the first sprite cell to display

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[startSpriteCellID](../interfaces/IParticleSystem.md#startspritecellid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[startSpriteCellID](BaseParticleSystem.md#startspritecellid)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:256

___

### targetStopDuration

• **targetStopDuration**: `number` = `0`

The amount of time the particle system is running (depends of the overall update speed).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[targetStopDuration](../interfaces/IParticleSystem.md#targetstopduration)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[targetStopDuration](BaseParticleSystem.md#targetstopduration)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:113

___

### textureMask

• **textureMask**: [`Color4`](Color4.md)

An optional mask to filter some colors out of the texture, or filter a part of the alpha channel

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[textureMask](BaseParticleSystem.md#texturemask)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:555

___

### translationPivot

• **translationPivot**: [`Vector2`](Vector2.md)

Gets or sets a Vector2 used to move the pivot (by default (0,0))

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[translationPivot](../interfaces/IParticleSystem.md#translationpivot)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[translationPivot](BaseParticleSystem.md#translationpivot)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:279

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the particle system

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[uniqueId](BaseParticleSystem.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:68

___

### updateSpeed

• **updateSpeed**: `number` = `0.01`

The overall motion speed (0.01 is default update speed, faster updates = faster animation)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[updateSpeed](../interfaces/IParticleSystem.md#updatespeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[updateSpeed](BaseParticleSystem.md#updatespeed)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:108

___

### worldOffset

• **worldOffset**: [`Vector3`](Vector3.md)

Gets or sets a world offset applied to all particles

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[worldOffset](BaseParticleSystem.md#worldoffset)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:307

___

### BLENDMODE\_ADD

▪ `Static` **BLENDMODE\_ADD**: `number` = `2`

Add current color and particle color multiplied by particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_ADD](BaseParticleSystem.md#blendmode_add)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:49

___

### BLENDMODE\_MULTIPLY

▪ `Static` **BLENDMODE\_MULTIPLY**: `number` = `3`

Multiply current color with particle color

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_MULTIPLY](BaseParticleSystem.md#blendmode_multiply)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:53

___

### BLENDMODE\_MULTIPLYADD

▪ `Static` **BLENDMODE\_MULTIPLYADD**: `number` = `4`

Multiply current color with particle color then add current color and particle color multiplied by particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_MULTIPLYADD](BaseParticleSystem.md#blendmode_multiplyadd)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:58

___

### BLENDMODE\_ONEONE

▪ `Static` **BLENDMODE\_ONEONE**: `number` = `0`

Source color is added to the destination color without alpha affecting the result

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_ONEONE](BaseParticleSystem.md#blendmode_oneone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:41

___

### BLENDMODE\_STANDARD

▪ `Static` **BLENDMODE\_STANDARD**: `number` = `1`

Blend current color and particle color using particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_STANDARD](BaseParticleSystem.md#blendmode_standard)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:45

## Accessors

### activeParticleCount

• `get` **activeParticleCount**(): `number`

Gets or set the number of active particles

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:126

• `set` **activeParticleCount**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:130

___

### billboardMode

• `get` **billboardMode**(): `number`

Gets or sets the billboard mode to use when isBillboardBased = true.
Value can be: ParticleSystem.BILLBOARDMODE_ALL, ParticleSystem.BILLBOARDMODE_Y, ParticleSystem.BILLBOARDMODE_STRETCHED

#### Returns

`number`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[billboardMode](../interfaces/IParticleSystem.md#billboardmode)

#### Inherited from

BaseParticleSystem.billboardMode

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:572

• `set` **billboardMode**(`value`): `void`

Gets or sets the billboard mode to use when isBillboardBased = true.
Value can be: ParticleSystem.BILLBOARDMODE_ALL, ParticleSystem.BILLBOARDMODE_Y, ParticleSystem.BILLBOARDMODE_STRETCHED

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[billboardMode](../interfaces/IParticleSystem.md#billboardmode)

#### Inherited from

BaseParticleSystem.billboardMode

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:576

___

### direction1

• `get` **direction1**(): [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

BaseParticleSystem.direction1

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:471

• `set` **direction1**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

BaseParticleSystem.direction1

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:479

___

### direction2

• `get` **direction2**(): [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

BaseParticleSystem.direction2

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:489

• `set` **direction2**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

BaseParticleSystem.direction2

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:497

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Inherited from

BaseParticleSystem.imageProcessingConfiguration

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:626

• `set` **imageProcessingConfiguration**(`value`): `void`

Sets the Default image processing configuration used either in the this material.

If sets to null, the scene one is in use.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Inherited from

BaseParticleSystem.imageProcessingConfiguration

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:635

___

### isAnimationSheetEnabled

• `get` **isAnimationSheetEnabled**(): `boolean`

Gets or sets whether an animation sprite sheet is enabled or not on the particle system

#### Returns

`boolean`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isAnimationSheetEnabled](../interfaces/IParticleSystem.md#isanimationsheetenabled)

#### Inherited from

BaseParticleSystem.isAnimationSheetEnabled

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:312

• `set` **isAnimationSheetEnabled**(`value`): `void`

Gets or sets a boolean indicating if a spritesheet is used to animate the particles texture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isAnimationSheetEnabled](../interfaces/IParticleSystem.md#isanimationsheetenabled)

#### Inherited from

BaseParticleSystem.isAnimationSheetEnabled

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:316

___

### isBillboardBased

• `get` **isBillboardBased**(): `boolean`

Gets or sets a boolean indicating if the particles must be rendered as billboard or aligned with the direction

#### Returns

`boolean`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isBillboardBased](../interfaces/IParticleSystem.md#isbillboardbased)

#### Inherited from

BaseParticleSystem.isBillboardBased

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:590

• `set` **isBillboardBased**(`value`): `void`

Gets or sets a boolean indicating if the particles must be rendered as billboard or aligned with the direction

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isBillboardBased](../interfaces/IParticleSystem.md#isbillboardbased)

#### Inherited from

BaseParticleSystem.isBillboardBased

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:594

___

### maxEmitBox

• `get` **maxEmitBox**(): [`Vector3`](Vector3.md)

Maximum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

BaseParticleSystem.maxEmitBox

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:525

• `set` **maxEmitBox**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

BaseParticleSystem.maxEmitBox

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:533

___

### minEmitBox

• `get` **minEmitBox**(): [`Vector3`](Vector3.md)

Minimum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

BaseParticleSystem.minEmitBox

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:507

• `set` **minEmitBox**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

BaseParticleSystem.minEmitBox

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:515

___

### noiseTexture

• `get` **noiseTexture**(): [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

Gets or sets a texture used to add random noise to particle positions

#### Returns

[`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[noiseTexture](../interfaces/IParticleSystem.md#noisetexture)

#### Inherited from

BaseParticleSystem.noiseTexture

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:211

• `set` **noiseTexture**(`value`): `void`

Gets or sets a texture used to add random noise to particle positions

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md) |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[noiseTexture](../interfaces/IParticleSystem.md#noisetexture)

#### Inherited from

BaseParticleSystem.noiseTexture

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:215

___

### onBeforeDrawParticlesObservable

• `get` **onBeforeDrawParticlesObservable**(): [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Observable that will be called just before the particles are drawn

#### Returns

[`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onBeforeDrawParticlesObservable](../interfaces/IParticleSystem.md#onbeforedrawparticlesobservable)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:287

___

### useRampGradients

• `get` **useRampGradients**(): `boolean`

Not supported by GPUParticleSystem
Gets or sets a boolean indicating that ramp gradients must be used

**`See`**

https://doc.babylonjs.com/babylon101/particles#ramp-gradients

#### Returns

`boolean`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[useRampGradients](../interfaces/IParticleSystem.md#userampgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:695

• `set` **useRampGradients**(`value`): `void`

Gets or sets a boolean indicating that ramp gradients must be used

**`See`**

https://doc.babylonjs.com/babylon101/particles#ramp-gradients

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[useRampGradients](../interfaces/IParticleSystem.md#userampgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:700

___

### vertexShaderName

• `get` **vertexShaderName**(): `string`

Gets the name of the particle vertex shader

#### Returns

`string`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[vertexShaderName](../interfaces/IParticleSystem.md#vertexshadername)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:298

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Gets a boolean indicating if the GPU particles can be rendered on current browser

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:91

## Methods

### \_addFactorGradient

▸ `Private` **_addFactorGradient**(`factorGradients`, `gradient`, `factor`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `factorGradients` | [`FactorGradient`](FactorGradient.md)[] |
| `gradient` | `number` |
| `factor` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:399

___

### \_attachImageProcessingConfiguration

▸ `Protected` **_attachImageProcessingConfiguration**(`configuration`): `void`

Attaches a new image processing configuration to the Standard Material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_attachImageProcessingConfiguration](BaseParticleSystem.md#_attachimageprocessingconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:643

___

### \_createAngularSpeedGradientTexture

▸ `Private` **_createAngularSpeedGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1412

___

### \_createColorGradientTexture

▸ `Private` **_createColorGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1428

___

### \_createDragGradientTexture

▸ `Private` **_createDragGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1424

___

### \_createFactorGradientTexture

▸ `Private` **_createFactorGradientTexture**(`factorGradients`, `textureName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `factorGradients` | [`Nullable`](../modules.md#nullable)[`IValueGradient`](../interfaces/IValueGradient.md)[] |
| `textureName` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1388

___

### \_createLimitVelocityGradientTexture

▸ `Private` **_createLimitVelocityGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1420

___

### \_createSizeGradientTexture

▸ `Private` **_createSizeGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1408

___

### \_createVelocityGradientTexture

▸ `Private` **_createVelocityGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1416

___

### \_createVertexBuffers

▸ `Private` **_createVertexBuffers**(`updateBuffer`, `renderBuffer`, `spriteSource`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `updateBuffer` | [`Buffer`](Buffer.md) |
| `renderBuffer` | [`Buffer`](Buffer.md) |
| `spriteSource` | [`Buffer`](Buffer.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:855

___

### \_getCustomDrawWrapper

▸ `Private` **_getCustomDrawWrapper**(`blendMode?`): [`Nullable`](../modules.md#nullable)`DrawWrapper`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `blendMode` | `number` | `0` |

#### Returns

[`Nullable`](../modules.md#nullable)`DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:267

___

### \_hasTargetStopDurationDependantGradient

▸ `Protected` **_hasTargetStopDurationDependantGradient**(): ``null`` \| `boolean`

#### Returns

``null`` \| `boolean`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_hasTargetStopDurationDependantGradient](BaseParticleSystem.md#_hastargetstopdurationdependantgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:352

___

### \_initialize

▸ `Private` **_initialize**(`force?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `force` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:931

___

### \_refreshColorGradient

▸ `Private` **_refreshColorGradient**(`reorder?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `reorder` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:333

___

### \_refreshFactorGradient

▸ `Private` **_refreshFactorGradient**(`factorGradients`, `textureName`, `reorder?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `factorGradients` | [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] | `undefined` |
| `textureName` | `string` | `undefined` |
| `reorder` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:438

___

### \_releaseBuffers

▸ `Private` **_releaseBuffers**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1676

___

### \_removeGradientAndTexture

▸ `Protected` **_removeGradientAndTexture**(`gradient`, `gradients`, `texture`): [`BaseParticleSystem`](BaseParticleSystem.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `gradient` | `number` |
| `gradients` | [`Nullable`](../modules.md#nullable)[`IValueGradient`](../interfaces/IValueGradient.md)[] |
| `texture` | [`RawTexture`](RawTexture.md) |

#### Returns

[`BaseParticleSystem`](BaseParticleSystem.md)

#### Overrides

BaseParticleSystem.\_removeGradientAndTexture

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:305

___

### \_render

▸ `Private` **_render**(`blendMode`, `emitterWM`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `blendMode` | `number` |
| `emitterWM` | [`Matrix`](Matrix.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1451

___

### \_reset

▸ `Protected` **_reset**(): `void`

#### Returns

`void`

#### Overrides

BaseParticleSystem.\_reset

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:851

___

### addAlphaRemapGradient

▸ **addAlphaRemapGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addAlphaRemapGradient](../interfaces/IParticleSystem.md#addalpharemapgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:646

___

### addAngularSpeedGradient

▸ **addAngularSpeedGradient**(`gradient`, `factor`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the angular speed to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addAngularSpeedGradient](../interfaces/IParticleSystem.md#addangularspeedgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:468

___

### addColorGradient

▸ **addColorGradient**(`gradient`, `color1`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `color1` | [`Color4`](Color4.md) | defines the color to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addColorGradient](../interfaces/IParticleSystem.md#addcolorgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:318

___

### addColorRemapGradient

▸ **addColorRemapGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addColorRemapGradient](../interfaces/IParticleSystem.md#addcolorremapgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:626

___

### addDragGradient

▸ **addDragGradient**(`gradient`, `factor`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the drag value to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addDragGradient](../interfaces/IParticleSystem.md#adddraggradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:561

___

### addEmitRateGradient

▸ **addEmitRateGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addEmitRateGradient](../interfaces/IParticleSystem.md#addemitrategradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:590

___

### addLifeTimeGradient

▸ **addLifeTimeGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addLifeTimeGradient](../interfaces/IParticleSystem.md#addlifetimegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:708

___

### addLimitVelocityGradient

▸ **addLimitVelocityGradient**(`gradient`, `factor`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the limit velocity value to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addLimitVelocityGradient](../interfaces/IParticleSystem.md#addlimitvelocitygradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:530

___

### addRampGradient

▸ **addRampGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addRampGradient](../interfaces/IParticleSystem.md#addrampgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:666

___

### addSizeGradient

▸ **addSizeGradient**(`gradient`, `factor`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the size factor to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addSizeGradient](../interfaces/IParticleSystem.md#addsizegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:412

___

### addStartSizeGradient

▸ **addStartSizeGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addStartSizeGradient](../interfaces/IParticleSystem.md#addstartsizegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:608

___

### addVelocityGradient

▸ **addVelocityGradient**(`gradient`, `factor`): [`GPUParticleSystem`](GPUParticleSystem.md)

Adds a new velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the velocity to affect to the specified gradient |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addVelocityGradient](../interfaces/IParticleSystem.md#addvelocitygradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:499

___

### animate

▸ **animate**(`preWarm?`): `void`

Animates the particle system for the current frame by emitting new particles and or animating the living ones.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `preWarm` | `boolean` | `false` | defines if we are in the pre-warmimg phase |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[animate](../interfaces/IParticleSystem.md#animate)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1377

___

### clone

▸ **clone**(`name`, `newEmitter`): [`GPUParticleSystem`](GPUParticleSystem.md)

Clones the particle system.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the cloned object |
| `newEmitter` | `any` | The new emitter to use |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the cloned particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[clone](../interfaces/IParticleSystem.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1775

___

### createBoxEmitter

▸ **createBoxEmitter**(`direction1`, `direction2`, `minEmitBox`, `maxEmitBox`): [`BoxParticleEmitter`](BoxParticleEmitter.md)

Creates a Box Emitter for the particle system. (emits between direction1 and direction2 from withing the box defined by minEmitBox and maxEmitBox)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction1` | [`Vector3`](Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `direction2` | [`Vector3`](Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `minEmitBox` | [`Vector3`](Vector3.md) | Particles are emitted from the box between minEmitBox and maxEmitBox |
| `maxEmitBox` | [`Vector3`](Vector3.md) | Particles are emitted from the box between minEmitBox and maxEmitBox |

#### Returns

[`BoxParticleEmitter`](BoxParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createBoxEmitter](../interfaces/IParticleSystem.md#createboxemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createBoxEmitter](BaseParticleSystem.md#createboxemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:803

___

### createConeEmitter

▸ **createConeEmitter**(`radius?`, `angle?`): [`ConeParticleEmitter`](ConeParticleEmitter.md)

Creates a Cone Emitter for the particle system (emits from the cone to the particle position)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the cone to emit from |
| `angle` | `number` | `undefined` | The base angle of the cone |

#### Returns

[`ConeParticleEmitter`](ConeParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createConeEmitter](../interfaces/IParticleSystem.md#createconeemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createConeEmitter](BaseParticleSystem.md#createconeemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:789

___

### createCylinderEmitter

▸ **createCylinderEmitter**(`radius?`, `height?`, `radiusRange?`, `directionRandomizer?`): [`CylinderParticleEmitter`](CylinderParticleEmitter.md)

Creates a Cylinder Emitter for the particle system (emits from the cylinder to the particle position)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the emission cylinder |
| `height` | `number` | `1` | The height of the emission cylinder |
| `radiusRange` | `number` | `1` | The range of emission [0-1] 0 Surface only, 1 Entire Radius |
| `directionRandomizer` | `number` | `0` | How much to randomize the particle direction [0-1] |

#### Returns

[`CylinderParticleEmitter`](CylinderParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createCylinderEmitter](../interfaces/IParticleSystem.md#createcylinderemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createCylinderEmitter](BaseParticleSystem.md#createcylinderemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:756

___

### createDirectedCylinderEmitter

▸ **createDirectedCylinderEmitter**(`radius?`, `height?`, `radiusRange?`, `direction1?`, `direction2?`): [`CylinderDirectedParticleEmitter`](CylinderDirectedParticleEmitter.md)

Creates a Directed Cylinder Emitter for the particle system (emits between direction1 and direction2)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the cylinder to emit from |
| `height` | `number` | `1` | The height of the emission cylinder |
| `radiusRange` | `number` | `1` | the range of the emission cylinder [0-1] 0 Surface only, 1 Entire Radius (1 by default) |
| `direction1` | [`Vector3`](Vector3.md) | `undefined` | Particles are emitted between the direction1 and direction2 from within the cylinder |
| `direction2` | [`Vector3`](Vector3.md) | `undefined` | Particles are emitted between the direction1 and direction2 from within the cylinder |

#### Returns

[`CylinderDirectedParticleEmitter`](CylinderDirectedParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createDirectedCylinderEmitter](../interfaces/IParticleSystem.md#createdirectedcylinderemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createDirectedCylinderEmitter](BaseParticleSystem.md#createdirectedcylinderemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:771

___

### createDirectedSphereEmitter

▸ **createDirectedSphereEmitter**(`radius?`, `direction1?`, `direction2?`): [`SphereDirectedParticleEmitter`](SphereDirectedParticleEmitter.md)

Creates a Directed Sphere Emitter for the particle system (emits between direction1 and direction2)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the sphere to emit from |
| `direction1` | [`Vector3`](Vector3.md) | `undefined` | Particles are emitted between the direction1 and direction2 from within the sphere |
| `direction2` | [`Vector3`](Vector3.md) | `undefined` | Particles are emitted between the direction1 and direction2 from within the sphere |

#### Returns

[`SphereDirectedParticleEmitter`](SphereDirectedParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createDirectedSphereEmitter](../interfaces/IParticleSystem.md#createdirectedsphereemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createDirectedSphereEmitter](BaseParticleSystem.md#createdirectedsphereemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:742

___

### createHemisphericEmitter

▸ **createHemisphericEmitter**(`radius?`, `radiusRange?`): [`HemisphericParticleEmitter`](HemisphericParticleEmitter.md)

Creates a Hemisphere Emitter for the particle system (emits along the hemisphere radius)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the hemisphere to emit from |
| `radiusRange` | `number` | `1` | The range of the hemisphere to emit from [0-1] 0 Surface Only, 1 Entire Radius |

#### Returns

[`HemisphericParticleEmitter`](HemisphericParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createHemisphericEmitter](../interfaces/IParticleSystem.md#createhemisphericemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createHemisphericEmitter](BaseParticleSystem.md#createhemisphericemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:717

___

### createPointEmitter

▸ **createPointEmitter**(`direction1`, `direction2`): [`PointParticleEmitter`](PointParticleEmitter.md)

Creates a Point Emitter for the particle system (emits directly from the emitter position)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction1` | [`Vector3`](Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `direction2` | [`Vector3`](Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |

#### Returns

[`PointParticleEmitter`](PointParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createPointEmitter](../interfaces/IParticleSystem.md#createpointemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createPointEmitter](BaseParticleSystem.md#createpointemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:702

___

### createSphereEmitter

▸ **createSphereEmitter**(`radius?`, `radiusRange?`): [`SphereParticleEmitter`](SphereParticleEmitter.md)

Creates a Sphere Emitter for the particle system (emits along the sphere radius)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | The radius of the sphere to emit from |
| `radiusRange` | `number` | `1` | The range of the sphere to emit from [0-1] 0 Surface Only, 1 Entire Radius |

#### Returns

[`SphereParticleEmitter`](SphereParticleEmitter.md)

the emitter

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[createSphereEmitter](../interfaces/IParticleSystem.md#createsphereemitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[createSphereEmitter](BaseParticleSystem.md#createsphereemitter)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:729

___

### dispose

▸ **dispose**(`disposeTexture?`): `void`

Disposes the particle system and free the associated resources

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposeTexture` | `boolean` | `true` | defines if the particule texture must be disposed as well (true by default) |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[dispose](../interfaces/IParticleSystem.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1696

___

### fillDefines

▸ **fillDefines**(`defines`, `blendMode?`): `void`

Fill the defines array according to the current settings of the particle system

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `defines` | `string`[] | `undefined` | Array to be updated |
| `blendMode` | `number` | `0` | blend mode to take into account when updating the array |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[fillDefines](../interfaces/IParticleSystem.md#filldefines)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1285

___

### fillUniformsAttributesAndSamplerNames

▸ **fillUniformsAttributesAndSamplerNames**(`uniforms`, `attributes`, `samplers`): `void`

Fill the uniforms, attributes and samplers arrays according to the current settings of the particle system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniforms` | `string`[] | Uniforms array to fill |
| `attributes` | `string`[] | Attributes array to fill |
| `samplers` | `string`[] | Samplers array to fill |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[fillUniformsAttributesAndSamplerNames](../interfaces/IParticleSystem.md#filluniformsattributesandsamplernames)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1353

___

### forceRefreshGradients

▸ **forceRefreshGradients**(): `void`

Force the system to rebuild all gradients that need to be resync

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[forceRefreshGradients](../interfaces/IParticleSystem.md#forcerefreshgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:355

___

### getActiveCount

▸ **getActiveCount**(): `number`

Gets the number of particles active at the same time.

#### Returns

`number`

The number of active particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getActiveCount](../interfaces/IParticleSystem.md#getactivecount)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:202

___

### getAlphaRemapGradients

▸ **getAlphaRemapGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of alpha remap gradients.
You must use addAlphaRemapGradient and removeAlphaRemapGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of alpha remap gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getAlphaRemapGradients](../interfaces/IParticleSystem.md#getalpharemapgradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getAlphaRemapGradients](BaseParticleSystem.md#getalpharemapgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:418

___

### getAngularSpeedGradients

▸ **getAngularSpeedGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of angular speed gradients.
You must use addAngularSpeedGradient and removeAngularSpeedGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of angular speed gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getAngularSpeedGradients](../interfaces/IParticleSystem.md#getangularspeedgradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getAngularSpeedGradients](BaseParticleSystem.md#getangularspeedgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:436

___

### getCapacity

▸ **getCapacity**(): `number`

Gets the maximum number of particles active at the same time.

#### Returns

`number`

The max number of active particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getCapacity](../interfaces/IParticleSystem.md#getcapacity)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:113

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "GPUParticleSystem"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getClassName](../interfaces/IParticleSystem.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:254

___

### getColorGradients

▸ **getColorGradients**(): [`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[]

Gets the current list of color gradients.
You must use addColorGradient and removeColorGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[]

the list of color gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getColorGradients](../interfaces/IParticleSystem.md#getcolorgradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getColorGradients](BaseParticleSystem.md#getcolorgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:391

___

### getColorRemapGradients

▸ **getColorRemapGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of color remap gradients.
You must use addColorRemapGradient and removeColorRemapGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of color remap gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getColorRemapGradients](../interfaces/IParticleSystem.md#getcolorremapgradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getColorRemapGradients](BaseParticleSystem.md#getcolorremapgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:409

___

### getCustomEffect

▸ **getCustomEffect**(`blendMode?`): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Gets the custom effect used to render the particles

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `blendMode` | `number` | `0` | Blend mode for which the effect should be retrieved |

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

The effect

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getCustomEffect](../interfaces/IParticleSystem.md#getcustomeffect)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:263

___

### getDragGradients

▸ **getDragGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of drag gradients.
You must use addDragGradient and removeDragGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of drag gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getDragGradients](../interfaces/IParticleSystem.md#getdraggradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getDragGradients](BaseParticleSystem.md#getdraggradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:370

___

### getEmitRateGradients

▸ **getEmitRateGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of emit rate gradients.
You must use addEmitRateGradient and removeEmitRateGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of emit rate gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getEmitRateGradients](../interfaces/IParticleSystem.md#getemitrategradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getEmitRateGradients](BaseParticleSystem.md#getemitrategradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:463

___

### getLifeTimeGradients

▸ **getLifeTimeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of life time gradients.
You must use addLifeTimeGradient and removeLifeTimeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of life time gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getLifeTimeGradients](../interfaces/IParticleSystem.md#getlifetimegradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getLifeTimeGradients](BaseParticleSystem.md#getlifetimegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:427

___

### getLimitVelocityGradients

▸ **getLimitVelocityGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of limit velocity gradients.
You must use addLimitVelocityGradient and removeLimitVelocityGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of limit velocity gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getLimitVelocityGradients](../interfaces/IParticleSystem.md#getlimitvelocitygradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getLimitVelocityGradients](BaseParticleSystem.md#getlimitvelocitygradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:382

___

### getRampGradients

▸ **getRampGradients**(): [`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[]

Not supported by GPUParticleSystem

#### Returns

[`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[]

the list of ramp gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getRampGradients](../interfaces/IParticleSystem.md#getrampgradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:686

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get hosting scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getScene](../interfaces/IParticleSystem.md#getscene)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getScene](BaseParticleSystem.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:330

___

### getSizeGradients

▸ **getSizeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of size gradients.
You must use addSizeGradient and removeSizeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of size gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getSizeGradients](../interfaces/IParticleSystem.md#getsizegradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getSizeGradients](BaseParticleSystem.md#getsizegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:400

___

### getStartSizeGradients

▸ **getStartSizeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of start size gradients.
You must use addStartSizeGradient and removeStartSizeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of start size gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getStartSizeGradients](../interfaces/IParticleSystem.md#getstartsizegradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getStartSizeGradients](BaseParticleSystem.md#getstartsizegradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:454

___

### getVelocityGradients

▸ **getVelocityGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of velocity gradients.
You must use addVelocityGradient and removeVelocityGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of velocity gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getVelocityGradients](../interfaces/IParticleSystem.md#getvelocitygradients)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[getVelocityGradients](BaseParticleSystem.md#getvelocitygradients)

#### Defined in

https://github.com/babylon.js/core/src/Particles/baseParticleSystem.ts:445

___

### isReady

▸ **isReady**(): `boolean`

Is this system ready to be used/rendered

#### Returns

`boolean`

true if the system is ready

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isReady](../interfaces/IParticleSystem.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:148

___

### isStarted

▸ **isStarted**(): `boolean`

Gets if the system has been started. (Note: this will still be true after stop is called)

#### Returns

`boolean`

True if it has been started, otherwise false.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isStarted](../interfaces/IParticleSystem.md#isstarted)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:178

___

### isStopped

▸ **isStopped**(): `boolean`

Gets if the system has been stopped. (Note: rendering is still happening but the system is frozen)

#### Returns

`boolean`

True if it has been stopped, otherwise false.

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:186

___

### isStopping

▸ **isStopping**(): `boolean`

Gets a boolean indicating that the system is stopping

#### Returns

`boolean`

true if the system is currently stopping

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isStopping](../interfaces/IParticleSystem.md#isstopping)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:194

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the particle system

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[rebuild](../interfaces/IParticleSystem.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1672

___

### removeAlphaRemapGradient

▸ **removeAlphaRemapGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:656

___

### removeAngularSpeedGradient

▸ **removeAngularSpeedGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeAngularSpeedGradient](../interfaces/IParticleSystem.md#removeangularspeedgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:486

___

### removeColorGradient

▸ **removeColorGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeColorGradient](../interfaces/IParticleSystem.md#removecolorgradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:371

___

### removeColorRemapGradient

▸ **removeColorRemapGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:636

___

### removeDragGradient

▸ **removeDragGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeDragGradient](../interfaces/IParticleSystem.md#removedraggradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:579

___

### removeEmitRateGradient

▸ **removeEmitRateGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeEmitRateGradient](../interfaces/IParticleSystem.md#removeemitrategradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:599

___

### removeLifeTimeGradient

▸ **removeLifeTimeGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeLifeTimeGradient](../interfaces/IParticleSystem.md#removelifetimegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:718

___

### removeLimitVelocityGradient

▸ **removeLimitVelocityGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeLimitVelocityGradient](../interfaces/IParticleSystem.md#removelimitvelocitygradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:548

___

### removeRampGradient

▸ **removeRampGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:676

___

### removeSizeGradient

▸ **removeSizeGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeSizeGradient](../interfaces/IParticleSystem.md#removesizegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:431

___

### removeStartSizeGradient

▸ **removeStartSizeGradient**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Not supported by GPUParticleSystem

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeStartSizeGradient](../interfaces/IParticleSystem.md#removestartsizegradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:617

___

### removeVelocityGradient

▸ **removeVelocityGradient**(`gradient`): [`GPUParticleSystem`](GPUParticleSystem.md)

Remove a specific velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeVelocityGradient](../interfaces/IParticleSystem.md#removevelocitygradient)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:517

___

### render

▸ **render**(`preWarm?`, `forceUpdateOnly?`): `number`

Renders the particle system in its current state

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `preWarm` | `boolean` | `false` | defines if the system should only update the particles but not render them |
| `forceUpdateOnly` | `boolean` | `false` | if true, force to only update the particles and never display them (meaning, even if preWarm=false, when forceUpdateOnly=true the particles won't be displayed) |

#### Returns

`number`

the current number of particles

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[render](../interfaces/IParticleSystem.md#render)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1537

___

### reset

▸ **reset**(): `void`

Remove all active particles

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[reset](../interfaces/IParticleSystem.md#reset)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:243

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:381

___

### serialize

▸ **serialize**(`serializeTexture?`): `any`

Serializes the particle system to a JSON object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `serializeTexture` | `boolean` | `false` | defines if the texture must be serialized as well |

#### Returns

`any`

the JSON object

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[serialize](../interfaces/IParticleSystem.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1820

___

### setCustomEffect

▸ **setCustomEffect**(`effect`, `blendMode?`): `void`

Sets the custom effect used to render the particles

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `undefined` | The effect to set |
| `blendMode` | `number` | `0` | Blend mode for which the effect should be set |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[setCustomEffect](../interfaces/IParticleSystem.md#setcustomeffect)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:276

___

### start

▸ **start**(`delay?`): `void`

Starts the particle system and begins to emit

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `delay` | `number` | defines the delay in milliseconds before starting the system (this.startDelay by default) |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[start](../interfaces/IParticleSystem.md#start)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:210

___

### stop

▸ **stop**(): `void`

Stops the particle system.

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[stop](../interfaces/IParticleSystem.md#stop)

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:233

___

### Parse

▸ `Static` **Parse**(`parsedParticleSystem`, `sceneOrEngine`, `rootUrl`, `doNotStart?`, `capacity?`): [`GPUParticleSystem`](GPUParticleSystem.md)

Parses a JSON object to create a GPU particle system.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `parsedParticleSystem` | `any` | `undefined` | The JSON object to parse |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene or the engine to create the particle system in |
| `rootUrl` | `string` | `undefined` | The root url to use to load external dependencies like texture |
| `doNotStart` | `boolean` | `false` | Ignore the preventAutoStart attribute and does not start |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

[`GPUParticleSystem`](GPUParticleSystem.md)

the parsed GPU particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/gpuParticleSystem.ts:1841

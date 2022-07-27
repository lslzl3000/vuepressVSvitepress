[@dev/core](../README.md) / [Exports](../modules.md) / ParticleSystem

# Class: ParticleSystem

This represents a particle system in Babylon.
Particles are often small sprites used to simulate hard-to-reproduce phenomena like fire, smoke, water, or abstract visual effects like magic glitter and faery dust.
Particles can take different shapes while emitted like box, sphere, cone or you can write your custom function.

**`Example`**

```ts
https://doc.babylonjs.com/babylon101/particles
```

## Hierarchy

- [`BaseParticleSystem`](BaseParticleSystem.md)

  ↳ **`ParticleSystem`**

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- [`IAnimatable`](../interfaces/IAnimatable.md)
- [`IParticleSystem`](../interfaces/IParticleSystem.md)

## Table of contents

### Constructors

- [constructor](ParticleSystem.md#constructor)

### Properties

- [\_actualFrame](ParticleSystem.md#_actualframe)
- [\_alive](ParticleSystem.md#_alive)
- [\_alphaRemapGradients](ParticleSystem.md#_alpharemapgradients)
- [\_angularSpeedGradients](ParticleSystem.md#_angularspeedgradients)
- [\_capacity](ParticleSystem.md#_capacity)
- [\_colorDiff](ParticleSystem.md#_colordiff)
- [\_colorGradients](ParticleSystem.md#_colorgradients)
- [\_colorRemapGradients](ParticleSystem.md#_colorremapgradients)
- [\_createParticle](ParticleSystem.md#_createparticle)
- [\_currentRenderId](ParticleSystem.md#_currentrenderid)
- [\_customWrappers](ParticleSystem.md#_customwrappers)
- [\_dragGradients](ParticleSystem.md#_draggradients)
- [\_drawWrappers](ParticleSystem.md#_drawwrappers)
- [\_emitFromParticle](ParticleSystem.md#_emitfromparticle)
- [\_emitRateGradients](ParticleSystem.md#_emitrategradients)
- [\_emitterInverseWorldMatrix](ParticleSystem.md#_emitterinverseworldmatrix)
- [\_emitterWorldMatrix](ParticleSystem.md#_emitterworldmatrix)
- [\_engine](ParticleSystem.md#_engine)
- [\_epsilon](ParticleSystem.md#_epsilon)
- [\_imageProcessingConfiguration](ParticleSystem.md#_imageprocessingconfiguration)
- [\_imageProcessingConfigurationDefines](ParticleSystem.md#_imageprocessingconfigurationdefines)
- [\_indexBuffer](ParticleSystem.md#_indexbuffer)
- [\_lifeTimeGradients](ParticleSystem.md#_lifetimegradients)
- [\_limitVelocityGradients](ParticleSystem.md#_limitvelocitygradients)
- [\_newPartsExcess](ParticleSystem.md#_newpartsexcess)
- [\_onDisposeObserver](ParticleSystem.md#_ondisposeobserver)
- [\_particles](ParticleSystem.md#_particles)
- [\_rampGradients](ParticleSystem.md#_rampgradients)
- [\_rampGradientsTexture](ParticleSystem.md#_rampgradientstexture)
- [\_rawTextureWidth](ParticleSystem.md#_rawtexturewidth)
- [\_rootParticleSystem](ParticleSystem.md#_rootparticlesystem)
- [\_rootUrl](ParticleSystem.md#_rooturl)
- [\_scaledColorStep](ParticleSystem.md#_scaledcolorstep)
- [\_scaledDirection](ParticleSystem.md#_scaleddirection)
- [\_scaledGravity](ParticleSystem.md#_scaledgravity)
- [\_scaledUpdateSpeed](ParticleSystem.md#_scaledupdatespeed)
- [\_scene](ParticleSystem.md#_scene)
- [\_sizeGradients](ParticleSystem.md#_sizegradients)
- [\_spriteBuffer](ParticleSystem.md#_spritebuffer)
- [\_startSizeGradients](ParticleSystem.md#_startsizegradients)
- [\_started](ParticleSystem.md#_started)
- [\_stockParticles](ParticleSystem.md#_stockparticles)
- [\_stopped](ParticleSystem.md#_stopped)
- [\_subEmitters](ParticleSystem.md#_subemitters)
- [\_useInstancing](ParticleSystem.md#_useinstancing)
- [\_useRampGradients](ParticleSystem.md#_userampgradients)
- [\_velocityGradients](ParticleSystem.md#_velocitygradients)
- [\_vertexArrayObject](ParticleSystem.md#_vertexarrayobject)
- [\_vertexBuffer](ParticleSystem.md#_vertexbuffer)
- [\_vertexBufferSize](ParticleSystem.md#_vertexbuffersize)
- [\_vertexBuffers](ParticleSystem.md#_vertexbuffers)
- [\_vertexData](ParticleSystem.md#_vertexdata)
- [activeSubSystems](ParticleSystem.md#activesubsystems)
- [animations](ParticleSystem.md#animations)
- [beginAnimationFrom](ParticleSystem.md#beginanimationfrom)
- [beginAnimationLoop](ParticleSystem.md#beginanimationloop)
- [beginAnimationOnStart](ParticleSystem.md#beginanimationonstart)
- [beginAnimationTo](ParticleSystem.md#beginanimationto)
- [blendMode](ParticleSystem.md#blendmode)
- [color1](ParticleSystem.md#color1)
- [color2](ParticleSystem.md#color2)
- [colorDead](ParticleSystem.md#colordead)
- [customShader](ParticleSystem.md#customshader)
- [defaultProjectionMatrix](ParticleSystem.md#defaultprojectionmatrix)
- [defaultViewMatrix](ParticleSystem.md#defaultviewmatrix)
- [disposeOnStop](ParticleSystem.md#disposeonstop)
- [emitRate](ParticleSystem.md#emitrate)
- [emitter](ParticleSystem.md#emitter)
- [endSpriteCellID](ParticleSystem.md#endspritecellid)
- [forceDepthWrite](ParticleSystem.md#forcedepthwrite)
- [gravity](ParticleSystem.md#gravity)
- [id](ParticleSystem.md#id)
- [isLocal](ParticleSystem.md#islocal)
- [layerMask](ParticleSystem.md#layermask)
- [limitVelocityDamping](ParticleSystem.md#limitvelocitydamping)
- [manualEmitCount](ParticleSystem.md#manualemitcount)
- [maxAngularSpeed](ParticleSystem.md#maxangularspeed)
- [maxEmitPower](ParticleSystem.md#maxemitpower)
- [maxInitialRotation](ParticleSystem.md#maxinitialrotation)
- [maxLifeTime](ParticleSystem.md#maxlifetime)
- [maxScaleX](ParticleSystem.md#maxscalex)
- [maxScaleY](ParticleSystem.md#maxscaley)
- [maxSize](ParticleSystem.md#maxsize)
- [minAngularSpeed](ParticleSystem.md#minangularspeed)
- [minEmitPower](ParticleSystem.md#minemitpower)
- [minInitialRotation](ParticleSystem.md#mininitialrotation)
- [minLifeTime](ParticleSystem.md#minlifetime)
- [minScaleX](ParticleSystem.md#minscalex)
- [minScaleY](ParticleSystem.md#minscaley)
- [minSize](ParticleSystem.md#minsize)
- [name](ParticleSystem.md#name)
- [noiseStrength](ParticleSystem.md#noisestrength)
- [onAnimationEnd](ParticleSystem.md#onanimationend)
- [onDisposeObservable](ParticleSystem.md#ondisposeobservable)
- [onStoppedObservable](ParticleSystem.md#onstoppedobservable)
- [particleEmitterType](ParticleSystem.md#particleemittertype)
- [particleTexture](ParticleSystem.md#particletexture)
- [preWarmCycles](ParticleSystem.md#prewarmcycles)
- [preWarmStepOffset](ParticleSystem.md#prewarmstepoffset)
- [preventAutoStart](ParticleSystem.md#preventautostart)
- [recycleParticle](ParticleSystem.md#recycleparticle)
- [renderingGroupId](ParticleSystem.md#renderinggroupid)
- [snippetId](ParticleSystem.md#snippetid)
- [spriteCellChangeSpeed](ParticleSystem.md#spritecellchangespeed)
- [spriteCellHeight](ParticleSystem.md#spritecellheight)
- [spriteCellLoop](ParticleSystem.md#spritecellloop)
- [spriteCellWidth](ParticleSystem.md#spritecellwidth)
- [spriteRandomStartCell](ParticleSystem.md#spriterandomstartcell)
- [startDelay](ParticleSystem.md#startdelay)
- [startDirectionFunction](ParticleSystem.md#startdirectionfunction)
- [startPositionFunction](ParticleSystem.md#startpositionfunction)
- [startSpriteCellID](ParticleSystem.md#startspritecellid)
- [subEmitters](ParticleSystem.md#subemitters)
- [targetStopDuration](ParticleSystem.md#targetstopduration)
- [textureMask](ParticleSystem.md#texturemask)
- [translationPivot](ParticleSystem.md#translationpivot)
- [uniqueId](ParticleSystem.md#uniqueid)
- [updateFunction](ParticleSystem.md#updatefunction)
- [updateSpeed](ParticleSystem.md#updatespeed)
- [worldOffset](ParticleSystem.md#worldoffset)
- [BILLBOARDMODE\_ALL](ParticleSystem.md#billboardmode_all)
- [BILLBOARDMODE\_STRETCHED](ParticleSystem.md#billboardmode_stretched)
- [BILLBOARDMODE\_Y](ParticleSystem.md#billboardmode_y)
- [BLENDMODE\_ADD](ParticleSystem.md#blendmode_add)
- [BLENDMODE\_MULTIPLY](ParticleSystem.md#blendmode_multiply)
- [BLENDMODE\_MULTIPLYADD](ParticleSystem.md#blendmode_multiplyadd)
- [BLENDMODE\_ONEONE](ParticleSystem.md#blendmode_oneone)
- [BLENDMODE\_STANDARD](ParticleSystem.md#blendmode_standard)

### Accessors

- [billboardMode](ParticleSystem.md#billboardmode)
- [direction1](ParticleSystem.md#direction1)
- [direction2](ParticleSystem.md#direction2)
- [imageProcessingConfiguration](ParticleSystem.md#imageprocessingconfiguration)
- [indexBuffer](ParticleSystem.md#indexbuffer)
- [isAnimationSheetEnabled](ParticleSystem.md#isanimationsheetenabled)
- [isBillboardBased](ParticleSystem.md#isbillboardbased)
- [maxEmitBox](ParticleSystem.md#maxemitbox)
- [minEmitBox](ParticleSystem.md#minemitbox)
- [noiseTexture](ParticleSystem.md#noisetexture)
- [onBeforeDrawParticlesObservable](ParticleSystem.md#onbeforedrawparticlesobservable)
- [onDispose](ParticleSystem.md#ondispose)
- [particles](ParticleSystem.md#particles)
- [useRampGradients](ParticleSystem.md#userampgradients)
- [vertexBuffers](ParticleSystem.md#vertexbuffers)
- [vertexShaderName](ParticleSystem.md#vertexshadername)

### Methods

- [\_addFactorGradient](ParticleSystem.md#_addfactorgradient)
- [\_appendParticleVertices](ParticleSystem.md#_appendparticlevertices)
- [\_attachImageProcessingConfiguration](ParticleSystem.md#_attachimageprocessingconfiguration)
- [\_createIndexBuffer](ParticleSystem.md#_createindexbuffer)
- [\_createRampGradientTexture](ParticleSystem.md#_createrampgradienttexture)
- [\_createVertexBuffers](ParticleSystem.md#_createvertexbuffers)
- [\_fetchR](ParticleSystem.md#_fetchr)
- [\_getCustomDrawWrapper](ParticleSystem.md#_getcustomdrawwrapper)
- [\_hasTargetStopDurationDependantGradient](ParticleSystem.md#_hastargetstopdurationdependantgradient)
- [\_prepareSubEmitterInternalArray](ParticleSystem.md#_preparesubemitterinternalarray)
- [\_removeFactorGradient](ParticleSystem.md#_removefactorgradient)
- [\_removeFromRoot](ParticleSystem.md#_removefromroot)
- [\_render](ParticleSystem.md#_render)
- [\_reset](ParticleSystem.md#_reset)
- [\_resetEffect](ParticleSystem.md#_reseteffect)
- [\_stopSubEmitters](ParticleSystem.md#_stopsubemitters)
- [\_syncRampGradientTexture](ParticleSystem.md#_syncrampgradienttexture)
- [\_update](ParticleSystem.md#_update)
- [addAlphaRemapGradient](ParticleSystem.md#addalpharemapgradient)
- [addAngularSpeedGradient](ParticleSystem.md#addangularspeedgradient)
- [addColorGradient](ParticleSystem.md#addcolorgradient)
- [addColorRemapGradient](ParticleSystem.md#addcolorremapgradient)
- [addDragGradient](ParticleSystem.md#adddraggradient)
- [addEmitRateGradient](ParticleSystem.md#addemitrategradient)
- [addLifeTimeGradient](ParticleSystem.md#addlifetimegradient)
- [addLimitVelocityGradient](ParticleSystem.md#addlimitvelocitygradient)
- [addRampGradient](ParticleSystem.md#addrampgradient)
- [addSizeGradient](ParticleSystem.md#addsizegradient)
- [addStartSizeGradient](ParticleSystem.md#addstartsizegradient)
- [addVelocityGradient](ParticleSystem.md#addvelocitygradient)
- [animate](ParticleSystem.md#animate)
- [clone](ParticleSystem.md#clone)
- [createBoxEmitter](ParticleSystem.md#createboxemitter)
- [createConeEmitter](ParticleSystem.md#createconeemitter)
- [createCylinderEmitter](ParticleSystem.md#createcylinderemitter)
- [createDirectedCylinderEmitter](ParticleSystem.md#createdirectedcylinderemitter)
- [createDirectedSphereEmitter](ParticleSystem.md#createdirectedsphereemitter)
- [createHemisphericEmitter](ParticleSystem.md#createhemisphericemitter)
- [createPointEmitter](ParticleSystem.md#createpointemitter)
- [createSphereEmitter](ParticleSystem.md#createsphereemitter)
- [dispose](ParticleSystem.md#dispose)
- [fillDefines](ParticleSystem.md#filldefines)
- [fillUniformsAttributesAndSamplerNames](ParticleSystem.md#filluniformsattributesandsamplernames)
- [forceRefreshGradients](ParticleSystem.md#forcerefreshgradients)
- [getActiveCount](ParticleSystem.md#getactivecount)
- [getAlphaRemapGradients](ParticleSystem.md#getalpharemapgradients)
- [getAngularSpeedGradients](ParticleSystem.md#getangularspeedgradients)
- [getCapacity](ParticleSystem.md#getcapacity)
- [getClassName](ParticleSystem.md#getclassname)
- [getColorGradients](ParticleSystem.md#getcolorgradients)
- [getColorRemapGradients](ParticleSystem.md#getcolorremapgradients)
- [getCustomEffect](ParticleSystem.md#getcustomeffect)
- [getDragGradients](ParticleSystem.md#getdraggradients)
- [getEmitRateGradients](ParticleSystem.md#getemitrategradients)
- [getLifeTimeGradients](ParticleSystem.md#getlifetimegradients)
- [getLimitVelocityGradients](ParticleSystem.md#getlimitvelocitygradients)
- [getRampGradients](ParticleSystem.md#getrampgradients)
- [getScene](ParticleSystem.md#getscene)
- [getSizeGradients](ParticleSystem.md#getsizegradients)
- [getStartSizeGradients](ParticleSystem.md#getstartsizegradients)
- [getVelocityGradients](ParticleSystem.md#getvelocitygradients)
- [isAlive](ParticleSystem.md#isalive)
- [isReady](ParticleSystem.md#isready)
- [isStarted](ParticleSystem.md#isstarted)
- [isStopping](ParticleSystem.md#isstopping)
- [rebuild](ParticleSystem.md#rebuild)
- [removeAlphaRemapGradient](ParticleSystem.md#removealpharemapgradient)
- [removeAngularSpeedGradient](ParticleSystem.md#removeangularspeedgradient)
- [removeColorGradient](ParticleSystem.md#removecolorgradient)
- [removeColorRemapGradient](ParticleSystem.md#removecolorremapgradient)
- [removeDragGradient](ParticleSystem.md#removedraggradient)
- [removeEmitRateGradient](ParticleSystem.md#removeemitrategradient)
- [removeLifeTimeGradient](ParticleSystem.md#removelifetimegradient)
- [removeLimitVelocityGradient](ParticleSystem.md#removelimitvelocitygradient)
- [removeRampGradient](ParticleSystem.md#removerampgradient)
- [removeSizeGradient](ParticleSystem.md#removesizegradient)
- [removeStartSizeGradient](ParticleSystem.md#removestartsizegradient)
- [removeVelocityGradient](ParticleSystem.md#removevelocitygradient)
- [render](ParticleSystem.md#render)
- [reset](ParticleSystem.md#reset)
- [resetDrawCache](ParticleSystem.md#resetdrawcache)
- [serialize](ParticleSystem.md#serialize)
- [setCustomEffect](ParticleSystem.md#setcustomeffect)
- [start](ParticleSystem.md#start)
- [stop](ParticleSystem.md#stop)
- [Parse](ParticleSystem.md#parse)

## Constructors

### constructor

• **new ParticleSystem**(`name`, `capacity`, `sceneOrEngine`, `customEffect?`, `isAnimationSheetEnabled?`, `epsilon?`)

Instantiates a particle system.
Particles are often small sprites used to simulate hard-to-reproduce phenomena like fire, smoke, water, or abstract visual effects like magic glitter and faery dust.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the particle system |
| `capacity` | `number` | `undefined` | The max number of particles alive at the same time |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene the particle system belongs to or the engine to use if no scene |
| `customEffect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `null` | a custom effect used to change the way particles are rendered by default |
| `isAnimationSheetEnabled` | `boolean` | `false` | Must be true if using a spritesheet to animate the particles texture |
| `epsilon` | `number` | `0.01` | Offset used to render the particles |

#### Overrides

[BaseParticleSystem](BaseParticleSystem.md).[constructor](BaseParticleSystem.md#constructor)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:314

## Properties

### \_actualFrame

• `Private` **\_actualFrame**: `number` = `0`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:141

___

### \_alive

• `Private` **\_alive**: `boolean`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:135

___

### \_alphaRemapGradients

• `Protected` **\_alphaRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_alphaRemapGradients](BaseParticleSystem.md#_alpharemapgradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:350

___

### \_angularSpeedGradients

• `Protected` **\_angularSpeedGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_angularSpeedGradients](BaseParticleSystem.md#_angularspeedgradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:342

___

### \_capacity

• `Private` **\_capacity**: `number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:120

___

### \_colorDiff

• `Private` **\_colorDiff**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:131

___

### \_colorGradients

• `Protected` **\_colorGradients**: [`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_colorGradients](BaseParticleSystem.md#_colorgradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:339

___

### \_colorRemapGradients

• `Protected` **\_colorRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_colorRemapGradients](BaseParticleSystem.md#_colorremapgradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:349

___

### \_createParticle

• `Private` **\_createParticle**: () => [`Particle`](Particle.md)

#### Type declaration

▸ (): [`Particle`](Particle.md)

##### Returns

[`Particle`](Particle.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1426

___

### \_currentRenderId

• `Private` **\_currentRenderId**: `number` = `-1`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:134

___

### \_customWrappers

• `Private` **\_customWrappers**: `Object`

#### Index signature

▪ [blendMode: `number`]: [`Nullable`](../modules.md#nullable)`DrawWrapper`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:129

___

### \_dragGradients

• `Protected` **\_dragGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_dragGradients](BaseParticleSystem.md#_draggradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:345

___

### \_drawWrappers

• `Private` **\_drawWrappers**: `DrawWrapper`[][]

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:128

___

### \_emitFromParticle

• `Private` **\_emitFromParticle**: (`particle`: [`Particle`](Particle.md)) => `void`

#### Type declaration

▸ (`particle`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `particle` | [`Particle`](Particle.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1463

___

### \_emitRateGradients

• `Protected` **\_emitRateGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_emitRateGradients](BaseParticleSystem.md#_emitrategradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:346

___

### \_emitterInverseWorldMatrix

• `Private` **\_emitterInverseWorldMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:81

___

### \_emitterWorldMatrix

• `Private` **\_emitterWorldMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:80

___

### \_engine

• `Protected` **\_engine**: [`ThinEngine`](ThinEngine.md)

The engine the particle system belongs to.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_engine](BaseParticleSystem.md#_engine)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:611

___

### \_epsilon

• `Private` **\_epsilon**: `number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:119

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the standard Material.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_imageProcessingConfiguration](BaseParticleSystem.md#_imageprocessingconfiguration)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:621

___

### \_imageProcessingConfigurationDefines

• `Protected` **\_imageProcessingConfigurationDefines**: `ImageProcessingConfigurationDefines`

Local cache of defines for image processing.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_imageProcessingConfigurationDefines](BaseParticleSystem.md#_imageprocessingconfigurationdefines)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:616

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:127

___

### \_lifeTimeGradients

• `Protected` **\_lifeTimeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_lifeTimeGradients](BaseParticleSystem.md#_lifetimegradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:341

___

### \_limitVelocityGradients

• `Protected` **\_limitVelocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_limitVelocityGradients](BaseParticleSystem.md#_limitvelocitygradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:344

___

### \_newPartsExcess

• `Private` **\_newPartsExcess**: `number` = `0`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:122

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`IParticleSystem`](../interfaces/IParticleSystem.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:107

___

### \_particles

• `Private` **\_particles**: [`Particle`](Particle.md)[]

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:118

___

### \_rampGradients

• `Protected` **\_rampGradients**: [`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_rampGradients](BaseParticleSystem.md#_rampgradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:348

___

### \_rampGradientsTexture

• `Private` **\_rampGradientsTexture**: [`Nullable`](../modules.md#nullable)[`RawTexture`](RawTexture.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:160

___

### \_rawTextureWidth

• `Private` `Readonly` **\_rawTextureWidth**: ``256``

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:159

___

### \_rootParticleSystem

• `Private` **\_rootParticleSystem**: [`Nullable`](../modules.md#nullable)[`ParticleSystem`](ParticleSystem.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:209

___

### \_rootUrl

• `Protected` **\_rootUrl**: `string` = `""`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_rootUrl](BaseParticleSystem.md#_rooturl)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:205

___

### \_scaledColorStep

• `Private` **\_scaledColorStep**: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:130

___

### \_scaledDirection

• `Private` **\_scaledDirection**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:132

___

### \_scaledGravity

• `Private` **\_scaledGravity**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:133

___

### \_scaledUpdateSpeed

• `Private` **\_scaledUpdateSpeed**: `number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:142

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

The scene the particle system belongs to.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_scene](BaseParticleSystem.md#_scene)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:606

___

### \_sizeGradients

• `Protected` **\_sizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_sizeGradients](BaseParticleSystem.md#_sizegradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:340

___

### \_spriteBuffer

• `Private` **\_spriteBuffer**: [`Nullable`](../modules.md#nullable)[`Buffer`](Buffer.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:126

___

### \_startSizeGradients

• `Protected` **\_startSizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_startSizeGradients](BaseParticleSystem.md#_startsizegradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:347

___

### \_started

• `Private` **\_started**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:139

___

### \_stockParticles

• `Private` **\_stockParticles**: [`Particle`](Particle.md)[]

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:121

___

### \_stopped

• `Private` **\_stopped**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:140

___

### \_subEmitters

• `Private` **\_subEmitters**: [`SubEmitter`](SubEmitter.md)[][]

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:193

___

### \_useInstancing

• `Private` **\_useInstancing**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:136

___

### \_useRampGradients

• `Private` **\_useRampGradients**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:161

___

### \_velocityGradients

• `Protected` **\_velocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_velocityGradients](BaseParticleSystem.md#_velocitygradients)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:343

___

### \_vertexArrayObject

• `Private` **\_vertexArrayObject**: [`Nullable`](../modules.md#nullable)`WebGLVertexArrayObject`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:137

___

### \_vertexBuffer

• `Private` **\_vertexBuffer**: [`Nullable`](../modules.md#nullable)[`Buffer`](Buffer.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:124

___

### \_vertexBufferSize

• `Private` **\_vertexBufferSize**: `number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:143

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`VertexBuffer`](VertexBuffer.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:125

___

### \_vertexData

• `Private` **\_vertexData**: `Float32Array`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:123

___

### activeSubSystems

• **activeSubSystems**: [`ParticleSystem`](ParticleSystem.md)[]

The current active Sub-systems, this property is used by the root particle system only.

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:202

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

List of animations used by the particle system.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[animations](../interfaces/IParticleSystem.md#animations)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[animations](BaseParticleSystem.md#animations)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:63

___

### beginAnimationFrom

• **beginAnimationFrom**: `number` = `0`

Gets or sets the frame to start the animation from when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationFrom](../interfaces/IParticleSystem.md#beginanimationfrom)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationFrom](BaseParticleSystem.md#beginanimationfrom)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:292

___

### beginAnimationLoop

• **beginAnimationLoop**: `boolean` = `false`

Gets or sets a boolean indicating if animations must loop when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationLoop](../interfaces/IParticleSystem.md#beginanimationloop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationLoop](BaseParticleSystem.md#beginanimationloop)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:302

___

### beginAnimationOnStart

• **beginAnimationOnStart**: `boolean` = `false`

Gets or sets a boolean indicating that hosted animations (in the system.animations array) must be started when system.start() is called

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationOnStart](../interfaces/IParticleSystem.md#beginanimationonstart)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationOnStart](BaseParticleSystem.md#beginanimationonstart)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:287

___

### beginAnimationTo

• **beginAnimationTo**: `number` = `60`

Gets or sets the frame to end the animation on when beginAnimationOnStart is true

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[beginAnimationTo](../interfaces/IParticleSystem.md#beginanimationto)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[beginAnimationTo](BaseParticleSystem.md#beginanimationto)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:297

___

### blendMode

• **blendMode**: `number` = `BaseParticleSystem.BLENDMODE_ONEONE`

Blend mode use to render the particle, it can be either ParticleSystem.BLENDMODE_ONEONE or ParticleSystem.BLENDMODE_STANDARD.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[blendMode](../interfaces/IParticleSystem.md#blendmode)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[blendMode](BaseParticleSystem.md#blendmode)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:235

___

### color1

• **color1**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[color1](../interfaces/IParticleSystem.md#color1)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[color1](BaseParticleSystem.md#color1)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:542

___

### color2

• **color2**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[color2](../interfaces/IParticleSystem.md#color2)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[color2](BaseParticleSystem.md#color2)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:546

___

### colorDead

• **colorDead**: [`Color4`](Color4.md)

Color the particle will have at the end of its lifetime

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[colorDead](../interfaces/IParticleSystem.md#colordead)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[colorDead](BaseParticleSystem.md#colordead)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:550

___

### customShader

• **customShader**: `any` = `null`

This can help using your own shader to render the particle system.
The according effect will be created

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[customShader](BaseParticleSystem.md#customshader)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:197

___

### defaultProjectionMatrix

• **defaultProjectionMatrix**: [`Matrix`](Matrix.md)

Gets or sets a matrix to use to compute projection

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[defaultProjectionMatrix](../interfaces/IParticleSystem.md#defaultprojectionmatrix)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:164

___

### defaultViewMatrix

• **defaultViewMatrix**: [`Matrix`](Matrix.md)

Gets or sets a matrix to use to compute view

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:167

___

### disposeOnStop

• **disposeOnStop**: `boolean` = `false`

Specifies whether the particle system will be disposed once it reaches the end of the animation.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[disposeOnStop](../interfaces/IParticleSystem.md#disposeonstop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[disposeOnStop](BaseParticleSystem.md#disposeonstop)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:118

___

### emitRate

• **emitRate**: `number` = `10`

The maximum number of particles to emit per frame

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[emitRate](../interfaces/IParticleSystem.md#emitrate)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[emitRate](BaseParticleSystem.md#emitrate)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:98

___

### emitter

• **emitter**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

The emitter represents the Mesh or position we are attaching the particle system to.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[emitter](../interfaces/IParticleSystem.md#emitter)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[emitter](BaseParticleSystem.md#emitter)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:93

___

### endSpriteCellID

• **endSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the last sprite cell to display

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[endSpriteCellID](../interfaces/IParticleSystem.md#endspritecellid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[endSpriteCellID](BaseParticleSystem.md#endspritecellid)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:260

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Forces the particle to write their depth information to the depth buffer. This can help preventing other draw calls
to override the particles.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[forceDepthWrite](BaseParticleSystem.md#forcedepthwrite)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:241

___

### gravity

• **gravity**: [`Vector3`](Vector3.md)

You can use gravity if you want to give an orientation to your particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[gravity](../interfaces/IParticleSystem.md#gravity)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[gravity](BaseParticleSystem.md#gravity)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:337

___

### id

• **id**: `string`

The id of the Particle system.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[id](../interfaces/IParticleSystem.md#id)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[id](BaseParticleSystem.md#id)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:73

___

### isLocal

• **isLocal**: `boolean` = `false`

Specifies if the particles are updated in emitter local space or world space

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[isLocal](../interfaces/IParticleSystem.md#islocal)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:207

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

The layer mask we are rendering the particles through.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[layerMask](../interfaces/IParticleSystem.md#layermask)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[layerMask](BaseParticleSystem.md#layermask)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:191

___

### limitVelocityDamping

• **limitVelocityDamping**: `number` = `0.4`

Gets or sets a value indicating the damping to apply if the limit velocity factor is reached

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[limitVelocityDamping](../interfaces/IParticleSystem.md#limitvelocitydamping)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[limitVelocityDamping](BaseParticleSystem.md#limitvelocitydamping)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:375

___

### manualEmitCount

• **manualEmitCount**: `number` = `-1`

If you want to launch only a few particles at once, that can be done, as well.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[manualEmitCount](../interfaces/IParticleSystem.md#manualemitcount)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[manualEmitCount](BaseParticleSystem.md#manualemitcount)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:103

___

### maxAngularSpeed

• **maxAngularSpeed**: `number` = `0`

Maximum angular speed of emitting particles (Z-axis rotation for each particle).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxAngularSpeed](../interfaces/IParticleSystem.md#maxangularspeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxAngularSpeed](BaseParticleSystem.md#maxangularspeed)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:181

___

### maxEmitPower

• **maxEmitPower**: `number` = `1`

Maximum power of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxEmitPower](../interfaces/IParticleSystem.md#maxemitpower)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxEmitPower](BaseParticleSystem.md#maxemitpower)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:127

___

### maxInitialRotation

• **maxInitialRotation**: `number` = `0`

Gets or sets the maximal initial rotation in radians.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxInitialRotation](../interfaces/IParticleSystem.md#maxinitialrotation)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxInitialRotation](BaseParticleSystem.md#maxinitialrotation)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:172

___

### maxLifeTime

• **maxLifeTime**: `number` = `1`

Maximum life time of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxLifeTime](../interfaces/IParticleSystem.md#maxlifetime)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxLifeTime](BaseParticleSystem.md#maxlifetime)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:136

___

### maxScaleX

• **maxScaleX**: `number` = `1`

Maximum scale of emitting particles on X axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxScaleX](../interfaces/IParticleSystem.md#maxscalex)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxScaleX](BaseParticleSystem.md#maxscalex)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:154

___

### maxScaleY

• **maxScaleY**: `number` = `1`

Maximum scale of emitting particles on Y axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxScaleY](../interfaces/IParticleSystem.md#maxscaley)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxScaleY](BaseParticleSystem.md#maxscaley)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:163

___

### maxSize

• **maxSize**: `number` = `1`

Maximum Size of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[maxSize](../interfaces/IParticleSystem.md#maxsize)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[maxSize](BaseParticleSystem.md#maxsize)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:145

___

### minAngularSpeed

• **minAngularSpeed**: `number` = `0`

Minimum angular speed of emitting particles (Z-axis rotation for each particle).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minAngularSpeed](../interfaces/IParticleSystem.md#minangularspeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minAngularSpeed](BaseParticleSystem.md#minangularspeed)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:177

___

### minEmitPower

• **minEmitPower**: `number` = `1`

Minimum power of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minEmitPower](../interfaces/IParticleSystem.md#minemitpower)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minEmitPower](BaseParticleSystem.md#minemitpower)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:123

___

### minInitialRotation

• **minInitialRotation**: `number` = `0`

Gets or sets the minimal initial rotation in radians.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minInitialRotation](../interfaces/IParticleSystem.md#mininitialrotation)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minInitialRotation](BaseParticleSystem.md#mininitialrotation)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:168

___

### minLifeTime

• **minLifeTime**: `number` = `1`

Minimum life time of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minLifeTime](../interfaces/IParticleSystem.md#minlifetime)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minLifeTime](BaseParticleSystem.md#minlifetime)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:132

___

### minScaleX

• **minScaleX**: `number` = `1`

Minimum scale of emitting particles on X axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minScaleX](../interfaces/IParticleSystem.md#minscalex)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minScaleX](BaseParticleSystem.md#minscalex)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:150

___

### minScaleY

• **minScaleY**: `number` = `1`

Minimum scale of emitting particles on Y axis.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minScaleY](../interfaces/IParticleSystem.md#minscaley)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minScaleY](BaseParticleSystem.md#minscaley)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:159

___

### minSize

• **minSize**: `number` = `1`

Minimum Size of emitting particles.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[minSize](../interfaces/IParticleSystem.md#minsize)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[minSize](BaseParticleSystem.md#minsize)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:141

___

### name

• **name**: `string`

The friendly name of the Particle system.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[name](../interfaces/IParticleSystem.md#name)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[name](BaseParticleSystem.md#name)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:78

___

### noiseStrength

• **noiseStrength**: [`Vector3`](Vector3.md)

Gets or sets the strength to apply to the noise value (default is (10, 10, 10))

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[noiseStrength](../interfaces/IParticleSystem.md#noisestrength)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[noiseStrength](BaseParticleSystem.md#noisestrength)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:225

___

### onAnimationEnd

• **onAnimationEnd**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

Callback triggered when the particle animation is ending.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[onAnimationEnd](BaseParticleSystem.md#onanimationend)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:230

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`IParticleSystem`](../interfaces/IParticleSystem.md)

An event triggered when the system is disposed

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onDisposeObservable](../interfaces/IParticleSystem.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:101

___

### onStoppedObservable

• **onStoppedObservable**: [`Observable`](Observable.md)[`IParticleSystem`](../interfaces/IParticleSystem.md)

An event triggered when the system is stopped

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onStoppedObservable](../interfaces/IParticleSystem.md#onstoppedobservable)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:105

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

packages/dev/core/src/Particles/baseParticleSystem.ts:561

___

### particleTexture

• **particleTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The texture used to render each particle. (this can be a spritesheet)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[particleTexture](../interfaces/IParticleSystem.md#particletexture)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[particleTexture](BaseParticleSystem.md#particletexture)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:186

___

### preWarmCycles

• **preWarmCycles**: `number` = `0`

Gets or sets a value indicating how many cycles (or frames) must be executed before first rendering (this value has to be set before starting the system). Default is 0

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[preWarmCycles](../interfaces/IParticleSystem.md#prewarmcycles)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preWarmCycles](BaseParticleSystem.md#prewarmcycles)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:244

___

### preWarmStepOffset

• **preWarmStepOffset**: `number` = `1`

Gets or sets a value indicating the time step multiplier to use in pre-warm mode (default is 1)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[preWarmStepOffset](../interfaces/IParticleSystem.md#prewarmstepoffset)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preWarmStepOffset](BaseParticleSystem.md#prewarmstepoffset)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:247

___

### preventAutoStart

• **preventAutoStart**: `boolean` = `false`

By default particle system starts as soon as they are created. This prevents the
automatic start to happen and let you decide when to start emitting particles.

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[preventAutoStart](BaseParticleSystem.md#preventautostart)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:203

___

### recycleParticle

• **recycleParticle**: (`particle`: [`Particle`](Particle.md)) => `void`

#### Type declaration

▸ (`particle`): `void`

"Recycles" one of the particle by copying it back to the "stock" of particles and removing it from the active list.
Its lifetime will start back at 0.

##### Parameters

| Name | Type |
| :------ | :------ |
| `particle` | [`Particle`](Particle.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1407

___

### renderingGroupId

• **renderingGroupId**: `number` = `0`

The rendering group used by the Particle system to chose when to render.

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[renderingGroupId](../interfaces/IParticleSystem.md#renderinggroupid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[renderingGroupId](BaseParticleSystem.md#renderinggroupid)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:88

___

### snippetId

• **snippetId**: `string`

Snippet ID if the particle system was created from the snippet server

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[snippetId](../interfaces/IParticleSystem.md#snippetid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[snippetId](BaseParticleSystem.md#snippetid)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:83

___

### spriteCellChangeSpeed

• **spriteCellChangeSpeed**: `number` = `1`

If using a spritesheet (isAnimationSheetEnabled) defines the speed of the sprite loop (default is 1 meaning the animation will play once during the entire particle lifetime)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellChangeSpeed](../interfaces/IParticleSystem.md#spritecellchangespeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellChangeSpeed](BaseParticleSystem.md#spritecellchangespeed)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:252

___

### spriteCellHeight

• **spriteCellHeight**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell height to use

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellHeight](../interfaces/IParticleSystem.md#spritecellheight)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellHeight](BaseParticleSystem.md#spritecellheight)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:268

___

### spriteCellLoop

• **spriteCellLoop**: `boolean` = `true`

If using a spritesheet (isAnimationSheetEnabled), defines wether the sprite animation is looping

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellLoop](../interfaces/IParticleSystem.md#spritecellloop)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellLoop](BaseParticleSystem.md#spritecellloop)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:272

___

### spriteCellWidth

• **spriteCellWidth**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell width to use

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteCellWidth](../interfaces/IParticleSystem.md#spritecellwidth)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteCellWidth](BaseParticleSystem.md#spritecellwidth)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:264

___

### spriteRandomStartCell

• **spriteRandomStartCell**: `boolean` = `false`

This allows the system to random pick the start cell ID between startSpriteCellID and endSpriteCellID

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[spriteRandomStartCell](../interfaces/IParticleSystem.md#spriterandomstartcell)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[spriteRandomStartCell](BaseParticleSystem.md#spriterandomstartcell)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:276

___

### startDelay

• **startDelay**: `number` = `0`

Defines the delay in milliseconds before starting the system (0 by default)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[startDelay](../interfaces/IParticleSystem.md#startdelay)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[startDelay](BaseParticleSystem.md#startdelay)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:363

___

### startDirectionFunction

• **startDirectionFunction**: (`worldMatrix`: [`Matrix`](Matrix.md), `directionToUpdate`: [`Vector3`](Vector3.md), `particle`: [`Particle`](Particle.md), `isLocal`: `boolean`) => `void`

#### Type declaration

▸ (`worldMatrix`, `directionToUpdate`, `particle`, `isLocal`): `void`

This function can be defined to specify initial direction for every new particle.
It by default use the emitterType defined function

##### Parameters

| Name | Type |
| :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) |
| `directionToUpdate` | [`Vector3`](Vector3.md) |
| `particle` | [`Particle`](Particle.md) |
| `isLocal` | `boolean` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:87

___

### startPositionFunction

• **startPositionFunction**: (`worldMatrix`: [`Matrix`](Matrix.md), `positionToUpdate`: [`Vector3`](Vector3.md), `particle`: [`Particle`](Particle.md), `isLocal`: `boolean`) => `void`

#### Type declaration

▸ (`worldMatrix`, `positionToUpdate`, `particle`, `isLocal`): `void`

This function can be defined to specify initial position for every new particle.
It by default use the emitterType defined function

##### Parameters

| Name | Type |
| :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) |
| `positionToUpdate` | [`Vector3`](Vector3.md) |
| `particle` | [`Particle`](Particle.md) |
| `isLocal` | `boolean` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:92

___

### startSpriteCellID

• **startSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the first sprite cell to display

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[startSpriteCellID](../interfaces/IParticleSystem.md#startspritecellid)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[startSpriteCellID](BaseParticleSystem.md#startspritecellid)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:256

___

### subEmitters

• **subEmitters**: ([`ParticleSystem`](ParticleSystem.md) \| [`SubEmitter`](SubEmitter.md) \| [`SubEmitter`](SubEmitter.md)[])[]

The Sub-emitters templates that will be used to generate the sub particle system to be associated with the system, this property is used by the root particle system only.
When a particle is spawned, an array will be chosen at random and all the emitters in that array will be attached to the particle.  (Default: [])

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:191

___

### targetStopDuration

• **targetStopDuration**: `number` = `0`

The amount of time the particle system is running (depends of the overall update speed).

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[targetStopDuration](../interfaces/IParticleSystem.md#targetstopduration)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[targetStopDuration](BaseParticleSystem.md#targetstopduration)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:113

___

### textureMask

• **textureMask**: [`Color4`](Color4.md)

An optional mask to filter some colors out of the texture, or filter a part of the alpha channel

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[textureMask](BaseParticleSystem.md#texturemask)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:555

___

### translationPivot

• **translationPivot**: [`Vector2`](Vector2.md)

Gets or sets a Vector2 used to move the pivot (by default (0,0))

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[translationPivot](../interfaces/IParticleSystem.md#translationpivot)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[translationPivot](BaseParticleSystem.md#translationpivot)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:279

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the particle system

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[uniqueId](BaseParticleSystem.md#uniqueid)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:68

___

### updateFunction

• **updateFunction**: (`particles`: [`Particle`](Particle.md)[]) => `void`

#### Type declaration

▸ (`particles`): `void`

This function can be defined to provide custom update for active particles.
This function will be called instead of regular update (age, position, color, etc.).
Do not forget that this function will be called on every frame so try to keep it simple and fast :)

##### Parameters

| Name | Type |
| :------ | :------ |
| `particles` | [`Particle`](Particle.md)[] |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:78

___

### updateSpeed

• **updateSpeed**: `number` = `0.01`

The overall motion speed (0.01 is default update speed, faster updates = faster animation)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[updateSpeed](../interfaces/IParticleSystem.md#updatespeed)

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[updateSpeed](BaseParticleSystem.md#updatespeed)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:108

___

### worldOffset

• **worldOffset**: [`Vector3`](Vector3.md)

Gets or sets a world offset applied to all particles

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[worldOffset](BaseParticleSystem.md#worldoffset)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:307

___

### BILLBOARDMODE\_ALL

▪ `Static` `Readonly` **BILLBOARDMODE\_ALL**: ``7``

Billboard mode will apply to all axes

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:67

___

### BILLBOARDMODE\_STRETCHED

▪ `Static` `Readonly` **BILLBOARDMODE\_STRETCHED**: ``8``

Special billboard mode where the particle will be biilboard to the camera but rotated to align with direction

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:71

___

### BILLBOARDMODE\_Y

▪ `Static` `Readonly` **BILLBOARDMODE\_Y**: ``2``

Billboard mode will only apply to Y axis

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:63

___

### BLENDMODE\_ADD

▪ `Static` **BLENDMODE\_ADD**: `number` = `2`

Add current color and particle color multiplied by particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_ADD](BaseParticleSystem.md#blendmode_add)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:49

___

### BLENDMODE\_MULTIPLY

▪ `Static` **BLENDMODE\_MULTIPLY**: `number` = `3`

Multiply current color with particle color

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_MULTIPLY](BaseParticleSystem.md#blendmode_multiply)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:53

___

### BLENDMODE\_MULTIPLYADD

▪ `Static` **BLENDMODE\_MULTIPLYADD**: `number` = `4`

Multiply current color with particle color then add current color and particle color multiplied by particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_MULTIPLYADD](BaseParticleSystem.md#blendmode_multiplyadd)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:58

___

### BLENDMODE\_ONEONE

▪ `Static` **BLENDMODE\_ONEONE**: `number` = `0`

Source color is added to the destination color without alpha affecting the result

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_ONEONE](BaseParticleSystem.md#blendmode_oneone)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:41

___

### BLENDMODE\_STANDARD

▪ `Static` **BLENDMODE\_STANDARD**: `number` = `1`

Blend current color and particle color using particle’s alpha

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[BLENDMODE_STANDARD](BaseParticleSystem.md#blendmode_standard)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:45

## Accessors

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

packages/dev/core/src/Particles/baseParticleSystem.ts:572

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

packages/dev/core/src/Particles/baseParticleSystem.ts:576

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

packages/dev/core/src/Particles/baseParticleSystem.ts:471

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

packages/dev/core/src/Particles/baseParticleSystem.ts:479

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

packages/dev/core/src/Particles/baseParticleSystem.ts:489

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

packages/dev/core/src/Particles/baseParticleSystem.ts:497

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Inherited from

BaseParticleSystem.imageProcessingConfiguration

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:626

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

packages/dev/core/src/Particles/baseParticleSystem.ts:635

___

### indexBuffer

• `get` **indexBuffer**(): [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

Gets the index buffer used by the particle system (or null if no index buffer is used (if _useInstancing=true))

#### Returns

[`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:300

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

packages/dev/core/src/Particles/baseParticleSystem.ts:312

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

packages/dev/core/src/Particles/baseParticleSystem.ts:316

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

packages/dev/core/src/Particles/baseParticleSystem.ts:590

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

packages/dev/core/src/Particles/baseParticleSystem.ts:594

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

packages/dev/core/src/Particles/baseParticleSystem.ts:525

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

packages/dev/core/src/Particles/baseParticleSystem.ts:533

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

packages/dev/core/src/Particles/baseParticleSystem.ts:507

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

packages/dev/core/src/Particles/baseParticleSystem.ts:515

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

packages/dev/core/src/Particles/baseParticleSystem.ts:211

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

packages/dev/core/src/Particles/baseParticleSystem.ts:215

___

### onBeforeDrawParticlesObservable

• `get` **onBeforeDrawParticlesObservable**(): [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Observable that will be called just before the particles are drawn

#### Returns

[`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[onBeforeDrawParticlesObservable](../interfaces/IParticleSystem.md#onbeforedrawparticlesobservable)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:275

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Sets a callback that will be triggered when the system is disposed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:111

___

### particles

• `get` **particles**(): [`Particle`](Particle.md)[]

Gets the current list of active particles

#### Returns

[`Particle`](Particle.md)[]

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:215

___

### useRampGradients

• `get` **useRampGradients**(): `boolean`

Gets or sets a boolean indicating that ramp gradients must be used

**`See`**

https://doc.babylonjs.com/babylon101/particles#ramp-gradients

#### Returns

`boolean`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[useRampGradients](../interfaces/IParticleSystem.md#userampgradients)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:172

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

packages/dev/core/src/Particles/particleSystem.ts:176

___

### vertexBuffers

• `get` **vertexBuffers**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject){ `[key: string]`: [`VertexBuffer`](VertexBuffer.md);  }

Gets the vertex buffers used by the particle system

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject){ `[key: string]`: [`VertexBuffer`](VertexBuffer.md);  }

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:293

___

### vertexShaderName

• `get` **vertexShaderName**(): `string`

Gets the name of the particle vertex shader

#### Returns

`string`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[vertexShaderName](../interfaces/IParticleSystem.md#vertexshadername)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:286

## Methods

### \_addFactorGradient

▸ `Private` **_addFactorGradient**(`factorGradients`, `gradient`, `factor`, `factor2?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `factorGradients` | [`FactorGradient`](FactorGradient.md)[] |
| `gradient` | `number` |
| `factor` | `number` |
| `factor2?` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:581

___

### \_appendParticleVertices

▸ `Private` **_appendParticleVertices**(`offset`, `particle`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `offset` | `number` |
| `particle` | [`Particle`](Particle.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1982

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

packages/dev/core/src/Particles/baseParticleSystem.ts:643

___

### \_createIndexBuffer

▸ `Private` **_createIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1151

___

### \_createRampGradientTexture

▸ `Private` **_createRampGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:889

___

### \_createVertexBuffers

▸ `Private` **_createVertexBuffers**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1083

___

### \_fetchR

▸ `Private` **_fetchR**(`u`, `v`, `width`, `height`, `pixels`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `u` | `number` |
| `v` | `number` |
| `width` | `number` |
| `height` | `number` |
| `pixels` | `Uint8Array` |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1049

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

packages/dev/core/src/Particles/particleSystem.ts:252

___

### \_hasTargetStopDurationDependantGradient

▸ `Protected` **_hasTargetStopDurationDependantGradient**(): ``null`` \| `boolean`

#### Returns

``null`` \| `boolean`

#### Inherited from

[BaseParticleSystem](BaseParticleSystem.md).[_hasTargetStopDurationDependantGradient](BaseParticleSystem.md#_hastargetstopdurationdependantgradient)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:352

___

### \_prepareSubEmitterInternalArray

▸ `Private` **_prepareSubEmitterInternalArray**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1194

___

### \_removeFactorGradient

▸ `Private` **_removeFactorGradient**(`factorGradients`, `gradient`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `factorGradients` | [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] |
| `gradient` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:596

___

### \_removeFromRoot

▸ `Private` **_removeFromRoot**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1450

___

### \_render

▸ `Private` **_render**(`blendMode`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `blendMode` | `number` |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:2037

___

### \_reset

▸ `Protected` **_reset**(): `void`

#### Returns

`void`

#### Overrides

BaseParticleSystem.\_reset

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1060

___

### \_resetEffect

▸ `Private` **_resetEffect**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1064

___

### \_stopSubEmitters

▸ `Private` **_stopSubEmitters**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1416

___

### \_syncRampGradientTexture

▸ `Private` **_syncRampGradientTexture**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:926

___

### \_update

▸ `Private` **_update**(`newParticles`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newParticles` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1482

___

### addAlphaRemapGradient

▸ **addAlphaRemapGradient**(`gradient`, `min`, `max`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new alpha remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `min` | `number` | defines the alpha remap minimal range |
| `max` | `number` | defines the alpha remap maximal range |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addAlphaRemapGradient](../interfaces/IParticleSystem.md#addalpharemapgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:702

___

### addAngularSpeedGradient

▸ **addAngularSpeedGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the angular speed  to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addAngularSpeedGradient](../interfaces/IParticleSystem.md#addangularspeedgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:730

___

### addColorGradient

▸ **addColorGradient**(`gradient`, `color1`, `color2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `color1` | [`Color4`](Color4.md) | defines the color to affect to the specified gradient |
| `color2?` | [`Color4`](Color4.md) | defines an additional color used to define a range ([color, color2]) with main color to pick the final color from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

this particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addColorGradient](../interfaces/IParticleSystem.md#addcolorgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:991

___

### addColorRemapGradient

▸ **addColorRemapGradient**(`gradient`, `min`, `max`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new color remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `min` | `number` | defines the color remap minimal range |
| `max` | `number` | defines the color remap maximal range |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addColorRemapGradient](../interfaces/IParticleSystem.md#addcolorremapgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:674

___

### addDragGradient

▸ **addDragGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the drag value to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addDragGradient](../interfaces/IParticleSystem.md#adddraggradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:814

___

### addEmitRateGradient

▸ **addEmitRateGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new emit rate gradient (please note that this will only work if you set the targetStopDuration property)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the emit rate value to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addEmitRateGradient](../interfaces/IParticleSystem.md#addemitrategradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:842

___

### addLifeTimeGradient

▸ **addLifeTimeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new life time gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the life time factor to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addLifeTimeGradient](../interfaces/IParticleSystem.md#addlifetimegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:618

___

### addLimitVelocityGradient

▸ **addLimitVelocityGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the limit velocity value to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addLimitVelocityGradient](../interfaces/IParticleSystem.md#addlimitvelocitygradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:786

___

### addRampGradient

▸ **addRampGradient**(`gradient`, `color`): [`ParticleSystem`](ParticleSystem.md)

Adds a new ramp gradient used to remap particle colors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `color` | [`Color3`](Color3.md) | defines the color to affect to the specified gradient |

#### Returns

[`ParticleSystem`](ParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addRampGradient](../interfaces/IParticleSystem.md#addrampgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:955

___

### addSizeGradient

▸ **addSizeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the size factor to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addSizeGradient](../interfaces/IParticleSystem.md#addsizegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:646

___

### addStartSizeGradient

▸ **addStartSizeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new start size gradient (please note that this will only work if you set the targetStopDuration property)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the start size value to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addStartSizeGradient](../interfaces/IParticleSystem.md#addstartsizegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:869

___

### addVelocityGradient

▸ **addVelocityGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Adds a new velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the velocity to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[addVelocityGradient](../interfaces/IParticleSystem.md#addvelocitygradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:758

___

### animate

▸ **animate**(`preWarmOnly?`): `void`

Animates the particle system for the current frame by emitting new particles and or animating the living ones.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `preWarmOnly` | `boolean` | `false` | will prevent the system from updating the vertex buffer (default is false) |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[animate](../interfaces/IParticleSystem.md#animate)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1886

___

### clone

▸ **clone**(`name`, `newEmitter`): [`ParticleSystem`](ParticleSystem.md)

Clones the particle system.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the cloned object |
| `newEmitter` | `any` | The new emitter to use |

#### Returns

[`ParticleSystem`](ParticleSystem.md)

the cloned particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[clone](../interfaces/IParticleSystem.md#clone)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:2254

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

packages/dev/core/src/Particles/baseParticleSystem.ts:803

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

packages/dev/core/src/Particles/baseParticleSystem.ts:789

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

packages/dev/core/src/Particles/baseParticleSystem.ts:756

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

packages/dev/core/src/Particles/baseParticleSystem.ts:771

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

packages/dev/core/src/Particles/baseParticleSystem.ts:742

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

packages/dev/core/src/Particles/baseParticleSystem.ts:717

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

packages/dev/core/src/Particles/baseParticleSystem.ts:702

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

packages/dev/core/src/Particles/baseParticleSystem.ts:729

___

### dispose

▸ **dispose**(`disposeTexture?`): `void`

Disposes the particle system and free the associated resources

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposeTexture` | `boolean` | `true` | defines if the particle texture must be disposed as well (true by default) |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[dispose](../interfaces/IParticleSystem.md#dispose)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:2166

___

### fillDefines

▸ **fillDefines**(`defines`, `blendMode`): `void`

Fill the defines array according to the current settings of the particle system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `string`[] | Array to be updated |
| `blendMode` | `number` | blend mode to take into account when updating the array |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[fillDefines](../interfaces/IParticleSystem.md#filldefines)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1750

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

packages/dev/core/src/Particles/particleSystem.ts:1819

___

### forceRefreshGradients

▸ **forceRefreshGradients**(): `void`

Force the system to rebuild all gradients that need to be resync

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[forceRefreshGradients](../interfaces/IParticleSystem.md#forcerefreshgradients)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:922

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

packages/dev/core/src/Particles/particleSystem.ts:223

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

packages/dev/core/src/Particles/baseParticleSystem.ts:418

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

packages/dev/core/src/Particles/baseParticleSystem.ts:436

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

packages/dev/core/src/Particles/particleSystem.ts:1174

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "ParticleSystem"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getClassName](../interfaces/IParticleSystem.md#getclassname)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:231

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

packages/dev/core/src/Particles/baseParticleSystem.ts:391

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

packages/dev/core/src/Particles/baseParticleSystem.ts:409

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

packages/dev/core/src/Particles/particleSystem.ts:248

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

packages/dev/core/src/Particles/baseParticleSystem.ts:370

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

packages/dev/core/src/Particles/baseParticleSystem.ts:463

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

packages/dev/core/src/Particles/baseParticleSystem.ts:427

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

packages/dev/core/src/Particles/baseParticleSystem.ts:382

___

### getRampGradients

▸ **getRampGradients**(): [`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[]

Gets the current list of ramp gradients.
You must use addRampGradient and removeRampGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[]

the list of ramp gradients

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[getRampGradients](../interfaces/IParticleSystem.md#getrampgradients)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:917

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

packages/dev/core/src/Particles/baseParticleSystem.ts:330

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

packages/dev/core/src/Particles/baseParticleSystem.ts:400

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

packages/dev/core/src/Particles/baseParticleSystem.ts:454

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

packages/dev/core/src/Particles/baseParticleSystem.ts:445

___

### isAlive

▸ **isAlive**(): `boolean`

Gets whether there are still active particles in the system.

#### Returns

`boolean`

True if it is alive, otherwise false.

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1182

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

packages/dev/core/src/Particles/particleSystem.ts:2016

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

packages/dev/core/src/Particles/particleSystem.ts:1190

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

packages/dev/core/src/Particles/particleSystem.ts:239

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the particle system.

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[rebuild](../interfaces/IParticleSystem.md#rebuild)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1994

___

### removeAlphaRemapGradient

▸ **removeAlphaRemapGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific alpha remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:717

___

### removeAngularSpeedGradient

▸ **removeAngularSpeedGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeAngularSpeedGradient](../interfaces/IParticleSystem.md#removeangularspeedgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:745

___

### removeColorGradient

▸ **removeColorGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

this particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeColorGradient](../interfaces/IParticleSystem.md#removecolorgradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1017

___

### removeColorRemapGradient

▸ **removeColorRemapGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific color remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:689

___

### removeDragGradient

▸ **removeDragGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeDragGradient](../interfaces/IParticleSystem.md#removedraggradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:829

___

### removeEmitRateGradient

▸ **removeEmitRateGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific emit rate gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeEmitRateGradient](../interfaces/IParticleSystem.md#removeemitrategradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:856

___

### removeLifeTimeGradient

▸ **removeLifeTimeGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific life time gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeLifeTimeGradient](../interfaces/IParticleSystem.md#removelifetimegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:633

___

### removeLimitVelocityGradient

▸ **removeLimitVelocityGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeLimitVelocityGradient](../interfaces/IParticleSystem.md#removelimitvelocitygradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:801

___

### removeRampGradient

▸ **removeRampGradient**(`gradient`): [`ParticleSystem`](ParticleSystem.md)

Remove a specific ramp gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`ParticleSystem`](ParticleSystem.md)

the current particle system

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:973

___

### removeSizeGradient

▸ **removeSizeGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeSizeGradient](../interfaces/IParticleSystem.md#removesizegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:661

___

### removeStartSizeGradient

▸ **removeStartSizeGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific start size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeStartSizeGradient](../interfaces/IParticleSystem.md#removestartsizegradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:883

___

### removeVelocityGradient

▸ **removeVelocityGradient**(`gradient`): [`IParticleSystem`](../interfaces/IParticleSystem.md)

Remove a specific velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)

the current particle system

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[removeVelocityGradient](../interfaces/IParticleSystem.md#removevelocitygradient)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:773

___

### render

▸ **render**(): `number`

Renders the particle system in its current state.

#### Returns

`number`

the current number of particles

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[render](../interfaces/IParticleSystem.md#render)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:2133

___

### reset

▸ **reset**(): `void`

Remove all active particles

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[reset](../interfaces/IParticleSystem.md#reset)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1308

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1037

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

packages/dev/core/src/Particles/particleSystem.ts:2298

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

packages/dev/core/src/Particles/particleSystem.ts:261

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

packages/dev/core/src/Particles/particleSystem.ts:1213

___

### stop

▸ **stop**(`stopSubEmitters?`): `void`

Stops the particle system.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `stopSubEmitters` | `boolean` | `true` | if true it will stop the current system and all created sub-Systems if false it will stop the current root system only, this param is used by the root particle system only. the default value is true. |

#### Returns

`void`

#### Implementation of

[IParticleSystem](../interfaces/IParticleSystem.md).[stop](../interfaces/IParticleSystem.md#stop)

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:1289

___

### Parse

▸ `Static` **Parse**(`parsedParticleSystem`, `sceneOrEngine`, `rootUrl`, `doNotStart?`, `capacity?`): [`ParticleSystem`](ParticleSystem.md)

Parses a JSON object to create a particle system.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `parsedParticleSystem` | `any` | `undefined` | The JSON object to parse |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | `undefined` | The scene or the engine to create the particle system in |
| `rootUrl` | `string` | `undefined` | The root url to use to load external dependencies like texture |
| `doNotStart` | `boolean` | `false` | Ignore the preventAutoStart attribute and does not start |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

[`ParticleSystem`](ParticleSystem.md)

the Parsed particle system

#### Defined in

packages/dev/core/src/Particles/particleSystem.ts:2945

[@dev/core](../README.md) / [Exports](../modules.md) / BaseParticleSystem

# Class: BaseParticleSystem

This represents the base class for particle system in Babylon.
Particles are often small sprites used to simulate hard-to-reproduce phenomena like fire, smoke, water, or abstract visual effects like magic glitter and faery dust.
Particles can take different shapes while emitted like box, sphere, cone or you can write your custom function.

**`Example`**

```ts
https://doc.babylonjs.com/babylon101/particles
```

## Hierarchy

- **`BaseParticleSystem`**

  ↳ [`GPUParticleSystem`](GPUParticleSystem.md)

  ↳ [`ParticleSystem`](ParticleSystem.md)

## Table of contents

### Constructors

- [constructor](BaseParticleSystem.md#constructor)

### Properties

- [\_alphaRemapGradients](BaseParticleSystem.md#_alpharemapgradients)
- [\_angularSpeedGradients](BaseParticleSystem.md#_angularspeedgradients)
- [\_colorGradients](BaseParticleSystem.md#_colorgradients)
- [\_colorRemapGradients](BaseParticleSystem.md#_colorremapgradients)
- [\_dragGradients](BaseParticleSystem.md#_draggradients)
- [\_emitRateGradients](BaseParticleSystem.md#_emitrategradients)
- [\_engine](BaseParticleSystem.md#_engine)
- [\_imageProcessingConfiguration](BaseParticleSystem.md#_imageprocessingconfiguration)
- [\_imageProcessingConfigurationDefines](BaseParticleSystem.md#_imageprocessingconfigurationdefines)
- [\_lifeTimeGradients](BaseParticleSystem.md#_lifetimegradients)
- [\_limitVelocityGradients](BaseParticleSystem.md#_limitvelocitygradients)
- [\_noiseTexture](BaseParticleSystem.md#_noisetexture)
- [\_rampGradients](BaseParticleSystem.md#_rampgradients)
- [\_rootUrl](BaseParticleSystem.md#_rooturl)
- [\_scene](BaseParticleSystem.md#_scene)
- [\_sizeGradients](BaseParticleSystem.md#_sizegradients)
- [\_startSizeGradients](BaseParticleSystem.md#_startsizegradients)
- [\_velocityGradients](BaseParticleSystem.md#_velocitygradients)
- [animations](BaseParticleSystem.md#animations)
- [beginAnimationFrom](BaseParticleSystem.md#beginanimationfrom)
- [beginAnimationLoop](BaseParticleSystem.md#beginanimationloop)
- [beginAnimationOnStart](BaseParticleSystem.md#beginanimationonstart)
- [beginAnimationTo](BaseParticleSystem.md#beginanimationto)
- [blendMode](BaseParticleSystem.md#blendmode)
- [color1](BaseParticleSystem.md#color1)
- [color2](BaseParticleSystem.md#color2)
- [colorDead](BaseParticleSystem.md#colordead)
- [customShader](BaseParticleSystem.md#customshader)
- [disposeOnStop](BaseParticleSystem.md#disposeonstop)
- [emitRate](BaseParticleSystem.md#emitrate)
- [emitter](BaseParticleSystem.md#emitter)
- [endSpriteCellID](BaseParticleSystem.md#endspritecellid)
- [forceDepthWrite](BaseParticleSystem.md#forcedepthwrite)
- [gravity](BaseParticleSystem.md#gravity)
- [id](BaseParticleSystem.md#id)
- [layerMask](BaseParticleSystem.md#layermask)
- [limitVelocityDamping](BaseParticleSystem.md#limitvelocitydamping)
- [manualEmitCount](BaseParticleSystem.md#manualemitcount)
- [maxAngularSpeed](BaseParticleSystem.md#maxangularspeed)
- [maxEmitPower](BaseParticleSystem.md#maxemitpower)
- [maxInitialRotation](BaseParticleSystem.md#maxinitialrotation)
- [maxLifeTime](BaseParticleSystem.md#maxlifetime)
- [maxScaleX](BaseParticleSystem.md#maxscalex)
- [maxScaleY](BaseParticleSystem.md#maxscaley)
- [maxSize](BaseParticleSystem.md#maxsize)
- [minAngularSpeed](BaseParticleSystem.md#minangularspeed)
- [minEmitPower](BaseParticleSystem.md#minemitpower)
- [minInitialRotation](BaseParticleSystem.md#mininitialrotation)
- [minLifeTime](BaseParticleSystem.md#minlifetime)
- [minScaleX](BaseParticleSystem.md#minscalex)
- [minScaleY](BaseParticleSystem.md#minscaley)
- [minSize](BaseParticleSystem.md#minsize)
- [name](BaseParticleSystem.md#name)
- [noiseStrength](BaseParticleSystem.md#noisestrength)
- [onAnimationEnd](BaseParticleSystem.md#onanimationend)
- [particleEmitterType](BaseParticleSystem.md#particleemittertype)
- [particleTexture](BaseParticleSystem.md#particletexture)
- [preWarmCycles](BaseParticleSystem.md#prewarmcycles)
- [preWarmStepOffset](BaseParticleSystem.md#prewarmstepoffset)
- [preventAutoStart](BaseParticleSystem.md#preventautostart)
- [renderingGroupId](BaseParticleSystem.md#renderinggroupid)
- [snippetId](BaseParticleSystem.md#snippetid)
- [spriteCellChangeSpeed](BaseParticleSystem.md#spritecellchangespeed)
- [spriteCellHeight](BaseParticleSystem.md#spritecellheight)
- [spriteCellLoop](BaseParticleSystem.md#spritecellloop)
- [spriteCellWidth](BaseParticleSystem.md#spritecellwidth)
- [spriteRandomStartCell](BaseParticleSystem.md#spriterandomstartcell)
- [startDelay](BaseParticleSystem.md#startdelay)
- [startSpriteCellID](BaseParticleSystem.md#startspritecellid)
- [targetStopDuration](BaseParticleSystem.md#targetstopduration)
- [textureMask](BaseParticleSystem.md#texturemask)
- [translationPivot](BaseParticleSystem.md#translationpivot)
- [uniqueId](BaseParticleSystem.md#uniqueid)
- [updateSpeed](BaseParticleSystem.md#updatespeed)
- [worldOffset](BaseParticleSystem.md#worldoffset)
- [BLENDMODE\_ADD](BaseParticleSystem.md#blendmode_add)
- [BLENDMODE\_MULTIPLY](BaseParticleSystem.md#blendmode_multiply)
- [BLENDMODE\_MULTIPLYADD](BaseParticleSystem.md#blendmode_multiplyadd)
- [BLENDMODE\_ONEONE](BaseParticleSystem.md#blendmode_oneone)
- [BLENDMODE\_STANDARD](BaseParticleSystem.md#blendmode_standard)

### Accessors

- [billboardMode](BaseParticleSystem.md#billboardmode)
- [direction1](BaseParticleSystem.md#direction1)
- [direction2](BaseParticleSystem.md#direction2)
- [imageProcessingConfiguration](BaseParticleSystem.md#imageprocessingconfiguration)
- [isAnimationSheetEnabled](BaseParticleSystem.md#isanimationsheetenabled)
- [isBillboardBased](BaseParticleSystem.md#isbillboardbased)
- [maxEmitBox](BaseParticleSystem.md#maxemitbox)
- [minEmitBox](BaseParticleSystem.md#minemitbox)
- [noiseTexture](BaseParticleSystem.md#noisetexture)

### Methods

- [\_attachImageProcessingConfiguration](BaseParticleSystem.md#_attachimageprocessingconfiguration)
- [\_hasTargetStopDurationDependantGradient](BaseParticleSystem.md#_hastargetstopdurationdependantgradient)
- [createBoxEmitter](BaseParticleSystem.md#createboxemitter)
- [createConeEmitter](BaseParticleSystem.md#createconeemitter)
- [createCylinderEmitter](BaseParticleSystem.md#createcylinderemitter)
- [createDirectedCylinderEmitter](BaseParticleSystem.md#createdirectedcylinderemitter)
- [createDirectedSphereEmitter](BaseParticleSystem.md#createdirectedsphereemitter)
- [createHemisphericEmitter](BaseParticleSystem.md#createhemisphericemitter)
- [createPointEmitter](BaseParticleSystem.md#createpointemitter)
- [createSphereEmitter](BaseParticleSystem.md#createsphereemitter)
- [getAlphaRemapGradients](BaseParticleSystem.md#getalpharemapgradients)
- [getAngularSpeedGradients](BaseParticleSystem.md#getangularspeedgradients)
- [getColorGradients](BaseParticleSystem.md#getcolorgradients)
- [getColorRemapGradients](BaseParticleSystem.md#getcolorremapgradients)
- [getDragGradients](BaseParticleSystem.md#getdraggradients)
- [getEmitRateGradients](BaseParticleSystem.md#getemitrategradients)
- [getLifeTimeGradients](BaseParticleSystem.md#getlifetimegradients)
- [getLimitVelocityGradients](BaseParticleSystem.md#getlimitvelocitygradients)
- [getScene](BaseParticleSystem.md#getscene)
- [getSizeGradients](BaseParticleSystem.md#getsizegradients)
- [getStartSizeGradients](BaseParticleSystem.md#getstartsizegradients)
- [getVelocityGradients](BaseParticleSystem.md#getvelocitygradients)

## Constructors

### constructor

• **new BaseParticleSystem**(`name`)

Instantiates a particle system.
Particles are often small sprites used to simulate hard-to-reproduce phenomena like fire, smoke, water, or abstract visual effects like magic glitter and faery dust.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the particle system |

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:691

## Properties

### \_alphaRemapGradients

• `Protected` **\_alphaRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:350

___

### \_angularSpeedGradients

• `Protected` **\_angularSpeedGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:342

___

### \_colorGradients

• `Protected` **\_colorGradients**: [`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:339

___

### \_colorRemapGradients

• `Protected` **\_colorRemapGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:349

___

### \_dragGradients

• `Protected` **\_dragGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:345

___

### \_emitRateGradients

• `Protected` **\_emitRateGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:346

___

### \_engine

• `Protected` **\_engine**: [`ThinEngine`](ThinEngine.md)

The engine the particle system belongs to.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:611

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the standard Material.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:621

___

### \_imageProcessingConfigurationDefines

• `Protected` **\_imageProcessingConfigurationDefines**: `ImageProcessingConfigurationDefines`

Local cache of defines for image processing.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:616

___

### \_lifeTimeGradients

• `Protected` **\_lifeTimeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:341

___

### \_limitVelocityGradients

• `Protected` **\_limitVelocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:344

___

### \_noiseTexture

• `Private` **\_noiseTexture**: [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:206

___

### \_rampGradients

• `Protected` **\_rampGradients**: [`Nullable`](../modules.md#nullable)[`Color3Gradient`](Color3Gradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:348

___

### \_rootUrl

• `Protected` **\_rootUrl**: `string` = `""`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:205

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

The scene the particle system belongs to.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:606

___

### \_sizeGradients

• `Protected` **\_sizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:340

___

### \_startSizeGradients

• `Protected` **\_startSizeGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:347

___

### \_velocityGradients

• `Protected` **\_velocityGradients**: [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[] = `null`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:343

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

List of animations used by the particle system.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:63

___

### beginAnimationFrom

• **beginAnimationFrom**: `number` = `0`

Gets or sets the frame to start the animation from when beginAnimationOnStart is true

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:292

___

### beginAnimationLoop

• **beginAnimationLoop**: `boolean` = `false`

Gets or sets a boolean indicating if animations must loop when beginAnimationOnStart is true

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:302

___

### beginAnimationOnStart

• **beginAnimationOnStart**: `boolean` = `false`

Gets or sets a boolean indicating that hosted animations (in the system.animations array) must be started when system.start() is called

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:287

___

### beginAnimationTo

• **beginAnimationTo**: `number` = `60`

Gets or sets the frame to end the animation on when beginAnimationOnStart is true

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:297

___

### blendMode

• **blendMode**: `number` = `BaseParticleSystem.BLENDMODE_ONEONE`

Blend mode use to render the particle, it can be either ParticleSystem.BLENDMODE_ONEONE or ParticleSystem.BLENDMODE_STANDARD.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:235

___

### color1

• **color1**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:542

___

### color2

• **color2**: [`Color4`](Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:546

___

### colorDead

• **colorDead**: [`Color4`](Color4.md)

Color the particle will have at the end of its lifetime

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:550

___

### customShader

• **customShader**: `any` = `null`

This can help using your own shader to render the particle system.
The according effect will be created

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:197

___

### disposeOnStop

• **disposeOnStop**: `boolean` = `false`

Specifies whether the particle system will be disposed once it reaches the end of the animation.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:118

___

### emitRate

• **emitRate**: `number` = `10`

The maximum number of particles to emit per frame

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:98

___

### emitter

• **emitter**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

The emitter represents the Mesh or position we are attaching the particle system to.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:93

___

### endSpriteCellID

• **endSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the last sprite cell to display

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:260

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Forces the particle to write their depth information to the depth buffer. This can help preventing other draw calls
to override the particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:241

___

### gravity

• **gravity**: [`Vector3`](Vector3.md)

You can use gravity if you want to give an orientation to your particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:337

___

### id

• **id**: `string`

The id of the Particle system.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:73

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

The layer mask we are rendering the particles through.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:191

___

### limitVelocityDamping

• **limitVelocityDamping**: `number` = `0.4`

Gets or sets a value indicating the damping to apply if the limit velocity factor is reached

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:375

___

### manualEmitCount

• **manualEmitCount**: `number` = `-1`

If you want to launch only a few particles at once, that can be done, as well.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:103

___

### maxAngularSpeed

• **maxAngularSpeed**: `number` = `0`

Maximum angular speed of emitting particles (Z-axis rotation for each particle).

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:181

___

### maxEmitPower

• **maxEmitPower**: `number` = `1`

Maximum power of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:127

___

### maxInitialRotation

• **maxInitialRotation**: `number` = `0`

Gets or sets the maximal initial rotation in radians.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:172

___

### maxLifeTime

• **maxLifeTime**: `number` = `1`

Maximum life time of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:136

___

### maxScaleX

• **maxScaleX**: `number` = `1`

Maximum scale of emitting particles on X axis.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:154

___

### maxScaleY

• **maxScaleY**: `number` = `1`

Maximum scale of emitting particles on Y axis.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:163

___

### maxSize

• **maxSize**: `number` = `1`

Maximum Size of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:145

___

### minAngularSpeed

• **minAngularSpeed**: `number` = `0`

Minimum angular speed of emitting particles (Z-axis rotation for each particle).

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:177

___

### minEmitPower

• **minEmitPower**: `number` = `1`

Minimum power of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:123

___

### minInitialRotation

• **minInitialRotation**: `number` = `0`

Gets or sets the minimal initial rotation in radians.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:168

___

### minLifeTime

• **minLifeTime**: `number` = `1`

Minimum life time of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:132

___

### minScaleX

• **minScaleX**: `number` = `1`

Minimum scale of emitting particles on X axis.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:150

___

### minScaleY

• **minScaleY**: `number` = `1`

Minimum scale of emitting particles on Y axis.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:159

___

### minSize

• **minSize**: `number` = `1`

Minimum Size of emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:141

___

### name

• **name**: `string`

The friendly name of the Particle system.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:78

___

### noiseStrength

• **noiseStrength**: [`Vector3`](Vector3.md)

Gets or sets the strength to apply to the noise value (default is (10, 10, 10))

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:225

___

### onAnimationEnd

• **onAnimationEnd**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

Callback triggered when the particle animation is ending.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:230

___

### particleEmitterType

• **particleEmitterType**: [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

The particle emitter type defines the emitter used by the particle system.
It can be for example box, sphere, or cone...

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:561

___

### particleTexture

• **particleTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The texture used to render each particle. (this can be a spritesheet)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:186

___

### preWarmCycles

• **preWarmCycles**: `number` = `0`

Gets or sets a value indicating how many cycles (or frames) must be executed before first rendering (this value has to be set before starting the system). Default is 0

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:244

___

### preWarmStepOffset

• **preWarmStepOffset**: `number` = `1`

Gets or sets a value indicating the time step multiplier to use in pre-warm mode (default is 1)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:247

___

### preventAutoStart

• **preventAutoStart**: `boolean` = `false`

By default particle system starts as soon as they are created. This prevents the
automatic start to happen and let you decide when to start emitting particles.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:203

___

### renderingGroupId

• **renderingGroupId**: `number` = `0`

The rendering group used by the Particle system to chose when to render.

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:88

___

### snippetId

• **snippetId**: `string`

Snippet ID if the particle system was created from the snippet server

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:83

___

### spriteCellChangeSpeed

• **spriteCellChangeSpeed**: `number` = `1`

If using a spritesheet (isAnimationSheetEnabled) defines the speed of the sprite loop (default is 1 meaning the animation will play once during the entire particle lifetime)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:252

___

### spriteCellHeight

• **spriteCellHeight**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell height to use

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:268

___

### spriteCellLoop

• **spriteCellLoop**: `boolean` = `true`

If using a spritesheet (isAnimationSheetEnabled), defines wether the sprite animation is looping

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:272

___

### spriteCellWidth

• **spriteCellWidth**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell width to use

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:264

___

### spriteRandomStartCell

• **spriteRandomStartCell**: `boolean` = `false`

This allows the system to random pick the start cell ID between startSpriteCellID and endSpriteCellID

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:276

___

### startDelay

• **startDelay**: `number` = `0`

Defines the delay in milliseconds before starting the system (0 by default)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:363

___

### startSpriteCellID

• **startSpriteCellID**: `number` = `0`

If using a spritesheet (isAnimationSheetEnabled) defines the first sprite cell to display

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:256

___

### targetStopDuration

• **targetStopDuration**: `number` = `0`

The amount of time the particle system is running (depends of the overall update speed).

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:113

___

### textureMask

• **textureMask**: [`Color4`](Color4.md)

An optional mask to filter some colors out of the texture, or filter a part of the alpha channel

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:555

___

### translationPivot

• **translationPivot**: [`Vector2`](Vector2.md)

Gets or sets a Vector2 used to move the pivot (by default (0,0))

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:279

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the particle system

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:68

___

### updateSpeed

• **updateSpeed**: `number` = `0.01`

The overall motion speed (0.01 is default update speed, faster updates = faster animation)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:108

___

### worldOffset

• **worldOffset**: [`Vector3`](Vector3.md)

Gets or sets a world offset applied to all particles

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:307

___

### BLENDMODE\_ADD

▪ `Static` **BLENDMODE\_ADD**: `number` = `2`

Add current color and particle color multiplied by particle’s alpha

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:49

___

### BLENDMODE\_MULTIPLY

▪ `Static` **BLENDMODE\_MULTIPLY**: `number` = `3`

Multiply current color with particle color

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:53

___

### BLENDMODE\_MULTIPLYADD

▪ `Static` **BLENDMODE\_MULTIPLYADD**: `number` = `4`

Multiply current color with particle color then add current color and particle color multiplied by particle’s alpha

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:58

___

### BLENDMODE\_ONEONE

▪ `Static` **BLENDMODE\_ONEONE**: `number` = `0`

Source color is added to the destination color without alpha affecting the result

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:41

___

### BLENDMODE\_STANDARD

▪ `Static` **BLENDMODE\_STANDARD**: `number` = `1`

Blend current color and particle color using particle’s alpha

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:45

## Accessors

### billboardMode

• `get` **billboardMode**(): `number`

Gets or sets the billboard mode to use when isBillboardBased = true.
Value can be: ParticleSystem.BILLBOARDMODE_ALL, ParticleSystem.BILLBOARDMODE_Y, ParticleSystem.BILLBOARDMODE_STRETCHED

#### Returns

`number`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:572

• `set` **billboardMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:576

___

### direction1

• `get` **direction1**(): [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:471

• `set` **direction1**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:479

___

### direction2

• `get` **direction2**(): [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:489

• `set` **direction2**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:497

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:635

___

### isAnimationSheetEnabled

• `get` **isAnimationSheetEnabled**(): `boolean`

Gets or sets whether an animation sprite sheet is enabled or not on the particle system

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:312

• `set` **isAnimationSheetEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:316

___

### isBillboardBased

• `get` **isBillboardBased**(): `boolean`

Gets or sets a boolean indicating if the particles must be rendered as billboard or aligned with the direction

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:590

• `set` **isBillboardBased**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:594

___

### maxEmitBox

• `get` **maxEmitBox**(): [`Vector3`](Vector3.md)

Maximum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:525

• `set` **maxEmitBox**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:533

___

### minEmitBox

• `get` **minEmitBox**(): [`Vector3`](Vector3.md)

Minimum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.
This only works when particleEmitterTyps is a BoxParticleEmitter

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:507

• `set` **minEmitBox**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:515

___

### noiseTexture

• `get` **noiseTexture**(): [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

Gets or sets a texture used to add random noise to particle positions

#### Returns

[`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:211

• `set` **noiseTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:215

## Methods

### \_attachImageProcessingConfiguration

▸ `Protected` **_attachImageProcessingConfiguration**(`configuration`): `void`

Attaches a new image processing configuration to the Standard Material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:643

___

### \_hasTargetStopDurationDependantGradient

▸ `Protected` **_hasTargetStopDurationDependantGradient**(): ``null`` \| `boolean`

#### Returns

``null`` \| `boolean`

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:352

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:729

___

### getAlphaRemapGradients

▸ **getAlphaRemapGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of alpha remap gradients.
You must use addAlphaRemapGradient and removeAlphaRemapGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of alpha remap gradients

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:436

___

### getColorGradients

▸ **getColorGradients**(): [`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[]

Gets the current list of color gradients.
You must use addColorGradient and removeColorGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorGradient`](ColorGradient.md)[]

the list of color gradients

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:409

___

### getDragGradients

▸ **getDragGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

Gets the current list of drag gradients.
You must use addDragGradient and removeDragGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](FactorGradient.md)[]

the list of drag gradients

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:382

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get hosting scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene

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

#### Defined in

packages/dev/core/src/Particles/baseParticleSystem.ts:445

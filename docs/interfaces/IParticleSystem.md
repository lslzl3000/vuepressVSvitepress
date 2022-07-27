[@dev/core](../README.md) / [Exports](../modules.md) / IParticleSystem

# Interface: IParticleSystem

Interface representing a particle system in Babylon.js.
This groups the common functionalities that needs to be implemented in order to create a particle system.
A particle system represents a way to manage particles from their emission to their animation and rendering.

## Implemented by

- [`GPUParticleSystem`](../classes/GPUParticleSystem.md)
- [`ParticleSystem`](../classes/ParticleSystem.md)

## Table of contents

### Properties

- [animations](IParticleSystem.md#animations)
- [beginAnimationFrom](IParticleSystem.md#beginanimationfrom)
- [beginAnimationLoop](IParticleSystem.md#beginanimationloop)
- [beginAnimationOnStart](IParticleSystem.md#beginanimationonstart)
- [beginAnimationTo](IParticleSystem.md#beginanimationto)
- [billboardMode](IParticleSystem.md#billboardmode)
- [blendMode](IParticleSystem.md#blendmode)
- [color1](IParticleSystem.md#color1)
- [color2](IParticleSystem.md#color2)
- [colorDead](IParticleSystem.md#colordead)
- [defaultProjectionMatrix](IParticleSystem.md#defaultprojectionmatrix)
- [disposeOnStop](IParticleSystem.md#disposeonstop)
- [emitRate](IParticleSystem.md#emitrate)
- [emitter](IParticleSystem.md#emitter)
- [endSpriteCellID](IParticleSystem.md#endspritecellid)
- [gravity](IParticleSystem.md#gravity)
- [id](IParticleSystem.md#id)
- [isAnimationSheetEnabled](IParticleSystem.md#isanimationsheetenabled)
- [isBillboardBased](IParticleSystem.md#isbillboardbased)
- [isLocal](IParticleSystem.md#islocal)
- [layerMask](IParticleSystem.md#layermask)
- [limitVelocityDamping](IParticleSystem.md#limitvelocitydamping)
- [manualEmitCount](IParticleSystem.md#manualemitcount)
- [maxAngularSpeed](IParticleSystem.md#maxangularspeed)
- [maxEmitPower](IParticleSystem.md#maxemitpower)
- [maxInitialRotation](IParticleSystem.md#maxinitialrotation)
- [maxLifeTime](IParticleSystem.md#maxlifetime)
- [maxScaleX](IParticleSystem.md#maxscalex)
- [maxScaleY](IParticleSystem.md#maxscaley)
- [maxSize](IParticleSystem.md#maxsize)
- [minAngularSpeed](IParticleSystem.md#minangularspeed)
- [minEmitPower](IParticleSystem.md#minemitpower)
- [minInitialRotation](IParticleSystem.md#mininitialrotation)
- [minLifeTime](IParticleSystem.md#minlifetime)
- [minScaleX](IParticleSystem.md#minscalex)
- [minScaleY](IParticleSystem.md#minscaley)
- [minSize](IParticleSystem.md#minsize)
- [name](IParticleSystem.md#name)
- [noiseStrength](IParticleSystem.md#noisestrength)
- [noiseTexture](IParticleSystem.md#noisetexture)
- [onBeforeDrawParticlesObservable](IParticleSystem.md#onbeforedrawparticlesobservable)
- [onDisposeObservable](IParticleSystem.md#ondisposeobservable)
- [onStoppedObservable](IParticleSystem.md#onstoppedobservable)
- [particleEmitterType](IParticleSystem.md#particleemittertype)
- [particleTexture](IParticleSystem.md#particletexture)
- [preWarmCycles](IParticleSystem.md#prewarmcycles)
- [preWarmStepOffset](IParticleSystem.md#prewarmstepoffset)
- [renderingGroupId](IParticleSystem.md#renderinggroupid)
- [snippetId](IParticleSystem.md#snippetid)
- [spriteCellChangeSpeed](IParticleSystem.md#spritecellchangespeed)
- [spriteCellHeight](IParticleSystem.md#spritecellheight)
- [spriteCellLoop](IParticleSystem.md#spritecellloop)
- [spriteCellWidth](IParticleSystem.md#spritecellwidth)
- [spriteRandomStartCell](IParticleSystem.md#spriterandomstartcell)
- [startDelay](IParticleSystem.md#startdelay)
- [startSpriteCellID](IParticleSystem.md#startspritecellid)
- [targetStopDuration](IParticleSystem.md#targetstopduration)
- [translationPivot](IParticleSystem.md#translationpivot)
- [updateSpeed](IParticleSystem.md#updatespeed)
- [useRampGradients](IParticleSystem.md#userampgradients)
- [vertexShaderName](IParticleSystem.md#vertexshadername)

### Methods

- [addAlphaRemapGradient](IParticleSystem.md#addalpharemapgradient)
- [addAngularSpeedGradient](IParticleSystem.md#addangularspeedgradient)
- [addColorGradient](IParticleSystem.md#addcolorgradient)
- [addColorRemapGradient](IParticleSystem.md#addcolorremapgradient)
- [addDragGradient](IParticleSystem.md#adddraggradient)
- [addEmitRateGradient](IParticleSystem.md#addemitrategradient)
- [addLifeTimeGradient](IParticleSystem.md#addlifetimegradient)
- [addLimitVelocityGradient](IParticleSystem.md#addlimitvelocitygradient)
- [addRampGradient](IParticleSystem.md#addrampgradient)
- [addSizeGradient](IParticleSystem.md#addsizegradient)
- [addStartSizeGradient](IParticleSystem.md#addstartsizegradient)
- [addVelocityGradient](IParticleSystem.md#addvelocitygradient)
- [animate](IParticleSystem.md#animate)
- [clone](IParticleSystem.md#clone)
- [createBoxEmitter](IParticleSystem.md#createboxemitter)
- [createConeEmitter](IParticleSystem.md#createconeemitter)
- [createCylinderEmitter](IParticleSystem.md#createcylinderemitter)
- [createDirectedCylinderEmitter](IParticleSystem.md#createdirectedcylinderemitter)
- [createDirectedSphereEmitter](IParticleSystem.md#createdirectedsphereemitter)
- [createHemisphericEmitter](IParticleSystem.md#createhemisphericemitter)
- [createPointEmitter](IParticleSystem.md#createpointemitter)
- [createSphereEmitter](IParticleSystem.md#createsphereemitter)
- [dispose](IParticleSystem.md#dispose)
- [fillDefines](IParticleSystem.md#filldefines)
- [fillUniformsAttributesAndSamplerNames](IParticleSystem.md#filluniformsattributesandsamplernames)
- [forceRefreshGradients](IParticleSystem.md#forcerefreshgradients)
- [getActiveCount](IParticleSystem.md#getactivecount)
- [getAlphaRemapGradients](IParticleSystem.md#getalpharemapgradients)
- [getAngularSpeedGradients](IParticleSystem.md#getangularspeedgradients)
- [getCapacity](IParticleSystem.md#getcapacity)
- [getClassName](IParticleSystem.md#getclassname)
- [getColorGradients](IParticleSystem.md#getcolorgradients)
- [getColorRemapGradients](IParticleSystem.md#getcolorremapgradients)
- [getCustomEffect](IParticleSystem.md#getcustomeffect)
- [getDragGradients](IParticleSystem.md#getdraggradients)
- [getEmitRateGradients](IParticleSystem.md#getemitrategradients)
- [getLifeTimeGradients](IParticleSystem.md#getlifetimegradients)
- [getLimitVelocityGradients](IParticleSystem.md#getlimitvelocitygradients)
- [getRampGradients](IParticleSystem.md#getrampgradients)
- [getScene](IParticleSystem.md#getscene)
- [getSizeGradients](IParticleSystem.md#getsizegradients)
- [getStartSizeGradients](IParticleSystem.md#getstartsizegradients)
- [getVelocityGradients](IParticleSystem.md#getvelocitygradients)
- [isReady](IParticleSystem.md#isready)
- [isStarted](IParticleSystem.md#isstarted)
- [isStopping](IParticleSystem.md#isstopping)
- [rebuild](IParticleSystem.md#rebuild)
- [removeAngularSpeedGradient](IParticleSystem.md#removeangularspeedgradient)
- [removeColorGradient](IParticleSystem.md#removecolorgradient)
- [removeDragGradient](IParticleSystem.md#removedraggradient)
- [removeEmitRateGradient](IParticleSystem.md#removeemitrategradient)
- [removeLifeTimeGradient](IParticleSystem.md#removelifetimegradient)
- [removeLimitVelocityGradient](IParticleSystem.md#removelimitvelocitygradient)
- [removeSizeGradient](IParticleSystem.md#removesizegradient)
- [removeStartSizeGradient](IParticleSystem.md#removestartsizegradient)
- [removeVelocityGradient](IParticleSystem.md#removevelocitygradient)
- [render](IParticleSystem.md#render)
- [reset](IParticleSystem.md#reset)
- [serialize](IParticleSystem.md#serialize)
- [setCustomEffect](IParticleSystem.md#setcustomeffect)
- [start](IParticleSystem.md#start)
- [stop](IParticleSystem.md#stop)

## Properties

### animations

• **animations**: [`Animation`](../classes/Animation.md)[]

List of animations used by the particle system.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:33

___

### beginAnimationFrom

• **beginAnimationFrom**: `number`

Gets or sets the frame to start the animation from when beginAnimationOnStart is true

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:243

___

### beginAnimationLoop

• **beginAnimationLoop**: `boolean`

Gets or sets a boolean indicating if animations must loop when beginAnimationOnStart is true

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:253

___

### beginAnimationOnStart

• **beginAnimationOnStart**: `boolean`

Gets or sets a boolean indicating that hosted animations (in the system.animations array) must be started when system.start() is called

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:238

___

### beginAnimationTo

• **beginAnimationTo**: `number`

Gets or sets the frame to end the animation on when beginAnimationOnStart is true

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:248

___

### billboardMode

• **billboardMode**: `number`

Gets or sets the billboard mode to use when isBillboardBased = true.
Value can be: ParticleSystem.BILLBOARDMODE_ALL, ParticleSystem.BILLBOARDMODE_Y, ParticleSystem.BILLBOARDMODE_STRETCHED

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:230

___

### blendMode

• **blendMode**: `number`

Blend mode use to render the particle, it can be either ParticleSystem.BLENDMODE_ONEONE, ParticleSystem.BLENDMODE_STANDARD or ParticleSystem.BLENDMODE_ADD.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:77

___

### color1

• **color1**: [`Color4`](../classes/Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:118

___

### color2

• **color2**: [`Color4`](../classes/Color4.md)

Random color of each particle after it has been emitted, between color1 and color2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:122

___

### colorDead

• **colorDead**: [`Color4`](../classes/Color4.md)

Color the particle will have at the end of its lifetime.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:127

___

### defaultProjectionMatrix

• **defaultProjectionMatrix**: [`Matrix`](../classes/Matrix.md)

Gets or sets a matrix to use to compute projection

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:274

___

### disposeOnStop

• **disposeOnStop**: `boolean`

Specifies whether the particle system will be disposed once it reaches the end of the animation.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:258

___

### emitRate

• **emitRate**: `number`

The maximum number of particles to emit per frame until we reach the activeParticleCount value

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:132

___

### emitter

• **emitter**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](../classes/AbstractMesh.md) \| [`Vector3`](../classes/Vector3.md)

The emitter represents the Mesh or position we are attaching the particle system to.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:45

___

### endSpriteCellID

• **endSpriteCellID**: `number`

If using a spritesheet (isAnimationSheetEnabled) defines the last sprite cell to display

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:192

___

### gravity

• **gravity**: [`Vector3`](../classes/Vector3.md)

You can use gravity if you want to give an orientation to your particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:137

___

### id

• **id**: `string`

The id of the Particle system.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:37

___

### isAnimationSheetEnabled

• **isAnimationSheetEnabled**: `boolean`

Gets or sets a boolean indicating if a spritesheet is used to animate the particles texture

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:213

___

### isBillboardBased

• **isBillboardBased**: `boolean`

Gets or sets a boolean indicating if the particles must be rendered as billboard or aligned with the direction

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:49

___

### isLocal

• **isLocal**: `boolean`

Specifies if the particles are updated in emitter local space or world space

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:268

___

### layerMask

• **layerMask**: `number`

The layer mask we are rendering the particles through.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:57

___

### limitVelocityDamping

• **limitVelocityDamping**: `number`

Gets or sets a value indicating the damping to apply if the limit velocity factor is reached

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:233

___

### manualEmitCount

• **manualEmitCount**: `number`

If you want to launch only a few particles at once, that can be done, as well.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:263

___

### maxAngularSpeed

• **maxAngularSpeed**: `number`

Maximum angular speed of emitting particles (Z-axis rotation for each particle).

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:154

___

### maxEmitPower

• **maxEmitPower**: `number`

Maximum power of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:146

___

### maxInitialRotation

• **maxInitialRotation**: `number`

Gets or sets the maximal initial rotation in radians.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:162

___

### maxLifeTime

• **maxLifeTime**: `number`

Maximum life time of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:86

___

### maxScaleX

• **maxScaleX**: `number`

Maximum scale of emitting particles on X axis.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:104

___

### maxScaleY

• **maxScaleY**: `number`

Maximum scale of emitting particles on Y axis.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:113

___

### maxSize

• **maxSize**: `number`

Maximum Size of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:95

___

### minAngularSpeed

• **minAngularSpeed**: `number`

Minimum angular speed of emitting particles (Z-axis rotation for each particle).

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:150

___

### minEmitPower

• **minEmitPower**: `number`

Minimum power of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:142

___

### minInitialRotation

• **minInitialRotation**: `number`

Gets or sets the minimal initial rotation in radians.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:158

___

### minLifeTime

• **minLifeTime**: `number`

Minimum life time of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:82

___

### minScaleX

• **minScaleX**: `number`

Minimum scale of emitting particles on X axis.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:100

___

### minScaleY

• **minScaleY**: `number`

Minimum scale of emitting particles on Y axis.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:109

___

### minSize

• **minSize**: `number`

Minimum Size of emitting particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:91

___

### name

• **name**: `string`

The name of the Particle system.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:41

___

### noiseStrength

• **noiseStrength**: [`Vector3`](../classes/Vector3.md)

Gets or sets the strength to apply to the noise value (default is (10, 10, 10))

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:224

___

### noiseTexture

• **noiseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](../classes/BaseTexture.md)

Gets or sets a texture used to add random noise to particle positions

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:221

___

### onBeforeDrawParticlesObservable

• **onBeforeDrawParticlesObservable**: [`Observable`](../classes/Observable.md)[`Nullable`](../modules.md#nullable)[`Effect`](../classes/Effect.md)

Observable that will be called just before the particles are drawn

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:398

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](../classes/Observable.md)[`IParticleSystem`](IParticleSystem.md)

An event triggered when the system is disposed

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:311

___

### onStoppedObservable

• **onStoppedObservable**: [`Observable`](../classes/Observable.md)[`IParticleSystem`](IParticleSystem.md)

An event triggered when the system is stopped

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:315

___

### particleEmitterType

• **particleEmitterType**: [`Nullable`](../modules.md#nullable)[`IParticleEmitterType`](IParticleEmitterType.md)

The particle emitter type defines the emitter used by the particle system.
It can be for example box, sphere, or cone...

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:167

___

### particleTexture

• **particleTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](../classes/BaseTexture.md)

The texture used to render each particle. (this can be a spritesheet)

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:72

___

### preWarmCycles

• **preWarmCycles**: `number`

Gets or sets a value indicating how many cycles (or frames) must be executed before first rendering (this value has to be set before starting the system). Default is 0

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:175

___

### preWarmStepOffset

• **preWarmStepOffset**: `number`

Gets or sets a value indicating the time step multiplier to use in pre-warm mode (default is 1)

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:179

___

### renderingGroupId

• **renderingGroupId**: `number`

The rendering group used by the Particle system to chose when to render.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:53

___

### snippetId

• **snippetId**: `string`

Snippet ID if the particle system was created from the snippet server

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:271

___

### spriteCellChangeSpeed

• **spriteCellChangeSpeed**: `number`

If using a spritesheet (isAnimationSheetEnabled) defines the speed of the sprite loop (default is 1 meaning the animation will play once during the entire particle lifetime)

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:184

___

### spriteCellHeight

• **spriteCellHeight**: `number`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell height to use

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:204

___

### spriteCellLoop

• **spriteCellLoop**: `boolean`

If using a spritesheet (isAnimationSheetEnabled), defines whether the sprite animation is looping

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:196

___

### spriteCellWidth

• **spriteCellWidth**: `number`

If using a spritesheet (isAnimationSheetEnabled), defines the sprite cell width to use

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:200

___

### spriteRandomStartCell

• **spriteRandomStartCell**: `boolean`

This allows the system to random pick the start cell ID between startSpriteCellID and endSpriteCellID

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:208

___

### startDelay

• **startDelay**: `number`

Defines the delay in milliseconds before starting the system (0 by default)

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:171

___

### startSpriteCellID

• **startSpriteCellID**: `number`

If using a spritesheet (isAnimationSheetEnabled) defines the first sprite cell to display

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:188

___

### targetStopDuration

• **targetStopDuration**: `number`

The amount of time the particle system is running (depends of the overall update speed).

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:67

___

### translationPivot

• **translationPivot**: [`Vector2`](../classes/Vector2.md)

Gets or sets a Vector2 used to move the pivot (by default (0,0))

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:216

___

### updateSpeed

• **updateSpeed**: `number`

The overall motion speed (0.01 is default update speed, faster updates = faster animation)

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:62

___

### useRampGradients

• **useRampGradients**: `boolean`

Gets or sets a boolean indicating that ramp gradients must be used

**`See`**

https://doc.babylonjs.com/babylon101/particles#ramp-gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:611

___

### vertexShaderName

• **vertexShaderName**: `string`

Gets the name of the particle vertex shader

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:402

## Methods

### addAlphaRemapGradient

▸ **addAlphaRemapGradient**(`gradient`, `min`, `max`): [`IParticleSystem`](IParticleSystem.md)

Adds a new alpha remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `min` | `number` | defines the alpha remap minimal range |
| `max` | `number` | defines the alpha remap maximal range |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:635

___

### addAngularSpeedGradient

▸ **addAngularSpeedGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the angular speed to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:457

___

### addColorGradient

▸ **addColorGradient**(`gradient`, `color1`, `color2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `color1` | [`Color4`](../classes/Color4.md) | defines the color to affect to the specified gradient |
| `color2?` | [`Color4`](../classes/Color4.md) | defines an additional color used to define a range ([color, color2]) with main color to pick the final color from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:411

___

### addColorRemapGradient

▸ **addColorRemapGradient**(`gradient`, `min`, `max`): [`IParticleSystem`](IParticleSystem.md)

Adds a new color remap gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `min` | `number` | defines the color remap minimal range |
| `max` | `number` | defines the color remap maximal range |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:620

___

### addDragGradient

▸ **addDragGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the drag to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:511

___

### addEmitRateGradient

▸ **addEmitRateGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new emit rate gradient (please note that this will only work if you set the targetStopDuration property)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the emit rate to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:531

___

### addLifeTimeGradient

▸ **addLifeTimeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new life time gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the life time factor to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:573

___

### addLimitVelocityGradient

▸ **addLimitVelocityGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the limit velocity to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:497

___

### addRampGradient

▸ **addRampGradient**(`gradient`, `color`): [`IParticleSystem`](IParticleSystem.md)

Adds a new ramp gradient used to remap particle colors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `color` | [`Color3`](../classes/Color3.md) | defines the color to affect to the specified gradient |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:600

___

### addSizeGradient

▸ **addSizeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the size factor to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:425

___

### addStartSizeGradient

▸ **addStartSizeGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new start size gradient (please note that this will only work if you set the targetStopDuration property)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the start size to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:552

___

### addVelocityGradient

▸ **addVelocityGradient**(`gradient`, `factor`, `factor2?`): [`IParticleSystem`](IParticleSystem.md)

Adds a new velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to use (between 0 and 1) |
| `factor` | `number` | defines the velocity to affect to the specified gradient |
| `factor2?` | `number` | defines an additional factor used to define a range ([factor, factor2]) with main value to pick the final value from |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:477

___

### animate

▸ **animate**(): `void`

Animates the particle system for this frame.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:297

___

### clone

▸ **clone**(`name`, `newEmitter`): [`Nullable`](../modules.md#nullable)[`IParticleSystem`](IParticleSystem.md)

Clones the particle system.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the cloned object |
| `newEmitter` | `any` | The new emitter to use |

#### Returns

[`Nullable`](../modules.md#nullable)[`IParticleSystem`](IParticleSystem.md)

the cloned particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:322

___

### createBoxEmitter

▸ **createBoxEmitter**(`direction1`, `direction2`, `minEmitBox`, `maxEmitBox`): [`BoxParticleEmitter`](../classes/BoxParticleEmitter.md)

Creates a Box Emitter for the particle system. (emits between direction1 and direction2 from withing the box defined by minEmitBox and maxEmitBox)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction1` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `direction2` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `minEmitBox` | [`Vector3`](../classes/Vector3.md) | Particles are emitted from the box between minEmitBox and maxEmitBox |
| `maxEmitBox` | [`Vector3`](../classes/Vector3.md) | Particles are emitted from the box between minEmitBox and maxEmitBox |

#### Returns

[`BoxParticleEmitter`](../classes/BoxParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:713

___

### createConeEmitter

▸ **createConeEmitter**(`radius`, `angle`): [`ConeParticleEmitter`](../classes/ConeParticleEmitter.md)

Creates a Cone Emitter for the particle system (emits from the cone to the particle position)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the cone to emit from |
| `angle` | `number` | The base angle of the cone |

#### Returns

[`ConeParticleEmitter`](../classes/ConeParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:703

___

### createCylinderEmitter

▸ **createCylinderEmitter**(`radius`, `height`, `radiusRange`, `directionRandomizer`): [`CylinderParticleEmitter`](../classes/CylinderParticleEmitter.md)

Creates a Cylinder Emitter for the particle system (emits from the cylinder to the particle position)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the emission cylinder |
| `height` | `number` | The height of the emission cylinder |
| `radiusRange` | `number` | The range of emission [0-1] 0 Surface only, 1 Entire Radius |
| `directionRandomizer` | `number` | How much to randomize the particle direction [0-1] |

#### Returns

[`CylinderParticleEmitter`](../classes/CylinderParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:684

___

### createDirectedCylinderEmitter

▸ **createDirectedCylinderEmitter**(`radius`, `height`, `radiusRange`, `direction1`, `direction2`): [`SphereDirectedParticleEmitter`](../classes/SphereDirectedParticleEmitter.md)

Creates a Directed Cylinder Emitter for the particle system (emits between direction1 and direction2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the cylinder to emit from |
| `height` | `number` | The height of the emission cylinder |
| `radiusRange` | `number` | the range of the emission cylinder [0-1] 0 Surface only, 1 Entire Radius (1 by default) |
| `direction1` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the cylinder |
| `direction2` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the cylinder |

#### Returns

[`SphereDirectedParticleEmitter`](../classes/SphereDirectedParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:695

___

### createDirectedSphereEmitter

▸ **createDirectedSphereEmitter**(`radius`, `direction1`, `direction2`): [`SphereDirectedParticleEmitter`](../classes/SphereDirectedParticleEmitter.md)

Creates a Directed Sphere Emitter for the particle system (emits between direction1 and direction2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the sphere to emit from |
| `direction1` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the sphere |
| `direction2` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the sphere |

#### Returns

[`SphereDirectedParticleEmitter`](../classes/SphereDirectedParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:674

___

### createHemisphericEmitter

▸ **createHemisphericEmitter**(`radius`, `radiusRange`): [`HemisphericParticleEmitter`](../classes/HemisphericParticleEmitter.md)

Creates a Hemisphere Emitter for the particle system (emits along the hemisphere radius)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the hemisphere to emit from |
| `radiusRange` | `number` | The range of the hemisphere to emit from [0-1] 0 Surface Only, 1 Entire Radius |

#### Returns

[`HemisphericParticleEmitter`](../classes/HemisphericParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:657

___

### createPointEmitter

▸ **createPointEmitter**(`direction1`, `direction2`): [`PointParticleEmitter`](../classes/PointParticleEmitter.md)

Creates a Point Emitter for the particle system (emits directly from the emitter position)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `direction1` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |
| `direction2` | [`Vector3`](../classes/Vector3.md) | Particles are emitted between the direction1 and direction2 from within the box |

#### Returns

[`PointParticleEmitter`](../classes/PointParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:649

___

### createSphereEmitter

▸ **createSphereEmitter**(`radius`, `radiusRange`): [`SphereParticleEmitter`](../classes/SphereParticleEmitter.md)

Creates a Sphere Emitter for the particle system (emits along the sphere radius)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radius` | `number` | The radius of the sphere to emit from |
| `radiusRange` | `number` | The range of the sphere to emit from [0-1] 0 Surface Only, 1 Entire Radius |

#### Returns

[`SphereParticleEmitter`](../classes/SphereParticleEmitter.md)

the emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:665

___

### dispose

▸ **dispose**(`disposeTexture?`): `void`

Dispose the particle system and frees its associated resources.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `disposeTexture?` | `boolean` | defines if the particle texture must be disposed as well (true by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:307

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

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:387

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

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:394

___

### forceRefreshGradients

▸ **forceRefreshGradients**(): `void`

Force the system to rebuild all gradients that need to be resync

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:335

___

### getActiveCount

▸ **getActiveCount**(): `number`

Gets the number of particles active at the same time.

#### Returns

`number`

The number of active particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:286

___

### getAlphaRemapGradients

▸ **getAlphaRemapGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of alpha remap gradients.
You must use addAlphaRemapGradient and removeAlphaRemapGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of alpha remap gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:641

___

### getAngularSpeedGradients

▸ **getAngularSpeedGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of angular speed gradients.
You must use addAngularSpeedGradient and removeAngularSpeedGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of angular speed gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:449

___

### getCapacity

▸ **getCapacity**(): `number`

Gets the maximum number of particles active at the same time.

#### Returns

`number`

The max number of active particles.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:280

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "ParticleSystem"

#### Returns

`string`

a string containing the class name

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:368

___

### getColorGradients

▸ **getColorGradients**(): [`Nullable`](../modules.md#nullable)[`ColorGradient`](../classes/ColorGradient.md)[]

Gets the current list of color gradients.
You must use addColorGradient and removeColorGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorGradient`](../classes/ColorGradient.md)[]

the list of color gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:437

▸ **getColorGradients**(): [`Nullable`](../modules.md#nullable)[`ColorGradient`](../classes/ColorGradient.md)[]

Gets the current list of color gradients.
You must use addColorGradient and removeColorGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorGradient`](../classes/ColorGradient.md)[]

the list of color gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:592

___

### getColorRemapGradients

▸ **getColorRemapGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of color remap gradients.
You must use addColorRemapGradient and removeColorRemapGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of color remap gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:626

___

### getCustomEffect

▸ **getCustomEffect**(`blendMode`): [`Nullable`](../modules.md#nullable)[`Effect`](../classes/Effect.md)

Gets the custom effect used to render the particles

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blendMode` | `number` | Blend mode for which the effect should be retrieved |

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](../classes/Effect.md)

The effect

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:374

___

### getDragGradients

▸ **getDragGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of drag gradients.
You must use addDragGradient and removeDragGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of drag gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:523

___

### getEmitRateGradients

▸ **getEmitRateGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of emit rate gradients.
You must use addEmitRateGradient and removeEmitRateGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of emit rate gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:543

___

### getLifeTimeGradients

▸ **getLifeTimeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of life time gradients.
You must use addLifeTimeGradient and removeLifeTimeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of life time gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:585

___

### getLimitVelocityGradients

▸ **getLimitVelocityGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of limit velocity gradients.
You must use addLimitVelocityGradient and removeLimitVelocityGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of limit velocity gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:489

___

### getRampGradients

▸ **getRampGradients**(): [`Nullable`](../modules.md#nullable)[`Color3Gradient`](../classes/Color3Gradient.md)[]

Gets the current list of ramp gradients.
You must use addRampGradient and removeRampGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`Color3Gradient`](../classes/Color3Gradient.md)[]

the list of ramp gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:606

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](../classes/Scene.md)

Get hosting scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](../classes/Scene.md)

the scene

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:719

___

### getSizeGradients

▸ **getSizeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of size gradients.
You must use addSizeGradient and removeSizeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of size gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:443

___

### getStartSizeGradients

▸ **getStartSizeGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of start size gradients.
You must use addStartSizeGradient and removeStartSizeGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of start size gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:564

___

### getVelocityGradients

▸ **getVelocityGradients**(): [`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

Gets the current list of velocity gradients.
You must use addVelocityGradient and removeVelocityGradient to update this list

#### Returns

[`Nullable`](../modules.md#nullable)[`FactorGradient`](../classes/FactorGradient.md)[]

the list of velocity gradients

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:469

___

### isReady

▸ **isReady**(): `boolean`

Is this system ready to be used/rendered

#### Returns

`boolean`

true if the system is ready

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:363

___

### isStarted

▸ **isStarted**(): `boolean`

Gets if the system has been started. (Note: this will still be true after stop is called)

#### Returns

`boolean`

True if it has been started, otherwise false.

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:292

___

### isStopping

▸ **isStopping**(): `boolean`

Gets a boolean indicating that the system is stopping

#### Returns

`boolean`

true if the system is currently stopping

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:357

___

### rebuild

▸ **rebuild**(): `void`

Rebuild the particle system

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:332

___

### removeAngularSpeedGradient

▸ **removeAngularSpeedGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific angular speed gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:463

___

### removeColorGradient

▸ **removeColorGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific color gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:417

___

### removeDragGradient

▸ **removeDragGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific drag gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:517

___

### removeEmitRateGradient

▸ **removeEmitRateGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific emit rate gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:537

___

### removeLifeTimeGradient

▸ **removeLifeTimeGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific life time gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:579

___

### removeLimitVelocityGradient

▸ **removeLimitVelocityGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific limit velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:503

___

### removeSizeGradient

▸ **removeSizeGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:431

___

### removeStartSizeGradient

▸ **removeStartSizeGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific start size gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:558

___

### removeVelocityGradient

▸ **removeVelocityGradient**(`gradient`): [`IParticleSystem`](IParticleSystem.md)

Remove a specific velocity gradient

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gradient` | `number` | defines the gradient to remove |

#### Returns

[`IParticleSystem`](IParticleSystem.md)

the current particle system

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:483

___

### render

▸ **render**(): `number`

Renders the particle system in its current state.

#### Returns

`number`

the current number of particles

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:302

___

### reset

▸ **reset**(): `void`

Remove all active particles

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:351

___

### serialize

▸ **serialize**(`serializeTexture`): `any`

Serializes the particle system to a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializeTexture` | `boolean` | defines if the texture must be serialized as well |

#### Returns

`any`

the JSON object

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:328

___

### setCustomEffect

▸ **setCustomEffect**(`effect`, `blendMode`): `void`

Sets the custom effect used to render the particles

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](../classes/Effect.md) | The effect to set |
| `blendMode` | `number` | Blend mode for which the effect should be set |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:380

___

### start

▸ **start**(`delay?`): `void`

Starts the particle system and begins to emit

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `delay?` | `number` | defines the delay in milliseconds before starting the system (0 by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:341

___

### stop

▸ **stop**(): `void`

Stops the particle system.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/IParticleSystem.ts:346

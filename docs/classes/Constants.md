[@dev/core](../README.md) / [Exports](../modules.md) / Constants

# Class: Constants

Defines the cross module used constants to avoid circular dependencies

## Table of contents

### Constructors

- [constructor](Constants.md#constructor)

### Properties

- [ACTION\_NothingTrigger](Constants.md#action_nothingtrigger)
- [ACTION\_OnCenterPickTrigger](Constants.md#action_oncenterpicktrigger)
- [ACTION\_OnDoublePickTrigger](Constants.md#action_ondoublepicktrigger)
- [ACTION\_OnEveryFrameTrigger](Constants.md#action_oneveryframetrigger)
- [ACTION\_OnIntersectionEnterTrigger](Constants.md#action_onintersectionentertrigger)
- [ACTION\_OnIntersectionExitTrigger](Constants.md#action_onintersectionexittrigger)
- [ACTION\_OnKeyDownTrigger](Constants.md#action_onkeydowntrigger)
- [ACTION\_OnKeyUpTrigger](Constants.md#action_onkeyuptrigger)
- [ACTION\_OnLeftPickTrigger](Constants.md#action_onleftpicktrigger)
- [ACTION\_OnLongPressTrigger](Constants.md#action_onlongpresstrigger)
- [ACTION\_OnPickDownTrigger](Constants.md#action_onpickdowntrigger)
- [ACTION\_OnPickOutTrigger](Constants.md#action_onpickouttrigger)
- [ACTION\_OnPickTrigger](Constants.md#action_onpicktrigger)
- [ACTION\_OnPickUpTrigger](Constants.md#action_onpickuptrigger)
- [ACTION\_OnPointerOutTrigger](Constants.md#action_onpointerouttrigger)
- [ACTION\_OnPointerOverTrigger](Constants.md#action_onpointerovertrigger)
- [ACTION\_OnRightPickTrigger](Constants.md#action_onrightpicktrigger)
- [ALPHA\_ADD](Constants.md#alpha_add)
- [ALPHA\_ALPHATOCOLOR](Constants.md#alpha_alphatocolor)
- [ALPHA\_COMBINE](Constants.md#alpha_combine)
- [ALPHA\_DISABLE](Constants.md#alpha_disable)
- [ALPHA\_EQUATION\_ADD](Constants.md#alpha_equation_add)
- [ALPHA\_EQUATION\_DARKEN](Constants.md#alpha_equation_darken)
- [ALPHA\_EQUATION\_MAX](Constants.md#alpha_equation_max)
- [ALPHA\_EQUATION\_MIN](Constants.md#alpha_equation_min)
- [ALPHA\_EQUATION\_REVERSE\_SUBTRACT](Constants.md#alpha_equation_reverse_subtract)
- [ALPHA\_EQUATION\_SUBSTRACT](Constants.md#alpha_equation_substract)
- [ALPHA\_EXCLUSION](Constants.md#alpha_exclusion)
- [ALPHA\_INTERPOLATE](Constants.md#alpha_interpolate)
- [ALPHA\_LAYER\_ACCUMULATE](Constants.md#alpha_layer_accumulate)
- [ALPHA\_MAXIMIZED](Constants.md#alpha_maximized)
- [ALPHA\_MULTIPLY](Constants.md#alpha_multiply)
- [ALPHA\_ONEONE](Constants.md#alpha_oneone)
- [ALPHA\_ONEONE\_ONEONE](Constants.md#alpha_oneone_oneone)
- [ALPHA\_ONEONE\_ONEZERO](Constants.md#alpha_oneone_onezero)
- [ALPHA\_PREMULTIPLIED](Constants.md#alpha_premultiplied)
- [ALPHA\_PREMULTIPLIED\_PORTERDUFF](Constants.md#alpha_premultiplied_porterduff)
- [ALPHA\_REVERSEONEMINUS](Constants.md#alpha_reverseoneminus)
- [ALPHA\_SCREENMODE](Constants.md#alpha_screenmode)
- [ALPHA\_SRC\_DSTONEMINUSSRCALPHA](Constants.md#alpha_src_dstoneminussrcalpha)
- [ALPHA\_SUBTRACT](Constants.md#alpha_subtract)
- [ALWAYS](Constants.md#always)
- [BUFFER\_CREATIONFLAG\_INDEX](Constants.md#buffer_creationflag_index)
- [BUFFER\_CREATIONFLAG\_READ](Constants.md#buffer_creationflag_read)
- [BUFFER\_CREATIONFLAG\_READWRITE](Constants.md#buffer_creationflag_readwrite)
- [BUFFER\_CREATIONFLAG\_STORAGE](Constants.md#buffer_creationflag_storage)
- [BUFFER\_CREATIONFLAG\_UNIFORM](Constants.md#buffer_creationflag_uniform)
- [BUFFER\_CREATIONFLAG\_VERTEX](Constants.md#buffer_creationflag_vertex)
- [BUFFER\_CREATIONFLAG\_WRITE](Constants.md#buffer_creationflag_write)
- [DECR](Constants.md#decr)
- [DECR\_WRAP](Constants.md#decr_wrap)
- [DELAYLOADSTATE\_LOADED](Constants.md#delayloadstate_loaded)
- [DELAYLOADSTATE\_LOADING](Constants.md#delayloadstate_loading)
- [DELAYLOADSTATE\_NONE](Constants.md#delayloadstate_none)
- [DELAYLOADSTATE\_NOTLOADED](Constants.md#delayloadstate_notloaded)
- [EQUAL](Constants.md#equal)
- [FOVMODE\_HORIZONTAL\_FIXED](Constants.md#fovmode_horizontal_fixed)
- [FOVMODE\_VERTICAL\_FIXED](Constants.md#fovmode_vertical_fixed)
- [GEQUAL](Constants.md#gequal)
- [GL\_ALPHA\_EQUATION\_ADD](Constants.md#gl_alpha_equation_add)
- [GL\_ALPHA\_EQUATION\_MAX](Constants.md#gl_alpha_equation_max)
- [GL\_ALPHA\_EQUATION\_MIN](Constants.md#gl_alpha_equation_min)
- [GL\_ALPHA\_EQUATION\_REVERSE\_SUBTRACT](Constants.md#gl_alpha_equation_reverse_subtract)
- [GL\_ALPHA\_EQUATION\_SUBTRACT](Constants.md#gl_alpha_equation_subtract)
- [GL\_ALPHA\_FUNCTION\_CONSTANT\_ALPHA](Constants.md#gl_alpha_function_constant_alpha)
- [GL\_ALPHA\_FUNCTION\_CONSTANT\_COLOR](Constants.md#gl_alpha_function_constant_color)
- [GL\_ALPHA\_FUNCTION\_DST\_ALPHA](Constants.md#gl_alpha_function_dst_alpha)
- [GL\_ALPHA\_FUNCTION\_DST\_COLOR](Constants.md#gl_alpha_function_dst_color)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_ALPHA](Constants.md#gl_alpha_function_one_minus_constant_alpha)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_COLOR](Constants.md#gl_alpha_function_one_minus_constant_color)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_ALPHA](Constants.md#gl_alpha_function_one_minus_dst_alpha)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_COLOR](Constants.md#gl_alpha_function_one_minus_dst_color)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_ALPHA](Constants.md#gl_alpha_function_one_minus_src_alpha)
- [GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_COLOR](Constants.md#gl_alpha_function_one_minus_src_color)
- [GL\_ALPHA\_FUNCTION\_SRC](Constants.md#gl_alpha_function_src)
- [GL\_ALPHA\_FUNCTION\_SRC\_ALPHA](Constants.md#gl_alpha_function_src_alpha)
- [GL\_ALPHA\_FUNCTION\_SRC\_ALPHA\_SATURATED](Constants.md#gl_alpha_function_src_alpha_saturated)
- [GREATER](Constants.md#greater)
- [INCR](Constants.md#incr)
- [INCR\_WRAP](Constants.md#incr_wrap)
- [INPUT\_ALT\_KEY](Constants.md#input_alt_key)
- [INPUT\_CTRL\_KEY](Constants.md#input_ctrl_key)
- [INPUT\_META\_KEY1](Constants.md#input_meta_key1)
- [INPUT\_META\_KEY2](Constants.md#input_meta_key2)
- [INPUT\_META\_KEY3](Constants.md#input_meta_key3)
- [INPUT\_SHIFT\_KEY](Constants.md#input_shift_key)
- [INVERT](Constants.md#invert)
- [KEEP](Constants.md#keep)
- [LEQUAL](Constants.md#lequal)
- [LESS](Constants.md#less)
- [MATERIAL\_AllDirtyFlag](Constants.md#material_alldirtyflag)
- [MATERIAL\_AttributesDirtyFlag](Constants.md#material_attributesdirtyflag)
- [MATERIAL\_ClockWiseSideOrientation](Constants.md#material_clockwisesideorientation)
- [MATERIAL\_CounterClockWiseSideOrientation](Constants.md#material_counterclockwisesideorientation)
- [MATERIAL\_FresnelDirtyFlag](Constants.md#material_fresneldirtyflag)
- [MATERIAL\_LightDirtyFlag](Constants.md#material_lightdirtyflag)
- [MATERIAL\_LineListDrawMode](Constants.md#material_linelistdrawmode)
- [MATERIAL\_LineLoopDrawMode](Constants.md#material_lineloopdrawmode)
- [MATERIAL\_LineStripDrawMode](Constants.md#material_linestripdrawmode)
- [MATERIAL\_MiscDirtyFlag](Constants.md#material_miscdirtyflag)
- [MATERIAL\_PointFillMode](Constants.md#material_pointfillmode)
- [MATERIAL\_PointListDrawMode](Constants.md#material_pointlistdrawmode)
- [MATERIAL\_PrePassDirtyFlag](Constants.md#material_prepassdirtyflag)
- [MATERIAL\_TextureDirtyFlag](Constants.md#material_texturedirtyflag)
- [MATERIAL\_TriangleFanDrawMode](Constants.md#material_trianglefandrawmode)
- [MATERIAL\_TriangleFillMode](Constants.md#material_trianglefillmode)
- [MATERIAL\_TriangleStripDrawMode](Constants.md#material_trianglestripdrawmode)
- [MATERIAL\_WireFrameFillMode](Constants.md#material_wireframefillmode)
- [MAX\_SUPPORTED\_UV\_SETS](Constants.md#max_supported_uv_sets)
- [MESHES\_CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY](Constants.md#meshes_cullingstrategy_boundingsphere_only)
- [MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION](Constants.md#meshes_cullingstrategy_optimistic_inclusion)
- [MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY](Constants.md#meshes_cullingstrategy_optimistic_inclusion_then_bsphere_only)
- [MESHES\_CULLINGSTRATEGY\_STANDARD](Constants.md#meshes_cullingstrategy_standard)
- [NEVER](Constants.md#never)
- [NOTEQUAL](Constants.md#notequal)
- [ORTHOGRAPHIC\_CAMERA](Constants.md#orthographic_camera)
- [PARTICLES\_BILLBOARDMODE\_ALL](Constants.md#particles_billboardmode_all)
- [PARTICLES\_BILLBOARDMODE\_STRETCHED](Constants.md#particles_billboardmode_stretched)
- [PARTICLES\_BILLBOARDMODE\_Y](Constants.md#particles_billboardmode_y)
- [PERSPECTIVE\_CAMERA](Constants.md#perspective_camera)
- [PREPASS\_ALBEDO\_SQRT\_TEXTURE\_TYPE](Constants.md#prepass_albedo_sqrt_texture_type)
- [PREPASS\_COLOR\_TEXTURE\_TYPE](Constants.md#prepass_color_texture_type)
- [PREPASS\_DEPTH\_TEXTURE\_TYPE](Constants.md#prepass_depth_texture_type)
- [PREPASS\_IRRADIANCE\_TEXTURE\_TYPE](Constants.md#prepass_irradiance_texture_type)
- [PREPASS\_NORMAL\_TEXTURE\_TYPE](Constants.md#prepass_normal_texture_type)
- [PREPASS\_POSITION\_TEXTURE\_TYPE](Constants.md#prepass_position_texture_type)
- [PREPASS\_REFLECTIVITY\_TEXTURE\_TYPE](Constants.md#prepass_reflectivity_texture_type)
- [PREPASS\_VELOCITY\_TEXTURE\_TYPE](Constants.md#prepass_velocity_texture_type)
- [REPLACE](Constants.md#replace)
- [RIG\_MODE\_CUSTOM](Constants.md#rig_mode_custom)
- [RIG\_MODE\_NONE](Constants.md#rig_mode_none)
- [RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH](Constants.md#rig_mode_stereoscopic_anaglyph)
- [RIG\_MODE\_STEREOSCOPIC\_INTERLACED](Constants.md#rig_mode_stereoscopic_interlaced)
- [RIG\_MODE\_STEREOSCOPIC\_OVERUNDER](Constants.md#rig_mode_stereoscopic_overunder)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED](Constants.md#rig_mode_stereoscopic_sidebyside_crosseyed)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL](Constants.md#rig_mode_stereoscopic_sidebyside_parallel)
- [RIG\_MODE\_VR](Constants.md#rig_mode_vr)
- [RIG\_MODE\_WEBVR](Constants.md#rig_mode_webvr)
- [SCALEMODE\_CEILING](Constants.md#scalemode_ceiling)
- [SCALEMODE\_FLOOR](Constants.md#scalemode_floor)
- [SCALEMODE\_NEAREST](Constants.md#scalemode_nearest)
- [SCENELOADER\_DETAILED\_LOGGING](Constants.md#sceneloader_detailed_logging)
- [SCENELOADER\_MINIMAL\_LOGGING](Constants.md#sceneloader_minimal_logging)
- [SCENELOADER\_NO\_LOGGING](Constants.md#sceneloader_no_logging)
- [SCENELOADER\_SUMMARY\_LOGGING](Constants.md#sceneloader_summary_logging)
- [SNAPSHOTRENDERING\_FAST](Constants.md#snapshotrendering_fast)
- [SNAPSHOTRENDERING\_STANDARD](Constants.md#snapshotrendering_standard)
- [SnippetUrl](Constants.md#snippeturl)
- [TEXTUREFORMAT\_ALPHA](Constants.md#textureformat_alpha)
- [TEXTUREFORMAT\_BGRA](Constants.md#textureformat_bgra)
- [TEXTUREFORMAT\_COMPRESSED\_RGB8\_ETC2](Constants.md#textureformat_compressed_rgb8_etc2)
- [TEXTUREFORMAT\_COMPRESSED\_RGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2](Constants.md#textureformat_compressed_rgb8_punchthrough_alpha1_etc2)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA8\_ETC2\_EAC](Constants.md#textureformat_compressed_rgba8_etc2_eac)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA\_ASTC\_4x4](Constants.md#textureformat_compressed_rgba_astc_4x4)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA\_BPTC\_UNORM](Constants.md#textureformat_compressed_rgba_bptc_unorm)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT1](Constants.md#textureformat_compressed_rgba_s3tc_dxt1)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT3](Constants.md#textureformat_compressed_rgba_s3tc_dxt3)
- [TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT5](Constants.md#textureformat_compressed_rgba_s3tc_dxt5)
- [TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_SIGNED\_FLOAT](Constants.md#textureformat_compressed_rgb_bptc_signed_float)
- [TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_UNSIGNED\_FLOAT](Constants.md#textureformat_compressed_rgb_bptc_unsigned_float)
- [TEXTUREFORMAT\_COMPRESSED\_RGB\_ETC1\_WEBGL](Constants.md#textureformat_compressed_rgb_etc1_webgl)
- [TEXTUREFORMAT\_COMPRESSED\_RGB\_S3TC\_DXT1](Constants.md#textureformat_compressed_rgb_s3tc_dxt1)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ASTC\_4x4\_KHR](Constants.md#textureformat_compressed_srgb8_alpha8_astc_4x4_khr)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ETC2\_EAC](Constants.md#textureformat_compressed_srgb8_alpha8_etc2_eac)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ETC2](Constants.md#textureformat_compressed_srgb8_etc2)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2](Constants.md#textureformat_compressed_srgb8_punchthrough_alpha1_etc2)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_BPTC\_UNORM](Constants.md#textureformat_compressed_srgb_alpha_bptc_unorm)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT1\_EXT](Constants.md#textureformat_compressed_srgb_alpha_s3tc_dxt1_ext)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT3\_EXT](Constants.md#textureformat_compressed_srgb_alpha_s3tc_dxt3_ext)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT5\_EXT](Constants.md#textureformat_compressed_srgb_alpha_s3tc_dxt5_ext)
- [TEXTUREFORMAT\_COMPRESSED\_SRGB\_S3TC\_DXT1\_EXT](Constants.md#textureformat_compressed_srgb_s3tc_dxt1_ext)
- [TEXTUREFORMAT\_DEPTH16](Constants.md#textureformat_depth16)
- [TEXTUREFORMAT\_DEPTH24](Constants.md#textureformat_depth24)
- [TEXTUREFORMAT\_DEPTH24UNORM\_STENCIL8](Constants.md#textureformat_depth24unorm_stencil8)
- [TEXTUREFORMAT\_DEPTH24\_STENCIL8](Constants.md#textureformat_depth24_stencil8)
- [TEXTUREFORMAT\_DEPTH32FLOAT\_STENCIL8](Constants.md#textureformat_depth32float_stencil8)
- [TEXTUREFORMAT\_DEPTH32\_FLOAT](Constants.md#textureformat_depth32_float)
- [TEXTUREFORMAT\_LUMINANCE](Constants.md#textureformat_luminance)
- [TEXTUREFORMAT\_LUMINANCE\_ALPHA](Constants.md#textureformat_luminance_alpha)
- [TEXTUREFORMAT\_R](Constants.md#textureformat_r)
- [TEXTUREFORMAT\_RED](Constants.md#textureformat_red)
- [TEXTUREFORMAT\_RED\_INTEGER](Constants.md#textureformat_red_integer)
- [TEXTUREFORMAT\_RG](Constants.md#textureformat_rg)
- [TEXTUREFORMAT\_RGB](Constants.md#textureformat_rgb)
- [TEXTUREFORMAT\_RGBA](Constants.md#textureformat_rgba)
- [TEXTUREFORMAT\_RGBA\_INTEGER](Constants.md#textureformat_rgba_integer)
- [TEXTUREFORMAT\_RGB\_INTEGER](Constants.md#textureformat_rgb_integer)
- [TEXTUREFORMAT\_RG\_INTEGER](Constants.md#textureformat_rg_integer)
- [TEXTUREFORMAT\_R\_INTEGER](Constants.md#textureformat_r_integer)
- [TEXTURETYPE\_BYTE](Constants.md#texturetype_byte)
- [TEXTURETYPE\_FLOAT](Constants.md#texturetype_float)
- [TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV](Constants.md#texturetype_float_32_unsigned_int_24_8_rev)
- [TEXTURETYPE\_HALF\_FLOAT](Constants.md#texturetype_half_float)
- [TEXTURETYPE\_INT](Constants.md#texturetype_int)
- [TEXTURETYPE\_SHORT](Constants.md#texturetype_short)
- [TEXTURETYPE\_UNDEFINED](Constants.md#texturetype_undefined)
- [TEXTURETYPE\_UNSIGNED\_BYTE](Constants.md#texturetype_unsigned_byte)
- [TEXTURETYPE\_UNSIGNED\_INT](Constants.md#texturetype_unsigned_int)
- [TEXTURETYPE\_UNSIGNED\_INTEGER](Constants.md#texturetype_unsigned_integer)
- [TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV](Constants.md#texturetype_unsigned_int_10f_11f_11f_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_24\_8](Constants.md#texturetype_unsigned_int_24_8)
- [TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV](Constants.md#texturetype_unsigned_int_2_10_10_10_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV](Constants.md#texturetype_unsigned_int_5_9_9_9_rev)
- [TEXTURETYPE\_UNSIGNED\_SHORT](Constants.md#texturetype_unsigned_short)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4](Constants.md#texturetype_unsigned_short_4_4_4_4)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1](Constants.md#texturetype_unsigned_short_5_5_5_1)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5](Constants.md#texturetype_unsigned_short_5_6_5)
- [TEXTURE\_BILINEAR\_SAMPLINGMODE](Constants.md#texture_bilinear_samplingmode)
- [TEXTURE\_CLAMP\_ADDRESSMODE](Constants.md#texture_clamp_addressmode)
- [TEXTURE\_CREATIONFLAG\_STORAGE](Constants.md#texture_creationflag_storage)
- [TEXTURE\_CUBIC\_MODE](Constants.md#texture_cubic_mode)
- [TEXTURE\_EQUIRECTANGULAR\_MODE](Constants.md#texture_equirectangular_mode)
- [TEXTURE\_EXPLICIT\_MODE](Constants.md#texture_explicit_mode)
- [TEXTURE\_FILTERING\_QUALITY\_HIGH](Constants.md#texture_filtering_quality_high)
- [TEXTURE\_FILTERING\_QUALITY\_LOW](Constants.md#texture_filtering_quality_low)
- [TEXTURE\_FILTERING\_QUALITY\_MEDIUM](Constants.md#texture_filtering_quality_medium)
- [TEXTURE\_FILTERING\_QUALITY\_OFFLINE](Constants.md#texture_filtering_quality_offline)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](Constants.md#texture_fixed_equirectangular_mirrored_mode)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE](Constants.md#texture_fixed_equirectangular_mode)
- [TEXTURE\_INVCUBIC\_MODE](Constants.md#texture_invcubic_mode)
- [TEXTURE\_LINEAR\_LINEAR](Constants.md#texture_linear_linear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR](Constants.md#texture_linear_linear_miplinear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST](Constants.md#texture_linear_linear_mipnearest)
- [TEXTURE\_LINEAR\_NEAREST](Constants.md#texture_linear_nearest)
- [TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR](Constants.md#texture_linear_nearest_miplinear)
- [TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST](Constants.md#texture_linear_nearest_mipnearest)
- [TEXTURE\_MIRROR\_ADDRESSMODE](Constants.md#texture_mirror_addressmode)
- [TEXTURE\_NEAREST\_LINEAR](Constants.md#texture_nearest_linear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR](Constants.md#texture_nearest_linear_miplinear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST](Constants.md#texture_nearest_linear_mipnearest)
- [TEXTURE\_NEAREST\_NEAREST](Constants.md#texture_nearest_nearest)
- [TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR](Constants.md#texture_nearest_nearest_miplinear)
- [TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST](Constants.md#texture_nearest_nearest_mipnearest)
- [TEXTURE\_NEAREST\_SAMPLINGMODE](Constants.md#texture_nearest_samplingmode)
- [TEXTURE\_PLANAR\_MODE](Constants.md#texture_planar_mode)
- [TEXTURE\_PROJECTION\_MODE](Constants.md#texture_projection_mode)
- [TEXTURE\_SKYBOX\_MODE](Constants.md#texture_skybox_mode)
- [TEXTURE\_SPHERICAL\_MODE](Constants.md#texture_spherical_mode)
- [TEXTURE\_TRILINEAR\_SAMPLINGMODE](Constants.md#texture_trilinear_samplingmode)
- [TEXTURE\_WRAP\_ADDRESSMODE](Constants.md#texture_wrap_addressmode)
- [ZERO](Constants.md#zero)

## Constructors

### constructor

• **new Constants**()

## Properties

### ACTION\_NothingTrigger

▪ `Static` `Readonly` **ACTION\_NothingTrigger**: ``0``

Nothing

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:415

___

### ACTION\_OnCenterPickTrigger

▪ `Static` `Readonly` **ACTION\_OnCenterPickTrigger**: ``4``

On center pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:435

___

### ACTION\_OnDoublePickTrigger

▪ `Static` `Readonly` **ACTION\_OnDoublePickTrigger**: ``6``

On double pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:445

___

### ACTION\_OnEveryFrameTrigger

▪ `Static` `Readonly` **ACTION\_OnEveryFrameTrigger**: ``11``

On every frame

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:476

___

### ACTION\_OnIntersectionEnterTrigger

▪ `Static` `Readonly` **ACTION\_OnIntersectionEnterTrigger**: ``12``

On intersection enter

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:481

___

### ACTION\_OnIntersectionExitTrigger

▪ `Static` `Readonly` **ACTION\_OnIntersectionExitTrigger**: ``13``

On intersection exit

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:486

___

### ACTION\_OnKeyDownTrigger

▪ `Static` `Readonly` **ACTION\_OnKeyDownTrigger**: ``14``

On key down

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:491

___

### ACTION\_OnKeyUpTrigger

▪ `Static` `Readonly` **ACTION\_OnKeyUpTrigger**: ``15``

On key up

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:496

___

### ACTION\_OnLeftPickTrigger

▪ `Static` `Readonly` **ACTION\_OnLeftPickTrigger**: ``2``

On left pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:425

___

### ACTION\_OnLongPressTrigger

▪ `Static` `Readonly` **ACTION\_OnLongPressTrigger**: ``8``

On long press

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:461

___

### ACTION\_OnPickDownTrigger

▪ `Static` `Readonly` **ACTION\_OnPickDownTrigger**: ``5``

On pick down

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:440

___

### ACTION\_OnPickOutTrigger

▪ `Static` `Readonly` **ACTION\_OnPickOutTrigger**: ``16``

On pick out.
This trigger will only be raised if you also declared a OnPickDown

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:456

___

### ACTION\_OnPickTrigger

▪ `Static` `Readonly` **ACTION\_OnPickTrigger**: ``1``

On pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:420

___

### ACTION\_OnPickUpTrigger

▪ `Static` `Readonly` **ACTION\_OnPickUpTrigger**: ``7``

On pick up

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:450

___

### ACTION\_OnPointerOutTrigger

▪ `Static` `Readonly` **ACTION\_OnPointerOutTrigger**: ``10``

On pointer out

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:471

___

### ACTION\_OnPointerOverTrigger

▪ `Static` `Readonly` **ACTION\_OnPointerOverTrigger**: ``9``

On pointer over

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:466

___

### ACTION\_OnRightPickTrigger

▪ `Static` `Readonly` **ACTION\_OnRightPickTrigger**: ``3``

On right pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:430

___

### ALPHA\_ADD

▪ `Static` `Readonly` **ALPHA\_ADD**: ``1``

Defines that alpha blending is SRC ALPHA * SRC + DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:7

___

### ALPHA\_ALPHATOCOLOR

▪ `Static` `Readonly` **ALPHA\_ALPHATOCOLOR**: ``12``

Defines that alpha blending is SRC * DST ALPHA + DST
Alpha will be set to 0

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:41

___

### ALPHA\_COMBINE

▪ `Static` `Readonly` **ALPHA\_COMBINE**: ``2``

Defines that alpha blending is SRC ALPHA * SRC + (1 - SRC ALPHA) * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:9

___

### ALPHA\_DISABLE

▪ `Static` `Readonly` **ALPHA\_DISABLE**: ``0``

Defines that alpha blending is disabled

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:5

___

### ALPHA\_EQUATION\_ADD

▪ `Static` `Readonly` **ALPHA\_EQUATION\_ADD**: ``0``

Defines that alpha blending equation a SUM

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:68

___

### ALPHA\_EQUATION\_DARKEN

▪ `Static` `Readonly` **ALPHA\_EQUATION\_DARKEN**: ``5``

Defines that alpha blending equation a DARKEN operation:
It takes the min of the src and sums the alpha channels.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:81

___

### ALPHA\_EQUATION\_MAX

▪ `Static` `Readonly` **ALPHA\_EQUATION\_MAX**: ``3``

Defines that alpha blending equation a MAX operation

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:74

___

### ALPHA\_EQUATION\_MIN

▪ `Static` `Readonly` **ALPHA\_EQUATION\_MIN**: ``4``

Defines that alpha blending equation a MIN operation

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:76

___

### ALPHA\_EQUATION\_REVERSE\_SUBTRACT

▪ `Static` `Readonly` **ALPHA\_EQUATION\_REVERSE\_SUBTRACT**: ``2``

Defines that alpha blending equation a REVERSE SUBSTRACTION

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:72

___

### ALPHA\_EQUATION\_SUBSTRACT

▪ `Static` `Readonly` **ALPHA\_EQUATION\_SUBSTRACT**: ``1``

Defines that alpha blending equation a SUBSTRACTION

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:70

___

### ALPHA\_EXCLUSION

▪ `Static` `Readonly` **ALPHA\_EXCLUSION**: ``16``

Defines that alpha blending is SRC * (1 - DST) + DST * (1 - SRC)
Alpha will be set to DST ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:60

___

### ALPHA\_INTERPOLATE

▪ `Static` `Readonly` **ALPHA\_INTERPOLATE**: ``9``

Defines that alpha blending is CST * SRC + (1 - CST) * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:26

___

### ALPHA\_LAYER\_ACCUMULATE

▪ `Static` `Readonly` **ALPHA\_LAYER\_ACCUMULATE**: ``17``

Defines that alpha blending is SRC * SRC ALPHA + DST * (1 - SRC ALPHA)
Alpha will be set to SRC ALPHA + (1 - SRC ALPHA) * DST ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:65

___

### ALPHA\_MAXIMIZED

▪ `Static` `Readonly` **ALPHA\_MAXIMIZED**: ``5``

Defines that alpha blending is SRC ALPHA * SRC + (1 - SRC) * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:15

___

### ALPHA\_MULTIPLY

▪ `Static` `Readonly` **ALPHA\_MULTIPLY**: ``4``

Defines that alpha blending is SRC * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:13

___

### ALPHA\_ONEONE

▪ `Static` `Readonly` **ALPHA\_ONEONE**: ``6``

Defines that alpha blending is SRC + DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:17

___

### ALPHA\_ONEONE\_ONEONE

▪ `Static` `Readonly` **ALPHA\_ONEONE\_ONEONE**: ``11``

Defines that alpha blending is SRC + DST
Alpha will be set to SRC ALPHA + DST ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:36

___

### ALPHA\_ONEONE\_ONEZERO

▪ `Static` `Readonly` **ALPHA\_ONEONE\_ONEZERO**: ``15``

Defines that alpha blending is SRC + DST
Alpha will be set to SRC ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:55

___

### ALPHA\_PREMULTIPLIED

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED**: ``7``

Defines that alpha blending is SRC + (1 - SRC ALPHA) * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:19

___

### ALPHA\_PREMULTIPLIED\_PORTERDUFF

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED\_PORTERDUFF**: ``8``

Defines that alpha blending is SRC + (1 - SRC ALPHA) * DEST
Alpha will be set to (1 - SRC ALPHA) * DEST ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:24

___

### ALPHA\_REVERSEONEMINUS

▪ `Static` `Readonly` **ALPHA\_REVERSEONEMINUS**: ``13``

Defines that alpha blending is SRC * (1 - DST) + DST * (1 - SRC)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:45

___

### ALPHA\_SCREENMODE

▪ `Static` `Readonly` **ALPHA\_SCREENMODE**: ``10``

Defines that alpha blending is SRC + (1 - SRC) * DEST
Alpha will be set to SRC ALPHA + (1 - SRC ALPHA) * DEST ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:31

___

### ALPHA\_SRC\_DSTONEMINUSSRCALPHA

▪ `Static` `Readonly` **ALPHA\_SRC\_DSTONEMINUSSRCALPHA**: ``14``

Defines that alpha blending is SRC + DST * (1 - SRC ALPHA)
Alpha will be set to SRC ALPHA + DST ALPHA * (1 - SRC ALPHA)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:50

___

### ALPHA\_SUBTRACT

▪ `Static` `Readonly` **ALPHA\_SUBTRACT**: ``3``

Defines that alpha blending is DEST - SRC * DEST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:11

___

### ALWAYS

▪ `Static` `Readonly` **ALWAYS**: ``519``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will always pass. i.e. Pixels will be drawn in the order they are drawn

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:96

___

### BUFFER\_CREATIONFLAG\_INDEX

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_INDEX**: ``16``

Flag to create a buffer suitable to be used as an index buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:615

___

### BUFFER\_CREATIONFLAG\_READ

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_READ**: ``1``

Flag to create a readable buffer (the buffer can be the source of a copy)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:605

___

### BUFFER\_CREATIONFLAG\_READWRITE

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_READWRITE**: ``3``

Flag to create a readable and writable buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:609

___

### BUFFER\_CREATIONFLAG\_STORAGE

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_STORAGE**: ``32``

Flag to create a buffer suitable to be used as a storage buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:617

___

### BUFFER\_CREATIONFLAG\_UNIFORM

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_UNIFORM**: ``4``

Flag to create a buffer suitable to be used as a uniform buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:611

___

### BUFFER\_CREATIONFLAG\_VERTEX

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_VERTEX**: ``8``

Flag to create a buffer suitable to be used as a vertex buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:613

___

### BUFFER\_CREATIONFLAG\_WRITE

▪ `Static` `Readonly` **BUFFER\_CREATIONFLAG\_WRITE**: ``2``

Flag to create a writable buffer (the buffer can be the destination of a copy)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:607

___

### DECR

▪ `Static` `Readonly` **DECR**: ``7683``

Passed to stencilOperation to specify that stencil value must be decremented

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:120

___

### DECR\_WRAP

▪ `Static` `Readonly` **DECR\_WRAP**: ``34056``

Passed to stencilOperation to specify that stencil value must be decremented with wrapping

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:126

___

### DELAYLOADSTATE\_LOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADED**: ``1``

Defines that the resource was successfully delay loaded

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:86

___

### DELAYLOADSTATE\_LOADING

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADING**: ``2``

Defines that the resource is currently delay loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:88

___

### DELAYLOADSTATE\_NONE

▪ `Static` `Readonly` **DELAYLOADSTATE\_NONE**: ``0``

Defines that the resource is not delayed

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:84

___

### DELAYLOADSTATE\_NOTLOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_NOTLOADED**: ``4``

Defines that the resource is delayed and has not started loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:90

___

### EQUAL

▪ `Static` `Readonly` **EQUAL**: ``514``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is equals to the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:100

___

### FOVMODE\_HORIZONTAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_HORIZONTAL\_FIXED**: ``1``

This setting aligns the left and right bounds of the viewport to the left and right bounds of the camera frustum.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:682

___

### FOVMODE\_VERTICAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_VERTICAL\_FIXED**: ``0``

This is the default FOV mode for perspective cameras.
This setting aligns the upper and lower bounds of the viewport to the upper and lower bounds of the camera frustum.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:678

___

### GEQUAL

▪ `Static` `Readonly` **GEQUAL**: ``518``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than or equal to the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:106

___

### GL\_ALPHA\_EQUATION\_ADD

▪ `Static` `Readonly` **GL\_ALPHA\_EQUATION\_ADD**: ``32774``

Alpha blend equation: ADD

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:732

___

### GL\_ALPHA\_EQUATION\_MAX

▪ `Static` `Readonly` **GL\_ALPHA\_EQUATION\_MAX**: ``32776``

Alpha equation: MAX

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:736

___

### GL\_ALPHA\_EQUATION\_MIN

▪ `Static` `Readonly` **GL\_ALPHA\_EQUATION\_MIN**: ``32775``

Alpha equation: MIN

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:734

___

### GL\_ALPHA\_EQUATION\_REVERSE\_SUBTRACT

▪ `Static` `Readonly` **GL\_ALPHA\_EQUATION\_REVERSE\_SUBTRACT**: ``32779``

Alpha equation: REVERSE_SUBTRACT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:740

___

### GL\_ALPHA\_EQUATION\_SUBTRACT

▪ `Static` `Readonly` **GL\_ALPHA\_EQUATION\_SUBTRACT**: ``32778``

Alpha equation: SUBTRACT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:738

___

### GL\_ALPHA\_FUNCTION\_CONSTANT\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_CONSTANT\_ALPHA**: ``32771``

Alpha blend function: CONSTANT_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:765

___

### GL\_ALPHA\_FUNCTION\_CONSTANT\_COLOR

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_CONSTANT\_COLOR**: ``32769``

Alpha blend function: CONSTANT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:761

___

### GL\_ALPHA\_FUNCTION\_DST\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_DST\_ALPHA**: ``772``

Alpha blend function: DST_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:751

___

### GL\_ALPHA\_FUNCTION\_DST\_COLOR

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_DST\_COLOR**: ``774``

Alpha blend function: ONE_MINUS_DST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:755

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_ALPHA**: ``32772``

Alpha blend function: ONE_MINUS_CONSTANT_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:767

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_COLOR

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_CONSTANT\_COLOR**: ``32770``

Alpha blend function: ONE_MINUS_CONSTANT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:763

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_ALPHA**: ``773``

Alpha blend function: ONE_MINUS_DST_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:753

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_COLOR

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_DST\_COLOR**: ``775``

Alpha blend function: ONE_MINUS_DST

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:757

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_ALPHA**: ``771``

Alpha blend function: ONE_MINUS_SRC_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:749

___

### GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_COLOR

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_ONE\_MINUS\_SRC\_COLOR**: ``769``

Alpha blend function: ONE_MINUS_SRC

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:745

___

### GL\_ALPHA\_FUNCTION\_SRC

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_SRC**: ``768``

Alpha blend function: SRC

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:743

___

### GL\_ALPHA\_FUNCTION\_SRC\_ALPHA

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_SRC\_ALPHA**: ``770``

Alpha blend function: SRC_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:747

___

### GL\_ALPHA\_FUNCTION\_SRC\_ALPHA\_SATURATED

▪ `Static` `Readonly` **GL\_ALPHA\_FUNCTION\_SRC\_ALPHA\_SATURATED**: ``776``

Alpha blend function: SRC_ALPHA_SATURATED

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:759

___

### GREATER

▪ `Static` `Readonly` **GREATER**: ``516``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:104

___

### INCR

▪ `Static` `Readonly` **INCR**: ``7682``

Passed to stencilOperation to specify that stencil value must be incremented

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:118

___

### INCR\_WRAP

▪ `Static` `Readonly` **INCR\_WRAP**: ``34055``

Passed to stencilOperation to specify that stencil value must be incremented with wrapping

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:124

___

### INPUT\_ALT\_KEY

▪ `Static` `Readonly` **INPUT\_ALT\_KEY**: ``18``

Constant used as key code for Alt key

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:629

___

### INPUT\_CTRL\_KEY

▪ `Static` `Readonly` **INPUT\_CTRL\_KEY**: ``17``

Constant used as key code for Ctrl key

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:634

___

### INPUT\_META\_KEY1

▪ `Static` `Readonly` **INPUT\_META\_KEY1**: ``91``

Constant used as key code for Meta key (Left Win, Left Cmd)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:639

___

### INPUT\_META\_KEY2

▪ `Static` `Readonly` **INPUT\_META\_KEY2**: ``92``

Constant used as key code for Meta key (Right Win)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:644

___

### INPUT\_META\_KEY3

▪ `Static` `Readonly` **INPUT\_META\_KEY3**: ``93``

Constant used as key code for Meta key (Right Win, Right Cmd)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:649

___

### INPUT\_SHIFT\_KEY

▪ `Static` `Readonly` **INPUT\_SHIFT\_KEY**: ``16``

Constant used as key code for Shift key

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:654

___

### INVERT

▪ `Static` `Readonly` **INVERT**: ``5386``

Passed to stencilOperation to specify that stencil value must be inverted

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:122

___

### KEEP

▪ `Static` `Readonly` **KEEP**: ``7680``

Passed to stencilOperation to specify that stencil value must be kept

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:112

___

### LEQUAL

▪ `Static` `Readonly` **LEQUAL**: ``515``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than or equal to the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:102

___

### LESS

▪ `Static` `Readonly` **LESS**: ``513``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:98

___

### MATERIAL\_AllDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_AllDirtyFlag**: ``63``

The all dirty flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:362

___

### MATERIAL\_AttributesDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:350

___

### MATERIAL\_ClockWiseSideOrientation

▪ `Static` `Readonly` **MATERIAL\_ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:405

___

### MATERIAL\_CounterClockWiseSideOrientation

▪ `Static` `Readonly` **MATERIAL\_CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:409

___

### MATERIAL\_FresnelDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:346

___

### MATERIAL\_LightDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_LightDirtyFlag**: ``2``

The dirty light flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:342

___

### MATERIAL\_LineListDrawMode

▪ `Static` `Readonly` **MATERIAL\_LineListDrawMode**: ``4``

Returns the line list draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:383

___

### MATERIAL\_LineLoopDrawMode

▪ `Static` `Readonly` **MATERIAL\_LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:387

___

### MATERIAL\_LineStripDrawMode

▪ `Static` `Readonly` **MATERIAL\_LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:391

___

### MATERIAL\_MiscDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:354

___

### MATERIAL\_PointFillMode

▪ `Static` `Readonly` **MATERIAL\_PointFillMode**: ``2``

Returns the point fill mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:375

___

### MATERIAL\_PointListDrawMode

▪ `Static` `Readonly` **MATERIAL\_PointListDrawMode**: ``3``

Returns the point list draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:379

___

### MATERIAL\_PrePassDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:358

___

### MATERIAL\_TextureDirtyFlag

▪ `Static` `Readonly` **MATERIAL\_TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:338

___

### MATERIAL\_TriangleFanDrawMode

▪ `Static` `Readonly` **MATERIAL\_TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:400

___

### MATERIAL\_TriangleFillMode

▪ `Static` `Readonly` **MATERIAL\_TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:367

___

### MATERIAL\_TriangleStripDrawMode

▪ `Static` `Readonly` **MATERIAL\_TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:396

___

### MATERIAL\_WireFrameFillMode

▪ `Static` `Readonly` **MATERIAL\_WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:371

___

### MAX\_SUPPORTED\_UV\_SETS

▪ `Static` `Readonly` **MAX\_SUPPORTED\_UV\_SETS**: ``6``

Maximum number of uv sets supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:726

___

### MESHES\_CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY

▪ `Static` `Readonly` **MESHES\_CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY**: ``1``

Culling strategy : Bounding Sphere Only.
 This is an exclusion test. It's faster than the standard strategy because the bounding box is not tested.
 It's also less accurate than the standard because some not visible objects can still be selected.
 Test : is the bounding sphere outside the frustum ?
 If not, then the cullable object is in the frustum.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:524

___

### MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION

▪ `Static` `Readonly` **MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION**: ``2``

Culling strategy : Optimistic Inclusion.
 This in an inclusion test first, then the standard exclusion test.
 This can be faster when a cullable object is expected to be almost always in the camera frustum.
 This could also be a little slower than the standard test when the tested object center is not the frustum but one of its bounding box vertex is still inside.
 Anyway, it's as accurate as the standard strategy.
 Test :
 Is the cullable object bounding sphere center in the frustum ?
 If not, apply the default culling strategy.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:534

___

### MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY

▪ `Static` `Readonly` **MESHES\_CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY**: ``3``

Culling strategy : Optimistic Inclusion then Bounding Sphere Only.
 This in an inclusion test first, then the bounding sphere only exclusion test.
 This can be the fastest test when a cullable object is expected to be almost always in the camera frustum.
 This could also be a little slower than the BoundingSphereOnly strategy when the tested object center is not in the frustum but its bounding sphere still intersects it.
 It's less accurate than the standard strategy and as accurate as the BoundingSphereOnly strategy.
 Test :
 Is the cullable object bounding sphere center in the frustum ?
 If not, apply the Bounding Sphere Only strategy. No Bounding Box is tested here.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:544

___

### MESHES\_CULLINGSTRATEGY\_STANDARD

▪ `Static` `Readonly` **MESHES\_CULLINGSTRATEGY\_STANDARD**: ``0``

Default culling strategy : this is an exclusion test and it's the more accurate.
 Test order :
 Is the bounding sphere outside the frustum ?
 If not, are the bounding box vertices outside the frustum ?
 It not, then the cullable object is in the frustum.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:517

___

### NEVER

▪ `Static` `Readonly` **NEVER**: ``512``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will never pass. i.e. Nothing will be drawn

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:94

___

### NOTEQUAL

▪ `Static` `Readonly` **NOTEQUAL**: ``517``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is not equal to the stored value

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:108

___

### ORTHOGRAPHIC\_CAMERA

▪ `Static` `Readonly` **ORTHOGRAPHIC\_CAMERA**: ``1``

This helps creating camera with an orthographic mode.
Orthographic is commonly used in engineering as a means to produce object specifications that communicate dimensions unambiguously, each line of 1 unit length (cm, meter..whatever) will appear to have the same length everywhere on the drawing. This allows the drafter to dimension only a subset of lines and let the reader know that other lines of that length on the drawing are also that length in reality. Every parallel line in the drawing is also parallel in the object.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:672

___

### PARTICLES\_BILLBOARDMODE\_ALL

▪ `Static` `Readonly` **PARTICLES\_BILLBOARDMODE\_ALL**: ``7``

Billboard mode will apply to all axes

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:505

___

### PARTICLES\_BILLBOARDMODE\_STRETCHED

▪ `Static` `Readonly` **PARTICLES\_BILLBOARDMODE\_STRETCHED**: ``8``

Special billboard mode where the particle will be biilboard to the camera but rotated to align with direction

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:509

___

### PARTICLES\_BILLBOARDMODE\_Y

▪ `Static` `Readonly` **PARTICLES\_BILLBOARDMODE\_Y**: ``2``

Billboard mode will only apply to Y axis

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:501

___

### PERSPECTIVE\_CAMERA

▪ `Static` `Readonly` **PERSPECTIVE\_CAMERA**: ``0``

This is the default projection mode used by the cameras.
It helps recreating a feeling of perspective and better appreciate depth.
This is the best way to simulate real life cameras.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:667

___

### PREPASS\_ALBEDO\_SQRT\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_ALBEDO\_SQRT\_TEXTURE\_TYPE**: ``7``

Constant used to retrieve albedo index in the textures array in the prepass
using the getIndex(Constants.PREPASS_ALBEDO_SQRT_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:602

___

### PREPASS\_COLOR\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_COLOR\_TEXTURE\_TYPE**: ``4``

Constant used to retrieve the lit color texture index in the textures array in the prepass
using the getIndex(Constants.PREPASS_COLOR_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:587

___

### PREPASS\_DEPTH\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_DEPTH\_TEXTURE\_TYPE**: ``5``

Constant used to retrieve depth index in the textures array in the prepass
using the getIndex(Constants.PREPASS_DEPTH_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:592

___

### PREPASS\_IRRADIANCE\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_IRRADIANCE\_TEXTURE\_TYPE**: ``0``

Constant used to retrieve the irradiance texture index in the textures array in the prepass
using getIndex(Constants.PREPASS_IRRADIANCE_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:567

___

### PREPASS\_NORMAL\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_NORMAL\_TEXTURE\_TYPE**: ``6``

Constant used to retrieve normal index in the textures array in the prepass
using the getIndex(Constants.PREPASS_NORMAL_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:597

___

### PREPASS\_POSITION\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_POSITION\_TEXTURE\_TYPE**: ``1``

Constant used to retrieve the position texture index in the textures array in the prepass
using getIndex(Constants.PREPASS_POSITION_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:572

___

### PREPASS\_REFLECTIVITY\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_REFLECTIVITY\_TEXTURE\_TYPE**: ``3``

Constant used to retrieve the reflectivity texture index in the textures array in the prepass
using the getIndex(Constants.PREPASS_REFLECTIVITY_TEXTURE_TYPE)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:582

___

### PREPASS\_VELOCITY\_TEXTURE\_TYPE

▪ `Static` `Readonly` **PREPASS\_VELOCITY\_TEXTURE\_TYPE**: ``2``

Constant used to retrieve the velocity texture index in the textures array in the prepass
using getIndex(Constants.PREPASS_VELOCITY_TEXTURE_INDEX)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:577

___

### REPLACE

▪ `Static` `Readonly` **REPLACE**: ``7681``

Passed to stencilOperation to specify that stencil value must be replaced

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:116

___

### RIG\_MODE\_CUSTOM

▪ `Static` `Readonly` **RIG\_MODE\_CUSTOM**: ``22``

Custom rig mode allowing rig cameras to be populated manually with any number of cameras

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:721

___

### RIG\_MODE\_NONE

▪ `Static` `Readonly` **RIG\_MODE\_NONE**: ``0``

This specifies there is no need for a camera rig.
Basically only one eye is rendered corresponding to the camera.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:688

___

### RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH**: ``10``

Simulates a camera Rig with one blue eye and one red eye.
This can be use with 3d blue and red glasses.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:693

___

### RIG\_MODE\_STEREOSCOPIC\_INTERLACED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_INTERLACED**: ``14``

Defines that both eyes of the camera will be rendered on successive lines interlaced for passive 3d monitors.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:709

___

### RIG\_MODE\_STEREOSCOPIC\_OVERUNDER

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_OVERUNDER**: ``13``

Defines that both eyes of the camera will be rendered over under each other.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:705

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED**: ``12``

Defines that both eyes of the camera will be rendered side by side with a none parallel target.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:701

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL**: ``11``

Defines that both eyes of the camera will be rendered side by side with a parallel target.

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:697

___

### RIG\_MODE\_VR

▪ `Static` `Readonly` **RIG\_MODE\_VR**: ``20``

Defines that both eyes of the camera should be renderered in a VR mode (carbox).

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:713

___

### RIG\_MODE\_WEBVR

▪ `Static` `Readonly` **RIG\_MODE\_WEBVR**: ``21``

Defines that both eyes of the camera should be renderered in a VR mode (webVR).

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:717

___

### SCALEMODE\_CEILING

▪ `Static` `Readonly` **SCALEMODE\_CEILING**: ``3``

Defines that texture rescaling will use a ceil to find the closer power of 2 size

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:333

___

### SCALEMODE\_FLOOR

▪ `Static` `Readonly` **SCALEMODE\_FLOOR**: ``1``

Defines that texture rescaling will use a floor to find the closer power of 2 size

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:329

___

### SCALEMODE\_NEAREST

▪ `Static` `Readonly` **SCALEMODE\_NEAREST**: ``2``

Defines that texture rescaling will look for the nearest power of 2 size

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:331

___

### SCENELOADER\_DETAILED\_LOGGING

▪ `Static` `Readonly` **SCENELOADER\_DETAILED\_LOGGING**: ``3``

Detailed logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:561

___

### SCENELOADER\_MINIMAL\_LOGGING

▪ `Static` `Readonly` **SCENELOADER\_MINIMAL\_LOGGING**: ``1``

Minimal logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:553

___

### SCENELOADER\_NO\_LOGGING

▪ `Static` `Readonly` **SCENELOADER\_NO\_LOGGING**: ``0``

No logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:549

___

### SCENELOADER\_SUMMARY\_LOGGING

▪ `Static` `Readonly` **SCENELOADER\_SUMMARY\_LOGGING**: ``2``

Summary logging while loading

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:557

___

### SNAPSHOTRENDERING\_FAST

▪ `Static` `Readonly` **SNAPSHOTRENDERING\_FAST**: ``1``

Fast snapshot rendering. In this mode, everything is static and only some limited form of dynamic behaviour is possible

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:660

___

### SNAPSHOTRENDERING\_STANDARD

▪ `Static` `Readonly` **SNAPSHOTRENDERING\_STANDARD**: ``0``

Standard snapshot rendering. In this mode, some form of dynamic behavior is possible (for eg, uniform buffers are still updated)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:657

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `"https://snippet.babylonjs.com"`

URL to the snippet server. Points to the public snippet server by default

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:770

___

### TEXTUREFORMAT\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_ALPHA**: ``0``

ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:139

___

### TEXTUREFORMAT\_BGRA

▪ `Static` `Readonly` **TEXTUREFORMAT\_BGRA**: ``12``

BGRA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:165

___

### TEXTUREFORMAT\_COMPRESSED\_RGB8\_ETC2

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB8\_ETC2**: ``37492``

Compressed ETC2 (RGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:211

___

### TEXTUREFORMAT\_COMPRESSED\_RGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2**: ``37494``

Compressed ETC2 (RGB+A1)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:215

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA8\_ETC2\_EAC

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA8\_ETC2\_EAC**: ``37496``

Compressed ETC2 (RGB+A)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:219

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA\_ASTC\_4x4

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA\_ASTC\_4x4**: ``37808``

Compressed ASTC 4x4

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:205

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA\_BPTC\_UNORM

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA\_BPTC\_UNORM**: ``36492``

Compressed BC7

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:181

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT1

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT1**: ``33777``

Compressed BC1 (RGBA)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:197

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT3

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT3**: ``33778``

Compressed BC2

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:193

___

### TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT5

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGBA\_S3TC\_DXT5**: ``33779``

Compressed BC3

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:189

___

### TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_SIGNED\_FLOAT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_SIGNED\_FLOAT**: ``36494``

Compressed BC6 signed float

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:187

___

### TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_UNSIGNED\_FLOAT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB\_BPTC\_UNSIGNED\_FLOAT**: ``36495``

Compressed BC6 unsigned float

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:185

___

### TEXTUREFORMAT\_COMPRESSED\_RGB\_ETC1\_WEBGL

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB\_ETC1\_WEBGL**: ``36196``

Compressed ETC1 (RGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:209

___

### TEXTUREFORMAT\_COMPRESSED\_RGB\_S3TC\_DXT1

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_RGB\_S3TC\_DXT1**: ``33776``

Compressed BC1 (RGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:199

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ASTC\_4x4\_KHR

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ASTC\_4x4\_KHR**: ``37840``

Compressed ASTC 4x4 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:207

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ETC2\_EAC

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ALPHA8\_ETC2\_EAC**: ``37497``

Compressed ETC2 (SRGB+1)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:221

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ETC2

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB8\_ETC2**: ``37493``

Compressed ETC2 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:213

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB8\_PUNCHTHROUGH\_ALPHA1\_ETC2**: ``37495``

Compressed ETC2 (SRGB+A1)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:217

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_BPTC\_UNORM

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_BPTC\_UNORM**: ``36493``

Compressed BC7 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:183

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT1\_EXT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT1\_EXT**: ``35917``

Compressed BC1 (SRGB+A)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:201

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT3\_EXT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT3\_EXT**: ``35918``

Compressed BC2 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:195

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT5\_EXT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB\_ALPHA\_S3TC\_DXT5\_EXT**: ``35919``

Compressed BC3 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:191

___

### TEXTUREFORMAT\_COMPRESSED\_SRGB\_S3TC\_DXT1\_EXT

▪ `Static` `Readonly` **TEXTUREFORMAT\_COMPRESSED\_SRGB\_S3TC\_DXT1\_EXT**: ``35916``

Compressed BC1 (SRGB)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:203

___

### TEXTUREFORMAT\_DEPTH16

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH16**: ``15``

Depth 16 bits

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:172

___

### TEXTUREFORMAT\_DEPTH24

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH24**: ``16``

Depth 24 bits

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:174

___

### TEXTUREFORMAT\_DEPTH24UNORM\_STENCIL8

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH24UNORM\_STENCIL8**: ``17``

Depth 24 bits unorm + Stencil 8 bits

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:176

___

### TEXTUREFORMAT\_DEPTH24\_STENCIL8

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH24\_STENCIL8**: ``13``

Depth 24 bits + Stencil 8 bits

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:168

___

### TEXTUREFORMAT\_DEPTH32FLOAT\_STENCIL8

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH32FLOAT\_STENCIL8**: ``18``

Depth 32 bits float + Stencil 8 bits

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:178

___

### TEXTUREFORMAT\_DEPTH32\_FLOAT

▪ `Static` `Readonly` **TEXTUREFORMAT\_DEPTH32\_FLOAT**: ``14``

Depth 32 bits float

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:170

___

### TEXTUREFORMAT\_LUMINANCE

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE**: ``1``

LUMINANCE

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:141

___

### TEXTUREFORMAT\_LUMINANCE\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE\_ALPHA**: ``2``

LUMINANCE_ALPHA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:143

___

### TEXTUREFORMAT\_R

▪ `Static` `Readonly` **TEXTUREFORMAT\_R**: ``6``

RED (2nd reference)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:151

___

### TEXTUREFORMAT\_RED

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED**: ``6``

RED

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:149

___

### TEXTUREFORMAT\_RED\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED\_INTEGER**: ``8``

RED_INTEGER

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:155

___

### TEXTUREFORMAT\_RG

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG**: ``7``

RG

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:153

___

### TEXTUREFORMAT\_RGB

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB**: ``4``

RGB

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:145

___

### TEXTUREFORMAT\_RGBA

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA**: ``5``

RGBA

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:147

___

### TEXTUREFORMAT\_RGBA\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA\_INTEGER**: ``11``

RGBA_INTEGER

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:163

___

### TEXTUREFORMAT\_RGB\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB\_INTEGER**: ``10``

RGB_INTEGER

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:161

___

### TEXTUREFORMAT\_RG\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG\_INTEGER**: ``9``

RG_INTEGER

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:159

___

### TEXTUREFORMAT\_R\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_R\_INTEGER**: ``8``

RED_INTEGER (2nd reference)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:157

___

### TEXTURETYPE\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_BYTE**: ``3``

BYTE

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:232

___

### TEXTURETYPE\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT**: ``1``

FLOAT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:228

___

### TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV**: ``15``

FLOAT_32_UNSIGNED_INT_24_8_REV

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:256

___

### TEXTURETYPE\_HALF\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_HALF\_FLOAT**: ``2``

HALF_FLOAT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:230

___

### TEXTURETYPE\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_INT**: ``6``

INT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:238

___

### TEXTURETYPE\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_SHORT**: ``4``

SHORT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:234

___

### TEXTURETYPE\_UNDEFINED

▪ `Static` `Readonly` **TEXTURETYPE\_UNDEFINED**: ``16``

UNDEFINED

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:258

___

### TEXTURETYPE\_UNSIGNED\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_BYTE**: ``0``

UNSIGNED_BYTE

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:224

___

### TEXTURETYPE\_UNSIGNED\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT**: ``0``

UNSIGNED_BYTE (2nd reference)

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:226

___

### TEXTURETYPE\_UNSIGNED\_INTEGER

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INTEGER**: ``7``

UNSIGNED_INT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:240

___

### TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV**: ``13``

UNSIGNED_INT_10F_11F_11F_REV

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:252

___

### TEXTURETYPE\_UNSIGNED\_INT\_24\_8

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_24\_8**: ``12``

UNSIGNED_INT_24_8

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:250

___

### TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV**: ``11``

UNSIGNED_INT_2_10_10_10_REV

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:248

___

### TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV**: ``14``

UNSIGNED_INT_5_9_9_9_REV

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:254

___

### TEXTURETYPE\_UNSIGNED\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT**: ``5``

UNSIGNED_SHORT

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:236

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4**: ``8``

UNSIGNED_SHORT_4_4_4_4

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:242

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1**: ``9``

UNSIGNED_SHORT_5_5_5_1

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:244

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5**: ``10``

UNSIGNED_SHORT_5_6_5

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:246

___

### TEXTURE\_BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and no mip

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:266

___

### TEXTURE\_CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:129

___

### TEXTURE\_CREATIONFLAG\_STORAGE

▪ `Static` `Readonly` **TEXTURE\_CREATIONFLAG\_STORAGE**: ``1``

Flag to create a storage texture

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:136

___

### TEXTURE\_CUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:301

___

### TEXTURE\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:309

___

### TEXTURE\_EXPLICIT\_MODE

▪ `Static` `Readonly` **TEXTURE\_EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:295

___

### TEXTURE\_FILTERING\_QUALITY\_HIGH

▪ `Static` `Readonly` **TEXTURE\_FILTERING\_QUALITY\_HIGH**: ``64``

High quality for texture filtering

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:319

___

### TEXTURE\_FILTERING\_QUALITY\_LOW

▪ `Static` `Readonly` **TEXTURE\_FILTERING\_QUALITY\_LOW**: ``8``

Low quality for texture filtering

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:325

___

### TEXTURE\_FILTERING\_QUALITY\_MEDIUM

▪ `Static` `Readonly` **TEXTURE\_FILTERING\_QUALITY\_MEDIUM**: ``16``

Medium quality for texture filtering

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:322

___

### TEXTURE\_FILTERING\_QUALITY\_OFFLINE

▪ `Static` `Readonly` **TEXTURE\_FILTERING\_QUALITY\_OFFLINE**: ``4096``

Offline (baking) quality for texture filtering

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:316

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:313

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:311

___

### TEXTURE\_INVCUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:307

___

### TEXTURE\_LINEAR\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:268

___

### TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:273

___

### TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:290

___

### TEXTURE\_LINEAR\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:292

___

### TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:288

___

### TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:286

___

### TEXTURE\_MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:133

___

### TEXTURE\_NEAREST\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:282

___

### TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:280

___

### TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:278

___

### TEXTURE\_NEAREST\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:263

___

### TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:284

___

### TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:276

___

### TEXTURE\_NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and no mip

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:261

___

### TEXTURE\_PLANAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:299

___

### TEXTURE\_PROJECTION\_MODE

▪ `Static` `Readonly` **TEXTURE\_PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:303

___

### TEXTURE\_SKYBOX\_MODE

▪ `Static` `Readonly` **TEXTURE\_SKYBOX\_MODE**: ``5``

Skybox coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:305

___

### TEXTURE\_SPHERICAL\_MODE

▪ `Static` `Readonly` **TEXTURE\_SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:297

___

### TEXTURE\_TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:271

___

### TEXTURE\_WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:131

___

### ZERO

▪ `Static` `Readonly` **ZERO**: ``0``

Passed to stencilOperation to specify that stencil value must be zero

#### Defined in

https://github.com/babylon.js/core/src/Engines/constants.ts:114

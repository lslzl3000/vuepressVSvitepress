[@dev/core](../README.md) / [Exports](../modules.md) / HandConstraintVisibility

# Enumeration: HandConstraintVisibility

Orientations for the hand zones and for the attached node

## Table of contents

### Enumeration Members

- [ALWAYS\_VISIBLE](HandConstraintVisibility.md#always_visible)
- [GAZE\_FOCUS](HandConstraintVisibility.md#gaze_focus)
- [PALM\_AND\_GAZE](HandConstraintVisibility.md#palm_and_gaze)
- [PALM\_UP](HandConstraintVisibility.md#palm_up)

## Enumeration Members

### ALWAYS\_VISIBLE

• **ALWAYS\_VISIBLE** = ``0``

Constraint is always visible

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:57

___

### GAZE\_FOCUS

• **GAZE\_FOCUS** = ``2``

Constraint is only visible when the user is looking at the constraint.
Uses XR Eye Tracking if enabled/available, otherwise uses camera direction

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:66

___

### PALM\_AND\_GAZE

• **PALM\_AND\_GAZE** = ``3``

Constraint is only visible when the palm is up and the user is looking at it

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:70

___

### PALM\_UP

• **PALM\_UP** = ``1``

Constraint is only visible when the palm is up

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:61

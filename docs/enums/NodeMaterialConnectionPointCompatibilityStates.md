[@dev/core](../README.md) / [Exports](../modules.md) / NodeMaterialConnectionPointCompatibilityStates

# Enumeration: NodeMaterialConnectionPointCompatibilityStates

Enum used to define the compatibility state between two connection points

## Table of contents

### Enumeration Members

- [Compatible](NodeMaterialConnectionPointCompatibilityStates.md#compatible)
- [HierarchyIssue](NodeMaterialConnectionPointCompatibilityStates.md#hierarchyissue)
- [TargetIncompatible](NodeMaterialConnectionPointCompatibilityStates.md#targetincompatible)
- [TypeIncompatible](NodeMaterialConnectionPointCompatibilityStates.md#typeincompatible)

## Enumeration Members

### Compatible

• **Compatible** = ``0``

Points are compatibles

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:14

___

### HierarchyIssue

• **HierarchyIssue** = ``3``

Points are incompatible because they are in the same hierarchy *

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:20

___

### TargetIncompatible

• **TargetIncompatible** = ``2``

Points are incompatible because of their targets (vertex vs fragment)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:18

___

### TypeIncompatible

• **TypeIncompatible** = ``1``

Points are incompatible because of their types

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialBlockConnectionPoint.ts:16

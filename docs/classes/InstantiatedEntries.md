[@dev/core](../README.md) / [Exports](../modules.md) / InstantiatedEntries

# Class: InstantiatedEntries

Class used to store the output of the AssetContainer.instantiateAllMeshesToScene function

## Table of contents

### Constructors

- [constructor](InstantiatedEntries.md#constructor)

### Properties

- [animationGroups](InstantiatedEntries.md#animationgroups)
- [rootNodes](InstantiatedEntries.md#rootnodes)
- [skeletons](InstantiatedEntries.md#skeletons)

## Constructors

### constructor

• **new InstantiatedEntries**()

## Properties

### animationGroups

• **animationGroups**: [`AnimationGroup`](AnimationGroup.md)[] = `[]`

List of new animation groups

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:40

___

### rootNodes

• **rootNodes**: [`TransformNode`](TransformNode.md)[] = `[]`

List of new root nodes (eg. nodes with no parent)

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:30

___

### skeletons

• **skeletons**: [`Skeleton`](Skeleton.md)[] = `[]`

List of new skeletons

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:35

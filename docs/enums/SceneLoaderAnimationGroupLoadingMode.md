[@dev/core](../README.md) / [Exports](../modules.md) / SceneLoaderAnimationGroupLoadingMode

# Enumeration: SceneLoaderAnimationGroupLoadingMode

Mode that determines how to handle old animation groups before loading new ones.

## Table of contents

### Enumeration Members

- [Clean](SceneLoaderAnimationGroupLoadingMode.md#clean)
- [NoSync](SceneLoaderAnimationGroupLoadingMode.md#nosync)
- [Stop](SceneLoaderAnimationGroupLoadingMode.md#stop)
- [Sync](SceneLoaderAnimationGroupLoadingMode.md#sync)

## Enumeration Members

### Clean

• **Clean** = ``0``

Reset all old animations to initial state then dispose them.

#### Defined in

packages/dev/core/src/Loading/sceneLoader.ts:290

___

### NoSync

• **NoSync** = ``3``

Old animations remains untouched.

#### Defined in

packages/dev/core/src/Loading/sceneLoader.ts:305

___

### Stop

• **Stop** = ``1``

Stop all old animations.

#### Defined in

packages/dev/core/src/Loading/sceneLoader.ts:295

___

### Sync

• **Sync** = ``2``

Restart old animations from first frame.

#### Defined in

packages/dev/core/src/Loading/sceneLoader.ts:300

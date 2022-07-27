[@dev/core](../README.md) / [Exports](../modules.md) / BabylonFileLoaderConfiguration

# Class: BabylonFileLoaderConfiguration

Helps setting up some configuration for the babylon file loader.

## Table of contents

### Constructors

- [constructor](BabylonFileLoaderConfiguration.md#constructor)

### Properties

- [LoaderInjectedPhysicsEngine](BabylonFileLoaderConfiguration.md#loaderinjectedphysicsengine)

## Constructors

### constructor

• **new BabylonFileLoaderConfiguration**()

## Properties

### LoaderInjectedPhysicsEngine

▪ `Static` **LoaderInjectedPhysicsEngine**: `any` = `undefined`

The loader does not allow injecting custom physics engine into the plugins.
Unfortunately in ES6, we need to manually inject them into the plugin.
So you could set this variable to your engine import to make it work.

#### Defined in

packages/dev/core/src/Loading/Plugins/babylonFileLoader.ts:47

[@dev/core](../README.md) / [Exports](../modules.md) / IEdgesRendererOptions

# Interface: IEdgesRendererOptions

Defines the additional options of the edges renderer

## Table of contents

### Properties

- [applyTessellation](IEdgesRendererOptions.md#applytessellation)
- [epsilonVertexAligned](IEdgesRendererOptions.md#epsilonvertexaligned)
- [epsilonVertexMerge](IEdgesRendererOptions.md#epsilonvertexmerge)
- [removeDegeneratedTriangles](IEdgesRendererOptions.md#removedegeneratedtriangles)
- [useAlternateEdgeFinder](IEdgesRendererOptions.md#usealternateedgefinder)
- [useFastVertexMerger](IEdgesRendererOptions.md#usefastvertexmerger)

## Properties

### applyTessellation

• `Optional` **applyTessellation**: `boolean`

Gets or sets a boolean indicating that tessellation should be applied before finding the edges. You may need to activate this option if your geometry is a bit
unusual, like having a vertex of a triangle in-between two vertices of an edge of another triangle. It happens often when using CSG to construct meshes.
This option is used only if useAlternateEdgeFinder = true

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:166

___

### epsilonVertexAligned

• `Optional` **epsilonVertexAligned**: `number`

The limit under which 3 vertices are considered to be aligned. 3 vertices PQR are considered aligned if distance(PQ) + distance(QR) - distance(PR)  epsilonVertexAligned
The default value is 1e-6
This option is used only if useAlternateEdgeFinder = true

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:173

___

### epsilonVertexMerge

• `Optional` **epsilonVertexMerge**: `number`

During edges processing, the vertices are merged if they are close enough: epsilonVertexMerge is the limit within which vertices are considered to be equal.
The default value is 1e-6
This option is used only if useAlternateEdgeFinder = true

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:159

___

### removeDegeneratedTriangles

• `Optional` **removeDegeneratedTriangles**: `boolean`

Gets or sets a boolean indicating that degenerated triangles should not be processed.
Degenerated triangles are triangles that have 2 or 3 vertices with the same coordinates

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:179

___

### useAlternateEdgeFinder

• `Optional` **useAlternateEdgeFinder**: `boolean`

Gets or sets a boolean indicating that the alternate edge finder algorithm must be used
If not defined, the default value is true

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:144

___

### useFastVertexMerger

• `Optional` **useFastVertexMerger**: `boolean`

Gets or sets a boolean indicating that the vertex merger fast processing must be used.
If not defined, the default value is true.
You should normally leave it undefined (or set it to true), except if you see some artifacts in the edges rendering (can happen with complex geometries)
This option is used only if useAlternateEdgeFinder = true

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:152

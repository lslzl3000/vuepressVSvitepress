[@dev/core](../README.md) / [Exports](../modules.md) / INavMeshParameters

# Interface: INavMeshParameters

Configures the navigation mesh creation

## Table of contents

### Properties

- [borderSize](INavMeshParameters.md#bordersize)
- [ch](INavMeshParameters.md#ch)
- [cs](INavMeshParameters.md#cs)
- [detailSampleDist](INavMeshParameters.md#detailsampledist)
- [detailSampleMaxError](INavMeshParameters.md#detailsamplemaxerror)
- [maxEdgeLen](INavMeshParameters.md#maxedgelen)
- [maxSimplificationError](INavMeshParameters.md#maxsimplificationerror)
- [maxVertsPerPoly](INavMeshParameters.md#maxvertsperpoly)
- [mergeRegionArea](INavMeshParameters.md#mergeregionarea)
- [minRegionArea](INavMeshParameters.md#minregionarea)
- [tileSize](INavMeshParameters.md#tilesize)
- [walkableClimb](INavMeshParameters.md#walkableclimb)
- [walkableHeight](INavMeshParameters.md#walkableheight)
- [walkableRadius](INavMeshParameters.md#walkableradius)
- [walkableSlopeAngle](INavMeshParameters.md#walkableslopeangle)

## Properties

### borderSize

• `Optional` **borderSize**: `number`

The size of the non-navigable border around the heightfield.

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:468

___

### ch

• **ch**: `number`

The y-axis cell size to use for fields. [Limit: > 0] [Units: wu]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:394

___

### cs

• **cs**: `number`

The xz-plane cell size to use for fields. [Limit: > 0] [Units: wu]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:389

___

### detailSampleDist

• **detailSampleDist**: `number`

Sets the sampling distance to use when generating the detail mesh.
(For height detail only.) [Limits: 0 or >= 0.9] [Units: wu]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:450

___

### detailSampleMaxError

• **detailSampleMaxError**: `number`

The maximum distance the detail mesh surface should deviate from heightfield
data. (For height detail only.) [Limit: >=0] [Units: wu]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:456

___

### maxEdgeLen

• **maxEdgeLen**: `number`

The maximum allowed length for contour edges along the border of the mesh. [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:421

___

### maxSimplificationError

• **maxSimplificationError**: `number`

The maximum distance a simplified contour's border edges should deviate
the original raw contour. [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:427

___

### maxVertsPerPoly

• **maxVertsPerPoly**: `number`

The maximum number of vertices allowed for polygons generated during the
contour to polygon conversion process. [Limit: >= 3]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:444

___

### mergeRegionArea

• **mergeRegionArea**: `number`

Any regions with a span count smaller than this value will, if possible,
be merged with larger regions. [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:438

___

### minRegionArea

• **minRegionArea**: `number`

The minimum number of cells allowed to form isolated island areas. [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:432

___

### tileSize

• `Optional` **tileSize**: `number`

If using obstacles, the navmesh must be subdivided internaly by tiles.
This member defines the tile cube side length in world units.
If no obstacles are needed, leave it undefined or 0.

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:463

___

### walkableClimb

• **walkableClimb**: `number`

Maximum ledge height that is considered to still be traversable. [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:410

___

### walkableHeight

• **walkableHeight**: `number`

Minimum floor to 'ceiling' height that will still allow the floor area to
be considered walkable. [Limit: >= 3] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:405

___

### walkableRadius

• **walkableRadius**: `number`

The distance to erode/shrink the walkable area of the heightfield away from
obstructions.  [Limit: >=0] [Units: vx]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:416

___

### walkableSlopeAngle

• **walkableSlopeAngle**: `number`

The maximum slope that is considered walkable. [Limits: 0 = value  90] [Units: Degrees]

#### Defined in

https://github.com/babylon.js/core/src/Navigation/INavigationEngine.ts:399

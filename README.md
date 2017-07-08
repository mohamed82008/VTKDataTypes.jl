# VTKDataTypes
## Overview
VTKDataTypes.jl presents a Julia types system for representing and manipulating VTK data natively in Julia. **VTKDataTypes.jl only supports Julia v0.6.**

## Summary of capabilities
### VTK data representation
You can use VTKDataTypes.jl to create your own VTK data object of any of the following types: `VTKUnstructuredData`, `VTKPolyData`, `VTKStructuredData`, `VTKRectilinearData`, `VTKImageData`, `VTKMultiblockData`, and `VTKTimeseriesData`. 2D and 3D are both supported and conversion functions are defined where they make sense.

### Decomposing and triangulation
You can use the `decompose` function to decompose your VTK data object to faces or lines averaging cell data of all participating cells in the process. The `triangulage` function is also defined for interfacing with other rendering and visualization modules which require a triangular mesh.

### Interfacing with GeometryTypes.jl
You can use the `GLMesh` function to change a VTK data object to a triangulated `HomogenousMesh`.

## Examples

Please refer to the `tests` folder for examples.

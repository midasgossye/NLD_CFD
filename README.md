# NLD_CFD

CFD simulation of cylinder in wind using atmospheric boundary layer wall functions and simpleFOAM solver. 

## Meshing

Standard blockmesh that gets adapted using SnappyHexMesh to incorporate cylinder. ExtrudeMesh to convert to 2D case.

```
blockMesh
surfaceFeatureExtract
snappyHexMesh.exe -overwrite
extrudeMesh.exe
```

## CFD Solver

simpleFOAM with RANS K-epsilon turbelence model

## Boundary conditions

atmBoundaryLayerInletVelocity at inlet

## References
Code based on A tutorial to urban wind flow using OpenFOAM by H˚akan Nilsson
[link to report](http://www.tfd.chalmers.se/~hani/kurser/OS_CFD_2017/DavidSegersson/report_David_Segersson.pdf)


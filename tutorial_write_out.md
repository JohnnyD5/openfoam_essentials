# 1. copy tutorials and run cavity
```
cp -r /opt/openfoam6/OpenFOAM-6/tutorials/incompressible/icoFoam/cavity /work/zhizhong/
```
```
cd /work/zhizhong/cavity/cavity
```
Generate mesh:
```
blockMesh
```
Run simulation:
```
icoFoam
```
Quickly clean all generated files:
```
rm - r *.*
```
Quickly clean all processor data:
```
rm -r proc*
```

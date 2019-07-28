# 1. Copy tutorials and run cavity
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
# 2. Useful tutorials on recompile openfoam
Change an existing solver to a new solver by changing the name:  
<https://www.youtube.com/watch?v=MiUDCOhbQaM>

Adding Passive Scalar Transport Equation to icoFoam  
<https://www.youtube.com/watch?v=L94iYGvZr9Q>

Go to openFoam folder 
```
cd /opt/openfoam6/OpenFOAM-6
```
go to applications:
```
cd applications
```
```
mkdir OFM11-training
```
Copy the icoFoam solver to OFM11-training
cp -r /opt/openfoam6/OpenFOAM-6/applications/solvers/incompressible/icoFoam

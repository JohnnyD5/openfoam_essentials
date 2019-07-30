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
# 2. Basic commands
Quickly clean all generated files:
```
rm - r *.*
```
Quickly clean all processor data:
```
rm -r proc*
```
Go to user application bin:
```cd $FOAM_USER_APPBIN```
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
```
cp -r /opt/openfoam6/OpenFOAM-6/applications/solvers/incompressible/icoFoam
```
Change the name to passiveScalarIcoFoam
```
mv icoFoam/ passiveScalarIcoFoam
```
Go to the passiveScalarIcoFoam folder
```
cd passiveScalarIcoFoam
```
Make changes to the make file
``` 
cd Make
```
``` 
vim files
```
1. change `icoFoam.C` to `passiveScalarIcoFoam.C`  
2. change `EXE = $(FOAM_APPBIN)/icoFoam` to `EXE = $(FOAM_USER_APPBIN)/passiveScalarIcoFoam`
```
cd ..
```
change `icoFoam.C` to `passiveScalarIcoFoam.C`  
```
mv icoFoam.C passiveScalarIcoFoam.C 
```


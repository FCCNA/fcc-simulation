# fcc-simulation

This repository is related to the simulation of the crystal. I started with the example B4c and I modified it to fit the necessities of FCC and BelleII.

## How to run it?

You should create your build directory and run 

```cmake -DGeant4_DIR=/path/to/geant4_installation /path/to/this_repository/Simulazione_Gaudino/B4c/```

after this you can run 

```make```

and finally 

```./exampleB4c```

If you want to change the XY dimension of the crystal you can change [here](https://github.com/FCCNA/fcc-simulation/blob/f7ff68a73854078eeef8a6a15fc049f2abc22fd8/crystal_simulation/B4c/src/DetectorConstruction.cc#L131)

If you want to change the length of the crystal you can change [here](https://github.com/FCCNA/fcc-simulation/blob/f7ff68a73854078eeef8a6a15fc049f2abc22fd8/crystal_simulation/B4c/src/DetectorConstruction.cc#L134)

The default material is CsI. By now you can run on Idle the command `/B4c/det/setMaterial BGO` to change to BGO. In [Issue 2](https://github.com/FCCNA/fcc-simulation/issues/2) we aim to add many materials to the list

Most of the material has been done with the help of Ilaria Rosa.

**DO NOT ADD THE BUILD DIRECTORY IN THE REPOSITORY**

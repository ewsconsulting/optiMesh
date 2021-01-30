# optiMesh

OpenFOAM mesh smoothing. Place the settings for optiMesh in a system/optiMeshDict file.

See the tutorials/omesh case for an example.

# Installation

run the Allwmake script

Installs everything to your $FOAM_USER_LIBBIN and $FOAM_USER_APPBIN directories.

Only tested with OpenFOAM-v2012

# Other tools included

* removeCells
* collapseCells
* moveLastToConstant

# Alternatives to laplacian smoothing
An objective optimizer is included in optiMesh (eg. optimizing the orthogonality), but I haven't yet seen it produce better results than laplacian smoothing (and it's much slower). 

# TODO
A better approach is probably to do implicit laplacian smoothing (which should be much fast than explicit laplacian smoothing in case of fine meshes).

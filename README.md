Some useful script and command lines for openFOAM v2XXX version

mapFields - contains command lines to map the flow field from prescribed directory
sampleDictPlane2 - sample script to sample boundary data; use by command: 'postProcess -func sampleDictPlane2'
forceelement - since for openFOAM v2XXX version, it is difficult to write a user-define postprocessing code, therefore, it is recommended to write a code and use in controlDict to postprocess the field. Here is an example. By using it, first incude the dict in controlDict by ' #include "forces" ' inside functions and then use 'icoFoam (or other solver name) -postProcess' to excute the postprocess code.

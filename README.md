gpbexporter
===========

Gameplay3d engine model exporter for Blender

this repo is a fork from the original work of forestmedina. 

this script is intended to be used directly from the python window, not as plugin. 
the reason for this is that it is in active development and is easier for me to debug and edit in the python window rather than reloading the plugin each time.

latest version main features (differences from forestmedina project):

- support export of binormal and tangent data. to enable this functionaly, please add in the mesh properties a custom attribute named "gpb_export_tangent" with a value of 1. 

- support for shared mesh data: prior versions duplicate mesh data when two objects shared a mesh block. this version keep a dictionary of meshes to avoid duplication issues, producing smaller gpb. 

- no export objects that are not in visible layers (useful to avoid helper objects to be exported in the gpb) 

how to run this file?

load gpb3_direct.py in your blender python window. 

go to the end of the file and change the default export path. 

press run!



item_description
================

This ROS package provides 3D models of common parts such as profiles for simulation and visualization purposes.
The word 'item' in the package name is meant to be ambiguous, referring to both the company popular for their profiles, item Industrietechnik GmbH, and parts in general.

Please note that most models are derived from technical specifications, technical drawings, or CAD files made available by the respective companies and their (re-)sellers.
As a result, all rights of the models belong to their respective owners.
This package is not supported by or affiliated with item Industrietechnik GmbH or other companies providing such parts in any way.


Adding Models
=============

Currently, only a few common parts are available. If something you need is missing from this package, please consider contributing.
This section gives you some pointers on how to add models using Blender and FreeCAD.

Note that in Blender, pressing the space bar opens a search that helps you locating functions and settings.


From a Cross Section
--------------------

Assuming you are not too familiar with modelling software, you can follow these steps:

1. Acquire a STEP file of the cross section model.
2. Import the STEP file into FreeCAD from within *Workbench → Mesh Design*.
3. Export the model as a Collada file (.dae).
4. Import the Collada file into Blender.
5. Adjust the *Transform → Dimensions* in *View3D: Properties* so that variable components have a dimension of 1 (assume the unit to be meters).
6. Use *Transform: Rotate* so that the X axis corresponds to length, Y to width, and Z to height (for profiles, length is the variable component).
7. Ensure that the origin is in the center (should usually already be the case).
8. Export the model as a Collada file (.dae) again.

Now, you can follow the example of existing parts to create corresponding macros and properties.
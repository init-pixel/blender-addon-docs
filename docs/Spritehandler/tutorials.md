# NO LONGER APPLICABLE


### Tutorial: Sprite Planes

1. Add Menu (SHIFT+ A) > Mesh > Create New Sprite Plane
2. Select Spritesheet file and choose a host type/Preset:
    * Animated : Index driven by current frame
    * Static : Index driven by random number
    * Particle Animated : Index driven by particle age
    * Particle Static : Index driven by particle index
3. Setup sheet by either:
    * Running operator: Object > Setup Spritesheet
    * Manually set the group node parameters and run operator: Object > Scale From Sprite Node


### Tutorial: Sprite Packing

Sprite packing is performed through the Spritesheet Generator Toolshelf in the UV/Image Editor

* Generate Spritesheet prompts to user to select sprites for packing and then generates an new sheet from them based on the 'X Cell Count'
* Regenerate Spritesheet last images used in Generate Spritesheet and repacks based on the 'X Cell Count'
* Enabling Sheet from Render will generate a spritesheet from animation renders. These sheets can also be used with Regenerate Spritesheet


### Tutorial: Atlas to Mesh

1. Add Menu (SHIFT+ A) > Particle Atlas to Mesh Group
2. Set creation parameters using the operator properties(Bottom left corner of 3d view)
    * Sheet Path : Atlas for conversion
    * Cells : Set atlas cell values
    * Subdivision : Controls the accuracy of the conversion
    * Dilate Alpha : Grows the alpha of each cell
    * Un-Subdivide : Enable/Disable mesh optimization
    * Decimate Factor : Number of optimization steps
    * Triangulate : Triangulate final meshes
    * Group : Create a new group and add mesh to it
    * Individual Group : Create, and apply, a unique group for each mesh
    * Island Clean : Remove small mesh islands based on their area.
    * Surface Type : Shader type to use for the new objects' material
3. Experiment with subdivision and alpha dilate values to get a feel for how they affect the mesh generation. Higher subdivision values are very computationally expensive and you should focus on alpha dilation to recover clipped details. Disable Un-Subdivide to better see generation process. Alpha dilation is likely to generate small floating islands that can be cleaned with the Island Clean parameter set to a low value.


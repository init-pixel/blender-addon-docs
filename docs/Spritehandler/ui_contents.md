# Interface Panel Contents
## Image Editor Panel

![Image Editor Panel](images/IMAGE_EDITOR_panel_screenshot.png)

| Create | Spritesheet Creation |
| - | - |
| Spritesheet from Files | Open's a file browser to select files to create a spritesheet from |
| Sheet from Render | When enabled, a spritesheet will automatically be create after rendering frame sequence |


| Edit | Spritesheet Editing |
| - | - |
| X Cells | How many horizontal cells to use |
| Padding X/Y | Per axis pixel padding for each cell |
| Origin X/Y | Normalized per axis origin adjustment of individual cells |
| Multiply Alpha | Wether to multiple color channels by Alpha |
| Use Resize | If enabled, the active image will be resized after creation/edit |
| Apply Edit | Regenerate active spritesheet image with the current values |


| Resize Image | Filtered Image Resizing |
| - | - |
| Scale | Factor by which to scale the image |
| Filter | Pixel filter to use. For pixel art, use Nearest. |
| Resize in Place | Toggle destructive resizing of image. Otherwise a copy is made |

## View 3D Panel

![View 3D Panel](images/VIEW_3D_panel_screenshot.png)
| Create Sheet Player | Create Geometry for using Spritesheets | 
| - | - |
| Image Selector | Select the spritesheet to use on the new sequencer mesh |
| New Sequencer | Create a plane and assign a new material with the player node group and chosen image |
| Edit Sequencer | Edit a previously created sequencer mesh |

| Geometry from Alpha | Create Geometry from Spritesheet Alphas |
| - | - |
| Image Selector | Select the image to use for creating the new geometry |
| Mesh from Alpha | Generate geometry from the alpha channel of the selected image |
| Mesh from Alpha | Edit/Regenerate geometry from image alpha |

| Helpers | Convenience Functions |
| --- | --- |
| Delete Small Islands | A cleanup tool to delete small polygon islands based on their area. |
| Origin to Bounding Box | Set the origins for all selected geometry to a chosen bounding box point, or point average. |

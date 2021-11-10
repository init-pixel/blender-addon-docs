# Node Switcher Blender Addon
## Overview
Blender addon for generating node networks to switch and/or blend between various
datatypes.

Currently supports all shader socket types used by Cycles/Eevee with plans to support other render engines in future.

## Updates
Oct 12th, 2021 | 0.2 | ID Key with Auto detect  
Sept 8th, 2021 | 0.1 | First Release  

## Switch Types
* ID/RGB Switcher. Switching based on the colors of an input with auto detection for image input.  
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZFIZPFnB7xc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

* Hard Switcher. Hard value based switching for arbitrary uniform socket types. 
![Hard Switching](gifs/hard_switching.gif)
* Soft Switcher. Blended value based switching for arbitrary uniform socket types
![Blended Switching](gifs/blended_frames.gif)
* Weighted average switch. Create a node network that calculates a weighted overage of the inputs. Not compatible with shader socket types.
![Weighted Average Switching](gifs/weighted_average_blending.gif)

## Parameters
* ID Key from Selected  
![New ID Keyer](images/new_id_switch.png)  
* ID Switch node  
![ID Switch Node](images/id_switch_node.png){: style="height:150px;width:150px"}  
* New Switcher From Selected  
![New Switch From Selected](images/new_switch.png){: style="height:150px;width:150px"}  

## New Node Groups
* Value Lerp
Linear interpolation of a value.
* Vector Lerp
Linear interpolation of a vector.
* Switch Node
Primary addon function, the different switch nodes,
* RGB Key
Color keyer node. Create a mask of the ID Map input using the Key color.
* ID Switcher
Color based switching and mask generation based on the colors of an input.

## Usage
### Tutorial: Create Switcher for ID Map
Select and image node containing the id map to be switched. Open the context menu (default: Right Click) and select "ID Switcher for Selected".

### Tutorial: Adding a Switcher For Selected
![New Switcher For Selected](gifs/switcher_from_selected.gif)
After selecting the nodes whose sockets you want to switch. Right click in an empty space and select "New Switcher For Selected Nodes". An operator will pop-up on which you can select the socket type to use for switching and a switching mode. See addon overview full descriptions of node switches.

### Tutorial: Adding a New Switcher
![New Switcher](gifs/new_switcher.gif)
The switcher node is available under the add nodes menu. Selection will trigger a pop-up on which you can can select the number of input sockets and the type of switch to create.

### Tutorial: Adding Bonus Nodes
All new nodes can be found in the add nodes menu under 'Converter'

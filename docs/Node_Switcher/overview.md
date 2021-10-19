# Node Switcher Blender Addon
## Overview
Blender addon for generating node networks to switch and/or blend between various
datatypes.

Currently supports all shader socket types used by Cycles/Eevee with plans to support other render engines in future.

## Updates
Oct 12, 2021 | 0.2 | ID Key with Auto detect
Sept 8, 2021 | 0.1 | First Release

## Switch Types

.. raw:: html
    <!-- <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://www.youtube.com/embed/ZFIZPFnB7xc" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div> -->
    <iframe width="560" height="315" src="https://www.youtube.com/embed/ZFIZPFnB7xc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

* ID/RGB Switcher. Switching based on


* Hard Switcher. Hard swithing for arbitrary uniform socket types. 
![Hard Switching](gifs/hard_switching.gif)
* Soft Switcher. Blended switching for arbitrary uniform socket types
![Blended Switching](gifs/blended_frames.gif)
* Weighted average switch. Create a node network that calculates a weighted overage of the inputs. Not compatible with shader socket types (Diffuse, Principled, etc).
![Weighted Average Switching](gifs/weighted_average_blending.gif)

## Usage
### Tutorial: Adding a Switcher For Selected
![New Switcher For Selected](gifs/switcher_from_selected.gif)
After selecting the nodes whose sockets you want to switch. Right click in an empty space and select "New Switcher For Selected Nodes". An operator will pop-up on which you can select the socket type to use for switching and a switching mode. See addon overview full descriptions of node switches.

### Tutorial: Adding a New Switcher
![New Switcher](gifs/new_switcher.gif)
The switcher node is available under the add nodes menu. Selection will trigger a pop-up on which you can can select the number of input sockets and the type of switch to create.

### Tutorial: Adding Bonus Nodes
The bonus nodes appear in the add node menus in the following locations:
Vector Lerp:
Value Lerp:

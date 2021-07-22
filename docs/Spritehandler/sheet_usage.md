# Spritesheet Usage
There are two general methods for Spritehandler to make use of spritesheets.
Spritesheets (and Atlases) are expected to be uniform, thought the meshing tool will work on any image with an alpha.

For static use (without the Frame node) it shouls
## 1. The Sequencer Node Group
> :warning: **The sequencer node is unreliable in Eevee**: Due to either an Eevee bug or an engine limitation,
the node group index will occasionally show the wrong frame. This appears mostly when using the node with the
addons time node. I hope that in time Eevee will work reliably, but it's out of my control for now.

TODO: Add video guide

Transcription:
There are many ways the sequencer node group can be used, but the most basic form is through the add sequencer object option.
For more complex uses, please refer to the demo files.
Start by selecting a spritesheet to be used for sequencing.
Using the add sequencer operator, found in the add menu, we're able to quickly setup the sheet inside a new material on a mesh that respects its aspect ratio.
There are a few presets that'll setup the sequencer node group for different uses.
Object that have been creating with the new sequencer button can also be editing.
TODO: Detail uses

## 2. Meshing Based on Alpha

TODO: Add video guide

Transcription:
Spritehandler can be used to generate mesh object based on the alpha channel of image.
By specifying the cell counts, the operator can output individual objects in a new collection.
The primary purpose of meshing images is for instancing, wether with Geometry Nodes, Particles, or Dupliverts/Duplifaces.
By creating a rough representation of the geometry, rather that using a simple plane with alpha, fewer transparency paths are required in rendering and render times are drastically reduced.

A full explanation of each menu item can be found in the [UI Content](ui_contents.md) page of the documentation.

# CSG Export & Node Converter - Godot
Tool Plugin for Godot Engine
=================================
Convert or Export CSG Meshes with 1 click 

How to use:
- Combine all your CSGMeshes under a CSGCombiner node then: 
- a) Press (Convert CSG to Mesh) to convert to a MeshInstance node
- b) Press (Export CSG to OBJ) in the Spatial Container Menu to save as a Wavefront OBJ file

Converting the CSGCombiner node to a MeshInstance will add a Trimesh Static Body if the CSG node has Use Collision enabled. If it has been converted before and a node exists, it will be replaced while conserving the Physics Material Override in the Static Body

Currently (Godot 3.4.3) CSG nodes do not support Physics Materials, this addon helps work with CSG nodes by converting the CSG geometry to a MeshInstance node that may override the physics properties


Original script: https://github.com/mohammedzero43/CSGExport-Godot

Limitations:
- Only works when you select 1 CSGCombiner node (Cant multiselect)

- Only material diffuse and emission colors will be exported (Textures and maps wont be exported, but you can add them manually in your 3D editing software) 

- The plugin is still experimental ,so please report for bugs at: mohammedzero43@gmail.com



![CSG Converter](https://user-images.githubusercontent.com/2546522/158038471-d6c34ff2-c104-4a65-a7e4-18eecfa56ad8.gif)



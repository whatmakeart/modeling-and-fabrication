---
title: "08.05 Export STL Blender"
date: 2020-01-26T23:11:13Z
draft: false
---

Blender's default unit scale is 1:1 meter. The default cube in a new Blender file is 2 units large, so it is a 2 x 2 x 2 meter cube. Scale is important for 3D prints. You can either model in meters, then scale the object to the correct size before export, or you can change the unit scale in Blender and work in millimeters. Sometimes it is easier to work larger and scale down but you may prefer to work at the exact size of the final object.

Exporting an STL from Blender is straightforward. Make sure you combine any objects made of multiple meshes with a boolean modifier set to exact. This way the part will be a solid, instead of being made up of different overlapping meshes.

## Turn of Smooth Preview

Smooth preview can trick you in to thinking that you have a smoother model than the actual geometry. Smooth shading is great for rendering and digital output but is not helpful for physical output like 3D printing. Make sure your model is in flat shading mode by right clicking on it in Object Mode and selecting "shade flat." If your model looks to angular or blocky, then add a subdivision modifier to your mesh and subdivide it as many times as needed to get a surface that is smooth enough. Unlike solid modeling programs, such as Fusion 360, the resolution of the subdivisions of the mesh determines the smoothness and fidelity of the exported geometry and 3D print. This is similar to pixel resolution in a jpg vs a vector file.

[![1 vs 6 subdivisions in Blender](2023-blender-1-6-subdivisions.jpg)](2023-blender-1-6-subdivisions.png)

Go to File > Export > STL ...

[![File Export STL Blender](2023-blender-file-export-stl.png)](2023-blender-file-export-stl.png)

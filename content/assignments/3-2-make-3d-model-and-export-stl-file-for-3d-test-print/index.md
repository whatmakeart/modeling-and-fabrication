---
title: "3.2 Make 3D Model and Export STL File for 3D Test Print"
date: 2020-01-26T23:11:13Z
draft: false
---

We will not only 3D model on our computers, we will output our digital models into the physical world. We will use different processes to make physical models but the first technique will be 3D printing. 3D printing is a quick way to be able to hold a complex 3D model in your hands. Some models can only be made by 3D printing. 3D printing is an additive process, meaning material is added to existing material rather than being cut away such as with a saw.

The test prints will be small and must fit within a 50mm x 50mm x 50mm box. (50mm is approximately 2 inches) You can see the size of your model in Fusion under properties from the browser.

## Ideation Sketches

Using thumbnail sketches, quickly design numerous ideas for a 3D test print. For now think about a small size object of about 1 cubic inch. This can be bigger than an inch in size but the total volume of the object should be less than 1 cubic inch. Think about organic forms, negative spaces, curvilinear lines and geometric surfaces.

When you finish your sketches scan them and upload them to the class Google Drive following the instructions below.

### Required Sketches

- 10 thumbnail sketches minimum - These should be 10 different ideas. Draw without constraint. Do not limit your ideas.
- 5 larger refined ideations minimum<- Choose some of your ideas from your thumbnails. Refine them and iterate on the concepts. Which parts do you like and which parts can you change to make your ideas better.
- 1 larger refined drawing - Pick one of the 5 developed sketches and continue to refine it and change it. Draw it larger in perspective. You can add shading and details to help communicate your vision.

## Model your design in Fusion 360

### General 3D Print Rules for FFD Printing without Dissolvable Supports

- Keep thin and small parts multiples of the nozzle size. The nozzle at the think[box] is .4mm absolute minimum size of fine objects is 1.2mm. A better size for thin walls and supports is 1.6mm. 1.5mm or 1.7 mm are not good. 2.0mm or 2.4mm are even better.
- Keep overhanging parts extending out less than 45 degrees. This allows layers to overlap a bit and slowly extend out wider. 45 degrees is the max otherwise the printer tries to print in mid air and all the filament falls to the ground.
- Objects must be fully connected and "manifold" or "watertight" You can't have pieces floating in the air or close but not touching. Don't have small voids. Make the pieces solid and uniform. You can have a hollow vase or container but all its parts and walls should be connected and solid.

<div class="gallery-grid-jimmy" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 10px;">

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_angles.png?target=e554cbfb-83ef-45dd-8ac4-8d5459e476f8)

<span class="caption-jimmy" style="font-size: 14px;">Red models will not print without supports but green models will because they rise up at 45 degrees</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_angles_square.png?target=d6a4e04e-93cc-4268-8e89-6c4ac16906e2)

<span class="caption-jimmy" style="font-size: 14px;">Red models will not print without supports but green models will because they rise up at 45 degrees</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_angles_round.png?target=d907914a-f85c-446f-bd19-d2392d5525d5)

<span class="caption-jimmy" style="font-size: 14px;">Red models will not print without supports but green models will because they rise up at 45 degrees</span>

</div>

</div>

### General Structural 3D Printing Guidelines

The following guidelines help achieve successful 3d Prints especially when designing containers, structural parts and pieces that need to be the correct size to match real world objects. These concepts still hold true for more organic creative work but may not be as necessary.

<div class="gallery-grid-jimmy" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 10px;">

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_guidlines.png?target=ef54c04a-dbda-4750-98c1-3eaae11e0dcf)

<span class="caption-jimmy" style="font-size: 14px;">Example of model showing Mechanical 3D Print Guidelines</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_gussets.png?target=0dfb2032-82aa-4932-a8c7-649650e10c42)

<span class="caption-jimmy" style="font-size: 14px;">Gussets or supporting pieces like wings give more structure to elements.</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_uniform_wall_thickness.png?target=8d831c8f-ce79-4ea7-89bc-e67f033b6ad8)

<span class="caption-jimmy" style="font-size: 14px;">Uniform Walls help with deformation and warping.</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_fillets.png?target=caa631d1-faea-4852-adb3-5e044e000b9a)

<span class="caption-jimmy" style="font-size: 14px;">Fillets or rounded interior corners add strength and help with warping. Ribs also shown, connect vertical pieces to other vertical pieces or walls.</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_ribs.png?target=9b70aaf9-21a5-4561-9a1c-33500ab14291)

<span class="caption-jimmy" style="font-size: 14px;">Chamfers or angled interior corners add strength and help with warping like fillets do.</span>

</div>

<div class="image-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">![](/ICS/icsfs/mm/2022_3d_print_round_corners.png?target=e0e6bae5-5375-4f61-93ac-66e12de4ec01)

<span class="caption-jimmy" style="font-size: 14px;">Rounded Corners put less stress on the corners and are smoother to print.</span>

</div>

</div>

### 3D Printing Terms

These are some common words and terminology used in 3D Printing

- Vertex - the base unit of a polygon model. It is a point in space defined by an x, y and z coordinate. Can be moved around and "welded" to other vertexes or connected to another vertex with an edge.
- Edge - the line connecting two vertexes in a polygon model. Edges make closed shaped that are called faces
- Face - the enclosed shape made by connected vertexes and edges. Can be a triangle, a quad (four-sides) or an N-Gon
- Triangle - simplest planar shape. STLs are made of triangle but triangles should be avoided if possible when modeling since they cannot be subdivided easily and do not make smooth forms.
- Quad - A four sided polygon. This is generally the best shape to make your model from.
- N-Gon - A polygon with (n) sides. These should be avoided. With T-Splines you may have some n-gons but it is best to make them into quads if you can.
- Mesh - The structure of a 3D model. It is made of of points (vertexes), edges and polygon faces.
- Bounding Box - the smallest box that your model can fit in. IT is a rectangular prism defined by a height, width and length.
- Raft - bottom support for a 3D print to help it adhere to the print bed when the print starts and to keep the print from falling over when the print gets taller.
- Infill - Support material in the middle of a 3D print. Can be made of different patterns and is usually not solid. Sometimes described in percentage terms, less infill will make a faster print and use less material while a higher percentage infill will take longer to print and use more material.
- Support Material - extra printed material used to support parts of the print that overhang more than 45 degrees in the horizontal direction. Sometime a model can be orientated on the printer at a different angle to avoid support material. Can be removed but often messes up the surface where it attached to the print.
- Parametric - A 3D model driven by defined dimensions and parameters
- Solid - A 3D model that is not a plane or open shape. It is a full solid object.
- Polygon - A 3 or more sided shape. The surfaces of 3D models are made of polygons
- STL (STereoLithography) - the most common file format used for 3D printing. It is made of a fine triangle mesh. This file format works for 3D printing but is not good for modeling. Always save the original model file so you can make changes. It is possible to edit an STL file but it is much easier to edit the original 3D model.
- Print in Place (PIP) - Method of printing moving parts such as hinges and joints in a 3D print in one operation. This produces forms that would not be possible with traditional manufacturing techniques.
- Fused Filament Fabrication (FFF) - Most common method of affordable 3D printing. This method uses a thermoplastic filament, or wire, on a spool that is fed through a nozzle. Heat melts the thermoplastic and new layers are fused to previous layers in order to make the print.

## Check the Bounding Box Size

Make sure your file is set to millimeters Check the properties of the component that you want to export to know the bounding box size.

The total bounding box should be less than 50mm in all directions.

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap;">

<div class="half-box" style="flex: 1 1 400px;">![](/ICS/icsfs/mm/2022_fusion_properties_browser.png?target=a646549e-38ba-4415-a854-1422508f972d)</div>

<div class="half-box" style="flex: 1 1 400px;">

Click on properties of the body or component in the browser. Right click on the component that you want to print. Then select properties.

</div>

</div>

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap;">

<div class="half-box" style="flex: 1 1 400px;">![](/ICS/icsfs/mm/2022_fusion_bounding_box.png?target=d1a9a8a7-bc16-40eb-9d18-e7e969be2cd1)</div>

<div class="half-box" style="flex: 1 1 400px;">

Then you can see the bounding box dimensions. These should be below 50mm in all directions of x y and z.

</div>

</div>

## Export STL file for 3D Test Print Watch the video on the tutorial page to export your model as an STL file. Choose File > 3D Print to save your STL Label the file YYYYMMDD Lastname Firstname 3D Test Print.stl ## Export .f3d file of Model from Fusion 360 Choose File > Export ... and save a .f3d version of your object. ## Apply materials and Export a Render Image The 3D print will be a solid color of PLA plastic. Choose a color and apply that material to your model. Set up a render scene with a 1:1 or 16:9 or 2:3 aspect ratio. Make one of the dimensions a minimum of 4000px. Export a render image with a good composition. Don't make the object too small in the image.

## Upload to Google Drive

Upload the following items to Google Drive:

- scans of your ideation sketches
- STL file of model
- .f3d file of model
- render image

---
title: "4.2 Model Laser Cut Project in Fusion 360"
date: 2020-01-26T23:11:13Z
draft: false
---

# Assignment Deliverables

1.  Fusion 360 .f3d file
2.  Rendering(s) of project with appearances applied (.png or .jpg)
3.  Illustrator .ai file of the cut paths (cut with red stroke .001 weight and engraving with blue stroke .5 weight)

<div class="flex-container-jimmy">

<div class="half-box">

Using your sketches, cardboard model, and third angle projections, make a model of your laser cut stand in Fusion 360\. Each piece of the project should be a separate component. This is necessary to be able to [lay the parts out flat](https://youtu.be/jeQPJHHwVN4) in Fusion 360 to produce and [export a DXF cut file](https://youtu.be/6JFHMV7A9TU) for use on the laser cutter. You will need to make a laser cutter tool in Fusion 360 and install a DXF post processor to produce a DXF file of your tool paths. There are video instructions below showing [how to make a laser cutter tool](https://youtu.be/-B6DXF9aE5s) and [how to install the DXF post processor](https://youtu.be/CBu6vl6Bqos).

You are required to use at least one user parameter dimension for "ply" or the thickness of the material you are cutting. Materials vary in width, so we will [measure the material before cutting](https://youtu.be/a7HOiBC_81s) on the laser cutter. When we know the real thickness of the material [using digital calipers](https://youtu.be/oOZjbbe6YZk), then we can change the "ply" variable and the model will produce an accurate cut file.

</div>

<div class="half-box">

![Laser Cut Stand Assembled](2021-Laser-Cut-Stand_Assembled.jpg)

<span class="caption-jimmy">Physical Prototype of Laser Cut Cell Phone Stand cut at think[box]</span>

</div>

</div>

# Process

## 1. Model Stand in Fusion 360

If you prefer, you can import your third angle projection sketches to use as guides you start your first sketch. You need to calibrate the size of the sketch to be the correct scale in your Fusion 360 file. Then you can use the sketch as a guide to create your digital sketch. This step is not necessary but some may like it. This video shows [how to import an image as a canvas](https://youtu.be/-3SMfrnWMTE) in Fusion 360.

If you are making detailed organic forms or drawing an image to use as the contours of the sides or other parts of your stand it can be difficult to draw complex shapes and images in Fusion. You can draw you image or character in Illustrator and export it as an SVG or DXF. Then you can import that file into Fusion 360\. Once in fusion the file acts as a sketch and you can extrude it right away to be a piece of your model. This workflow is better than drawing a complex organic form in Fusion.

Remember to make a new component at the top level of you model for each part. The top level should be the "parent" of each of the other components. The components should be at the same outline level in the browser and not nested inside each other.

Think about how your pieces will hold together.

- Will you use captive nut joints?
- Will you use pinned finger joints?
- Will you use tabs and holes?
- Will you have bendable living hinges?
- Will you use snap clips?

Remember to add tabs and holes and any other design features needed to attach the different pieces. You can use the "Combine" modify action to cut out pieces using other pieces as "tools".

---

---

---

---

## 5\. Create Toolpaths in the Manufacture Workspace

<div class="flex-container-jimmy">

<div class="half-box">

Follow the steps in this tutorial video to create a new setup in Fusion 360\. This is done in the Manufacture Workspace. You need to create the laser cutter tool first. It is important to create a new "Cutting" setup so you can make a new 2D Profile to cut out.

</div>

<div class="half-box">

![Laser Cut Stand Toolpaths](2021-Laser-Cut-Stand-CAM-Toolpaths.png

<span class="caption-jimmy">View of tool path layout in the Manufacture Workspace</span>

</div>

</div>

---

---

## 7. Add appearances and Export Render

<div class="flex-container-jimmy">

<div class="half-box">

In Fusion 360 add appearances to you model as you wish and export a render. Label the file YYYYMMDD Lastname Firstname Laser Cut Stand Render.png/jpg

Make the model look the way you want the final product to look. If you are going to paint pieces then paint the pieces in the render. If you will have etchings then put an image decal on to represent the etchings.

Make sure your render is well composed and high resolution with at least one direction 4000px. Choose a 4:3 16:9 or 1:1 aspect ratio. You can make multiple render views.

</div>

<div class="half-box">

![Laser Cut Stand Assembled](2021-Laser-Cut-Stand-Assembeled.jpg)

_<span class="caption-jimmy">Example of each part of the stand as a separate component at the top level assembly in Fusion 360.</span>_

</div>

</div>

--

<div class="video-card">

## Import SVG or DXF File from Illustrator into Fusion 360

<div class="iframe-16-9-container"><iframe class="youTubeIframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/aMBnke14Wgg?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-card">

<div class="video-card">

## Make a Manufacture Model Copy of Your Design

<div class="iframe-16-9-container"><iframe class="youTubeIframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/bhVPR4CUOUk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

</div>
# Grading Rubric

| Assessement                 | Weight    |
| --------------------------- | --------- |
| Model Quality               | 50 points |
| Render Image                | 20 points |
| Manufacture Workspace Setup | 10 points |
| Tool Path Export            | 10 points |
| File Management             | 10 points |

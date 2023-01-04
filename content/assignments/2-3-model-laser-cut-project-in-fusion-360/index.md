---
title: "2.3 Model Laser Cut Project in Fusion 360"
date: 2020-01-26T23:11:13Z
draft: false
---

<div class="flex-container-jimmy">
<div class="half-box">
<p>Using your sketches, cardboard model, and third angle projections, make a model of your laser cut stand in Fusion 360. Each piece of the project should be a separate component. This is necessary to be able to <a href="https://youtu.be/jeQPJHHwVN4">lay the parts out flat</a> in Fusion 360 to produce and <a href="https://youtu.be/6JFHMV7A9TU">export a DXF cut file</a> for use on the laser cutter. You will need to make a laser cutter tool in Fusion 360 and install a DXF post processor to produce a DXF file of your tool paths. There are video instructions below showing <a href="https://youtu.be/-B6DXF9aE5s">how to make a laser cutter tool</a> and <a href="https://youtu.be/CBu6vl6Bqos">how to install the DXF post processor</a>.</p>
<p>This project introduces custom <a href="https://youtu.be/H6W-Og4YyZ8">user parameters in Fusion 360</a>. These are like variables for dimensions that we can change and have the model update automatically. You are required to use at least one user dimension for "ply" or the thickness of the material you are cutting. Materials vary in width, so we will <a href="https://youtu.be/a7HOiBC_81s">measure the material before cutting</a> on the laser cutter. When we know the real thickness of the material <a href="https://youtu.be/oOZjbbe6YZk">using digital calipers</a>, then we can change the "ply" variable and the model will produce an accurate cut file.</p>
</div>
<div class="half-box"><a href="/ICS/icsfs/mm/2021_laser_cut_stand_assembeled.jpg?target=35a0bb77-1255-44ec-984b-951fe59cf0cd"><img src="/ICS/icsfs/mm/2021_laser_cut_stand_assembeled.jpg?target=35a0bb77-1255-44ec-984b-951fe59cf0cd" alt="" width="100%" height="auto" /></a>
<p><em><span class="caption-jimmy">Physical Prototype of Laser Cut Cell Phone Stand cut at think[box]</span></em></p>
</div>
</div>
<h1>Process</h1>
<h2>1. Model Stand in Fusion 360</h2>
<p>If you prefer, you can import your third angle projection sketches to use as guides you start your first sketch. You need to calibrate the size of the sketch to be the correct scale in your Fusion 360 file. Then you can use the sketch as a guide to create your digital sketch. This step is not necessary but some may like it. This video shows <a href="https://youtu.be/-3SMfrnWMTE">how to import an image as a canvas</a> in Fusion 360.</p>
<p>If you are making detailed organic forms or drawing an image to use as the contours of the sides or other parts of your stand it can be difficult to draw complex shapes and images in Fusion. You can draw you image or character in Illustrator and export it as an SVG or DXF. Then you can import that file into Fusion 360. Once in fusion the file acts as a sketch and you can extrude it right away to be a piece of your model. This workflow is better than drawing a complex organic form in Fusion.</p>
<p>Remember to make a new component at the top level of you model for each part. The top level should be the "parent" of each of the other components. The components should be at the same outline level in the browser and not nested inside each other.</p>
<p>Think about how your pieces will hold together.</p>
<ul>
<li>Will you use captive nut joints?</li>
<li>Will you use pinned finger joints?</li>
<li>Will you use tabs and holes?</li>
<li>Will you have bendable living hinges?</li>
<li>Will you use snap clips?</li>
</ul>
<p>Remember to add tabs and holes and any other design features needed to attach the different pieces. You can use the "Combine" modify action to cut out pieces using other pieces as "tools".</p>
<p>Types of Laser Cut Joints</p>
<p>There are many ways to join a laser cut project together ranging from gravity to glue to bolts to snap pieces. You can use a variety of ways to connect. Here are some example images of different methods of joining pieces together. There are many more ways. Search the internet for other methods of making laser cut joints.</p>
<div class="gallery-grid-jimmy">
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_finger_joints_laser_cut.png?target=c67e7170-3787-4891-a1be-b1d67b9ef76c" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Box with finger joints on all sides</p>
</div>
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_snap_joints_laser_cut_1.png?target=5b9cad82-7130-4e50-bf3a-3bcd90ae7932" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Snap joint pulled apart</p>
</div>
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_snap_joints_laser_cut_2.png?target=6dbb4191-1fe0-46d1-992e-eed2f5879dd0" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Snap joint pressed together</p>
</div>
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_captive_nut_joints_laser_cut.png?target=15440b0a-f014-4b24-9d0e-45ad786a6331" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Captive bolt / nut joints laid flat</p>
</div>
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_captive_nut_joints_laser_cut_2.png?target=271e9d84-1865-4f4f-954d-a139826c2d05" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Captive bolt / nut joint without aligning fingers</p>
</div>
<div class="imag-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_captive_nut_joints_with_fingers_laser_cut.png?target=bdf5e5eb-6629-478a-aaa1-530365e6a31d" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Captive bolt / nut joint with alignment tabs / fingers</p>
</div>
<div class="imaeg-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_pinned_finger_joints_laser_cut_colors.png?target=3c620664-0caf-4c08-9393-9f83f7a0faa7" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Pinned finger joint with different pieces colorized</p>
</div>
<div class="image-card-jimmy">
<div class="image-box-jimmy"><img class="fit-img-jimmy" src="/ICS/icsfs/mm/2022_pinned_finger_joints_laser_cut.png?target=9fd21b36-97de-4277-b7a1-fce7be9c1562" alt="" width="100%" height="auto" /></div>
<p class="caption-jimmy">Pinned finger joint</p>
</div>
</div>
<h2>Use User Parameters</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Use a user parameter of "ply" so you can update your design after measuring your material. Use this dimensions in your sketches as a guide rather than typing in the thickness of the plywood as a hard coded value. This allows for updating. You can also make parameters for the device width, the size of bolt holes and any other feature that you might want to change or have a relationship to other features.</p>
<p>You can also use a user parameter for the inner width to space out pieces. Use user parameters for anything that you want to reference or update later.</p>
</div>
<div class="half-box" style="display: flex; flex-direction: column;"><img src="/ICS/icsfs/mm/2021_laser_cut_user_parameters.png?target=5e8ff8e7-9c07-48e6-a77d-0850b5b5dc20" alt="" width="100%" height="auto" />
<p><em><span class="caption-jimmy">Example User Parameters in Fusion 360</span></em></p>
<img src="/ICS/icsfs/mm/2021_laser_cut_stand_components_and_parts.png?target=57ad1d89-963c-4d4a-bf3e-bafa6e3f4b3e" alt="" width="100%" height="auto" />
<p><em><span class="caption-jimmy">Example of each part of the stand as a separate component at the top level assembly in Fusion 360.</span></em></p>
</div>
</div>
<hr />
<h2>2. Layout a Manufacture Model Copy of All Pieces Flat for Cutting</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Once your model is complete and each piece is a separate and labeled component, you are ready to lay your pieces flat to create a DXF toolpath file for the laser cutter.</p>
<p>Change to the Manufacture Workspace.</p>
<p>Create a Manufacture Model in the Manufacture Workspace. This model is like a linked copy of your Design Model. It allows you to lay your pieces flat with out moving your Design Model. If you make changes to your Design Model after you lay your pieces flat then your Manufacture Model should update automatically. This video shows <a href="https://youtu.be/bhVPR4CUOUk">how to make a Manufacture Model</a>.</p>
<p>Draw a 12" x 12" sketch to represent your plywood. If you are using larger plywood or plexiglass then draw a larger sketch. If you are using a "remnant" or cutoff piece then draw your sketch to that size. Then use the Arrange command to lay your parts flat.</p>
<p>Follow the insturctions in <a href="https://youtu.be/jeQPJHHwVN4">the video</a> to arrange your parts flat. Note that the example model video uses the onle "joint" method to lay parts flat. You should use the <a href="https://youtu.be/jeQPJHHwVN4">updated method with the arrange command.</a></p>
</div>
<div class="half-box" style="display: flex; flex-wrap: wrap; flex-direction: column;">
<div style="display: flex; flex-wrap: wrap; align-items: flex-end;"><img src="/ICS/icsfs/mm/2021_laser_cut_stand_cam_layout_top.png?target=a8333f68-b5a2-4ac2-94e6-f5fcbc6fd349" alt="" width="3519" height="1600" />
<p><span class="caption-jimmy"><em>Top view of components of laser cut stand flat on plywood.</em></span></p>
</div>
<div class="half-box" style="width: 100%; max-height: auto; margin: 0 auto; display: flex; flex-wrap: wrap; flex-direction: column;">
<div style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe style="position: absolute; left: 0px; top: 0px; width: 100%; height: 100%; border: 0;" src="https://www.youtube.com/embed/jeQPJHHwVN4" width="300" height="150" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
<p><span class="caption-jimmy"><em>Top view of components of laser cut stand flat on plywood.</em></span></p>
</div>
</div>
</div>
<hr />
<h2>3. Install DXF Post Processor</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Follow the instructions in the video below to install the DXF Post Processor from Autodesk. This will allow you to export your laser cut tool paths from Fusion 360 as a DXF file that you can open and edit in Illustrator. This is the link to the <a href="https://cam.autodesk.com/hsmposts?p=dxf">DXF Post Processor from Autodesk</a>.</p>
<p>You can install it locally in Windows or Mac. <a href="https://knowledge.autodesk.com/support/fusion-360/learn-explore/caas/sfdcarticles/sfdcarticles/How-to-add-a-Post-Processor-to-your-Personal-Posts-in-Fusion-360.html">Local install instructions.</a></p>
<p>You can install it in the cloud as well, then you can use it anywhere. Make sure to enable cloud libraries first. <a href="https://knowledge.autodesk.com/support/fusion-360/learn-explore/caas/sfdcarticles/sfdcarticles/How-to-install-a-cloud-post-in-Fusion-360.html">Cloud install instructions.</a></p>
</div>
<div class="half-box" style="width: 100%; max-height: auto; margin: 0 auto;">
<div style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe style="position: absolute; left: 0px; top: 0px; width: 100%; height: 100%; border: 0;" src="https://www.youtube.com/embed/CBu6vl6Bqos" width="300" height="150" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<hr />
<h2>4. Create Laser Cut Tool in Fusion 360 with Specific Kerf</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Follow the instructions in the video below to create a laser cut tool in Fusion 360. Make sure you enter a kerf of .127 mm since that is the kerf of the laser cutters at the think[box]. If your pieces do not fit correctly you can then adjust this tool in Fusion 360 to correct the kerf for your desired fit.</p>
</div>
<div class="half-box" style="width: 100%; max-height: auto; margin: 0 auto;">
<div style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe style="position: absolute; left: 0px; top: 0px; width: 100%; height: 100%; border: 0;" src="https://www.youtube.com/embed/-B6DXF9aE5s" width="300" height="150" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<hr />
<h2>5. Create Toolpaths in the Manufacture Workspace</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Follow the steps in this tutorial video to create a new setup in Fusion 360. This is done in the Manufacture Workspace. You need to create the laser cutter tool first. It is important to create a new "Cutting" setup so you can make a new 2D Profile to cut out.</p>
</div>
<div class="half-box">
<p><img src="/ICS/icsfs/mm/2012_laser_cut_stand_cam_toolpaths.png?target=2e46e934-16b5-4512-84fd-845a119b7409" alt="" width="100%" height="auto" /></p>
<p><em><span class="caption-jimmy">View of tool path layout in the Manufacture Workspace</span></em></p>
</div>
</div>
<hr />
<h2>6. Save your Tool Paths as a DXF via Post Process</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>Select the tool path from your setup and then click on post process. Use the DXF post process that you installed earlier to export a DXF file. Make sure to add the .dxf file extension.</p>
</div>
<div class="half-box"><img src="/ICS/icsfs/mm/2021_laser_cut_stand_post_process.png?target=79fc07dc-ecc7-4f81-95f9-1baaa8d8651e" alt="" width="100%" height="auto" />
<p><em><span class="caption-jimmy">Example of each part of the stand as a separate component at the top level assembly in Fusion 360.</span></em></p>
</div>
</div>
<hr />
<h2>7. Add appearances and Export Render</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>In Fusion 360 add appearances to you model as you wish and export a render. Label the file YYYYMMDD Lastname Firstname Laser Cut Stand Render.png/jpg</p>
<p>Make the model look the way you want the final product to look. If you are going to paint pieces then paint the pieces in the render. If you will have etchings then put an image decal on to represent the etchings.</p>
<p>Make sure your render is well composed and high resolution with at least one direction 4000px. Choose a 4:3 16:9 or 1:1 aspect ratio. You can make multiple render views.</p>
</div>
<div class="half-box"><img src="/ICS/icsfs/mm/2021_laser_cut_stand_render_assembled.png?target=d2816632-cdbb-42b4-a186-d73d5c3d10f6" alt="" width="100%" height="auto" />
<p><em><span class="caption-jimmy">Example of each part of the stand as a separate component at the top level assembly in Fusion 360.</span></em></p>
</div>
</div>
<hr />
<h2>8. Open DXF in Illustrator and Adjust Stroke</h2>
<div class="flex-container-jimmy">
<div class="half-box">
<p>You need to change the stroke weight of the red strokes in Illustrator. Also you need to change the stroke color and weight of any strokes that you want to etch. You can also draw new strokes to etch while in Illustrator. Etched strokes need to be blue and .5. Make sure you scale the document 100% and have 1mm = 1mm.</p>
</div>
<div class="half-box"><img src="/ICS/icsfs/mm/2021_laser_cut_stand_in_illustrator.png?target=2abac7c8-b371-4bb8-b744-970cb43e82ec" alt="" width="100%" height="auto" />
<p><em><span class="caption-jimmy">Example of each part of the stand as a separate component at the top level assembly in Fusion 360.</span></em></p>
</div>
</div>
<h1>Files to Upload to Google Drive</h1>
<p>Make a labeled folder YYYYMMDD Lastname Firstname Laser Cut First Models and put the following files inside the folder. Label the individual files. Then upload the folder to the class Google Drive.</p>
<ol>
<li>Fusion 360 .f3d file</li>
<li>Rendering(s) of project with appearances applied (.png or .jpg)</li>
<li>Illustrator .ai file of the cut paths (cut with red stroke .001 weight and engraving with blue stroke .5 weight)</li>
</ol>
<h2>Google Drive Upload Folder</h2>
<p><a href="https://drive.google.com/drive/folders/1_nf7dl8bfijs609QyJQm1yPhFqdEmYzt?usp=sharing">https://drive.google.com/drive/folders/1_nf7dl8bfijs609QyJQm1yPhFqdEmYzt?usp=sharing</a></p>
<h1>Instructional Videos</h1>
<p>

</style>
<a href=https://www.youtube.com/embed/${idYoutube}?rel=0&autoplay=1>
    <img src=https://img.youtube.com/vi/${idYoutube}/hqdefault.jpg alt="YouTube thumbnail">
        <span class="playbutton">►</span></a>
               
                `;
                }
            });
        });
    </script>
</p>
<div class="video-grid" style="display: grid; align-items: end; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 1rem;">
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">1. Model Laser Cut Cell Phone Stand</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/7RAdmbOudoo?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Model a Living Hinge Bend for Laser Cutting</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/nt-44j15xeI?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Import SVG or DXF File from Illustrator into Fusion 360</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/aMBnke14Wgg?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Create Laser Cutter Tool with Specific Kerf</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/-B6DXF9aE5s?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Download and Install DXF Post Process for Fusion 360</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/CBu6vl6Bqos?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Fully Define Splines in Fusion 360 Sketch</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/ynBl9XJesDs?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Pattern Along Path or Spline</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/9xit7JRPQ0A?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Change Plywood Thickness Fusion 360</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/a7HOiBC_81s?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Fix Timeline Errors in Fusion 360</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/F3673fmEymo?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Make a Manufacture Model Copy of Your Design</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/bhVPR4CUOUk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Lay Parts Flat with Arrange for Laser Cutting</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/jeQPJHHwVN4?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Export DXF Toolpath with Kerf Compensation</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/6JFHMV7A9TU?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>

# Grading Rubric

| Asessement                  | Weight    |
| --------------------------- | --------- |
| Model Quality               | 50 points |
| Render Image                | 20 points |
| Manufacture Workspace Setup | 10 points |
| Tool Path Export            | 10 points |
| File Management             | 10 points |

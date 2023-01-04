---
title: "4.1 CNC Design Research"
date: 2020-01-26T23:11:13Z
draft: false
---

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">&nbsp;</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">&nbsp;</div>
</div>
<h1>CNC Stool / Chair / End Table / Game Console Stand</h1>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">We will continue learning parametric modeling in Fusion 360. Parametric modeling allows us to change our design depending on the materials that will be used to fabricate it as well as certain parameters that we might want to change for different users. In this project we will design a stool, chair, end table or another large supportive device with an intended purpose such as perfectly holding a PS5.&nbsp;</p>
<p style="margin-right: 1rem;">Stools come in different heights and we may want to easily customize a stool with the same design but fabricate it at a different height without actually remodeling everything. With parametric modeling we can set the height of a stool as a user parameter in our model and then have other dimensions of the design driven by that height. Simply typing a new value for the height will update the rest of the model.</p>
<p style="margin-right: 1rem;">In the previous project we learned about user parameters. We will continue to use user parameters in our designs and learn how to use formulas to make other dimensions driven by parameters.</p>
<p style="margin-right: 1rem;">In this project it is important that your 3D Digital Model is robust. What does that mean to have a robust model? When you use the dimension of ply for the thickness of the plywood you should periodically test different values of "ply" and any other user parameters that you have set. Check to see if you model updates and each piece is referenencing the size of other pieces. It is a good idea to change to value of ply each time you make a new component or piece of your model to make sure all the parameters are changing the model as expected.</p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;"><img src="/ICS/icsfs/mm/cnc-stool-example.jpg?target=819278b4-4d44-4a3d-b4c3-d5e845de1659" alt="" width="100%" height="auto" /></p>
</div>
</div>
<h1>CNC Routers vs Laser Cutters</h1>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">There are differences between a laser cutter and a CNC router. These differences include, kerf size, need for holding down a workpiece and the ability of the router to make pocket cuts or cuts that don&rsquo;t go all the way through the material.</p>
<p style="margin-right: 1rem;">There are differences between a laser cutter and a CNC router. These differences include, kerf size, need for holding down a workpiece and the ability of the router to make pocket cuts or cuts that don&rsquo;t go all the way through the material.</p>
<p style="margin-right: 1rem;">Laser cutters burn the edges of wood materials while CNC routers make a clean cut on the edges of plywood. Laser cutters have a limit on the size of the material thickness while CNC routers can cut through much thicker materials. This often requires multiple passes of the router bit over the material. When creating toolpaths, this "stepdown" ammount will be important. It is typically 1/2 of the diameter of your tool bit.</p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/oYxp6FXG27I?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<h2>Kerf Size and Dogbone Fillets</h2>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">A laser cutter has a very thin beam and although it can't cut a perfect inside corner, the corners it cuts are very square compared to the larger curves required by a CNC router bit. The default CNC router bit we will use on the Shopbot is &frac14; in. The laser cutter beam is merely 0.127 mm. Because of this larger kerf on the Shopbot we need to account for that on inside corners. We will use a technique called &ldquo;dog bone fillets&rdquo; to make space for our slots to fit in. These are called dog bone fillets because they look like cartoon dog bones. We can add these fillets parametrically in Fusion 360. The fillets are required for square parts to fit into inside corners.</p>
<p style="margin-right: 1rem;">There are two methods of making dogbone fillets, one is the classic "cartoon dogbone" and the other are "invisible". They are still cut into the wood but are positioned so the connecting piece covers the cuts and therefore the fillets are not seen in the final project.</p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/fjrEmJeM-qw?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<h2>Securing the Workpiece</h2>
<p>On the laser cutter we merely set our piece inside the cutter and don't need to hold it down. The router is a much larger and powerful machine and will knock the workpiece all over the place causing damage and potential injury. We need to firmly secure our material to the router table before using the machine. It is important to make sure that any Fasteners used to secure the workpiece do not come in contact with the spinning router bit.</p>
<h2>Pocket Cuts and Joints</h2>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">The laser cutter can only etch on to the surface of the material or cut all the way through. The router can make 3 dimensional cuts. It can round off the top and make three-dimensional sculptural forms by cutting away parts of the material. I can also make a pocket cut. A pocket cut is a cut that does not go all the way through the base material. This is not possible with a laser cutter.</p>
<p style="margin-right: 1rem;">We will use pocket cuts to secure different parts of our projects. This is a convenient way to make tabs on one part slot into another supporting piece. It is also way to hide the construction and undesirable joints that we don't want to see in the final design.</p>
<p style="margin-right: 1rem;">Aditional joints that can be made by CNC machines are lap joints, mitered lap joints, t-lap joints, mortise and tennon joints, keyed mortise and tennon joints and many others. This <a href="https://google.com/search?q=cnc+joints&amp;tbm=isch">Google Image Search</a> shows a great variety of <a href="https://google.com/search?q=cnc+joints&amp;tbm=isch">CNC joints</a> to try in your project.</p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/O5IR9pr9vdo?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<h1>Design Process</h1>
<h2>Research</h2>
<p>Before starting your project it is important to see what types of designs have been made. This can give you inspiration and new ideas for your project. You do not research other designs to copy them but to find out solutions that others have made. You can then take inspiration from those solutions and create your own designs and Concepts. This is an important part of any creative process.</p>
<div class="gallery-grid-jimmy" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 10px; justify-items: center; justify-content: center;">
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=cnc+stool&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/cnc-stool-search.png?target=75748d52-847e-485e-90bc-6f80d27679bc" alt="" /> </a></div>
<p><a href="https://google.com/search?q=cnc+stool&amp;tbm=isch">Google image Search of CNC Stools </a></p>
</div>
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=cnc+chair&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/cnc-chair-search.png?target=20b15277-d3cf-4475-baa7-acaaf33835f4" alt="" /> </a></div>
<p><a href="https://google.com/search?q=cnc+chair&amp;tbm=isch">Google image Search of CNC Chairs</a></p>
</div>
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=stool+design&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/stool-design-search.png?target=97ae22cd-2e55-477a-bfc1-267ca13569dd" alt="" /> </a></div>
<p><a href="https://google.com/search?q=stool+design&amp;tbm=isch">Google image Search of Stool Design </a></p>
</div>
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=cnc+plywood+table&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/cnc-plywood-table-search.png?target=7104b9b3-09b2-4556-a4bb-30516e54fcf0" /> </a></div>
<p><a href="https://google.com/search?q=cnc+plywood+table&amp;tbm=isch">Google image Search of CNC Tables</a></p>
</div>
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=cnc+joints&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/2022_cnc_joints_search.png?target=81288f5f-8017-4a4b-8551-9549aa233f3c" /> </a></div>
<p><a href="https://google.com/search?q=cnc+plywood+table&amp;tbm=isch">Google image Search of CNC Joints</a></p>
</div>
<div class="img-card-jimmy" style="display: flex; flex-direction: column; justify-content: stretch;">
<div class="image-box-jimmy" style="position: relative; width: 300px; height: 300px;"><a href="https://google.com/search?q=chair+living+hinge&amp;tbm=isch"> <img class="fit-img-jimmy" style="object-fit: cover; position: absolute; height: 100%; width: 100%; top: 0; left: 0;" src="/ICS/icsfs/mm/2022_chair_living_hinge_search.png?target=5efc0457-2a0c-4edc-a036-0991e9428df6" /> </a></div>
<p><a href="https://google.com/search?q=cnc+plywood+table&amp;tbm=isch">Google image Search of Chair Living Hinges</a></p>
</div>
</div>
<h2>Collect Images</h2>
<ol>
<li>
<p>Collect a minimum of 10 images of existing designs. You can take screenshots or download the images.&nbsp;</p>
</li>
<li>
<p>Organize the images into a folder called &ldquo;CNC Design Inspiration Images.&rdquo; Label each of the images with a descriptive title that includes the creator&rsquo;s name.&nbsp;</p>
</li>
<li>
<p>Put each of these images into a Google Slides Presentation. Use one slide per image.&nbsp;</p>
</li>
<li>
<p>On each slide write 2-3 sentences about why you selected this image and what your find intriguing about it.&nbsp;</p>
</li>
<li>
<p>Put a link on each slide to where you found the image.</p>
</li>
<li>
<p>Save the presentation as a PDF YYYYMMDD Lastname Firstname CNC Design Inspiration</p>
</li>
<li>
<p>Upload the PDF and the folder of Images to Google Drive</p>
</li>
</ol>
<h2>Research Design Parameters</h2>
<p>Look up standard stool heights, chair sizes, and table sizes. You can simply enter these search terms into Google. Write down what you find. You do not have to make something a standard size but generally it is a good place to start your design process.</p>
<h1>Design Requirements</h1>
<ul>
<li>Support the weight of a person or the intended item</li>
<li>Have considered aesthetics</li>
<li>Use 1/2" or 3/4" plywood</li>
<li>Use more than 1 type of joint</li>
<li>Have a considered and designed top surface, this could have engraving or decorative joints</li>
<li>Be a relatively standard size</li>
<li>Fit pieces on a half sheet of plywood or full sheet of plywood</li>
</ul>
<h2>Ideation Sketches</h2>
<ol>
<li>
<p>Make a minimum of 10 thumbnail sketches of ideas. Keep the ideas varied and different. Push yourself to be inspired by designs you researched but to come up with your own ideas and concepts.</p>
</li>
<li>
<p>After making initial sketches, choose 5 ideas and make larger refined sketches. You may need to draw these from different views and show details of how you plan to join the pieces together.</p>
</li>
<li>
<p>Choose your favorite idea and draw a larger final sketch. This could be a third angle projection drawn by hand or with a t-square that includes the Front, Top and Right views. It could also be a detailed rendered iage that is descriptive of its form and construction. Put dimensions on you drawing.&nbsp;</p>
</li>
<li>
<p>Scan or photograph your sketches. If using a scanner, make sure that the DPI is high enough and that the exposure on the scanner captures enough detail, especially if you have light sketches. If you are photographing your sketches, ensure that there is even lighting, no shadows. Make sure that there are no extra items in the photo. Make sure there are no distortions or trapezoid shapes from taking the photo at an angle. Keep the camera square to the paper.</p>
</li>
<li>
<p>Label you files YYYYMMDD Lastname Firstname CNC Ideation Sketches</p>
</li>
<li>
<p>Upload to Google Drive</p>
</li>
</ol>
<h2>Make a Scale Cardboard Model</h2>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">Make a cardboard model of your design. It is one thing to draw with pencil on paper, it is another to make a physical object. Problems and solutions that may not be apparent in your drawing will reveal themselves when you make a physical object. The model will be smaller than actual size.&nbsp;</p>
<p style="margin-right: 1rem;">You can cut the cardboard with hand tools or the laser cutter or both.</p>
<p style="margin-right: 1rem;">We will be using &frac34;&rdquo; or &frac12;&rdquo; plywood for this project. You can use a ratio to scale your model.</p>
<p style="margin-right: 1rem;">Measure the cardboard and use a ratio calculator to scale your model dimensions.</p>
<p style="margin-right: 1rem;">First calculate the scale factor of your materials. If your single sheet of cardboard measures ~3.3mm and 3/4" plywood is ~18mm then you have a scale factor of 11:60. This website can easily calculate the scale factor for you. <a href="https://www.ginifab.com/feeds/cm_to_inch/scale_factor_calculator.html">https://www.ginifab.com/feeds/cm_to_inch/scale_factor_calculator.html</a></p>
<p style="margin-right: 1rem;">Once you know the scale factor then you can determine how big the pieces of your cardboard model should be based on that scale factor. This website lets you enter a scale factor and then enter in your final desired design dimension. For example if you want something 30" tall, you put in a scale factor of 11:60, type 30" in the "real length" and set the "scale length" to mm to get the scaled model size in mm. (You can use inches for your cardboard model but millimeters are soooo much easier to use, count, divide. Notice I put in 30" because for some distances I know imperial units better but then I quickly convert to the easier to use metric system. Make sure you always double check your units.) This website will scale all your numbers. <a href="https://www.ginifab.com/feeds/cm_to_inch/scale_converter.html">https://www.ginifab.com/feeds/cm_to_inch/scale_converter.html</a></p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<div class="video-grid" style="display: grid; align-items: end; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 1rem;">
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/j-KeJDNf9HQ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/Tm7xTiLl4Hw?rel=0" width="560" height="315" frameborder="0">
                </iframe></div>
</div>
</div>
</div>
<h2>Photo Documentation of Cardboard Model</h2>
<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0;">
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<p style="margin-right: 1rem;">Take a minimum of two photos of your model. Take one from a 3/4 angle that shows a good representation of the form. Take the other from a composition of your choice.</p>
<p style="margin-right: 1rem;">Set up lights and a clean backdrop. You can check out lights and a camera from the CIA equipment checkout. You can also take your model to the think[box] and use the soft boxes and flashes already set up. Shoot in JPG and RAW and post process the images. <a href="https://www.youtube.com/watch?v=m0yZEWUSahk">White balance should be corrected</a> and the levels should be adjusted to have good exposure. Use Photoshop and <a href="https://www.youtube.com/watch?v=11jwSwUu2WI">Adobe Camera Raw</a> to make adjustments and to retouch any mistakes in the images. Label the photos YYYYMMDD CNC Cardboard Model</p>
</div>
<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/Cq_Cx_5Zhks?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>
<h1>Assignment Deliverables Summary</h1>
<ol>
<li>
<p>Folder of labeled design inspiration images (minimum 10)</p>
</li>
<li>
<p>PDF export of Google Slides Presentation of design inspiration</p>
</li>
<li>
<p>Minimum 10 Thumbnail Ideation Sketches</p>
</li>
<li>
<p>Minimum 5 larger refined Ideation Sketches</p>
</li>
<li>
<p>1 Larger Final Sketch of Design with dimensions</p>
</li>
<li>
<p>Minimum of 2 photos of scale Cardboard Model</p>
</li>
</ol>
<p>Upload everything in a single folder to the class Google Drive Folder</p>
<h2>Google Drive Folder Link</h2>
<p>Link: <a href="https://drive.google.com/drive/folders/1a1F1QWe0wM3KxJtZBd3XlCcKK_l8zar2">https://drive.google.com/drive/folders/1a1F1QWe0wM3KxJtZBd3XlCcKK_l8zar2</a></p>
<h1>Project Resources</h1>
<p>CIA Fab Studios Online Store - <a href="https://my.cia.edu/ICS/Student/Supply_Store/Fabrication_Studios/Wood/">https://my.cia.edu/ICS/Student/Supply_Store/Fabrication_Studios/Wood/</a></p>
<p>The Fab Studios sells pre-cut half sheets of 1/2" and 3/4" plywood. You can purchase it online at the Fab Studios' online store on myCIA.</p>
<p>&nbsp;</p>
<h2>Fusion 360 CNC Tutorial Videos</h2>
<div class="video-grid" style="display: grid; align-items: end; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 1rem;">
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Scale Cardboard Model to Plywood Thickness</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/j-KeJDNf9HQ
                    ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Laser Cutting vs CNC Router</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/oYxp6FXG27I?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Simple CNC Joints</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/O5IR9pr9vdo?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Invisible Dogbone Fillets</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/fjrEmJeM-qw?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Create ShopBot Tool Fusion</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/M9MQzYrLhGQ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Creat ShopBot Toolpaths in Fusion</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/_G-0i8BFEFs?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">CNC Hex Stool</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/9utpuieg5lI?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">CNC End Table</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/GzknioA34F8?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">CNC Two Level Table</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/I6FEMdtcrpI
                    ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">CNC Plywood Chair</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/GqXQ8TdzYRE?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Document Art with Cellphone</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/Cq_Cx_5Zhks?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Open Any Image in Camera Raw</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/ftMICesJwGc?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Quick White Balance in Photoshop</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/m0yZEWUSahk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">
<h2 style="padding: 1rem 0.5rem 0.3rem 1rem; margin: 0; font-size: 18px;">Camera Raw Tutorial</h2>
<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/11jwSwUu2WI?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
</div>
</div>

# Grading Rubric

| Assesment                     | Weight    |
| ----------------------------- | --------- |
| Design Research               | 20 points |
| 10 thumnails                  | 10 points |
| 5 revised sketches            | 20 points |
| Larger Final Sketch           | 20 points |
| Sketch Documentation          | 10 points |
| Cardboard Model               | 20 points |
| Cardboard Model Documentation | 20 points |
| File Management               | 10 points |

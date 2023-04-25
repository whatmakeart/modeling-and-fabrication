---
title: "14.05 Maya 3D Animation"
date: 2020-01-26T23:11:13Z
draft: false
---

## Animation

- [Maya Time Slider Settings](https://youtu.be/SYuaAMHzY_8)
- [Maya Add Renderable Camera](https://youtu.be/VfqYe8O6KlM)
- [Maya Render Image Sequence](https://youtu.be/vxvIUBeTkL0)
- [Maya Multiple Renderable Cameras](https://youtu.be/g0btNU7YPUo)

### Animation Rigs

- [Maya Sphere Ball Rig](https://youtu.be/3uYyw_q7L3o)
- [Maya Quadball Rig](https://youtu.be/zgNk7WGKV30)
- [Custom Rig Controllers](https://youtu.be/CtsTcsBHGdY)
- [Selection Child Highlighting](https://youtu.be/HuGrXTDwP7c)

### Animation

- [Maya Simple Ball Bounce](https://youtu.be/xWDiuV8-PZQ)
- [Maya Ball Bounce Animation Physics](https://youtu.be/v7qQTfDQ3Ac)

# 15 - 30 Second Animation in a 3D Environment

## Requirements

Must be a ~15-30 second long video composed in Adobe Premiere using images created and rendered in Autodesk Maya.

- Include multiple animated sequences from Maya.
- Have a ball character, may include additional characters.
- Have a structure, does not have to be a traditional narrative but must have story structure.
- Use 3 different camera angles in Maya
- Have multiple scenes.
- Have UV mapped objects with textures created by you in Maya, Substance Painter, Photoshop or other image software.
- Must show basic animation principles such as squash and stretch.
- Include sounds created by you.
- Include music from public domain or created by you.
- Have animated text as credits or intro.

# Objectives

Your objective is to demonstrate an understanding and competence of composition and other fundamental visual concepts as applied to moving art and sound. In addition you should demonstrate an ability to use basic principles such as squash and stretch. Create a purposeful composition. Use a variety of shots and camera angles. Use well-considered visual themes, including colors and general style of visual treatments and elements.

Draft a Story Spine that follows a basic narrative arc. This will give you guidelines and a plan to make your animation. Use the story spine to draw storyboards of the scenes and different camera angles that you want to use.

Create a 3D environment or "animation set" of 3D modeled objects. This Environment should be real world scale and be interesting enough to use as a setting for your bouncing ball animation. You can model different items for your scene and combine the meshes and group them together. You can save the items all in one Maya scene or save each item as a different scene and import them into your main scene.

Use the UV mapping editor in Maya to map the UVs of your objects and export UV snapshots for importing into Photoshop. Paint textures onto the UV snapshots and export the new textures to your "sourceimages" folder in your Maya project. Apply the Textures and edit as needed. You can also use Adobe's Substance Painter to add detailed textures. Smooth your object and then save it as an .obj file to import into Substance Painter. Then you can use all of the materials in Substance Painter.

Add lights to the scene. Make sure to only add "Arnold Lights." Do not use any of the older Maya lights or you will not be able to use the CIA Render Farm. Remember that you will have to increase the exposure of the lights to make your render show up in the Arnold Renderer.

Add multiple cameras to the scene. Animate a bouncing ball that travels through the scene in an interesting way. Use the animation principles of squash, stretch, exaggeration, anticipation and follow through. Use a minimum of 3 different camera angles and shot types. to apply textures to your objects. Export the different camera angles as separate sequence renders.

# Make an Animation Set(s) & Assets

## 1. Make a List of Needed Assets

After you make your storyboards, make a list of the items and settings for your animation. Is there a boat and water? Is there a box of donuts? Does the ball sit on a shelf? Think of the simple shapes and polygons that can start to make these objects. A box of donuts could start with a scaled cube and a bunch of torus primatives in it, a shelf is just multiple scaled cubes, a boat is a bit more complex but is an elongated cube with some vetecies moved around.

## 2. Set Your Maya Project

Before you begin making any objects in your Maya scene, make sure you set your project. We did this in class but you should go to File > Set Project and then choose your project folder everytime you start working in Maya. This makes sure you are working with the right files and folders. Always move a texture or external file into your project folder before importing into Maya.

## 3. 3D Model Objects

After you set your Maya Project, begin to create the assets that you need for your animation set. This includes objects, a ground plane, things in the background, walls, hills, etc. You can make multiple scene files and combine them or make everything in one scene file. Sometimes it is better to make an object as its own scene file and then import it into your main animation set scene file. This videos shows [how to import and reference other scenes into your main scene.](https://youtu.be/WDpYKvhSOYI) How you organize your files is up to you as long as all files are in your project folder.

Model multiple 3D objects to create an interesting visual environment to animate in. Add walls / furniture, rugs, chairs, tables, buildings and other objects forms. You setting(s) can be indoors or outdoors or both. Making a new scene file for different settings is a good idea. All scene files should be in your project's scenes folder. Think

## 4. Add Materials and Textures

After you finish modeling your objects, combine all the mesh parts with Mesh > Combine. Then delete the history and freeze the transformation. This video shows [how to delete history and freeze transformations](https://youtu.be/1SXvWTiMkjs). You will do tis multiple times on different objects as you model and make changes. Begin to add materials and textures to the objects in your scene. You can right click on your different objects while in Object Mode. Then select "Assign New Material". Click on Arnold in the menu and then select aiStandardSurface. In the Attribute Editor change the name of the aiStandardSurface to the name of your object. You can add "Shader" to the end of the name. Then select a color or a preset.

You can also add textures by 3D Painting in Maya. First [unwrap your object's UVs](https://youtu.be/8-TMjuvzZEU) and then assign a new Blinn material. The Maya 3D paint tools do not work on aiStandardSurface. This video shows [how to 3D paint in Maya](https://youtu.be/JIOns8Tkmhs)

Don't forget about using photo-based materials / textures. You can easily create seamless textures in Photoshop and then add them to your shader by clicking on the icon by color in the attribute editor of your shader. This video shows [how to create seamless textures in Photoshop](https://youtu.be/PJ7L4S5ylqg).

You can also UV unwrap your model and export it as an OBJ file to texture in Substance Painter. This video shows [how to quickly UV unwrap your object and export a OBJ file](https://youtu.be/8-TMjuvzZEU). Substance Painter is installed on the lab computers but you will need to download it from the Adobe Creative Cloud if using your laptop. Create a new file in Substance Painter, select the top default template and then select your exported OBJ file. Paint the textures you want and then export your textures to your "sourceimages" folder in you Maya Project. You can use the Substance plugin in Maya to assign your textures to a new material and then assign that material to your object. This video shows [how to make and export textures with Substance Painter](https://youtu.be/sCKc_6nTRPM).

## 5. Add Lights

If you try to render your animation scene with the Arnold Render view, everything will be black because there are no lights in the scene. You need to add lights from the Arnold lights menu. Only add Arnold lights. Do not add any Maya lights. If you select lights from the Arnold menu then you will only add Arnold Lights.

For a quick view of your set you can add a simple skydome light. This will light the whole scene evenly but is not the most interesting lighting. Instead of a skydome light or artificial sky light, add multiple Arnold Area Lights. These are flat squares like LED light panels. Press "r" on your keyboard to scale the lights up and press "e" to rotate them towards your objects, then press "w" to move them into position. In the attribute editor the default exposure value for Area lights is 0.00\. You need to increase this to somewhere between 8.00 and 16.00 (You scene may be different and may need more or less exposure). Each time you increase the exposure value it is like 1 F-stop on a camera and it doubles the amount of light.

Place as many lights as you need in different places in your scene. Vary the intensity and color of the lights. It is a good idea to label the lights with descriptive names in your Outliner on the left hand side of the screen so you don't get confused.

## 6. Add a Renderable Camera

After you add lights, then you should add a new Render Camera. This video shows [how to add a renderable camera](https://www.youtube.com/watch?v=VfqYe8O6KlM) to your Maya scene. You can look through this camera and position it for your scene. Then you can lock the camera so it does not move. Then you can switch back to the default perspective camera to continue modeling and editing your scene. Label the new camera that you created and then make sure to select it in the Arnold Renderview Window.

Add multiple cameras for the different shots and animations you want to create. You may want to make duplicate scenes for different actions. This video shows [how to add multiple renderable cameras](https://www.youtube.com/watch?v=g0btNU7YPUo) to your scene.

## 7. Make a Minimum of 1 Render of Your Animation Set(s)

After your lights and camera are set up, make and save a high resolution, high quality render of your scene. The default render settings are too low for presentation but are good for quick renders. To export your high quality render you need to change the render settings before rendering.

Change the render size to a minimum of HD_1080 1920x1080 and increase the Arnold - Camera (AA) samples to at least 5\. Remember to changes this back to the default HD_540 and 3 samples so your test renders go quickly while modeling.

## 8. Make an Archive ZIP of Your Scene

After you create your scene. Archive the Maya scene with the Maya scene archiver. If you do not archive the scene, then texture files will not be attached and you will only have the model data. To archive your scene, with your scene open, go to File > Archive Scene. This will create a zip of your scene and any needed texture files. It will create a zip file in your Project's scenes folder. This video [shows how to archve a Maya scene](https://youtu.be/gic-kMWKjNI).

Label this zip file as YYYYMMDD Lastname Firstname Archived Set Scene.zip Turn in to the class Google Drive Folder.

# Animate

## Create Character(s)

You are required to make a simple ball character. This could be a simple sphere polygon with a texture applied. It could be a [tennis ball](https://youtu.be/IfSis4ns8SY), [volley ball](https://youtu.be/E37FC_Uu0Vg), [soccer ball](https://youtu.be/GcDalspwhlc) or [golf ball](https://youtu.be/2wizG1Dsm8w) or a [teddy bear](https://youtu.be/2hq1F8gkn4A) from the tutorial videos. It could be a sphere that you have sculpted spikes or fur onto. As long as it is generally round and can be animated with squash and stretch. It does not have to roll but it can. It could bounce or "jump" everywhere. Attach a squash and stretch animation rig to this ball character.

Apply textures to the ball that you [3D Paint in Maya](https://youtu.be/JIOns8Tkmhs), [create in Photoshop](https://youtu.be/PJ7L4S5ylqg) or Substance Painter. This video shows [how to make and export textures with Substance Painter](https://youtu.be/sCKc_6nTRPM).

After you create your ball character you can make any other characters or objects to animate. Make additional stuff to be in your scenes to make it more visually interesting.

## Animate Your Characters

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0; gap: 1rem;">

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

After you have all your animation assets. Begin to animate. Remember that other things in the scene can move as well. Anything can animate. You can change the positioning of lights. The environment can change, the camera can move around.

We will use a basic animation rig for your ball. This will simplify your animation tasks by separating the squash / stretch from the rotation and position. You can make other rigs for other elements in your animation if you want. This [video shows how to make a ball animation rig](https://youtu.be/zgNk7WGKV30).

We will animate using keyframes. You can set keyframes in the channel box for individual parameters by right clicking and selecting "key selected". You can set all keyframes for a selected object by pressing "s" on your keyboard. You can also turn on automatic keyframes so it sets a keyframe everytime that you move the timeline and move your objects. This can be helpful but can also result in way to many accidental keyframes. This video shows [how to animate a bouncing ball](https://youtu.be/xWDiuV8-PZQ).

Don't forget that you can animate the camera as well. Camera motion, even if just a little bit can really make your scene come alive. You can layer tha background and foreground objects and have the camera "dolly" or move sideways to create a 3D parallax effect. By animating the camera, everything on the screen will have some motion.

You can also animation the position and intensity of lights. Your imagination is the only limit.

As you finish different animation sequences, [export them as rendered image sequences](https://youtu.be/v7qQTfDQ3Ac).

</div>

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/xWDiuV8-PZQ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

</div>

# Import into Premiere and Edit Video

After you have the different scenes of your animations [exported as a series of images](https://youtu.be/vxvIUBeTkL0) import them into Adobe Premiere for editing. You can [import a folder of images as an image sequence](https://youtu.be/X7w0xOprNDk) and premier will treat it as a video file. Video editing allows you to jump back and forth from different camera angles. You could simply [set up 4 cameras in Maya](https://youtu.be/g0btNU7YPUo), export each camera's view of your animation and then cut them together in Premiere. This is where you will add pacing to the cuts of your scenes and shots. This video shows [how to setup and organize your Premiere Project](https://youtu.be/zf8IDYvvUkY).

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0; gap: 1rem;">

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/zf8IDYvvUkY?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/X7w0xOprNDk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

</div>

# Add Music and Sound

<div class="flex-container-jimmy" style="display: flex; align-items: top; flex-wrap: wrap; margin-top: 0; margin-bottom: 0; gap: 1rem;">

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

In addition to rich visuals, adding music and sound to your animation will make it come alive. This video shows [how to add sound effects](https://youtu.be/Ds2QJryBf84) to your video. We will your Creative Commons Licensed music and sound effects to make the objects in our animation seem more real. We will also create our own sound effects. All CC licensed music and sounds must have proper written attribution in the credits at the end.

- Adobe Sound Effects: [https://www.adobe.com/products/audition/offers/AdobeAuditionDLCSFX.html](https://www.adobe.com/products/audition/offers/AdobeAuditionDLCSFX.html)
- FTP of Adobe Music Loops and Beds (Must use FTP to download) - [ftp://ftp.adobe.com/pub/adobe/audition/Loops/](ftp://ftp.adobe.com/pub/adobe/audition/Loops/)
- Kevin McLeod's Music: [https://incompetech.com/music/royalty-free/music.html](https://incompetech.com/music/royalty-free/music.html) Remember to [credit](https://incompetech.com/music/royalty-free/faq.html) Kevin's music exactly as he requests.

</div>

<div class="half-box" style="flex: 1 1 400px; margin-top: 0; margin-bottom: 0;">

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/Ds2QJryBf84?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

</div>

# Export an .mp4 of You Animation

Use the h.264 video codec to export an .mp4 of your animation and label the file YYYYMMDD Lastname Firstname 3D Animation.mp4

# Project Resources

## Technical Reminders

- Make a Maya Project and always set your project when working
- Put all your files, including your textures and other images into the proper folder structure for your Maya project.
- Use the increment and save feature of Maya.
- Delete the history of objects in your scene when not needed to keep Maya from crashing and running slow.
- Do NOT delete the history of any object after you rig it, you should delete the modeling history before rigging.
- Create a separate folder for your Video Editing
- Copy all needed files (image Sequences, sound files, etc.) into this Video Project folder.
- Save your Premiere project file in your Video Folder
- Save all project files in that folder. Do not rename files after importing them. Do not move files after importing them.

# Instructional Videos

<div class="video-grid" style="display: grid; align-items: end; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); grid-gap: 1rem;">

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Maya User Interface Introduction

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/-SpVNiRqeKY?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Maya Polygon Modeling Tools

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/eBEitxaRYQs?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Make Hole in Cube

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/EIKiJUmUH7A?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Polygon Modeling Exercise

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/lLItO9mBwxM?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Three Point Lighting for Rendering

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/1nYSVw6-GxA?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## UV Map a Cube

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/BFf4L5vDR84?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Create Seamless Textures

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/PJ7L4S5ylqg?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Basic UV Mapping

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/X0KGwPadukE?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Sphere Ball Rig

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/3uYyw_q7L3o?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Quadball Rig

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/zgNk7WGKV30?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Insert Reference Image

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/tXJFJa-nsAA?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Model a Teddy Bear

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/2hq1F8gkn4A?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Model Soccer Ball

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/GcDalspwhlc?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Model Golf Ball

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/2wizG1Dsm8w?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Model a Volley Ball

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/E37FC_Uu0Vg?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Model a Tennis Ball

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/IfSis4ns8SY?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## 3D Cut and Sew UV Unwrap

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/-KhoMBOqx0g?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Ball Bounce Animatinon

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/xWDiuV8-PZQ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Ball Bounce Physics

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/v7qQTfDQ3Ac?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## 3D Paint Tool

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/JIOns8Tkmhs?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Paint 3D Object

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/0JY8UA75qjI?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Add Render Camera

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/VfqYe8O6KlM?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Render Image Sequence

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/vxvIUBeTkL0?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Import Image Sequence Premiere

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/X7w0xOprNDk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Time Slider Settings

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/SYuaAMHzY_8?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Import vs Reference Assets

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/WDpYKvhSOYI?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Multiple Renderable Cameras

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/g0btNU7YPUo?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Set Up Premiere Video Editing Project

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/zf8IDYvvUkY?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

<div class="video-wrapper" style="border: 1px solid grey; display: flex; flex-direction: column; height: 100%; justify-content: space-between; margin: 0;">

## Add Sound Effects

<div class="youtube-box" style="position: relative; width: 100%; height: 0px; padding-top: 56.25%; margin-top: 0; margin-bottom: 0;"><iframe class="youtube-iframe" style="position: absolute; top: 0; bottom: 0; left: 0; width: 100%; height: 100%; border: 0; z-index: 1;" src="https://www.youtube.com/embed/Ds2QJryBf84?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>

</div>

# Grading Rubric

| Assessment                                       | Weight    |
| ------------------------------------------------ | --------- |
| Have Multiple Scenes                             | 50 points |
| Show Basic Animation Principles                  | 50 points |
| Folder of Exported Rendered Images               | 25 points |
| Use of Lighting and Rendering                    | 25 points |
| UV Textures Applied to Objects                   | 25 points |
| Use Sound Effects and Music to Enhance Animation | 25 points |
| Text Credits                                     | 25 Points |

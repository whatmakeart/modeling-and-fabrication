---
title: "13.02 3d Animation Sets"
date: 2020-01-26T23:11:13Z
draft: false
---

# Make an Animation Set(s) & Assets

## 1\. Make a List of Needed Assets

After you make your storyboards, make a list of the items and settings for your animation. Is there a boat and water? Is there a box of donuts? Does the ball sit on a shelf? Think of the simple shapes and polygons that can start to make these objects. A box of donuts could start with a scaled cube and a bunch of torus primatives in it, a shelf is just multiple scaled cubes, a boat is a bit more complex but is an elongated cube with some vetecies moved around.

## 2\. Set Your Maya Project

Before you begin making any objects in your Maya scene, make sure you set your project. We did this in class but you should go to File > Set Project and then choose your project folder everytime you start working in Maya. This makes sure you are working with the right files and folders. Always move a texture or external file into your project folder before importing into Maya.

## 3\. 3D Model Objects

After you set your Maya Project, begin to create the assets that you need for your animation set. This includes objects, a ground plane, things in the background, walls, hills, etc. You can make multiple scene files and combine them or make everything in one scene file. Sometimes it is better to make an object as its own scene file and then import it into your main animation set scene file. This videos shows [how to import and reference other scenes into your main scene.](https://youtu.be/WDpYKvhSOYI) How you organize your files is up to you as long as all files are in your project folder.

Model multiple 3D objects to create an interesting visual environment to animate in. Add walls / furniture, rugs, chairs, tables, buildings and other objects forms. You setting(s) can be indoors or outdoors or both. Making a new scene file for different settings is a good idea. All scene files should be in your project's scenes folder. Think

## 4\. Add Materials and Textures

After you finish modeling your objects, combine all the mesh parts with Mesh > Combine. Then delete the history and freeze the transformation. This video shows [how to delete history and freeze transformations](https://youtu.be/1SXvWTiMkjs). You will do tis multiple times on different objects as you model and make changes. Begin to add materials and textures to the objects in your scene. You can right click on your different objects while in Object Mode. Then select "Assign New Material". Click on Arnold in the menu and then select aiStandardSurface. In the Attribute Editor change the name of the aiStandardSurface to the name of your object. You can add "Shader" to the end of the name. Then select a color or a preset.

You can also add textures by 3D Painting in Maya. First [unwrap your object's UVs](https://youtu.be/8-TMjuvzZEU) and then assign a new Blinn material. The Maya 3D paint tools do not work on aiStandardSurface. This video shows [how to 3D paint in Maya](https://youtu.be/JIOns8Tkmhs)

Don't forget about using photo-based materials / textures. You can easily create seamless textures in Photoshop and then add them to your shader by clicking on the icon by color in the attribute editor of your shader. This video shows [how to create seamless textures in Photoshop](https://youtu.be/PJ7L4S5ylqg).

You can also UV unwrap your model and export it as an OBJ file to texture in Substance Painter. This video shows [how to quickly UV unwrap your object and export a OBJ file](https://youtu.be/8-TMjuvzZEU). Substance Painter is installed on the lab computers but you will need to download it from the Adobe Creative Cloud if using your laptop. Create a new file in Substance Painter, select the top default template and then select your exported OBJ file. Paint the textures you want and then export your textures to your "sourceimages" folder in you Maya Project. You can use the Substance plugin in Maya to assign your textures to a new material and then assign that material to your object. This video shows [how to make and export textures with Substance Painter](https://youtu.be/sCKc_6nTRPM).

## 5\. Add Lights

If you try to render your animation scene with the Arnold Render view, everything will be black because there are no lights in the scene. You need to add lights from the Arnold lights menu. Only add Arnold lights. Do not add any Maya lights. If you select lights from the Arnold menu then you will only add Arnold Lights.

For a quick view of your set you can add a simple skydome light. This will light the whole scene evenly but is not the most interesting lighting. Instead of a skydome light or artificial sky light, add multiple Arnold Area Lights. These are flat squares like LED light panels. Press "r" on your keyboard to scale the lights up and press "e" to rotate them towards your objects, then press "w" to move them into position. In the attribute editor the default exposure value for Area lights is 0.00\. You need to increase this to somewhere between 8.00 and 16.00 (You scene may be different and may need more or less exposure). Each time you increase the exposure value it is like 1 F-stop on a camera and it doubles the amount of light.

Place as many lights as you need in different places in your scene. Vary the intensity and color of the lights. It is a good idea to label the lights with descriptive names in your Outliner on the left hand side of the screen so you don't get confused.

## 6\. Add a Renderable Camera

After you add lights, then you should add a new Render Camera. This video shows [how to add a renderable camera](https://www.youtube.com/watch?v=VfqYe8O6KlM) to your Maya scene. You can look through this camera and position it for your scene. Then you can lock the camera so it does not move. Then you can switch back to the default perspective camera to continue modeling and editing your scene. Label the new camera that you created and then make sure to select it in the Arnold Renderview Window.

Add multiple cameras for the different shots and animations you want to create. You may want to make duplicate scenes for different actions. This video shows [how to add multiple renderable cameras](https://www.youtube.com/watch?v=g0btNU7YPUo) to your scene.

## 7\. Make a Minimum of 1 Render of Your Animation Set(s)

After your lights and camera are set up, make and save a high resolution, high quality render of your scene. The default render settings are too low for presentation but are good for quick renders. To export your high quality render you need to change the render settings before rendering.

Change the render size to a minimum of HD_1080 1920x1080 and increase the Arnold - Camera (AA) samples to at least 5\. Remember to changes this back to the default HD_540 and 3 samples so your test renders go quickly while modeling.

## 8\. Make an Archive ZIP of Your Scene

After you create your scene. Archive the Maya scene with the Maya scene archiver. If you do not archive the scene, then texture files will not be attached and you will only have the model data. To archive your scene, with your scene open, go to File > Archive Scene. This will create a zip of your scene and any needed texture files. It will create a zip file in your Project's scenes folder. This video [shows how to archve a Maya scene](https://youtu.be/gic-kMWKjNI).

Label this zip file as YYYYMMDD Lastname Firstname Archived Set Scene.zip Turn in to the class Google Drive Folder.

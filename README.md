# BlenderBackground
How to create a 3D background on Blender and import to Android Studio. You will learn how to dowbload 3D models and how to apply textures from 
## Table of Contents



## Installation

Download the newest Blender Release Candidate onto system:
[https://builder.blender.org/download/daily/](https://builder.blender.org/download/daily/)

Download the .zip file of the 3D Model:
[https://drive.google.com/file/d/1DyBhBpiQDfC5jdB3CQ9LoL4jLg8_2ZAN/view?usp=sharing](https://drive.google.com/file/d/1DyBhBpiQDfC5jdB3CQ9LoL4jLg8_2ZAN/view?usp=sharing)

  - Note: Once you download and unzip the file, make sure you open it and unzip all three internal files

## Importing 3D Model on Blender

1. Open Blender and Create a new General file
  
2. On the top right delete all scene objects
  - Note: On keyboard, press 'a' to select all objects, then press 'x' to delete them

3. On the top left click on 'File' then goto 'Import' and click on 'FBX' to import from your files

4. Locate Sci-fi white interior 3D model file and open file to locate the '1000 Museum fbx' file and import

## Rendering Textures onto 3D Model

1. On the top right, click on the circle farthest to the right to render the model\
![renderCircle_image](render_image.png)
  - Note: It is the circle highlighted in blue
2. Enable Node Wrangler to automatically format textures
  - Note: On the top left goto 'Edit' --> 'Preferences' --> 'Add ons' --> type 'Node Wrangler' and check it off

3. Select an Object and go to Shader Editor (ex: background)
   - Note: Hover mouse on the top right of the screen in the workspace until the pointer turns into a crosshair then drag and click to split
     *ADD DEMO
   - Click on Shade Editor button

4. Click on Principled BSDF and open the Node Wrangler tab then click on 'Add Principled Setup'

5. Go to the file of the 3D model and open the maps folder then drag and drop the 'view5' image onto the Shader Editor workspace
   
7. Connect the Color node from 'view5' to the Base color node in Principled BSDF


## Exporting 3D Model
1. Select all objects by pressing 'A' key then go to File and Export as .glb file
2. Deactivate the 'Animation' box and activate 'Selected Objects' in the 'Include' dropbox
3. Click 'Export to glTF'

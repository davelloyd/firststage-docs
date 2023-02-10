# Creating a Character for Firstage using Character Creator

This guide aims to provide you with the knowledge and resources to help you start to create realistic characters for use in Firststage using Character Creator 3 or CC3 as it will be referred to in this guide.

## Smart Gallery

Before you start in CC3 one thing you should want to install The Smart gallery Plug-in for CC3.\
The smart gallery is Reallusions streamlined way of managing and installing your assets from their content store and/or their market place.\
The Smart Gallery can be installed through the “Reallusion Hub” or via [this link here](https://www.reallusion.com/smartgallery/).

Once you have the Smart gallery successfully installed you can now open up CC3 into a “new Project”\
Once CC3 is launched open the smart gallery by using the shortcut Shift+F4, here you can find and download the free assets that are provided, most notably “CC3 base Character pack”, “CC3 Embedded Hair” and “CC3 Outfit and Accessory”.\
These packs will provide you enough content to start making your CC3 characters.

## Building a Base

A great Starting point for building your character is by utilizing the provided character presets to give you a strong starting point.\
To access the character presets you need to open the “Content Manager” window; the shortcut by default is F4.\
In this Window you will have various tabs across the top. You should start with the one named “Base”. In this tab are various sub-tabs all to do with the fundamental parts of your character from body shape to the colour of their fingernails.

Explore this first tab and start to build the general shape and look of your character.

## Shaping your Character

Now that you have a general shape of your character you may want to further refine and customize their looks by using the F6 shortcut you will be able to bring up the Modify window, in this window you have access to tools and sliders to alter your character in detail.\
The tab you need is labelled “Morphs”, in this tab you will find various useful sliders, these offer you a accurate way of designing your character, alternatively you can use your mouse to click and drag body parts of your character to modify them.

There are various methods for navigating this window, the first being the collapsible list located to the left of the window. clicking on any of the listed body parts will refine sliders to ones relevant to that body part.\
You can also search for specific sliders via the helpful search bar located in the top right of the window.\
The last method of refining the list is by selecting body parts on your character the related sliders will show up.

See these tutrorials on [modeling and skeletons](https://courses.reallusion.com/home/character-creator/modeling-and-skeleton)

## Skin & Makeup

Now you have a better shape and look for your character now you can make them look more believable by adding realistic skin detail.\
To start adding these details you need the tab labeled “Skin” located in the Content Manager.. The fastest way to get believable results is to use one of CC3s full skin presets; you should have a preset for females and one for males.\
In the Content Manager window (F4) , move to the “Makeup” tab and you will have a lot of creative options to fully customise your character's makeup as well as some presets.

Both the Skin and Makeup presets add customizable layers to your character, these can be located in the CC3 skingen Editor,\
The skingen editor can be located in the Modify window under the appearance tab and used by ticking the Checkbox.

Note: you will need to deactivate the skingen editor when you are finished editing the layers.

For further information see this tutorials on [skin and makeup](https://courses.reallusion.com/home/character-creator/skin-and-makeup).

## Hair

To add hair you will need to return to the content manager window and find the labeled tab “hair”.\
In CC3 you are not given a lot of hairstyles by default but you will have a choice of a small selection here which you can simply drag and drop onto your character or add by double clicking.

### **Changing hair hair colour**

**Legacy:**

Use your mouse cursor to select the piece of hair you want to change the colour of on your character.\
In the Modify window “F6” you need to go to the “Materials” tab\
Underneath the Texture Settings there will be an image labeled “Base Color”, to edit this you will want to right click it and go to “Adjust Color” this will bring up a small window where you can edit the colour of the hair.

**Smart Hair:**

Use your mouse cursor to select the piece of hair you want to change the colour of on your character.\
In the Modify window “F6” you need to go to the “Materials” tab.\
Expand the “Shader Settings” and then scroll to “Base color Map Strength”

In this section you will find a list of collapsable sections to customise your characters hair colour\
from strand colour to highlights.

If your character's hair is broken up into multiple pieces and you want to copy the colour across them all.\
Make sure you have the piece of hair that you want to keep copy the colour from\
At the top of The Materials page underneath the section labeled “Material List” there is a button called “Copy Shader Parameters”, press that button.\
Now select your other pieces of hair and in the same section there is a button named “Paste Shade Parameters” that will copy the exact colour and shader parameters over.

See these tutorials on [hair and eyebrows](https://courses.reallusion.com/home/character-creator/hair-bread-and-eyebrow):

**Shader Issues**

Character Creator exports its puppets with a transparent shader for hair. This can result in different layers of the hair looking wrong particularly at some viewing angles.

You can improve this by finding changing the render mode for the hair materials:

Find the hair materials - they are usually in the Materials folder inside the FBX file you imported for the character.\
Select each hair material (typically named "Hair\_Transparency\_x\_Pbr") and, in the Inspector panel, change the Rending Mode from Fade to Cutout.

## Clothes & accessories

All the clothes and accessories are located in two tabs in the Content Manager window, appropriately named Cloth and Accessory.\
All items you have installed will show in these two tabs and are a simple drag and drop to apply.

See these tutorials on [cloth & outfits](https://courses.reallusion.com/home/character-creator/cloth-and-outfits).

### **Single Sided Clothing**

Another common problem is clothing where you can often see through the 'inside' of a costume.

This can be fixed by replacing the shader of clothing materials with a double sided shader:

Select the material(s) you want to fix in the Materials folder.\
In the Inspector panel, change the Shader from Standard to Standard-DoubleSided.

### **Hiding Meshes**

Hiding meshes not only reduces the amount of data you are exporting but prevents unnecessary clipping when you later when you start to move and act with your character.\
This can be done quite quickly in CC3 using the “auto hide mesh” function.

To find it :\
Select on a piece of clothing\
Click Conform on the top toolbar\
Then open up the “Cloth layer Settings” In the bottom right of your screen (by default)\
It will open up a small window and you want the button that says “Auto Hide Mesh”

What it does is hides any meshes that are being covered up by another mesh on top of it.\
This can be further adjusted manually by using the edit mesh function of CC3

See this on [fixing visual defects](https://courses.reallusion.com/home/character-creator/cloth-and-outfits?v=character-creator-3-tutorial-fixing-visual-defects-part-1-mesh-editing).

## Exporting

When you are pleased with your character and ready to export it to unity, make sure you save a project file first by using the shortcut Ctrl+S or by navigating the file menu in the top left of the CC3 window.

To correctly export your character for Unity navigate through the File menu by goin **File > Export > FBX(Clothed character)**, this will bring up the Export window.\
In the Export window make sure that the “Target Tool Preset” is set to Unity 3D at the top of the window and “Delete Hidden Faces” is checked in the bottom of the window.

You are ready to Export.

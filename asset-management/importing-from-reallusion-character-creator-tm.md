# Importing from Reallusion Character Creator™

This guide assumes you have already [set up Unity and the Asset Importer project](https://firststage.moviestorm.co.uk/knowledgebase/set-up-unity/) so you can import assets into FirstStage.

### Install the Unity Plugin

First of all, we will need to download and install the [Unity Plugin from Reallusion](https://www.reallusion.com/character-creator/unity-auto-setup.html).

Then we need to import that into our Unity project (following the [instructions here](https://manual.reallusion.com/CC\_and\_IC\_Auto\_Setup\_Plugin/ENU/CC\_and\_iC\_Auto\_Setup/1.0/03\_for\_Unity/Installing\_CC\_Auto\_Setup\_to\_Unity.htm)):

1. Open up the Unity Asset Importer project.
2. In Unity, go to the Assets menu and select Import Package...
3.  Choose the path where the Reallusion unity plugin was installed - by default:

    C:\Program Files\Reallusion\Shared Plugins\Auto Setup\Unity\AutoSetup 1.1 for Unity 2019.3
4. Select the **3D** package in that folder to import.
5. You should now have a folder named "CC\_Assets" in your Unity Project.

### Export from Character Creator

Follow the [instructions here](https://manual.reallusion.com/CC\_and\_IC\_Auto\_Setup\_Plugin/ENU/CC\_and\_iC\_Auto\_Setup/1.0/03\_for\_Unity/Unity\_Importing\_Character\_FBX\_File.htm) to export a character suitable for import into Unity:

1. Create your character in Character Creator.
2. Go to the File > Export > FBX (Clothed Character) menu.
3. In the export wizard make sure you set the Target Tool Preset to Unity3D.
4. Click the Export button to export the character into a custom folder.

### Import the Character into Unity

1. Inside Unity, open up the CC\_Assets folder in the Project view.
2. Drag and drop the folder containing the exported character (from the previous step) into the CC\_Assets folder.
3. Unity will now do some processing which will take a short time to import the models and materials.
4. Inside that folder you should now find an FBX object for you character.
5. Drag and drop this into the default scene to check that it has imported correctly.

You may also find [this guide](https://magazine.reallusion.com/2018/12/13/character-creator-3-tutorial-exporting-cc3-base-characters-to-unity/) helpful for solving issues arising from exporting into Unity as well as [this forum thread](https://forum.unity.com/threads/character-creator-3-tutorial-part-1-exporting-a-cc3-character-base-to-unity.599911/).

### Rig the Character for FirstStage

We need to do just a little packaging to prepare the character for use in FirstStage:

1. In the root of the scene hierarchy, create an Empty gameobject (right click menu) and name it suitably. This will be the container for the character and its name will be used inside FirstStage.
2. Drag and drop the FBX object of the imported character inside this gameobject.
3. Select the container object in the hierarchy view and from the Inspector view, Add Component and look for the Puppet Setup component.
4. The main property to set in the Puppet Setup component is the height if your character is not 'normal' sized.
5. Finally create a prefab for your character by dragging the container object into a folder in your Project Assets.The folder should be suitably named - perhaps simply "Reallusion" to reflect its source.

### Export the Character to FirstStage

We can now export the character to FirstStage:

1. Select the prefab you just created in the Project view.
2. Open the FirstStage Repository view (Moviestorm > FirstStage Repository if not already open).
3. Press the Import button and you should then see your new character appear under the Pending folder.
4. Select your character in the Pending folder and give it the "Character" tag in the right hand panel.
5. Make sure the LOCAL repository is selected and then press the Commit button.
6. If you now start FirstStage, you should find your new character in the Asset browser by selecting Project Assets on the left.
7. If you are happy with the character, you could then choose a specific project and upload it to the cloud for everyone else working on the project to use.

### Common Issues

#### Hair

Character Creator exports its puppets with a transparent shader for hair. This can result in different layers of the hair looking wrong particularly at some viewing angles.

You can improve this by finding changing the render mode for the hair materials:

1. Find the hair materials - they are usually in the Materials folder inside the FBX file you imported for the character.
2. Select each hair material (typically named "Hair\_Transparency\_x\_Pbr") and, in the Inspector panel, change the Rending Mode from Fade to Cutout.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

#### Single Sided Clothing

Another common problem is clothing where you can often see through the 'inside' of a costume.&#x20;

This can be fixed by replacing the shader of clothing materials with a double sided shader:

1. Select the material(s) you want to fix in the Materials folder.
2. In the Inspector panel, change the Shader from Standard to Standard-DoubleSided.

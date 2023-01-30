# Importing a Ready Player Me avatar

This guide assumes you have already[ set up Unity and the Asset Importer project](https://firststage.moviestorm.co.uk/knowledgebase/set-up-unity/) so you can import assets into FirstStage.

### Install the Unity Plugin <a href="#_1ouuwpdgc1ma" id="_1ouuwpdgc1ma"></a>

Download the[ Ready Player Me SDK from here](https://bit.ly/RPM-Unity-SDK-Latest).

In Unity, install the package by going to Assets > Import Package > Custom Package

### Import the RPM Avatar into Unity <a href="#_5y2creowr3lh" id="_5y2creowr3lh"></a>

The avatar will come as a .glb file. Drop this into a folder in the Unity Editor Project view.

It should now show as a package in Unity containing meshes and materials.

### Set it up as a Character <a href="#_m2a9g55kiox6" id="_m2a9g55kiox6"></a>

In the Scene Hierarchy view, create an Empty Gameobject to use as container for your character. Change the name to the name you wish to use for this character.

Drag and drop the RPM avatar from the Project folder into the Hierarchy view and into the container object created earlier.

Right click on the avatar object and select Unpack

Add a PuppetSetup component to the container object.

Add an Animator component to the RPM avatar in the container and then configure it:

* Click in the Avatar box in the Animator component and select either FemaleAnimationTargetV2Avatar or MaleAnimationTargetV2Avatar

Create a new GameObject under the avatar object and call it Armature (must be spelled precisely this). Drag the Hips game object and put it in the Armature folder.

Drag the container object from the Hierarchy view to a folder in the Project view.

Your hierarchy should now look like

Container

Avatar

Armature

Hips

Wolf3D\_Body

etc...

### Commit to First Stage Repository <a href="#_bmw6upljvcuf" id="_bmw6upljvcuf"></a>

You can now import this into the First Stage Repository.

As usual, we advise you commit it to LOCAL and check that it is working correctly before pushing to the cloud.

### Method 2: Automatic Import <a href="#_9qff0vgj8bqf" id="_9qff0vgj8bqf"></a>

* Drag the RPM avatar from the Project view into the Scene Hierarchy view.
* Select this object in the Hierarchy view.
* Go to the menu Ready Player Me> Prepare {Male|Female} RPM Avatar as FirstStage Puppet
* You should now have a new top level object “Puppet” in the Hierarchy view and, if you expand that object, you will see the original avatar inside it.
* Rename the Puppet with the preferred character name.
* Drag the Puppet from the Hierarchy view into a suitable folder in the Project view, creating a prefab.
* This prefab can now be imported into FirstStage.

# Example - Unity Scene Import

## Downloading and importing from the Unity Asset Store

From the Unity Editor, download and import the scene asset.

[Source assets and import > 2. Import to the Unity Editor](https://firststage.moviestorm.co.uk/asset-management/1-source-assets-and-import/)

First, lets get organised and rename the Asset root folder from ‘Assets Main Folder’ to ‘PIOPIS’ (the Publisher’s name) to help with identification later on.

[Prepare for FirstStage > 1 - Organise the folder scheme](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

We will be making changes to the scene, so it is worth retaining the original by taking a copy of the ‘restaurant’ scene file in ‘Assets > Sample scene’ and putting it in the Asset root folder (PIOPIS). Open the newly copied scene to view and check for any obvious visible issues.

[Fixing common issues >](https://firststage.moviestorm.co.uk/asset-management/5-fix-common-issues/)

You should also check the Console window for errors when it loads. We cannot possibly anticipate what errors could occur and how to deal with them, but do recommend Googling the error message for guidance.

### Preparing the asset

#### Set the Floor layer

FirstStage needs floor geometry marked to allow users to teleport onto it and for characters to walk on it. Unity does this by putting objects into different layers.

Firstly, we need to locate the assets that make up the floor. Fortunately, the Restaurant assets are well named and organised by type, making it much easier to identify and select the floor objects by searching for “floor” in the Hierarchy window, which seems to locate all the floor tiles.

Selected, in the Inspector view, change the Layer to Ground. When the Unity Editor asks whether it should do this for children also, click Yes.

We also want to make stairs walkable on so select those (easiest is to seach for “stair”) and change the Layer to Ground on them also.

[Prepare for FirstStage > 3. Setting floor layers](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

#### Remove existing cameras

Example scenes often have a Player GameObject (often named ‘Player’ or ‘Controller’) to demonstrate the scene. If your scene has an obvious player object, or a camera rig, these objects should be removed as they will conflict with FirstStage when loaded.

[Prepare for FirstStage > 4. Remove existing cameras](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

#### Set the inital spawn point

In the scene root, create an empty game object called "LOCAL\_USER”. Place it at ground level where you would want to enter the scene.

[Prepare for FirstStage > 5. Set the inital spawn point](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

#### Test the scene

Open the FirstStage Repository view if it is not already open and make sure the LOCAL project is selected while we are testing the scene.

Select the scene asset in the Project view (you can jump to it from the Scene Hierarchy by right clicking on the scene name).

Press the Import button in the FirstStage view. You should now find your scene listed under the Pending group.

You can add a description to your scene to help when listing them in the FirstStage Office: select the scene and add a description in the right hand panel.

Now press the Commit button. The Unity Editor will freeze and pause briefly while the asset bundle is created.

Check the Console view in case any errors show up.

[Export to FirstStage](https://firststage.moviestorm.co.uk/asset-management/3-export-to-firststage/)

Now launch FirstStage and go to your project and create a new scene: the new stage (in our case, Restaurant) should appear in the list of available stages.

Once on set, you can have a look around and see how well it is working. You may find objects you missed when setting the floor layer.

[Test in FirstStage](https://firststage.moviestorm.co.uk/asset-management/4-test-in-firststage/)

#### Import supporting assets

What you will notice is that the props in the scene (e.g., tables, chairs) can not be interacted with: moved, deleted, etc. At this point they are just static set dressing.

To make the props interactive, we need to go back to the Unity Editor and import any supporting assets that we will want to interact with. This has the additional advantage of those assets to be placed on other stages as well.

Well organised packages will have their assets organised and typically there is a folder “Prefabs” and, in the case of the Restaurant package, there are several such folders organised by category.,

Most props can be imported without any further ceremony if they are just set dressing with no additional behaviour.

Select all the prefabs you want to import (do them in batches if easier) and press the Import button in the FirstStage repository view.

Note that some of the prefabs may be part of the construction of the building and background — walls, floors, etc., — we don’t usually want to manipulate these and so are best omitted from the import.

When we are happy with our collection of prefabs to import, press the Commit button.

We might also want to add some tags to our new assets to make them easier to find inside FirstStage.

[Prepare for FirstStage > 3. Extracting Assets from Scenes > 1. Separate and import Scene assets](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

#### Identify stage things

Now the prefabs are in the repository, we can identify all the game objects in the scene that are from an asset prefab so that FirstStage can work with them.

Simply select the menu option Moviestorm > Identify Stage Things

[Prepare for FirstStage > 3. Extracting Assets from Scenes > 2. Identify Stage assets](https://firststage.moviestorm.co.uk/asset-management/2-prepare-for-firststage/)

#### Test the scene with separate assets

Now we need to import and commit our scene again.

Launch FirstStage again and go back to the scene you created previously. You should now find that you can select and grab things in the scene which are instances of the assets you just imported.

We are now free to dress the set as we want it: removing things we don’t want, moving things where we do want and adding more things out of the asset repository.

[Export to FirstStage > 4. Save to your local FirstStage repository](https://firststage.moviestorm.co.uk/asset-management/3-export-to-firststage/)

#### Commit to the cloud

If you want anyone else in your project team to use this set or any of the assets you’ve imported, you need to commit them to the cloud.

In the Unity Editor, FirstStage repository view, change the Project from LOCAL to the one you are working on and then press the Commit button.

Again Unity will freeze as it builds the bundles, and it will take a bit longer this time as it has to upload the asset bundles to the server.

[Share in FirstStage > Make the asset available for remote collaboration](https://firststage.moviestorm.co.uk/asset-management/6-share-in-firststage-cloud/)

#### More improvements

Once you start working on the scene, you may find more changes you need to make to the base set. In which case you can just repeat the above process. Always test changes in the LOCAL repository first and only commit to the cloud when it is working.

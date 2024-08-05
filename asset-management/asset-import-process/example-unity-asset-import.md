# Example - Unity Asset Import

In this example we’ll import a single asset as an example, but most of the procedure applies to any scene.

Follow the links after each instruction for a more detailed guide.

#### ![](https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Old-Coin-asset-300x225.png)

## Preamble

Suppose you are blocking out a script that calls for a special coin for the lead character: it’s just a McGuffin so we could use almost anything as a stand-in, but perhaps we want something better for a specific sequence where the camera tracks a coin toss.

Since there isn’t anything in the public asset repository (at least at time of writing - we’re expanding it all the time), we need to find a model that we can import. There are several places we can look for a model such as [TurboSquid ](https://www.turbosquid.com/)which often has suitable assets but the first place we usually look is the [Unity Asset Store](https://assetstore.unity.com/) itself which has the advantage of having assets in the right format and easy to import.

And indeed, we find a model of an [Old Coin](https://assetstore.unity.com/packages/3d/props/old-coin-49530) in the asset store which will do the job just fine. Even better this one happens to be free!

#### Downloading and importing from the Unity Asset Store

So now we can download the asset directly from within the Unity Editor and import it into our Asset Importer project. Installing large asset packages may take some time. You should check the Console for any errors but hopefully there won’t be any.

Now that we’ve imported the asset, it should be visible somewhere in the Projects view of the Unity Editor. In this case we find it under Assets as “Japanese Coin”.

[Source assets and import > 2. Import to the Unity Editor](source-assets-and-import.md#import-into-the-unity-editor)

#### Preparing the asset

It is worth giving a little thought at this point to the naming of the asset. Generally the top level folder should be something that identifies the publisher or author. In many cases you would use the name of your organisation, but here we’ll create a new folder “Gnarly Potato” and move Japanese Coin into it.

[Prepare for FirstStage > 1.1 - Organise the folder scheme](prepare-assets-for-firststage.md#organise-the-folder-scheme)

When importing a 3rd party asset, you’ll usually be looking for some demo or example prefabs to start from. Often you’ll need to create some objects in the sample scene so you can rig them up and create prefabs suitable for FirstStage by dragging the completed game object(s) into a Project folder. You may be asked to create either an Original Prefab or a Prefab Variant: choose Original Prefab if you’re not familiar with Unity and how prefabs work.

[Fix common issues > 2 - Missing asset prefabs](fix-common-issues.md#id-2.-missing-asset-prefabs)

In this case, there is an example scene with an example game object for a single coin and for a pile of coins. However the material is broken and seems to have lost its textures. This is easy to fix (but occasionally tedious): select the broken material (in this case DefaultMat) and there are some textures in the same folder as the material with obvious names that can just be dragged and dropped on the corresponding slot in the material.

[Fix common issues > 1 - Textures](fix-common-issues.md#id-1.-textures)

We now drag the game object for the coin and for the pile of coins into the Japanese Coin folder creatiing prefabs. You might want to make sure they are clearly named at this point.

[Fix common issues > 2 - Missing asset prefabs](fix-common-issues.md#id-2.-missing-asset-prefabs)

#### Exporting the asset to FirstStage

Now we are ready to export it into the repository. As discussed on a previous page, summon the FirstStage repository view and make sure the LOCAL project is selected to start with.

[Export to FirstStage > 1. Select the target asset repository](export-to-firststage/#select-the-target-asset-repository)

Select the prefabs you have just created in the Project view and press the Import button in the FirstStage view.

[Export to FirstStage > 2a. Import the asset prefab files](export-to-firststage/#import-asset-prefabs)

You should now find entries for those prefabs in the Repository Pending list (you may have to expand some folders to find them). Select each asset in turn and add some tags to help us find it in the repository later on. In this case, we’ll just set them both to Prop.

[Export to FirstStage > 3. Add tags and a description](export-to-firststage/#add-tags-and-a-description)

Next we can commit the assets to the local repository by pressing the Commit button. Unity may now freeze for a while as it builds the asset bundle. Check the Console afterwards in case any errors were reported as this will avoid surprises later.

[Export to FirstStage > 4. Save to your local FirstStage repository](export-to-firststage/#save-to-firststage-repository)

#### Testing the asset in FirstStage

And now we can fire up FirstStage and we should find our new assets in the Asset Browser. If you can’t find them easily, select Project Assets from the left hand column to narrow the search.

And we very quickly find a problem with our new assets: the coin is 1.5m in diameter! In this case, this is easily fixed by checking the scale of the game objects and setting them to one.

[Fix common issues > 3. Scale, position and rotation](fix-common-issues.md#id-3.-scale-position-and-rotation)

So we select our updated prefabs and hit the Import button again. Note that the asset properties are remembered from the previous version so we can hit the Commit button to rebuild the asset bundle.

[Export to FirstStage > 4. Save to your local FirstStage repository](export-to-firststage/#save-to-firststage-repository)

Our new assets are now working fine and for something as simple as a coin we do not need to do anything else. However, at the moment you are the only one who can see them. This is fine if you are working on your own but if you are working with other team members you should finish by uploading the new assets to the FirstStage Project that you are working on.

#### Making the assets available for remote collaboration

To share the new assets for collaboration, go back to the FirstStage view in the Unity Editor and change the Project from LOCAL to whichever project you are working on (in my case it was the imaginatively named “Fight Scene”).

Now select the new assets as before and press the Import button and then the Commit button. This time the process will take longer as the asset bundle must be uploaded to the server and so will depend on your bandwidth.

And there we are! A new asset successfully imported into FirstStage!

[Share in FirstStage > Make the asset available for remote collaboration](share-in-firststage-cloud.md#make-the-asset-available-for-remote-collaboration)

Once you are comfortable importing simple props, we will look at some trickier cases…

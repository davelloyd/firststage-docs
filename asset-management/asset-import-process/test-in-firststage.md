# Test in FirstStage

As part of the import process, apart from reviewing the Asset or Scene in the Unity Editor, we recommend a more careful scrutiny within FirstStage itself before committing anything to a cloud project repository to share with others in your project production team

After you Export to FirstStage out of the Unity Editor, we suggest you launch FirstStage and undertake the following checks.

### Assets

Create and enter an Empty Set Scene.

Imported new Assets should be found in the Asset Library and placed on set to review.

#### Check the textures look correct

Lift each Asset up and view them from all angles and lighting conditions to ensure the textures are all correct. Use a Scene light source to check expectations for the types of texture map, as appropriate:

* Missing **Texture** map - Are there any flat grey textures?
* Missing **Specular** map - Does it shine correctly
* Missing **Normal** map - Is there no surface detail, such as bumps, grooves, and scratches that catch the light as if they are represented by real geometry?
* Missing **Cube** map - Are there no reflections?
* Missing **Alpha** map - Are there transparencyproblems?
* Missing **Detail** maps - Is the texture blurry when looked at closely?

#### Check the Assets look correct in the Asset Library

Here you can test for:

* **Scale** - Does it look the correct size
* **Orientation** - Is it the correct way up?
* **Position** - Is the Asset rotating around it’s centre?

#### Check the Assets are Tagged correctly

1. Can you find the Asset within Tags that you would expect to?\
   If no Tags have been added, the Assets will be in the root of the Asset Browser and not within any expected Tag filters.
2. Are there now very similar Tags?\
   This can happen when not matching an existing Tag exactly when adding them. That is why we provide a recommended [Asset Tag taxonomy](export-to-firststage/asset-tagging.md) as a starting point to keep things consistent and sensible. Having found a close duplicate, will need to go back and change that Asset’s Tag and re-import to remove the erroneous Tag from the Asset Browser.

_NB - A close look at 3d Asset sources on the internet will see that there is little consistency, and often taxonomies can be missing obvious Tags, or have very similar Tags, which are both a sign of a lack of planning that can come back to bite you if you expect to have a lot of Assets in your Asset Library._

### Scenes

Imported Scenes will be available within FirstStage as a new Stage.

Within your Project, create a new Scene using the new Stage and enter the Scene.

#### Check the ground is defined correctly

Teleport your way around the scene to check that all appropriate surfaces are set up correctly.

#### Check Assets have been separated from the Scene

If it is an imported Scene where you have additionally separated and imported selected Scene assets, check that all expected Assets in can be moved.

**If you find any issues, you will need to go back into the Unity Editor and fix the issues, then re-export LOCAL to check.**

# Importing from SketchUp

Unity can import SketchUp files directly and is very easy to use:

1. Start Unity with the Asset Importer project.
2. Create a folder with a suitable name under Assets in your Asset Importer project
3. Copy your SketchUp file into this folder.
4. Select your file and look at the Inspector panel. (Example image on the right)
5. You may need to check "Generate Back Face" if your model seems to be missing faces.
6. If you have any cameras in your scene, make sure you uncheck "Import Cameras" as these might cause conflicts.
7. If the scale of the model appears wrong, you may need to adjust the "Unit conversion" parameter.
8. In many cases, your model will now be ready.
9. Create an empty scene to test your model.
10. Drag the sketchup file from the Project view into the Hierarchy view or the Scene view.
11. You should now see your model in the Scene view.
12. You can make further changes to your model now: you might want to add or change materials, etc. See other guides for how to do this.
13. As SketchUp is often used for architectural models, you should select any meshes that you might want to walk on and change their layer to Ground.
14. Once you are happy with your model, save it as a new prefab by dragging it from the Hierarchy view into your folder in the Project view.
15. You are now ready to test this by [committing it to the local repository](https://firststage.moviestorm.co.uk/knowledgebase/4-test-in-firststage/).

Further details about using Unity's SketchUp importer can be found [here](https://docs.unity3d.com/Manual/class-SketchUpImporter.html).

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption><p>Example import settings</p></figcaption></figure>

### Importing as a Scene

SketchUp is often used to model buildings and environments. For these, it is often more appropriate to import a whole scene which can then be used as a stage inside FirstStage.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>Example stage imported from SketchUp</p></figcaption></figure>

In this case, you can just take the scene you created earlier to test the model in and give it a memorable name and import the whole scene:

1. Select the scene in the Project view
2. Go to the FirstStage view
3. Click Import.
4. Make sure the Local repository has been selected as destination while we're testing it.
5. Click Commit.
6. It should now be available inside FirstStage.

You might also find the guide on [importing scenes](https://firststage.moviestorm.co.uk/knowledgebase/example-2-unity-scene-import/) helpful.

# Share in FirstStage (Cloud)

![](https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/FS-asset-import-flowchart-6.png)

This guide is only required for those working in teams and needing to share imported Assets and Scenes with others.

_NB - Due to the time and cost of uploading, we fully recommend that you always_ [_test Assets and Scenes in your LOCAL repository first_](https://firststage.moviestorm.co.uk/asset-management/4-test-in-firststage/)_, and only commit to your cloud repository when issues are fixed._

### Make the asset available for remote collaboration

If you previously imported the assets to a LOCAL repository, and are happy that the assets look right and are behaving correctly, you may now want to share them for collaboration. To do this they will need to be moved to a shared cloud project repository.

![](https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Restaurant-Share-in-FirstStage.jpg)

1. In the FirstStage window, change the Project from LOCAL to the target cloud repository
2. Select the prefabs just created in the Project window and click the Import button in the FirstStage window. _**- HOW DO I FIND THEM ALL? FOR SCENES, THEY WILL BE THE SCENE ITSELF PLUS ALL THE PREFABS THAT COULD BE ORGANISED INTO FOLDERS?!!**_\
   The assets will now show under Pending in the FirstStage view.
3. Click the Commit button in the FirstStage window.\
   Unity will freeze whilst it builds the asset bundles and transmits them to the cloud repository. This process will likely take longer (depend on your bandwidth) than commiting them to a LOCAL repository, as the asset bundle must be uploaded to the cloud server.

**The new assets should now be available to use collaboratively in FirstStage.**

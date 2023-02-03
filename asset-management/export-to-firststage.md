# Export to FirstStage

![](https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/FS-asset-import-flowchart-3.png)

This guide will illustrate how to

1. Select the target asset repository
2. Import the Asset prefabs and Scene files
3. Add tags and a description
4. Save to your local FirstStage repository

### 1. Select the target asset repository

1. Open the FirstStage window (from the menu bar > Moviestorm > FirstStage Repository)
2. Select the desired Project (from the top multiple select button aligned with ‘Project:’)\
   NB - We recommend the LOCAL project to test out assets before sharing them with others, as it is faster when the assets do not need to be sent to the server
3. Close OR Dock the FirstStage window\
   We would recommend docking the FirstStage window into the Unity Editor of ease of use going forward. Drag the FirstStage window by the tab over the tabs of the Console window

### 2a. Import the asset prefab files

To import single assets, we select and import the asset prefab file.

1. Select the prefabs just created in the Project window and click the Import button in the FirstStage window.\
   The assets will now show under Pending in the FirstStage view.

### 2b Import the scene file

To import whole scenes, we select and import the scene file.

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Restaurant-Import-the-scene-to-LOCAL.jpg" alt=""><figcaption><p>2b.1 – FirstStage Repository – Scene pending</p></figcaption></figure>

1. Select the scene asset in the Project view and click the Import button in the FirstStage window.\
   _NB - Jump to it from the scene Hierarchy window by right-clicking on the scene name and clicking ‘Select Scene Asset’ from the drop down._\
   The scene will now show under Pending in the FirstStage view.

### 3. Add tags and a description

Tags will help locate assets when using the Asset Browser in FirstStage, by allowing filtering by tags.

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Coin-Adding-Tags-and-Description.jpg" alt=""><figcaption><p>3.2 - Add tags and description</p></figcaption></figure>

1. Expand the new asset pack in the FirstStage window Pending section
2. Select an asset and the information about that asset will be shown.\
   Add tags in the Tags field, separated by commas.\
   We provide a Asset Tagging guide that you would be welcome to use. For example, for the Japanese Coin, suitable tags could include ‘Prop’, ‘Non-food items’ and ‘Accessory’.\
   Add a description in the Description field. This may help with future word-based searches.
3. Click Save

### 4. Save to your local FirstStage repository

When you are ready

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Commit-to-repository.jpg" alt=""><figcaption><p>4.1 - Commit to the FirstStage repository</p></figcaption></figure>

1. Click the Commit button in the FirstStage window.\
   This will build the asset bundles and transmit them to the repository. As a result, Unity may now freeze for a while.

Check the Console afterwards in case any errors were reported as this will avoid surprises later.

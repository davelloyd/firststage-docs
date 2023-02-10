# Source assets and import

![](https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/FS-asset-import-flowchart-1.png)

This guide will illustrate how to source assets and import them into the Unity Editor to prepare for export to your FirstStage repository:

* Unity Asset Store
* Sketchup
* 3DS Max & Maya

## Unity Asset Store

To help illustrate this process, we have used the free [Old Coin](https://assetstore.unity.com/packages/3d/props/old-coin-49530) asset in the Unity Asset Store.

### Acquire the asset

Log in to the Unity Asset Store website.

As a free item, instead of ‘Add to Cart’ and having to go through the purchase process, it already displays the ‘Add to My Assets’ button. Click this and it is yours.

<figure><img src="../../.gitbook/assets/image (15) (1).png" alt=""><figcaption></figcaption></figure>

### Import into the Unity Editor

We can download the asset directly from within the Unity Editor and import it into our Asset Importer project.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

1. Open the **Package Manager** pane if it is not already: Window > Package Manager
2. Make sure you have **My Assets** selected in the top left **Packages** dropdown.
3. Find the asset you want to import and select it in the left hand pane.
4. The right hand pane will now show the asset details.
5. Click on the **Download** button on the bottom right.
6. This will be replaced by an **Import** button once the asset has been downloaded: click this to import.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Installing large asset packages may take some time to process. Once complete, you will now see the asset package listed in it’s own ‘Japanese Coin’ folder in the Project window (bottom left as standard).

{% hint style="info" %}
&#x20;You should check the **Console** window (bottom right as standard) for any errors. Most may be harmless but if there are problems with the assets, this is the first place to check.
{% endhint %}

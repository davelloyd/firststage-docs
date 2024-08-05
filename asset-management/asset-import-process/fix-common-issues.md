# Fix common issues

You are most likely to find issues with an asset that is already in FirstStage, as there is nothing like scrutinising an object from all angles in VR to check whether it is fit for purpose, but you may find issues in the Unity Editor as you personally [import an asset](./).

If they are 3rd party assets issues can be commonplace, as not every 3d artist that publishes assets will set them up in the same way.

Below is a list of common problems and a guide as to how they might be fixed.

* Missing textures
* Missing asset prefabs
* Scale issues
* Position issues

### 1. Textures

If an asset previewed in the sample scene appears flat grey, it is missing texture maps, so you will need to add the correct materials to the GameObjects.

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Coin-Fixing-textures.jpg" alt=""><figcaption><p>1.2 - Drag materials over Main Map slots to fix textures</p></figcaption></figure>

1. Inspect the DefaultMat material in the Project window (Japanese Coin > Materials > DefaultMat) to open it in the Inspector.
2. Drag the material maps (beginning with ‘deerka\_DefaultMaterial\_’) over the corresponding empty slots in the Inspector window, under ‘Main Maps’. There are three:

* '\_AlbedoTransparency' to Albedo
* '\_MetallicSmoothness' to Metallic
* '\_Normal' to ‘Normal Map’

The assets should not appear to be textured correctly.

### 2. Missing asset prefabs

A Unity Prefab Asset acts as a template from which you can create new prefab instances in the Scene. As a result, not all assets will require a prefab. E.g.

* Plate, knifes, fork and spoons would all want a prefab, so you can create table settings and be able to interact with each of the things on the table.
* A table with a number of settings may want a prefab, so that you can easily place lots of tables with settings around an empty restaurant.
* A complete restaurant would not want a prefab, as generally there will only be one set required for that.

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Coin-Creating-Prefab-Set-up-2.jpg" alt=""><figcaption><p>2.1 - Drag the GameObjects</p></figcaption></figure>

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2020/10/Unity-Editor-Coin-Creating-Prefab-2-Prefab-check-box.jpg" alt=""><figcaption><p>2.2 - Choose the type of prefab</p></figcaption></figure>

### 3. Scale, position and rotation

It is best not to change these settings before the asset has been imported and checked in FirstStage. Issues with these should be obvious when selecting the assets in the FirstStage Asset Browser, or when they are seen in context with the rest of the scene on set.

#### 1. Scale

Objects will be at the scale that the artist used, which could be based on any measurement system or scale, e.g. feet, inches, metres, centimetres, etc.. So often this issue will arise after it has been imported and viewed in FirstStage which uses one metre as a basic unit.

Generally, set the scale to 1 across all axis in order to get the asset to the original unit size. But if that does not correct it, you can use the Measure tool or the one metre floor grid in the Empty Set in FirstStage to establish how big the asset is. Divide that number by what that measurement should be, and then put that figure into each of the Scale fields. E.g. If the artist built a one metre cube with their scale set to feet and inches, the cube would be 3.28 units, which when brought into FirstStage would be 3.28 metres in size, so if the scale is set to 0.305 (1 / 3.28), it should appear as a one metre cube in FirstStage.

#### 2. Position

Most objects should be positioned at 0,0,0, unless they are meant to sit above or below ground, or be offset for some reason. E.g. A ground access hatch would want to extend downwards so that you can set the cover on the ground and the model extends beneath.

The key here is ease of use when placing an object, and that means point where you want it to go, and it is orientated correctly. However, it is very simple to move objects about in FirstStage, so unless you’ll be placing a lot of them, it is not something to worry about.

#### 3. Rotation

You might expect assets to orientate themselves so that they are correct when selected to place on set. E.g. It would be annoying if a car always arrived on it’s side.

The key here is to have the rotation set to the main axis, so that when placed the asset will align correctly with the world, and not require fiddly adjustment.

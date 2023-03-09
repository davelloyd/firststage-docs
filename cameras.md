# Cameras

FirstStage provides a powerful camera system. Cameras can be easily created with the Viewfinder and then animated with complex motion paths. Cameras can automatically look at targets and follow targets (the two targets do not need to be the same).

You can create cameras by going to the [Asset Library](basics/asset-library.md) and choosing the **Basic Camera** but the best way to create cameras is usually to use the Viewfinder:

{% content-ref url="basics/core-tools/viewfinder.md" %}
[viewfinder.md](basics/core-tools/viewfinder.md)
{% endcontent-ref %}

## Tracking Behaviour

The body of the camera can be attached to another thing and it will then follow that thing.

By default, a camera will follow its target rigidly: for example a security camera attached to a moving bus. But it does not need to: you can choose from a behaviours from rigid lock to a simple follow. You can also set the damping time on the motion to get a smoother camera path.

You can attach a camera by using the **Attach** handle available on the [Inspect Menu](basics/working-with-things/#inspect-menu). You can also set a camera to follow its Look Target.

<figure><img src=".gitbook/assets/Follow Test 2023-02-26 21-30-10.jpg" alt=""><figcaption></figcaption></figure>

## Look Behaviour <a href="#_enjm7xrw1oa7" id="_enjm7xrw1oa7"></a>

When a camera has a look target and that target moves, the camera will track the target if the target moves too far from the original position in the field of view. When the target moves a little too far, the camera will track softly as if on a spring. But when the target tries to move outside the camera’s field of view, the camera will track hard to ensure the target remains visible.

You can set how tightly the camera tracks its target.

The look target is recorded with a look keyframe allowing a shot that doesn’t start tracking until a given time or a shot that stops tracking at a certain point. You can also have shots that hand over from one target to another.

Note that if the camera has a look target, it is applied after the body follow behaviour.

## Cameras on the Wristpad <a href="#_yjzp7fnhledc" id="_yjzp7fnhledc"></a>

Go to Cameras on the Wristpad to view all the cameras in the scene.

All the cameras in the scene are shown in a column on the left. Click on a camera to show it in the main panel.

You can click on the main panel to enter the TTL space for that camera.

If you click the **Inspect** button on a camera, it will take you to the Cameras panel with that camera selected.


# Through The Lens

Point at a camera with the Navigator tool (the default on your off-hand) and you should see an icon popping up over the camera saying Through The Lens. Click and hold for a second to enter the TTL space: here you can adjust your camera framing and work with keyframes to create camera motion paths.

<figure><img src="../.gitbook/assets/Follow Test 2023-02-26 21-31-22.jpg" alt=""><figcaption></figcaption></figure>

## Main Monitor <a href="#_q8gqm9f9bxes" id="_q8gqm9f9bxes"></a>

The main monitor in front of you shows what the camera is seeing.

You can point at something in the camera view and click on it to set it as the **Look Target**. You can clear the look target from the radial menu.

You can also drag the viewpoint by pressing and holding the trigger.

## Timeline <a href="#_r2kuqu3u2p3u" id="_r2kuqu3u2p3u"></a>

Below the monitor is a timeline with three tracks for move, look and lens. You can set keyframes for each of these independently. The camera engine will then interpolate smoothly between these keyframes.

As well as moving keys, you can also hold a keyframe by dragging either end of the keyframe on the timeline: for the duration of the keyframe, that property will not change.

There are also transport controls beneath the timeline allowing you to start/stop and move between sections.

## Camera List <a href="#_cx5ivobs21cd" id="_cx5ivobs21cd"></a>

On the left of the monitor is a list of all the cameras in the scene. If you want to switch which camera you are working with, point at the thumbnail in the list and click on it.

## Nudge Handles <a href="#_d28o6ft5l27i" id="_d28o6ft5l27i"></a>

Immediately in front of you are nudge handles that let you move the camera in a smooth and controlled fashion. If you reach out to a handle, your hand will turn solid and you can grab the handle by holding the trigger.

<div>

<figure><img src="../.gitbook/assets/DUMMY 2023-02-26 20-16-12.jpg" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/DUMMY 2023-02-26 20-16-18.jpg" alt=""><figcaption></figcaption></figure>

</div>

On your left are three arrows which control movement of the camera in each of the three axes: forwards/backwards, up/down and left/right.

If you have a look target set, up/down and left/right will move the camera in orbit around the target rather than in a straight line.

On your right are three circles which control the orientation of the camera in each of three axes: pan, tilt and roll (or dutch tilt).

## Lens Controls <a href="#_uifgw1dilbru" id="_uifgw1dilbru"></a>

Between the nudge handles, there is a panel with sliders to control the focal depth, lens length, and aperture.

Note that if a target is set, the focal depth cannot be changed.

There is also a dropdown to let you choose a post-process profile to be applied to the lens. Post-process profiles let you specify color grading, lens flare and many other effects. The profiles available are taken from the Asset Repository: you can create new ones in Unity and commit them to the repository, after which they will be available for use.

## Following Behaviour <a href="#_6i1r38f850fm" id="_6i1r38f850fm"></a>

If the body of the camera is following another thing, it will show in the left hand panel.&#x20;

A dropdown lets you choose how the camera follows its target:

| Rigid Attach  | The camera will track its target rigidly moving and rotating as if attached to the target.                                                                                                                                                   |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Track         | The camera will maintain the same position relative to the target but will not swing round as the target turns.                                                                                                                              |
| Simple Follow | Mimics a human operator following a target: the camera tries to move as little as possible to maintain the distance and elevation from the target. Unlike the Tracking behaviour, it means that targets can move close and past the camera.  |

The **Damping** slider sets how quickly the camera body tracks the target. At 0, the camera tracks rigidly. Increasing the damping response time slows down how quickly the camera will catch with the target leading to smoother camera behaviour.

The **Cancel Follow** button lets you cancel the follow behaviour.

If you have a Look Target set, the **Follow Look Target** button will show and lets you set the Follow Target to the Look Target.

{% hint style="info" %}
Do not be surprised if the camera jumps when you change the follow behaviour as the camera tries to accomodate the new constraint. Often what the camera thinks is up will change.
{% endhint %}

For further insight, this may help:

{% embed url="https://docs.unity3d.com/Packages/com.unity.cinemachine@2.8/manual/CinemachineBindingModes.html" %}

## Look Behaviour

If the camera head is aiming at a target, it will show in the right hand panel.

The **Slack** slider lets you control how much slack the camera has in maintaining the target position in the view field: zero slack will keep the camera tight on the the target screen position; higher slack will let the target drift around and is usually desirable for more natural camera motion; maximum slack will even let the target drift off the screen altogether.

{% hint style="info" %}
The camera will only drift away from the target when the scene is running: it will always aim precisely when scrubbing time.
{% endhint %}

The **Cancel Look** button will cancel the Look Target.

## Post Processing

You can take advantage of [Unity's Post Processing Stack](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.2/manual/index.html) which provides useful effects such as:

* Auo Exposure & Bloom
* Chromatic Aberration & Lens Distortion
* Color Grading

You can choose from any Post Processing Profiles that have been created in Unity and then Camera List

On the left of the monitor is a list of all the cameras in the scene. If you want to switch which camera you are working with, point at the thumbnail in the list and click on it.imported it into the First Stage Repository.

## Camera Sensor


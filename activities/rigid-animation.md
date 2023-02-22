# Rigid Animation

{% embed url="https://youtu.be/gkTz6Dp6sq4" %}

Rigid body animation is perhaps the simplest of methods for moving any thing around your stage, including Sketches, Shapes, Props, Vehicles and Characters.

To start, point at the thing you want to animate, press the **Inspect** button and select **Start Motion** from the [Inspect Menu](../basics/working-with-things/#inspect-menu). (This step is not needed for character puppets as they are always animated.) This will create a keyframe on the Timeline.

You can now scrub the timeline and use the [Grabber](../basics/core-tools/grabber.md) to move the thing to create a new keyframe. When you scrub between those keyframes, the thing will move: it will follow a smooth spline between the points and uses speed curves to start and stop smoothly.

{% hint style="info" %}
The 'advance a beat' button on the [Transport Controls](../basics/working-with-time/#transport-controls) is very useful for pacing motion.
{% endhint %}

The animation will have an associated [Motion Path](../basics/working-with-time/motion-paths.md) visible in the scene. If it hides away, point at the thing again to bring it back. You can use this to scrub time to where you want.&#x20;

From the [Timeline](../basics/working-with-time/timeline.md), you can move keyframes in time to change the speed of the animation. You can also spped up or slow down the whole animation by dragging an end handle.

{% hint style="info" %}
**Build up your movement in stages:**\
For example, place a car, then move time and place the car a second time to create a straight motion path between those two points. Then scrub the motion path to points where the car is not moving naturally, and re-orientate the car to create new keyframes in between. Alternatively, the same technique can be applied by scrubbing on  the timeline.
{% endhint %}

## Changing the animation behaviour

<figure><img src="../.gitbook/assets/DUMMY 2023-02-22 14-11-04.jpg" alt=""><figcaption></figcaption></figure>

You can change how the animation behaves between keyframes, by going to the Timeline, pointing at the animation and pressing the **Inspect** button: then choose the **Edit** option in the pop-up menu.

<figure><img src="../.gitbook/assets/DUMMY 2023-02-22 14-11-11.jpg" alt=""><figcaption></figcaption></figure>

You can now see the properties for the animation:

| **Path Shape**    | <p>Choose between:<br><strong>Jump</strong> - motion jumps directly between keyframes <br><strong>Straight</strong> - motion moves in straight lines between keyframes<br><strong>Curve</strong> - motion follows a smooth curve between keyframes</p>                                                                                                               |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Speed Profile** | <p>Choose between:<br><strong>Uniform</strong> - motion is at a constant speed between keyframes<br><strong>Smooth Start And Stop</strong> - motion is mostly uniform but starts smoothly at the first keyframe and stops smoothly at the last.<br><strong>Pause At Each Key</strong> - motion starts and stops at each keyframe, coming to a brief pause there.</p> |

There is also an action, **Set Constant Speed**, which changes the timing of the keyframes so the thing travels equal distance in equal time.

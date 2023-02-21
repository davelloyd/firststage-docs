# Rigid Animation

Rigid body animation is perhaps the simplest of methods for moving any thing around your stage, including Sketches, Shapes, Props, Vehicles and Characters.

To start, point at the thing you want to animate, press the **Inspect** button and select **Start Motion** from the [Inspect Menu](../basics/working-with-things/#inspect-menu). (This step is not needed for character puppets as they are always animated.) This will create a keyframe on the Timeline.

You can now scrub the timeline and use the [Grabber](../basics/core-tools/grabber.md) to move the thing to create a new keyframe. When you scrub between those keyframes, the thing will move: it will follow a smooth spline between the points and uses speed curves to start and stop smoothly.

{% hint style="info" %}
The 'advance a beat' button on the [Transport Controls](../basics/working-with-time/#transport-controls) is very useful for pacing motion.
{% endhint %}

The animation will have an associated [Motion Path](../basics/working-with-time/motion-paths.md) visible in the scene. If it hides away, point at the thing again to bring it back. You can use this to scrub time to where you want.&#x20;

{% hint style="info" %}
**Build up your movement in stages:**\
For example, place a car, then move time and place the car a second time to create a straight motion path between those two points. Then scrub the motion path to points where the car is not moving naturally, and re-orientate the car to create new keyframes in between. Alternatively, the same technique can be applied by scrubbing on  the timeline.
{% endhint %}

From the [Timeline](../basics/working-with-time/timeline.md), you can move keyframes in timne to change the speed of the animation. You can also spped up or slow down the whole animation by dragging an end handle.

## Changing the animation behaviour


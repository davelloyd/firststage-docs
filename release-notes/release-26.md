---
description: 1st February 2021
---

# Release 26

## Animation

Release 26 brings a complete overhaul of animation within FirstStage.

Rigid animation, character animation and camera animation all behave the same way:

* Simply move the thing, pose the puppet or set the camera shot where you want it to be at the current time.
* Scrub time to set more keyframes and create motion.
* The motion path is shown as particles following the centre of the thing.
* Point at the motion path and you will see the time when it would be there, shown in cyan hovering above the path.
* Grab the motion path to scrub time directly without needing to go to the WristPad or TimeTool. You can then grab the thing itself to adjust the motion path or animation.
* Under the hood, motion paths use cubic interpolation and speed curves to give smoother and more convincing results.
* From the Timeline, you can move individual keyframes in time. Or you can move a sequence of keyframes.
* When you move a keyframe on the timeline, everything afterwards moves to preserve timings.
* You can grab the ends of a sequence of keyframes to change the ease in/out of the animation. If it has no ease out (shown with a square end), it will instead hold the final keyframe.

### Character Animation

The body motion of puppets (roughly, the character’s centre of mass) can be animated – much like for rigid objects: set the position simply by grabbing the whole character

Additionally puppets can have animated poses: set a pose simply by grabbing a part of the body (with the proximity/hand)  and moving it as desired.

### Camera Animation

Camera keyframes can be set and manipulated while Through The Lens.

Camera keyframes are grouped into three tracks:

* Look keys describe where the camera is pointing. This can either be pan/tilt or be targetted on another thing.
* Move keys describe where the camera is, simulating dolly or crane movement.
* Lens keys describe the camera lens settings: focal length, aperture/depth of field, focus distance. Lens keys can also include post-processing such as color grading.

There are several other improvements to camera tracking and interpolation between keyframes:

* Camera motion works similarly to rigid motion with cubic interpolation, speed curves and ease in/out
* A camera key can be stretched by dragging either end of it. This will hold that keyframe for its duration.
* When a camera is tracking a target, it will only move when the target moves outside of a small zone around athe original point and will then have damping applied. If the target tries to move outside the safe frame of the camera, the camera will track hard to keep the target in view.
* Interpolation between camera lens keys takes account of the target, focal length, aperture and focus distance to produce more natural motion. This is particularly important for a ‘dolly zoom’ shot.

### Motion Capture

As well as setting individual keyframes, you can also capture motion in various ways:

* Hand animate with the TimeTool
* Record a hand-held camera sequence (will show in a separate Mocap track).
* Take control of a puppet and perform using the headset and controllers – and additional Vive trackers for waist and feet if you have them.
* Body calibration in VR has been improved and allows you to adjust the relative position of the trackers.
* Stream motion data from Rokoko Smartsuits (now supports gloves and facial data as well).

Motion capture sequences behave similarly to keyframe sequences except that the individual keyframes are hidden. Instead, mocap sequences can be trimmed by dragging either end of the activity on the timeline – useful for removing pre-roll and post-roll from the performance.

Motion paths for mocap sequences can also be ‘warped’ by grabbing the actor at a point in time and moving them. Unlike a keyframe sequence, this does not set a keyframe but warps the whole path. It is best used for small corrections as it does not respect footsteps for humanoid characters.

### Motion Layering

The Timeline shows activities sorted by layer for each actor: the higher activities mask lower activities.

Humanoid animation includes a mask over body parts (head, arms, etc) and so a lower activities may still contribute animation if the higher activity’s mask does not include body parts that the lower activity drives.

This can be helpful when layering additional mocap or poses on top of a full body mocap sequence.

## Multiple Select and Grouping

* From the Inspector, a selection of things can be combined into a single rigid object.
* You can also combine objects by holding one in each hand and pressing the radial menu.
* Only passive assets (not characters or vehicles) can be so combined.

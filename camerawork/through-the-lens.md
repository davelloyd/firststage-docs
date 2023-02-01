# Through The Lens

Point at a camera with the Navigator tool (the default on your off-hand) and you should see an icon popping up over the camera saying Through The Lens. Click and hold for a second to end the TTL space: here you can adjust your camera framing and work with keyframes to create camera motion paths.

## Main Monitor <a href="#_q8gqm9f9bxes" id="_q8gqm9f9bxes"></a>

The main monitor in front of you shows what the camera is seeing.

You can point at something in the camera view and click on it to set it as the **Look Target**. You can clear the look target from the radial menu.

You can also drag the viewpoint by pressing and holding the trigger.

## Nudge Handles <a href="#_d28o6ft5l27i" id="_d28o6ft5l27i"></a>

Immediately in front of you are nudge handles that let you move the camera in a smooth and controlled fashion. If you reach out to a handle, your hand will turn solid and you can grab the handle by holding the trigger.

On your left are three arrows which control movement of the camera in each of the three axes: forwards/backwards, up/down and left/right.

If you have a look target set, up/down and left/right will move the camera in orbit around the target rather than in a straight line.

On your right are three circles which control the orientation of the camera in each of three axes: pan, tilt and roll (or dutch tilt).

## Lens Controls <a href="#_uifgw1dilbru" id="_uifgw1dilbru"></a>

Between the nudge handles, there is a panel with sliders to control the focal depth, lens length, and aperture.

Note that if a target is set, the focal depth cannot be changed.

There is also a dropdown to let you choose a post-process profile to be applied to the lens. Post-process profiles let you specify color grading, lens flare and many other effects. The profiles available are taken from the Asset Repository: you can create new ones in Unity and commit them to the repository, after which they will be available for use.

## Look Behaviour <a href="#_enjm7xrw1oa7" id="_enjm7xrw1oa7"></a>

When a camera has a look target and that target moves, the camera will track the target if the target moves too far from the original position in the field of view. When the target moves a little too far, the camera will track softly as if on a spring. But when the target tries to move outside the camera’s field of view, the camera will track hard to ensure the target remains visible.

The look target is recorded with a look keyframe allowing a shot that doesn’t start tracking until a given time or a shot that stops tracking at a certain point. You can also have shots that hand over from one target to another.

## Body Follow Behaviour <a href="#_6i1r38f850fm" id="_6i1r38f850fm"></a>

The body of the camera can be attached to another thing and it will then follow that thing.

By default, a camera will follow its target rigidly: for example a security camera attached to a moving bus. But it does not need to.

A dropdown lets you choose from the following behaviours:

| Rigid Lock    | The camera will follow its target rigidly moving and rotating as if connected to the target.                                         |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| No Roll       | The camera will follow its target rigidly, but with no roll.                                                                         |
| Keep Vertical | The camera will follow its target rigidly but with no tilt and no roll.                                                              |
| No Rotation   | The camera will only track the position of the target but maintains its original orientation.                                        |
| Follow        | Mimics a human operator following a target: the camera tries to move as little as possible to maintain the distance from the target. |
| No Target     | Cancels any follow behaviour                                                                                                         |

Note that if the camera has a look target, it is applied after the body follow behaviour.

## Timeline <a href="#_r2kuqu3u2p3u" id="_r2kuqu3u2p3u"></a>

Below the monitor is a timeline with three tracks for move, look and lens. You can set keyframes for each of these independently. The camera engine will then interpolate smoothly between these keyframes.

As well as moving keys, you can also hold a keyframe by dragging either end of the keyframe on the timeline: for the duration of the keyframe, that property will not change.

There are also transport controls beneath the timeline allowing you to start/stop and move between sections.

## Camera List <a href="#_cx5ivobs21cd" id="_cx5ivobs21cd"></a>

On the left of the monitor is a list of all the cameras in the scene. If you want to switch which camera you are working with, point at the thumbnail in the list and click on it.

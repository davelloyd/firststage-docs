# Cameras

FirstStage provides a powerful camera system. Cameras can be easily created with the Viewfinder and then animated with complex motion paths. Cameras can automatically look at targets and follow targets (the two targets do not need to be the same).

### Using the Viewfinder <a href="#_gi37kx4aa5b" id="_gi37kx4aa5b"></a>

You can summon a hand-held Viewfinder by pointing your controller at your head and pressing the A or Menu button. You can also summon it directly from the Tool Wheel.

The Viewfinder screen shows what the camera is seeing through the lens.

### Lens Controls <a href="#_6ayqyihy0vzk" id="_6ayqyihy0vzk"></a>

On the left hand side, there are three levers which allow you to adjust the focus, lens and aperture.

Note that the depth-of-field blurring is a real-time approximation and will not give large bokeh.

### Setting the Target <a href="#_fvczo6lrall6" id="_fvczo6lrall6"></a>

The camera will autofocus if it has a target. If you touch the trigger, it will set the target to whatever is at the centre of the screen. While continuing to touch the trigger, the target is held and you can then frame it so the target is anywhere in the field of view.

### Creating a Camera <a href="#_98phf9w4wevz" id="_98phf9w4wevz"></a>

Click the trigger to create a camera from the current viewpoint. There will then be a camera in front of you.

You can also click & hold the trigger to record handheld camera motion. When you do, the scene will start recording and activities will play out. There is a small amount of smoothing but this is not a steadicam.

### Through The Lens <a href="#_aln4k6tzbumk" id="_aln4k6tzbumk"></a>

Point at a camera with the Navigator tool (the default on your off-hand) and you should see an icon popping up over the camera saying Through The Lens. Click and hold for a second to end the TTL space: here you can adjust your camera framing and work with keyframes to create camera motion paths.

### Main Monitor <a href="#_q8gqm9f9bxes" id="_q8gqm9f9bxes"></a>

The main monitor in front of you shows what the camera is seeing.

You can point at something in the camera view and click on it to set it as the **Look Target**. You can clear the look target from the radial menu.

You can also drag the viewpoint by pressing and holding the trigger.

### Nudge Handles <a href="#_d28o6ft5l27i" id="_d28o6ft5l27i"></a>

Immediately in front of you are nudge handles that let you move the camera in a smooth and controlled fashion. If you reach out to a handle, your hand will turn solid and you can grab the handle by holding the trigger.

On your left are three arrows which control movement of the camera in each of the three axes: forwards/backwards, up/down and left/right.

If you have a look target set, up/down and left/right will move the camera in orbit around the target rather than in a straight line.

On your right are three circles which control the orientation of the camera in each of three axes: pan, tilt and roll (or dutch tilt).

### Lens Controls <a href="#_uifgw1dilbru" id="_uifgw1dilbru"></a>

Between the nudge handles, there is a panel with sliders to control the focal depth, lens length, and aperture.

Note that if a target is set, the focal depth cannot be changed.

There is also a dropdown to let you choose a post-process profile to be applied to the lens. Post-process profiles let you specify color grading, lens flare and many other effects. The profiles available are taken from the Asset Repository: you can create new ones in Unity and commit them to the repository, after which they will be available for use.

### Look Behaviour <a href="#_enjm7xrw1oa7" id="_enjm7xrw1oa7"></a>

When a camera has a look target and that target moves, the camera will track the target if the target moves too far from the original position in the field of view. When the target moves a little too far, the camera will track softly as if on a spring. But when the target tries to move outside the camera’s field of view, the camera will track hard to ensure the target remains visible.

The look target is recorded with a look keyframe allowing a shot that doesn’t start tracking until a given time or a shot that stops tracking at a certain point. You can also have shots that hand over from one target to another.

### Body Follow Behaviour <a href="#_6i1r38f850fm" id="_6i1r38f850fm"></a>

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

### Timeline <a href="#_r2kuqu3u2p3u" id="_r2kuqu3u2p3u"></a>

Below the monitor is a timeline with three tracks for move, look and lens. You can set keyframes for each of these independently. The camera engine will then interpolate smoothly between these keyframes.

As well as moving keys, you can also hold a keyframe by dragging either end of the keyframe on the timeline: for the duration of the keyframe, that property will not change.

There are also transport controls beneath the timeline allowing you to start/stop and move between sections.

### Camera List <a href="#_cx5ivobs21cd" id="_cx5ivobs21cd"></a>

On the left of the monitor is a list of all the cameras in the scene. If you want to switch which camera you are working with, point at the thumbnail in the list and click on it.

### Cameras on the Wristpad <a href="#_yjzp7fnhledc" id="_yjzp7fnhledc"></a>

Go to Cameras on the Wristpad to view all the cameras in the scene.

All the cameras in the scene are shown in a column on the left. Click on a camera to show it in the main panel.

You can click on the main panel to enter the TTL space for that camera.

If you click the **Inspect** button on a camera, it will take you to the Cameras panel with that camera selected.

### Camera Sequencer <a href="#_xg1e78vi87az" id="_xg1e78vi87az"></a>

The Camera Sequencer is a simple linear editor allowing you to cut between any of the cameras in the scene onto a Master track. This track can then be rendered and exported to video.

The Camera Sequencer does not support clips from other scenes or allow clips to overlap in time. However the timeline does not have to be full: any gaps will not be rendered, allowing dead time to be skipped.

For more sophisticated editing, export the video and import to your preferred non-linear editor of choice (e.g., Adobe Premiere, Final Cut, DaVinci Resolve, et al.)

The Camera Sequencer is available from the desktop.

The left hand column shows a list of thumbnails for all available cameras. Click on one of the cameras to see it in the central monitor.

### Cutting between cameras <a href="#_ci5ol683wfim" id="_ci5ol683wfim"></a>

Press the **Cut** button to create a clip on the timeline for current camera.

You can drag the clip along the timeline. You can also grab either end of the clip to trim the in and out points in time for that clip.

At the left end of the timeline is a thumbnail which shows the current master output. You can click on it to show the master in the central monitor.

### Exporting the master track <a href="#_3ggvbcwpyggc" id="_3ggvbcwpyggc"></a>

Press the **Export** button to export the video as a sequence of frames (to avoid temporal compression artefacts).

The video is placed in a folder in \<User>/Videos/\<Scene>\<Date>

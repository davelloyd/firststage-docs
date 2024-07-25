---
description: 23rd April 2019
---

# Release 17

## 2019-04-24 (Update b)

### Camera movement

* Cameras now have visible paths showing their movement during the scene. Cameras no longer move in straight lines: their paths are smoothed. Speed curves allow ease in/out of shots.
* You can grab a handle in the middle of a camera path and drag it out to change the shape of the path. The camera may move faster or slower as a result as needed to ensure it reaches the right place at the right time for keyed shots.
* The camera path also has a handle at the end (a simple arrowhead) that you can grab to extend an existing path. When the path is first created this handle is on the lens of the camera object. The camera moves at a default speed (1 m/s) along the new segment of path.
* By dragging the path handle onto a second camera, you can also join two cameras together as long as the shots of the second camera are all later than the shots of the first camera.
* When “Through The Lens” for a camera, the timeline also shows the speed curves for camera movement. Typically each key will ease in and out (default duration 0.5s).

### Handheld Camera

* Bring the controller up to your headset and press the menu button to show the Viewfinder for a handheld camera.
* While the Viewfinder is open, you can use it to frame your shot. The lens length, aperture and focus distance can all be adjusted with the levers on the left hand side: you can grab them with your left controller’s Pincher.
* Squeeze the trigger gently to target a point in the centre of the screen. While the trigger is squeezed, you can move the camera to adjust the framing of the target point in the viewfinder.
* Pressing the trigger all the way will take a shot: a new camera will be created. Holding the trigger down will start the scene rolling (after a 2 second pre-roll) and capture your camera movements until you release the trigger (when the scene will stop).
* Normally, the camera is stabilised to remove any roll (or Dutch) but you can click the controller’s grip button to unlock roll.

### Other Changes

* Fixed issue with Camera Sequencer desktop view always showing black.

## Update 2019-04-29 (R17c)

* Fixed issue with the Copier not keeping copied objects held in hand for immediate placement.
* Fixed issue with the Grid Copier: copied objects can now be moved afterwards.
* Beam lights are now working correctly again: beam is visible from both sides and shows the light’s colour.
* Sketches should now load correctly even with degenerate faces (those with zero area).
* When pulling a face, it will no longer automatically extrude if a face is blocked. It is now easy to extrude if you want to (with the thumbpad) but you might instead want to unlock the vertices (with the grip button).
* Fixed an issue where the Grabber would not work if the other controller was asleep.
* Fixed an issue with picking objects when they are attached to scenery (e.g., a flybar or the revolving stage).
* When IK handles are visible, walk path handles are now hidden to avoid accidental changes to the path.
* The grip buttons on the sides of the controllers now show a hint for what clicking it does: e.g., Keep Vertical or Rotate Lock.
* The Grabber has a custom controller model with animated jaws. It’s purpose should now be more obvious and feels more precise to use. This also replaces the “Fat Finger” when a controller is close to a handle.
* You can now grab an edge in a sketch to rotate it (use the grip button to toggle angle snap) or scale it.

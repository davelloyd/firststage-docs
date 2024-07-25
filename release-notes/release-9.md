---
description: 15th May 2018
---

# Release 9

## Update (a)

* More improvements to the Sketch tool:
  * If you draw a polygon on a face, that will now cut a hole in the face
  * If you extrude a face through a shape to the other side so that it cuts an opposing face, that will cut a tunnel through the shape.
  * If you draw a line between edges on a face, that will now cut the face on the line which can then be dragged or extruded.
* When you drag a face, the touchpad menu lets you extrude a face, inset a face or scale a face
* Snap controls, vertex lock and right angle drawing have been moved to settings on the Wrist Pad
* There is a window asset which when placed in a sketch will cut a box to hold it.
* Improvements to the Paint tool:
  * The Palette has been reworked and is now on the WristPad
  * There is now a Fill mode as well as the Airbrush: this paints a whole face with a material such as brick
  * When using a Material Fill, you can drag the material and orient it and scale it on the face.
* New asset for simple lighting (under Light tag)
* New Lighting Controls on the WristPad
* In many places the grip button now acts like a toggle (easier than keeping it held down)
* When moving a thing, click the grip to toggle between keeping it vertical or free orientation
* When dragging a face in a sketch, clicking the grip cycles through keeping it parallel, 15 degree snaps or completely free
* Caronte assets can now be controlled from the Timeline.
* Many improvements to Undo/Redo but still work-in-progress
* Tweaks to movement heuristics for deteriming scale/move/turn/climb

## Update (b)

* Fix for saving/loading certain scene elements.
* Fix for spectator cam getting confused when a camera is added to the scene.
* Fix for drawing from vertex to vertex to cut a face
* Fix for color picker (missing shaders)
* Movement up/down now happens in steps of 0.5m.
* Navigator: trigger now acts as a secondary grabber instead of dragging the world.
* Lighting panel shows marker colors for lights & light asset shows its marker color.
* Asset instances should now be correctly numbered.
* Most doors and windows should now cut their own box in a wall.

## Update (c)

* Tab key can be used to change between 3rd person and 1st person spectator views.
* Office UI brought onto screen window.
* Some fixes to Undo/Redo when moving things.

## Update (d)

* Fix for motion capture (was accidentally disabled)

## Update (e)

* Fix: Corridor and Old Town scenes had been accidentally disabled.
* Fix: Office did not get loaded correctly on 2nd visit.
* Spectator view in the Office has a fixed viewpoint.
* The controllers in the office have a “drumstick” on them to make the keyboard easier to use.
* The keyboard can now be moved: put your hand in it and pull the trigger to grab – use both hands to scale it.
* Keyboard keys now flash yellow when hit and deliver a haptic pulse for feedback.
* The range of the UI pointer has been limited (25cm) to reduce accidental interactions.
* Desktop UI can be hidden when in the Office (top right corner toggle).
* “Grip” movement controls now work in the Office.
* The Wristpad has been re-organised but it is still Work-In-Progress.
* Fix: Selecting the Lighting Controls the first time no longer changes the sun light to green.

## Update (f)

* Fix for issue when first logging into a clean install of First Stage
* Fix: Corridor really should be working now!
* The keyboard in the Office is now moved by the ends of the mallets not the hands.

## Update (g)

* Fix: Camera Monitor should now find a camera. Cycle through them by pressing the camera button repeatedly.
* Fix: scene should no longer appear…

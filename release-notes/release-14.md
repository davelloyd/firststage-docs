---
description: 21st January 2019
---

# Release 14

## Update (a)

* Major improvements to motion capture
  * Timeline now has the notion of an activity inspector or editor: click on the activity to reveal it.
  * The editor for motion capture activities includes a widget to mask which body parts the performance will drive.
  * The mocap editor also allows warp markers to be set which limit the effect of a path or time warp.
  * Grabbing the puppet body during a mocap clip allows you to adjust the body path.
  * Grabbing an IK handle during a mocap clip allows you to retarget hands and feet.
  * The mocap editor also allows you to adjust the speed of a warp segment.
  * Mocap data is stored separately to the scene to avoid unnecessary network traffic. Previously, long sessions could exceed the storage quota for a scene.
* Cameras now can have a look at target from inside the Camera TTL view you can set a focus and look at target by pointing at the screen and pressing the thumbpad
* Depth of Field is now supported on cameras – the bokeh effect is not large by default to keep post processing from impacting on performance.
* You can now choose a post processing profile for a camera allowing colour grading, bloom and other effects.
* You can adjust the aperture of the camera (and focus distance if no target) from the slider controls
* You can create a new post processing profile in the Unity Editor and then import it to the repository
* You can now import Textures for use as lighting gobos/cookies – just tag them with “Gobo”
* The WristPad will remain open if you look away while dragging items on it.
* Small improvements to HUD messages such as “Recording…”
* Major overhaul of the UI event system should make working with 2D interfaces easier
* Improved pointer beams
* Controllers are now stabilised
* Should be easier to drag UI items such as activities on timeline
* Fixed various bugs where UI pointer would be unexpectedly blocked
* Clicks only require a partial trigger press and have haptic feedback
* When inside the Asset Browser or Camera TTL the background is now flattened
* The asset browser now hides assets marked with the “broken” tag.

## Update (b)

* Fix for issue with UI dropdowns and overlays in VR
* Fix for issue when asset browser would not show when menu buttons pressed

## Update (c)

* Linz theatre now has revolving stages (prototype)
* Turn the stage by grabbing it and then using the radial menu left & right buttons
* Stages currently turn at 6 RPM
* Currently changes in the orientation of the stages is not recorded
* Now automatically parent things when placed on another thing (e.g. a turntable).
* Sketches also parent to the thing they are drawn on.
* Also walk path waypoints.
* Fix for some issues when loading scenes from before R14.
* Fix for issue when using the Office in VR to create a scene.
* When sketching on a surface, points should be more precisely on that surface.

## Update (d)

* Upgraded to Unity 2018.3.5 for bug fix for particle effects.
* Fixed an issue where sketches can lose geometry when saved.
* Sketch scale handles should now match the current bounds of the sketch.
* Sketch measurements now include corner angles.
* Fix for crash that occurred when scaling a thing sitting on (parented to) something that has been scaled.
* Fix for issue when manipulating a thing sitting on a scaled thing.
* Fix for issue where an asset would get stuck to the controller if clicked on in the browser (instead of press and hold): an extra click will now release it.
* You can now copy your scene to a different project.
* Fixed lots of exceptions thrown when going back to the Office

## Update (e)

* Added missing colliders in Linz Theater – can now walk on stage again.
* “Symbols” key on VR Keyboard now toggles between symbols and letters.
* Timeline can now be resized by dragging the zoom button left and right as well as up and down.
* Timetool record button now shows a different icon to stop recording.
* Improved sizes of assets in browser.
* Wristpad won’t appear when a tool is being used on that controller.
* Fix for desktop UI not starting correctly.

## Update (f)

* Fix for camera sequences failing to load.
* Selected camera on wristpad now runs at full framerate.

## Update (g)

* Fix when asset browsing for controller losing left/right buttons on 2nd visit
* Fix for crash with some scenes.
* Forced quality settings to fantastic.

---
description: 22nd August 2018
---

# Release 12

## Update (a)

* Rigid animation:
* Select the Time Tool and then point at a thing and grab with the trigger to record some motion
* The path can be editted afterwards using the Grab Tool
* Puppets can now be placed on things (e.g. Lottie on the trampoline)
* The WristPad now includes a Web Browser (Chromium).\
  Initially this is just used to show a Quick Reference Guide but more soon…
* Mocap from Rokoko Smartsuits can now be managed from the WristPad:
* Assign a suit directly to a puppet without VR control
* Calibrate a suit
* Fixed issue with Multi Select getting stuck
* Fixed issue when grabbing a scaled object and the pivot point jumped.
* Fixed direction of tilt control in camera TTL view.
* Fixed: changing the FOV of a camera now records a keyframe
* Fixed issue with calibrating Smartsuit against a puppet (was using bind pose instead of t-pose).
* Fixed issue when replaying a puppet’s walk and the puppet did not animate
* Fixed layout issue with lights on the Wristpad
* The Lighting Controls will now show the last light moved

## Update (b)

* Speech recognition has been re-enabled (oops)
* Say “Help” to summon a floating browser
* You can now animate an IK handle with the Time Tool (as with a rigid body)
* Support for asset bundles built for a specific platform (iOS or Win64)
* Architecture support for Obi Cloth dynamics
* Deleting a character should now clean up all paths, start/end handles etc.

## Update (c)

* Calibrate button on Mocap Controls is now enabled when a puppet is assigned.
* Mocap Controls have a record arm flag to control whether the puppet shows live/replay
* The Rokoko Smartsuit Studio should now be running at the same time with forwarding enabled to port 14043
* This allows use of the filters such as Locomotion from the Studio
* Lighting controls can now be keyframed like cameras – just change either intensity or spot angle while record is armed.
* Fixed issue with character sometimes spinning on a waypoint

## Update (d)

* Mocap is now applied to a proxy skeleton and then retargetted to the puppet skeleton. (Default body shape only)
* Mocap armed flag is cleared when recorded mocap is played back – can be reset from WristPad.
* You can now set a keyframe on a camera just by moving it (with the Hand tool)
* Time Tool can now animate selected groups of things at the same time
* Drawing a shape on an uneven floor will now make it exactly vertical.
* Fixed issue where the Airbrush did not reset after using “Wallpaper” mode
* Fixed issue when deleting something with rigid animation
* Fixed issue with menu button sending a commit message to currently selected UI element

## Update (e)

* Fixed rotation compensation on performer that was causing problems with hip bends.
* If a broken asset bundle is found in the cache, it will now be deleted and re-downloaded.
* Lighting panel no longer resets current light when WristPad hides/reappears
* Fixed issue with cameras showing up in the wrong place in the Asset Browser
* Reset scene on load to ensure cameras reflect keyframes

## Update (f)

* Reduced framerate for rendering cameras that are just being monitored – should improve performance with lots of cameras
* Fixed issue with camera focal length being reset in the Camera Sequencer view.
* Fixed issue where entering TTL mode would reset focal length and set a rogue keyframe.
* Fixed issue when trying to assign one of several suits to a puppet.

## Update (g)

* Fixed issue where scale would reset after using the scale handles and moving the timeline.

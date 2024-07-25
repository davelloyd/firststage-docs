---
description: 1st February 2018
---

# Release 7

## Update (a)

* Rokoko Smartsuit is now supported – if a suit is connected it will be used when the user “Takes Control” of a puppet (otherwise the VRIK fallback will be used).
* IK based animation has been greatly improved including support for animating the pivot (root) position – shown as a cube between the character’s feet.
* Timeline is now available on the wrist.
* Characters should follow paths more accurately and recover back to the path if knocked off.
* New camera steering controls.

## Update (b)

* Fixed: Path for IK handles (other than Pivot) didn’t show
* When Pivot IK handle is moved, Grounder IK is disabled preventing puppet from snapping back to ground
* Camera TTL now shows the view from the camera blurred as background

## Update (c)

* Camera pan & tilt now work by dragging instead of twisting – see if that is more natural.
* Roll (Dutch tilt) now goes the other way – you twist the camera not the scene.
* When dragging a control the touchpad is now a reset button that restores position, pan & tilt to when you started dragging. Roll is always reset to horizontal.
* Fixed: trying to move the camera after scrubbing through a keyframe sequence failed – should now work.
* Fixed: Lighting in Corridor scene was broken (inmcompatible with current version)
* Fixed: Smartsuit would only work in the Empty Stage as the receiver was not added to other scenes.

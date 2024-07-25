---
description: 27th March 2023
---

# Release 32

R32 is our first General Access release!

As well as many bug fixes across all features, here are the main changes:

## Documentation

FirstStage now has comprehensive [documentation](../)! We have rewritten and re-organised the old docs which were written during development and were often out of date.&#x20;

This is an ongoing effort of course, so please let us know where things are missing, out of date or just confusing!

## Camerawork

* [Cameras](../cameras.md) now support attach and follow behaviours with control over the damping to allow tighter or looser tracking.
* The look behaviour of cameras now has a similar control (Slack) over how quickly the camera tracks when the target moves.&#x20;
* The [Through The Lens](../camerawork/through-the-lens.md) control room has an improved control panel to manage follow and look behaviours.
* The TTL room also has a list of all cameras in the scene allowing you to switch between cameras without leaving the room.

## Asset Library

* You can now independently select which sets of assets you see: [public, project and/or local](../basics/asset-library.md#repository-scope).

## Crafting

* With the [Sketcher](../sketching.md), you can no longer accidentally draw a path with crossing edges which would produce broken geometry.
* Cutting faces is much more robust with the Sketcher.&#x20;
* The Lathe, Cylinder Section, and Sphere Section now have [inspectable](../basics/working-with-things/inspector.md) properties to control level of detail.

## Waldo

The [Waldo](../basics/working-with-things/moving-with-the-waldo.md) has been greatly improved:&#x20;

* You can now choose which set of axes the Waldo moves along: world, target or local.
* You can set the linear and angular snaps directly from the Waldo.
* You can move the Waldo to a more comfortable position.

## Misc

* Undo/Redo now have more informative descriptions for edits.
* You can now use a voice command "screenshot" or "screengrab" to grab a screenshot while in VR. (Requires Windows Voice Recognition.)


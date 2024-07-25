---
description: 6th April 2019
---

# Release 16

## New controller model for Animation Tool

To distinguish from Grab Tool

* When working on a sketch, you no longer need to switch to Grab Tool to move a face, edge or vertex:\
  simply touch the controller to the sketch to activate a proximity based grab (identified visually with a black knob).
* Pulling a face will automatically extrude it when it is blocked.
* You can also grab a face with both hands now to scale or rotate it.
* While moving a face with one hand, clicking the grip will allow the vertices to move as well as the plane.
* While rotating a face with two hands, clicking either grip will toggle angle snap on and off (initially on).
* The radial menu while pulling a face now only provides the extrude command as scale (inset and taper) are now done with two hands.
* Bent faces as a result of moving vertices are now automatically triangulated.
* Fix for issue where moving or scaling a window (with the nudge handles) in a sketched wall did not update the hole in the wall.
* When controlling something from the WristPad, a curved wire will guide you to the where that thing is in the scene.\
  Works for the Lights, Cameras, Stage Controls and Inspector.
* Depth of Field on cameras now uses the new Post Process V2 stack which provides better quality blur as well as many options for color grading, bloom, etc.
* Theatre: flybars are now numbered in the other direction.
* Fix for issue where destroying something blocked sketching working or stage controls showing
* Attachments between things (parenting) can now be removed by grabbing the attach ball and pressing the radial menu button.
* Fix for issue where showing the handles would show them on attached children instead.
* Nudge handles now have tighter colliders making it easier to pick between move, rotate and attach.
* Sketches are no longer walkable on by default. Go to the Inspector for a ground object to allow puppets to walk on it.
* Moving something normally is not allowed when handles (nudge, IK, etc) are visible as this is usually unintended.
* Puppets can now be animated rigidly (via the pivot) without needing to reveal the IK handles.
* Prototype editor for moving IK keyframes – click on the IK activity in the timeline to reveal.

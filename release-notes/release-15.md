---
description: 14th March 2019
---

# Release 15

## Update (a)

* Sketches now save painting brushstrokes:
  * Painted surfaces will be preserved across sessions
  * You can now undo/redo individual brushstrokes
  * If you are working collaboratively you will see when a remote user paints a surface
* New stage machinery: fly bars
* New panel on the WristPad for Stage Controls:
  * Each control has a slider and a record arm toggle
  * Each control can also be driven from the radial menu when pointing at it.
  * The state of each control is saved with the scene
  * Moving a control while recording with record armed will record all changes to an automation track that can be replayed.
* Improvements to rigid animation (still WIP)
* Refined the shape of the new pointer beams
* Fix for stage lights not saving colour settings.
* Improved behaviour when resizing flat thin objects (such as a rug).
* REGRESSION: Depth of field on cameras is currently broken.

## Update (b)

* Fix for loading previous scenes with rigid animation in them.
* Fix for vertical scrolling of timeline
* Introduced a new “pose ghost” when capturing mocap. Also changed starting position of performer to make it easier to interact with real-world props.

## Update (c)

* Accidentally left several experimental features in R15b. Now removed!

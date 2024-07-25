---
description: 9th July 2020
---

# Release 24

## Improved Script Management

* The Script View has been greatly improved. It now provides two columns:
* The right hand column lists all the activities in the scene in order of their start times.\
  Each activity is shown as a block with the start and stop times on the left hand edge.\
  You can scrub time by dragging within the block.\
  When you hover over an activity, a button appears allowing you to cue the activity to start at the current time.
* The left hand column lists all the active things in the scene.\
  If you click on any thing, it will filter the script to show activities for that thing.\
  If you hover on a thing, a button will appear allowing you to inspect the thing: taking you to the appropriate Inspector, Camera, Light or Stage Control view.

### **Script Markers**

* Script markers allow you to provide a bit of structure to the timeline. They can mark the start of shot sequences, blocks or events.
* In the Script view, markers are presented as section headings. The heading has the start time on the left hand edge. If you click on the heading, it will scrub time to the marker start.
* There is also a button to expand and or hide the block of activities between this marker and the next.
* If you hover over the heading several buttons will appear:
  * a button to edit the description
  * a button to cue the marker to start at the current time

There is always a default marker at the start of the scene.

1. Press the Create Section button and dictate a description for the marker (there are red numbers indicating that it is recording, and how many seconds you have been speaking for).\
   _NB – You may need to turn on ‘Online speech recognition’ in your Windows Privacy settings to be able to verbally label markers when you create them._
2. Press the button again when you’re finished.\
   FirstStage will then turn that into a text transcription.

_NB – Windows dictation recognition is pretty good (particularly if you spend a little effort training it) but it usually has problems with character names which can be a nuisance. In which case you can edit the description with a keyboard._

* In the Timeline view, markers are shown at the bottom of view as blocks spanning the start times of successive markers. Each block will show the description.
* You can drag markers along the timeline and they will also drag all activities that start afterwards preserving their timings relative to each marker.

## New way to get Handles

* The “?” icon on the thumbpad radial menu for the Grabber no longer cycles through the available handles (translation, rotation, scaling, attachment, etc) but instead opens up a wheel menu allowing you to select which handles are visible (or none) by twisting the controller exactly as when choosing tools.

## Asset Importing

* We have also been working hard to make it easier to import assets (props, models, scenes, etc) into FirstStage via Unity.
* Start here for our tutorials!

## Many polishes and fixes

* Dragging items on the timeline is much smoother and the timeline autoscrolls much more easily and smoothly when dragging an item towards the edge of the view.
* Handles for manipulaing activities on the timeline are now much easier to grab and work with: e.g., for trimming (or revealing) a mocap sequence or stretching a pose.
* Improvements to layering poses over mocap
* Improvements to using held props with mocap

---
description: 17th May 2021
---

# Release 27

## Attachments

Release 27 brings a complete overhaul of how things are attached to other things and many issues in this area have been fixed.

To attach something to something else so that it follows it rigidly:

* Point at the thing you want to attach with the Grabber
* Summon the Action Wheel by pressing the Inspect button.
* Select the Attach Handle
* Grab the Attach Handle and point it at what you want to attach to and release.
* If the thing is _animated_, you can attach it to different things at different times during the scene.
* When attaching something to a puppet, it attaches to specific parts of the body: hands, arms, head, body, legs and feet.

### Camera Follow

If you attach a camera to something, it follows the target using a more cinematic behaviour than a rigid mount:

* the camera accelerates and decelerates with damping;
* the camera maintains true vertical orientation;
* the camera will not swing round if the target turns.

## Performance Capture Improvements

* You can now wear feet and waist trackers while performing in VR. [See here for details](https://firststage.moviestorm.co.uk/mocap-trackers/).
* Walking and running has been improved so the spine does not pull the feet up on tiptoes.

## Audio Sources

There is a new primitive in the asset repository: an audio source. Visually it is just a translucent sphere but it can play audio clips as either a 3d source located at the centre of the sphere or a 2d source which is uniform regardless of where the camera is or which direction it is facing.

Audio sources supported include .OGG and .WAV (Unity doesn't support MP3 due to licensing issues), and they can be directed from the Audio panel on the WristPad. For each source, there will be a channel strip which controls it:

* a volume slider
* a switch to choose 2d vs 3d
* a play button lets you choose a file to play as a clip on the timeline

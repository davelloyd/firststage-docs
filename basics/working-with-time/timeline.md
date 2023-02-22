# Timeline

<figure><img src="../../.gitbook/assets/Warehouse Demo 8 2023-02-09 11-55-57.jpg" alt=""><figcaption></figcaption></figure>

The Timeline shows all the Activities that describe how the scene plays out: performances, animation, automation etc.

The [WristPad](../wristpad/) provides a view on the timeline as does the desktop and several other places.

The activities are organised into tracks by the thing the activities act upon.

## Scrubbing Time

You can scrub time by dragging the background of the Timeline.

You can scroll to anywhere in time using the scrollbar along the top. The arrows at the ends of the scrollbar thumb allow you to scale the timeline.

You can also scrub time by using the thumbpad/stick while pointing at the timeline.

## Activities

Activities are a key concept behind FirstStage: they describe the time-like behaviour of things.&#x20;

Activities act upon a _subject_ thing and occasionally other things (e.g., the activity for a character holding a prop has the character as _subject_ and the prop as _object_).

An activity has a Start Time and a Duration that determine when the activity plays. It is typically represented as a block on the timeline.&#x20;

You can drag an activity along the timeline to change when it happens.

For some activities, you can also stretch the duration or trim/reveal clips: point at the activity to reveal triangular handles at the end and then drag the handle.

If you press the **Inspect** button, a menu will pop up with options depending on the type of activity. One option will always be **Delete** and you can usually **Duplicate**.

Some activities (such as [Rigid Animation](../../activities/rigid-animation.md)) also have an **Edit** option which will take you to an inspector screen where you can change the behaviour of the activity. Press the top-left arrow or the thumbad back arrow to return to the main timeline.

### Keyframes

Some activities contain a series of keyframes that are interpolated between. Such an activity is shown with a transparent background and a solid pip for each keyframe.

You can drag the keyframe pip along the timeline to change its timing. To change the value of a keyframe you should scrub to the keyframe and then change the original property in the same way you first created it.

You can also delete a keyframe by summoning the menu with the **Inspect** button.

## Tracks

Every thing that has an activity will have a track on the timeline.

The track header (left hand column) shows the name of the thing. If you point at it, a menu will pop up with the following options:

* open the [Inspector](../working-with-things/inspector.md) on it.
* teleport right next to it.
* enable/disable all activities for it.

##



## &#x20;

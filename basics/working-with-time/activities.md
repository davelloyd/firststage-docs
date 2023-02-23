# Activities

Activities are a key concept behind FirstStage: they describe the time-like behaviour of things.&#x20;

Activities act upon a _subject_ thing and occasionally other things (e.g., the activity for a character holding a prop has the character as _subject_ and the prop as _object_).

An activity has a Start Time and a Duration that determine when the activity plays. It is typically represented as a block on the timeline.&#x20;

You can drag an activity along the timeline to change when it happens.

For some activities, you can also stretch the duration or trim/reveal clips: point at the activity to reveal triangular handles at the end and then drag the handle.

<figure><img src="../../.gitbook/assets/DUMMY 2023-02-22 17-06-57.jpg" alt=""><figcaption></figcaption></figure>

If you point at an activity on the Timeline and press the **Inspect** button, a menu will pop up with options depending on the type of activity.&#x20;

<figure><img src="../../.gitbook/assets/DUMMY 2023-02-22 14-11-04 (1).jpg" alt=""><figcaption></figcaption></figure>

| **Delete**    | Delete the activity from the timeline.                                                                                                                                                                                                                                                              |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Duplicate** | Duplicate the activity and place the copy immediately afterwards. This is useful for building a sequence of repeated actions.                                                                                                                                                                       |
| **Split**     | <p>Split the activity into two parts before and after the current time. </p><p><em>This is only available for clip activities which span the current time.</em></p>                                                                                                                                 |
| **Edit**      | <p>Shows a screen where you can change the behaviour of the activity.<br>Return here by pressing the top-left arrow or the thumbpad back arrow.<br><em>This is only available for some activities like</em> <a href="../../activities/rigid-animation/"><em>Rigid Animations</em></a><em>.</em></p> |

### Keyframes

Some activities contain a series of keyframes that are interpolated between. Such an activity is shown with a transparent background and a solid pip for each keyframe.

You can drag the keyframe pip along the timeline to change its timing. To change the value of a keyframe you should scrub to the keyframe and then change the original property in the same way you first created it.

You can also delete a keyframe by summoning the menu with the **Inspect** button.

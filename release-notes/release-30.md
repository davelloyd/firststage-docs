---
description: 18th July 2022
---

# Release 30

## New! Branching Scripts

FirstStage now supports non-linear scripts providing decision points which trigger different branches in the script. These are **very useful for interactive training, immersive learning, interactive fiction, immersive experiences**, as well as for mocking up alternative script decisions during previs when the script is not final.

For example, an interactive training script might include a scenario where the player can walk up to an instructor character, and in doing so triggers the appearance of a dialog where the instructor asks the player a testing question and the player simply chooses their preferred response, which takes the story down a specific conversational branch. Or the player is asked to choose which fire extinguisher to use for a particular type of fire, and they could then either select an available fire extinguishers leading to a sequence playing out showing the repercussions of that decision, or the player could actually have to pick up the fire extinguisher and use it, leading again to the appropriate outcome.

#### **Basic workflow**

1. Go to the Asset Repository and look in the _Interactive_ category for a trigger asset such as a Trigger Volume or Multiple Choice Dialog
2. Grab your chosen trigger asset and place it on the set
3. Scrub the Timeline to a convenient point to create the new branch (this will often be after the main part of the script at the point the user might trigger it).
4. Now switch to the branch triggered by the asset (see discussion of the individual triggers for how). Some triggers such as the Multiple Choice Dialog will have several branches depending on which option is chosen.
5. Just above the timeline you should now see the branch showing as the container into which all new activities will be placed.
6. Now construct the script for the branch just as usual: while the branch is active, all new activities will be placed in there.
7. Activities that are not part of the branch will be shown greyed out. They will still play out which is useful for background activities.
8. When you’ve finished working on that branch, click on the X icon to close the branch at which point do not be alarmed when all the activities in that branch vanish as they only show when the branch has been triggered.
9. You can now continue to work on the Main Timeline or switch to another branch.
10. To test the triggers and branches, go to the WristPad > Preferences and change your role to Player. Now when you hit Record on the Transport Controls, the Main Timeline will play out as usual, but you can now interact with the triggerable things and watch the branches play out when you do.
11. Once you have triggered some branches they will show on the timeline. You can then go back to the start and Play (rather than Record) to see how those choices played out without you needing to trigger them again.&#x20;
12. When you’re done testing, go back to the Preferences pane and set your role back to Author.

### Click to Trigger

This is one of the simplest types of triggers. Attach it to any thing in the scene to make that thing interactive.

When authoring, a simple control panel will popup when you point at the trigger.

* The Cue button will cue the branch at the current time just as if the branch had been triggered by the player.
* The Untrigger button will reset the branch so it is untriggered and any activities in the branch will no longer play or be visible on the Timeline.

When playing, the thing will highlight when pointed at and clicking on it will trigger its branch. Once triggered, the thing will no longer highlight.

#### Trigger Volume

There are several versions of this with different shapes of volume but they all work the same way: when the player enters the volume, the branch is triggered and plays out.

When authoring, a simple control panel will popup when you point at the trigger volume (same as for Click to Trigger).

When playing, the trigger volume will also act as a teleport target. Once triggered the volume will change colour to orange instead of cyan.

#### Multiple Choice Dialog

This allows for more complex branching narratives. It poses a question to the player and offers one or more alternative options for the player to choose as response.

When authoring, click on the pencil icon to edit the dialog:&#x20;

* You will be in an Office space with a form to fill in. Or the same form with be available on the desktop if you prefer to use a real keyboard.
* The first text box is the question or introductory text.
* You can then add options for the player to choose by clicking on the Add Choice button.
* Each choice has a text box which will be shown on the dialog.
* Below the text box is a selection box for the branch to be taken when that choice is chosen (along with buttons to Cue or Untrigger the branch).
* You do not need to choose a branch or create one as it will create a new branch if there isn’t one.
* But it can be useful to choose a branch if, for example, several choices (often in different dialogs) should go the same place. This is particularly common in branching narratives.
* Allow Single Choice Only lets you choose whether the player can try every option or can only choose one.

Once the choices have been set up, click on the Tick icon to return to the set.

You can now activate the branch for a choice by clicking on it. This will make that branch the target container for new activities on the timeline. When you click on a choice, any other choices will be de-activated and their branches untriggered.

Note that you can Show/Hide a dialog (from the Inspector) within the branch of another dialog to cascade dialogs and build up a conversation.

When playing, the player simply clicks on the choice they want which will then trigger that branch to be played out.

## Improved Motion Path Behaviour

There is a new option on the Inspect wheel menu: Start Motion (which replaces the previous Create Keyframe). Start Motion will start a new activity container instead of extending the previous activity container. This is useful when you have several bits of motion separated in time and do not one motion to affect the other.

You can now click on this activity on the Timeline to reveal an Inspector for the activity that lets you change some of the innate behaviour across all keyframes within the activity.

### Path Shape

This lets you change how the shape of the path is interpolated between keyframes:

* Curve - This uses a Catmull-Rom spline between points providing a natural, smoothly curving path. This is the default and usually the most natural.
* Straight - This uses straight lines between points which can be more appropriate in some circumstances.
* Jump - In this case, the thing will hold position between keyframes and then jump directly to the next keyframe. Can be useful for blocking out scenes where you only care about the key poses and not what happens between.

### Speed Profile

When moving a thing along a motion path, FirstStage calculates a speed curve that determines how far along the motion path the thing is at a given time. This curve can have different shapes giving different acceleration behaviours:

* Smooth Start Stop - This starts from the first keyframe at zero speed and accelerates smoothly between keyframes and then decelerates to zero speed at the last keyframe. This is the default and usually the most natural.
* Pause At Each Key - This is similar to Smooth Start Stop, but it also decelerates to zero into each keyframe and then accelerates out again. This has the effect of briefly pausing at each keyframe.
* Uniform - This sets a constant speed between each keyframe with no acceleration/deceleration. The resulting motion can be a bit jerky, but that may be less important than the motion being constant speed.

### Set Constant Speed

The action button, Set Constant Speed, changes the timing of each keyframe so that they cover equal distance in equal time.

{% embed url="https://youtu.be/Q7-dammoHng" %}

## **Motion Capture Improvements**

Motion Capture is a major part of FirstStage and is under continual development and as a result Release 30 brings many improvements and more will follow!

### Setup Room

The panel for setting up the mocap session has been re-organised. The following options are available:

* Record Speech - Enable this to record whatever you say during the mocap session. Useful for reading through a script.
* Grip Motion - Enable this to allow you to move during mocap using the grip buttons as you would outside mocap. This is primarily useful if you want to climb ladders etc. Note that the legs will not automatically follow: you will need to fix this with poses afterwards or use feet trackers and mime climbing insync with grabbing.
* Allow Grab - Enable this to allow you to pick up props during mocap. Note that you will only be able to pick up props that have been flagged as Holdable via the Inspector. This stops you inadvertently picking stuff up or picking up the wrong thing.
* Walk to Mark - Enable this to allow you to point at a mark with your left hand and click the trigger to make your puppet walk to it and you will follow.&#x20;
* Locomotion - Enable this and your puppet will follow you as you walk around your work area in reality.
* Keep Vertical - Disable this to allow your puppet to rotate away from the vertical. Useful for puppets attached to moving things - but beware the experience can be uncomfortable if you don’t have good VR legs.
* Drive Pivot - Disable this if you want your puppet to follow a previous animation layer.

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2022/08/R30-Mocap-Studio-1024x771.jpg" alt=""><figcaption></figcaption></figure>

### Walking around the Work Area

When you move around your work area, your puppet will follow (if Locomotion has been enabled). Previously, this was a rather clumsy procedural effect that looked like a drunken stagger. This has been upgraded to blend from a set of library animations. This is a big improvement but there is still a tendency for the puppet to lag behind you and small moves can suffer.

### Walk to Mark

When enabled, your left hand controller casts a beam (just like the Navigator) with a green target at the end. To walk to the target mark, press the Menu button (Vive) or B button (Index or Oculus). Note unlike the Navigator it is not bound to the trigger as that is needed for grabbing things.

Your puppet will then walk to the target and then stop. However you can change your destination at any time and the puppet will then move in that direction.

### Held Props

When you hold a prop, the prop will try to follow your controller (imagine a strong spring between it and you); the puppet’s hand will then match the prop. This can mean your real hand and your puppet’s hand don’t match, particularly if the prop collides with scenery.

For example, imagine placing a mug on a desk, you don’t want the mug to go through the desk yet you have no feedback in virtual reality where that is. So the mug gets stopped by the desk even if your real hand carries while your puppet’s hand is still correctly holding the mug.

You can now pick things up with two hands. This is another case where your puppet’s hands will track the held prop and your real hands may be separated from them.

**Note that things must be flagged as Holdable in the Inspector to be picked up now.**&#x20;

### Facial Mocap

You can now record voice via a mic connected to your PC at the same time as you record facial mocap on your iPhone.

A facial rig is now automatically provided for Reallusion’s CC3 characters.

### Importing External Mocap

You can now import human animation clips (e.g. from the Unity asset store, or Rokoko Studio) via the Unity Editor and FirstStage Repository Manager.

Animation clips will appear in the Asset Browser as a manequin playing out the particular animation. Grab it and drop it on a character to use it at the current timeline position.

## **Oculus Support**

<figure><img src="https://firststage.moviestorm.co.uk/wp-content/uploads/2022/08/Oculus-Support-scaled-1024x1024.jpg" alt=""><figcaption></figcaption></figure>

FirstStage now supports both the Oculus Rift and the Oculus Quest 2 (via Oculus Link or wifi Airlink).

Controller bindings are the same as for the Index controllers but without the touchpad as an alternative to the joystick.

Though FirstStage requires the PC connection to run in Authoring mode, watch out for future announcements of a Player mode that will run standalone on the Quest 2!

## **Other Fixes and Improvements**

### Remote Collaboration

We had some issues with users not reliably connecting to the same session. To fix this, when several people are working together one of them is now designated the _host_. If that person disconnects, one of the others will chosen and automatically become the new host. This will not affect anything for any of the remaining users, but the process should now work much better than before.

### Waldo

The Waldo now has a slide switch allowing you to choose which space the axes are aligned with:

* Local was the previous behaviour and aligns the axes with your work area.
* World aligns the axes with the world grid - North/South, East/West, Up/Down

Target aligns the axes with the selected thing allowing you to move it along the thing’s natural axes.

Note that in the Target case, when you rotate the object, the axes will also follow and rotate.

### Asset Browser

The Asset Browser has been re-organised around a central desk to hold the tags and other controls.

The desk height can be changed by proximity grabbing it and lifting, or by adjusting your height and position in front of it.

### New Parametric Shapes

To help with set building, there are several new shapes: Sphere Section and Cylinder Section. They can be found under the _Shape_ tag in the Asset Browser.

* Sphere Section - Gives you control over the external and internal radii, the sweep angle around the vertical axis, and the top and bottom extents. The handles for these are enabled with Edit Shape on the Inspect menu and work similarly to Sketches.
* Cylinder Section - Gives you control over the external and internal radii, the sweep angle around the vertical axis, and the top and bottom extents. The handles for these are enabled with Edit Shape on the Inspect menu and work similarly to Sketches.

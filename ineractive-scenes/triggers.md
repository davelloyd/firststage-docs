# Triggers

### Click to Trigger <a href="#_cnqemdvg2jfz" id="_cnqemdvg2jfz"></a>

This is one of the simplest types of triggers. Anchor it to any thing in the scene to make that thing interactive.

When authoring, a simple control panel will popup when you point at the trigger.

* The Cue button will cue the branch at the current time just as if the branch had been triggered by the player.
* The Untrigger button will reset the branch so it is untriggered and any activities in the branch will no longer play or be visible on the Timeline.

When playing, the thing will highlight when pointed at and clicking on it will trigger its branch. Once triggered, the thing will no longer highlight.

### Trigger Volume <a href="#_d97xm9hot79u" id="_d97xm9hot79u"></a>

There are several versions of this with different shapes of volume but they all work the same way: when the player enters the volume, the branch is triggered and plays out.

When authoring, a simple control panel will popup when you point at the trigger volume (same as for Click to Trigger).

When playing, the trigger volume will also act as a teleport target. Once triggered the volume will change colour to orange instead of cyan.

### Multiple Choice Dialog <a href="#_u2sim1hvmo26" id="_u2sim1hvmo26"></a>

This allows for more complex branching narratives. It poses a question to the player and offers one or more alternative options for the player to choose as response.

When authoring, click on the pencil icon to edit the dialog:

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

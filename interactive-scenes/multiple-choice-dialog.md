# Multiple Choice Dialog

The Multiple Choice Dialog poses a question to the player and offers one or more alternative options for the player to choose as response. Each option triggers its own script event allowing for more complex branching narratives.

<figure><img src="../.gitbook/assets/Fire Training v5 2023-02-17 17-52-15.jpg" alt=""><figcaption><p>A dialog as seen by the Player</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Fire Training v5 2023-02-17 17-51-57.jpg" alt=""><figcaption><p>A dialog as seen by the Author, showing wires to those things triggered by that choice.</p></figcaption></figure>

When authoring, click on the pencil icon to edit the dialog:

<figure><img src="../.gitbook/assets/Fire Training v5 2023-02-18 13-16-43 (1).jpg" alt=""><figcaption></figcaption></figure>

You will be in an Office space with a form to fill in:

* The first text box is the question or introductory text.
* You can then add options for the player to choose by clicking on the Add Choice button.
* Each choice has a text box which will be shown on the dialog.
* Below the text box is a selection box for the branch to be taken when that choice is chosen (along with buttons to Cue or Untrigger the branch).
* You do not need to choose a branch or create one as it will create a new branch if there isn’t one.
* But it can be useful to choose a branch if, for example, several choices (often in different dialogs) should go the same place. This is particularly common in branching narratives.
* Allow Single Choice Only lets you choose whether the player can try every option or can only choose one.

{% hint style="info" %}
The form to edit the dialog is also presented on the desktop where you can use a real keyboard to enter the question and answer texts.
{% endhint %}

Once the choices have been set up, click on the Tick icon to return to the set.

You can now activate the branch for a choice by clicking on it. This will make that branch the target container for new activities on the timeline. When you click on a choice, any other choices will be de-activated and their branches untriggered.

{% hint style="info" %}
You can Show/Hide one dialog (via the Inspector) within the branch of another dialog to cascade dialogs and build up a conversation.
{% endhint %}

When playing, the player simply clicks on the choice they want which will then trigger that branch to be played out.

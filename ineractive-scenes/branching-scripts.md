# Branching Scripts

FirstStage supports non-linear scripts providing decision points which trigger different branches in the script. These are very useful for interactive training, immersive learning, interactive fiction, immersive experiences, as well as for mocking up alternative script decisions during previs when the script is not final.

For example, an interactive training script might include an instructor character that the player can walk up to which triggers the appearance of a dialog where the instructor asks the player a question to test them. As a result of which option is chosen, the script may play out a sequence where the character instructs the player as required. Another section might ask the player to choose which fire extinguisher to use for a particular type of fire.The player would then click on one of the fire extinguishers available and then see a sequence played out showing whether they chose correctly - or not.

### Script Containers <a href="#_hn6k24od7x4n" id="_hn6k24od7x4n"></a>

Script containers hold sequences of activities on their own timeline. Script containers can be used to organise the timeline by breaking it up into blocks that match sections of the script.

Script containers have their own track at the bottom of the \[Timeline]:

* moving a container will move all activities within it.
* deleting a container will delete all activities within it

Script containers can overlap each other and of course, can overlay on top of the main timeline activities.

Script containers can also be events triggered by player interaction. For example a Multiple Choice Dialog would have a script container for each option that is triggered when the player selects that option.

When a script event is triggered, it is cued to now (i.e., its start time is set to the current master time) and will show on the timeline accordingly.

Before a script event is triggered, it is ‘uncued’ and will not show on the timeline. It will however show in the \[Script View] with a time of _Never_.

When authoring, the last cued script container is the **current container** and will appear on top of the timeline to indicate so. All new activities go into the current container (or the main timeline if not container is active).

You can cancel the current container at any time by clicking the cross in the top corner on the timeline and then new activities will go to the main timeline.

### Working with Branches <a href="#_l5dprdaevge" id="_l5dprdaevge"></a>

\[INTRO VIDEO]

The basic workflow is:

1. Go to the Asset Repository and look in the _Interactive_ category for a trigger asset such as a Trigger Volume or Multiple Choice Dialog
2. Grab your chosen trigger asset and place it on the set
3. Scrub the Timeline to a convenient point to create the new branch (this will often be after the main part of the script at the point the user might trigger it).
4. Now switch to the branch triggered by the asset (see discussion of the individual triggers for how). Some triggers such as the Multiple Choice Dialog will have several branches depending on which option is chosen.
5. Just above the timeline you should now see the branch showing as the container into which all new activities will be placed.
6. Now construct the script for the branch just as usual: while the branch is active, all new activities will be placed there.
7. Activities that are not part of the branch will be shown greyed out. They will still play out which is useful for background activities.
8. When you’ve finished working on that branch, click on the X icon to close the branch at which point do not be alarmed when all the activities in that branch vanish as they only show when the branch has been triggered.
9. You can now continue to work on the Main Timeline or switch to another branch.
10. To test the triggers and branches, go to the WristPad > Preferences and change your role to Player. Now when you hit Record on the Transport Controls, the Main Timeline will play out as usual, but you can now interact with the triggerable things and watch the branches play out when you do.
11. Once you have triggered some branches they will show on the timeline. You can then go back to the start and Play (rather than Record) to see how those choices played out without you needing to trigger them again.
12. When you’re done testing, go back to the Preferences pane and set your role back to Author.

### Player <a href="#_tf2ezwhl7p6" id="_tf2ezwhl7p6"></a>

When you set your role to Player, you have a much more limited range of things you can do:

* You can’t enter the Asset Store and create new things on set
* You can’t take control of characters, cameras, etc

### &#x20;<a href="#_76bnud3eopb4" id="_76bnud3eopb4"></a>

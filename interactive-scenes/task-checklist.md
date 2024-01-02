---
description: Coming Soon!
---

# Task Checklist

Task Checklists are a spatial dialog panel with a list of tasks: players must complete each task on the checklist before proceeding.

You can find a new Task Checklist in the Asset Library under _Interactive, Trigger_.

Once you have placed a checklist in the scene, you can edit it by clicking the pencil icon:

* Change the title text
* Add tasks

For each task, you will need to mark it complete as a consequence of some other script event:

1. Cue that event so it is the active script container at the top of the Timeline.
2. Click on the corresponding task in the checklist: this item should now have a tick to its left.
3. On the Timeline you should see an activity for the checklist which completes the chosen task.

The Task Checklist is itself a trigger: click on its Cue button to activate its event as the current script container. Any new activities will be triggered when the player has completed all tasks in the checklist.

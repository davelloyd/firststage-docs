# Collaboration

In FirstStage, you don't have to work alone: you can work with several team members at once in the same scene. Anyone who is a member of your [project's team](projects/project-team.md) can join you.

## Cloud Collaboration

FirstStage stores everything in a repository on a server in the cloud. All changes to the scene are recorded there.&#x20;

Every change you make is sent to the repository and it is also broadcast to any of your team members who are also in the same scene. As you work, changes will also happen around you as others work.

The repository view of the scene is definitive: all team members should see the same scene.&#x20;

## Peer-to-peer Collaboration

FirstStage relies on peer-to-peer networking to allow team members to see each other and talk to each other live on-set.&#x20;

Once on-set together you should be able to see other team members' heads and hands and be able to talk to them using the mic & earphones built into your VR headset.

If you pick something up, your team members will see that thing floating about as you move it.

If you perform inside a puppet, your team members will see your performance in real-time.

{% hint style="warning" %}
Peer to peer connections can be unreliable depending on you and your other team members' firewalls and internet connections. (We use a technique known as [NAT punchthrough](https://en.wikipedia.org/wiki/Hole\_punching\_\(networking\))).

We are working on a new improved networking solution which will not suffer from this problem.
{% endhint %}

### Ownership

If you grab something, everyone else will see it highlighted with your marker color and will not be able to grab it themselves. Similarly you may see things highlighted with someone else's color and you will not be able to modify it while they are working with it.

### Synchronise Clocks

By default when working on a scene, scrubbing the timeline or pressing play/record will only change time in your view of the scene: other team members will not be affected. This is normally what you want as it can be very confusing otherwise.

However it can be useful for team members to syncronise their clocks: indeed it can be essential when recording performances.

To do this go to the Transport Controls and click on the **Synchronise Clock** button (the stopwatch icon). This will toggle whether your notion of time is synchronised with other team members or not. The icon shows in three states:

| Icon color | State       | Description                                                                                                                           |
| ---------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| White      | Independent | Changing your time will not affect anyone else nor will anyone else change time for you.                                              |
| Red        | Master      | You have control over time. Changing time (scrub or play/record) will change it for those following you.                              |
| Yellow     | Follow      | You cannot change time yourself but are following whoever has the master control of time. As they change time, your time will follow. |

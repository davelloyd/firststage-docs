# Groups and Assemblies

It is often easiest to construct something from a collection of different shapes. Grouping them together makes them move and behave as a single thing.

[Select](../core-tools/selector.md) the things you want to group and go to the [Inspector](inspector.md) and press the **Group** button.&#x20;

Once grouped, you may want to [rename](inspector.md#renaming-things) it to something more helpful.

Groups behave as most other things: you can copy, destroy, animate them, etc.

## Assemblies

You may want to re-use particular groups in other scenes. Assemblies are basically groups that are save to the Asset Repository.

You can save a group as an assembly by going to the Inspector and pressing the **Save As Assembly** button.

In fact, assemblies don't have to come from groups: you can save a single shape (or any other thing) as an assembly.

## Opening Groups

While things are grouped, they can't be moved or otherwise edited individually. But it is common to want to modify an assembly after it has been grouped.&#x20;

You can **Ungroup** a group from the Inspector which will revert the collection to individual things.

You can also **Open** a group from the Inspector which will open the collection so that individual things can be moved, deleted or otherwise modified. However the collection is preserved (along with any properties such as name) and once you have finished editing the components, you can **Close** the collection and it will again behave as a single thing.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>An opened group showing the Inspector view and the individual components labelled.</p></figcaption></figure>


---
description: 23rd Jan 2024
---

# Release 34

## Quest Standalone Early Access

FirstStage is now available on the Quest 2/3/Pro running Standalone, i.e., without needing a PC to drive it.&#x20;

To start with, this is available as a sideload via SideQuest but we will be launching on the Meta store soon

[installing-on-quest-standalone.md](../basics/getting-started/installing-on-quest-standalone.md "mention")

{% hint style="info" %}
A Quest running standalone is nowhere near as powerful as a typical PC, so the graphical quality may not seem as high fidelity as when using a PC Link. For example, lighting is much more limited.&#x20;

However, FirstStage has been optimised for the Quest and works well. If you are careful with how many assets you use, and their complexity, you can make very effective scenes.
{% endhint %}

## Improved Asset Downloads

Previously, FirstStage would download all asset bundles on startup. This could lead to a long wait when first starting FirstStage and when bundles were updated.&#x20;

Asset bundles are now downloaded on demand. They are also unpacked after download for faster scene loads.&#x20;

These bundles are now hosted on Amazon's S3 service so should download significantly faster than before.

When loading a scene that uses assets that have not been downloaded yet, you will see a progress message in the&#x20;

In the Asset Library, if an asset has not been downloaded yet, you will see a placeholder with a message showing the progress in downloading and unpacking.

Palettes such as Materials will also show a placeholder with a progress message if the asset has not yet been downloaded.

## New Interaction Assets

[**Place To Trigger** ](../interactive-scenes/triggers/place-to-trigger.md)expects a particular thing to placed on it when it will trigger the branch.

[**Task Checklist** ](../interactive-scenes/task-checklist.md)shows a list of tasks which all must be completed before the branch is triggered.


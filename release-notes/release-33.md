---
description: 7th August 2023
---

# Release 33

This release has mostly been focussed on bug fixes and "quality of life" improvements.

## Improved Collaboration Support

We have migrated to Unity's new NetCode which offers several big advantages.

FirstStage now uses Unity's Relay Servers instead of NAT Punchthrough. This means that users wanting to join a scene for live collaboration should no longer face issues caused by firewalls (particularly corporate ones) which prevent the peers from connecting. Users should now reliably be able to join a scene.

FirstStage now uses the Vivox service for voice communications between users in the same scene. Vivox offers a higher quality, lower latency audio than our previous solution.

## Faster Scene Loading

Various improvements have been to speed up loading of scenes from the moment you click Enter to the moment you can do something in the scene.&#x20;

In one of our tests, a scene which took more than 3 minutes to load previously, now takes about 20 seconds to load!

There is now also a waiting area in VR while loading happens which is much more comfortable as loading leads to stalls giving unpleasant reprojection artefacts on the Vive or Index and even worse compression artefacts with the Quest and PC/Air Link.

{% hint style="warning" %}
Note that the next time you start FirstStage it will uncompress any asset bundles you have already downloaded. This may take some time. But it will mean the asset bundles load much faster.
{% endhint %}

## More Parametric Shapes

New parametric shapes:

* Cylinder: separate handles for radius & height
* Cone: separate handles for radius & height
* Truncated Cone: separate handles for upper & lower radii & height

### Convert Shapes to Sketches

To do more detailed edits to a shape such as moving a vertex, edge or face, you can convert a shape to a sketch from the [Inspector](../basics/working-with-things/inspector.md) by clicking on the **Convert to Sketch** action.

## Unity 2022

FirstStage has now moved to the Unity 2022 platform (previously we were on 2020). This has enabled many improvements particularly the support for live collaboration.

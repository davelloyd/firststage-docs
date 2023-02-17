# Audio

You can play audio clips in the scene by going to the [Asset Library](../asset-library.md) and placing an **Audio Source** in the scene.

As well as standalone sources, some things come with their own sources: for example, character puppets have a source for their voice which is used when playing back recorded dialog.

Audio sources can be either 2D (Stereo, independent of where the source is relative to the mic) or 3D (positional, depending on where the source is relative to the mic) or anywhere inbetween.

There is a simple mixing desk on the [WristPad](../wristpad/) which has a control strip for each source:

<figure><img src="../../.gitbook/assets/Controls Demo 2023-02-15 01-16-57.jpg" alt=""><figcaption></figcaption></figure>

**Volume** sets how loud the source is (1 is 0dB).

**Spatial Blend** sets the blend between stereo and positional sound (0 is stereo, 1 is full positional).

**Distance** sets the range of the source. You won't hear it beyond that range and the volume will reduce as you approach the limit.

The **Import** button lets you find an audio clip and play it on the audio source: you will find an entry on the timeline for it.

There is also a **Record Arm** button if you want to automate the levels so they vary during the scene.

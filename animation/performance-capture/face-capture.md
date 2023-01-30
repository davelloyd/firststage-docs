# Face Capture

You can use an iPhone X or later (must support face tracking) with FirstStage to capture facial animation. You will need to install the [Unity Face Capture app](https://apps.apple.com/us/app/unity-face-capture/id1544159771) on your phone to do so.

Face Capture is controlled from the \[Desktop interface] rather than VR. If the Motion Capture window is not showing go to the drop down menu (top right) and click on it to make it appear.

Facial animation will only work with puppets with suitable blendshapes on the face (see \[Importing a Character] for details). Some puppets may only have a jaw bone to animate the face: for these you will at least get basic “mouth flap” which may be sufficient for background characters. Most of the standard FirstStage character assets work with facial animation as do characters from ReadyPlayerMe or Reallusion Character Creator.

### Companion App <a href="#_7b85nyjzki5z" id="_7b85nyjzki5z"></a>

Start the Face Capture companion app on your device and Connect to the computer running FirstStage ([this may help](https://docs.unity3d.com/Packages/com.unity.live-capture@2.0/manual/setup-network.html) if you have problems connecting).

\[IMAGE: iPhone app]

### Assign a Character <a href="#_qguoinbue5tm" id="_qguoinbue5tm"></a>

The Motion Capture window should now show a source for your device in the left hand column. If you select it (if it’s the only one, it will be selected by default) the right hand pane will show the device name and a drop down menu which will allow you to assign the device to one of your characters. Initially it will be Unassigned. Choose the character for which you’d like to record some facial animation.

It is often helpful to create a camera targetting your character in close up. Then select that camera in the \[Camera Sequencer] so you can see how your character is responding to your facial performance.

### Filters <a href="#_5g9wg0kezr23" id="_5g9wg0kezr23"></a>

\[IMAGE: Motion Capture window]

Every character responds to facial animation differently depending on how it is rigged and the quality of its facial blendshapes. You can tailor your performance to the puppet but to make it easier, each of the main areas of the face - Jaw, Mouth, Eyes, Brows, Cheeks and Tongue - has a filter applied.

For each facial channel, there is a slider where you can set the range of expression to be used: if your character is prone to extreme expressions, reduce the upper limit; if your character seems to mumble, raise the lower limit. Underneath each slider, there is also a dial that lets you set the gain on each channel: gain is applied after the range reduction.

Experiment to get the best match between your expressions and the character’s.

### Record Voice <a href="#_kxivavagvbnr" id="_kxivavagvbnr"></a>

You can either record the performer’s voice at the same time or simply “mouth over” an existing dialogue track (or music track).

### Recording the Performance <a href="#_eyj24o2tcrnb" id="_eyj24o2tcrnb"></a>

Simply press Record on the \[Transport Controls] to record the performance and then press stop when done.

Afterwards, there will be a Face Mocap activity on the timeline for that character. You can move it about freely and you can also trim it to remove any start up or cool down.

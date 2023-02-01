# Camera Sequencer

The Camera Sequencer is a simple linear editor allowing you to cut between any of the cameras in the scene onto a Master track. This track can then be rendered and exported to video.

The Camera Sequencer does not support clips from other scenes or allow clips to overlap in time. However the timeline does not have to be full: any gaps will not be rendered, allowing dead time to be skipped.

For more sophisticated editing, export the video and import to your preferred non-linear editor of choice (e.g., Adobe Premiere, Final Cut, DaVinci Resolve, et al.)

The Camera Sequencer is available from the desktop.

The left hand column shows a list of thumbnails for all available cameras. Click on one of the cameras to see it in the central monitor.

### Cutting between cameras <a href="#_ci5ol683wfim" id="_ci5ol683wfim"></a>

Press the **Cut** button to create a clip on the timeline for current camera.

You can drag the clip along the timeline. You can also grab either end of the clip to trim the in and out points in time for that clip.

At the left end of the timeline is a thumbnail which shows the current master output. You can click on it to show the master in the central monitor.

### Exporting the master track <a href="#_3ggvbcwpyggc" id="_3ggvbcwpyggc"></a>

Press the **Export** button to export the video as a sequence of frames (to avoid temporal compression artefacts).

The video is placed in a folder in \<User>/Videos/\<Scene>\<Date>

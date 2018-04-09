---
image:
    thumbnail: /assets/images/teaser/short.jpg
---

From spring of 2016 through spring 2017, I worked with a team on an animated short film project as the technical director. I also did work in story development and writing, and modeling.

As TD, I worked to develop the entire pipeline for the project in conjunction with the Director and Pipeline TD. This culminated in the production of a complete document explaining our software choices, naming conventions, file management protocol, and a number of other important details. Through the course of the project, this pipeline changed significantly, but it served as a good base to get the project started. We used Maya, OptiTrack Motive, Substance Painter, and ZBrush for the core of our pipeline. Files were managed through a Git repository, with a custom hook written to notify the team of new commits via a Slack channel.

I was also been integrally involved in the motion capture pipeline. Prior to this project, the DMD department had no well documented pipeline for cleaning motion capture data, and all capture was done by recording joint angle data in MotionBuilder. The new workflow I developed was based on new documentation available from OptiTrack, and cleans up the data at the marker level, allowing for corrections in incorrectly assigned markers and filling gaps for occluded markers. A MotionBuilder preview is also used when recording to allow for previewing characters within the set. I also have experimented with relocating some of the motion capture cameras to reduce occlusion in particularly difficult shots. Retargeting is done directly in Maya to minimize the number of different software packages that an animator is required to use.

My largest responsibility was rigging the main characters for the project. The rigs needed to be usable by animators who didn't have a significant amount of experience in Maya, while still being flexible enough to accomodate any preferred style of animation. The rigs also needed to be able to seamlessly accept motion capture data without significant modification and blend between motion capture and fully manual animation. The rigs I developed share the same body base, allowing animators who are familiar with one of the rigs to work easily on any of the other ones. The rigs have Fk/IK switching legs and arms, smart foot roll, pose + FK hand controls, and a number of other useful features. The rigs use Maya's HIK system for retargeting. Below is a demo video of the rig's features.

Unfortunately, due to issues with scope and time constraints, the project was never completed. The character rigs were the last asset I delivered for the project.

{% include video id="199577618" provider="vimeo"%}
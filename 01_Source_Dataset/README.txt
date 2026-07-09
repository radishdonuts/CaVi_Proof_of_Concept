Source Dataset
==============

raw_videos
    Original input videos for COL_PH, SUN, EVE, and MID.

validated_ground_truth
    Validated STOP-frame references for the four video groups.

Video Mapping
-------------
COL_PH  col_ph1.mp4
SUN     sunset_6fps_17mins.mp4
EVE     evening_6fps_17mins.mp4
MID     midnight_6fps_17mins.mp4

The source videos are encoded at approximately 30 FPS. The research pipeline
samples them onto a 6 FPS processed timeline. In result files,
source_frame_idx identifies the original source-video frame and frame_idx
identifies the processed frame.

Ground truth marks STOP frames only. Any evaluated frame not marked as STOP
is treated as NON-STOP for STOP reliability validation.

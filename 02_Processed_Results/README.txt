Processed Results
=================

frame_results
    Per-frame raw and Zero-3DCE-enhanced outputs. Use source_frame_idx as the
    primary key when matching results to ground truth.

raw_annotated_videos
    Raw-input CaVi annotations at 6 FPS.

zero3dce_enhanced_annotated_videos
    Zero-3DCE-enhanced CaVi annotations at 6 FPS.

summary_tables
    Pipeline-generated summary outputs for each video group and condition.

side_by_side_evidence_reels
    Full or selected side-by-side visual comparisons and the scripts and CSVs
    used to prepare them.

Current Result Sets
-------------------
COL_PH  col_frame_results_raw.csv / col_frame_results_enhanced.csv
SUN     sun_frame_results_raw.csv / sun_frame_results_enhanced.csv
EVE     eve_frame_results_raw.csv / eve_frame_results_enhanced.csv
MID     mid_frame_results_raw.csv / mid_frame_results_enhanced.csv

The current COL_PH files correspond to col_ph1.mp4 and each contain 436
processed frames. Files prefixed with old_col and the side_by_side_evidence_
reels/old COL folder are historical outputs and are not part of the current
COL_PH metric result.

The annotated videos and evidence reels in this folder are the archived
research outputs. The interactive proof of concept is available at:
https://huggingface.co/spaces/klowzopen/cavi-zero3dce-prototype

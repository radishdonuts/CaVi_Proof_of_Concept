CaVi Proof of Concept
======================

Purpose
-------
This package contains the source data, processed results, model checkpoints,
and notebooks for the CaVi + Zero-3DCE collision-risk proof of concept.

The study evaluates whether Zero-3DCE improves the reliability of CaVi STOP
labels under low-light conditions. Its main result is the reduction of false
STOP outputs while correct STOP detection is maintained or improved.

Start Here
----------
1. Open the hosted proof-of-concept website:
   https://huggingface.co/spaces/klowzopen/cavi-zero3dce-prototype
2. Open 02_Processed_Results to inspect the complete CSV results and annotated
   videos used for analysis.
3. Open 04_Notebooks to inspect the research pipelines and supporting models.
4. Use 01_Source_Dataset and 03_Model_Checkpoints when reproducing the work.

Package Contents
----------------
01_Source_Dataset
    Original videos and validated STOP ground truth for COL_PH, SUN, EVE,
    and MID.

02_Processed_Results
    Raw and Zero-3DCE-enhanced frame results, annotated videos, summary
    outputs, and side-by-side evidence reels.

03_Model_Checkpoints
    Depth Anything V2, instance-segmentation, and Zero-3DCE model weights.

04_Notebooks
    The unified four-bin pipeline and the individual model notebooks.

Validation Scope
----------------
Ground truth marks frames that should be treated as STOP events. Frames not
marked as STOP are treated as NON-STOP. For STOP validation, STOP is a
predicted STOP, while CLEAR and WARNING are non-STOP outputs.

STOP reliability metrics are calculated from the complete frame_results CSV
timeline for each video group. The side-by-side reels are selected visual
evidence and are not the metric denominator.

Official COL_PH Results
-----------------------
Use the current files named col_frame_results_raw.csv and
col_frame_results_enhanced.csv. They correspond to col_ph1.mp4 and contain
436 evaluated frames. Files prefixed with old_col and material under old COL
are retained only as historical outputs and must not be used for current
COL_PH reporting.

Storage and Publication
-----------------------
The complete package is suitable for OneDrive, Google Drive, or another
large-file repository. The interactive proof of concept is hosted separately
on Hugging Face Spaces:
https://huggingface.co/spaces/klowzopen/cavi-zero3dce-prototype

Standard GitHub storage is not suitable for the complete package because of
the video and checkpoint sizes. Use Git LFS or publish the source code
separately from the large research artifacts.

# ANISE: Assembly-based Neural Implicit Surface rEconstruction

This is the official code for **ANISE**, an efficient neural part-aware shape representation that models 3D shapes as collection of neural part implicits that are assembled in the full shape. This representation allows for editable part-aware single-view and point cloud reconstruction and reconstruction conditioned on small set of reference parts. We establish current state-of-the-art in part-aware single view reconstruction and reconstruction based on part-retrieval.  

**ANISE: Assembly-based Neural Implicit Surface rEconstruction**

[**Project Page**](https://lodurality.github.io/ANISE/) | **Paper** ([TVCG](https://ieeexplore.ieee.org/abstract/document/10093999))

## ANISE pipeline
<p align="center"><img src="https://lodurality.github.io/ANISE/assets/anise_summary_cropped.png" width="100%"></p>

**An overview of our approach.** ANISE consists of three modules. The first module predicts a coarse part arrangement in the form of part transformations (_structure prediction_). Then, conditioned on these part transformations, the next module predicts an implicit function representing the actual geometry (_geometry prediction_). The last module transforms each part implicit functions according to the predicted transformations and combines them into a single output implicit function (_assembly_).

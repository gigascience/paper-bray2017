Supporting data for "A dataset of images and morphological profiles of 30,000 small-molecule treatments using the Cell Painting assay"
===============================================================================

Bray, M-A; Gustafsdottir, S, M; Rohban, M, H; Singh, S; Ljosa, V; Sokolnicki, K, L; Bittker, J, A; Bodycombe, N, E; Dančík, V; Hasaka, T, P; Hon, C, S; Kemp, M, M; Li, K; Walpita, D; Wawer, M, J; Golub, T, R; Schreiber, S, L; Clemons, P, A; Shamji, A, F; Carpenter, A, E
2016. GigaScience Database. http://dx.doi.org/10.5524/100200

Contact:
--------
Anne E. Carpenter, Ph.D.
Director, Imaging Platform
Broad Institute of Harvard and MIT
anne@broadinstitute.org, http://www.broadinstitute.org/~anne

Summary:
--------
This microscopy data set includes 919,874 five-channel fields of view representing 30,616 tested compounds, available at 'The Cell Image Library' repository. It also includes data files containing morphological features derived from each cell in each image, both at the single-cell level and population-averaged (i.e., the per-image level); the image analysis workflows that generated the morphological features are also provided. Quality-control metrics are provided as metadata, indicating fields of view that are out-of-focus (blurry) or containing highly fluorescent material or debris. Lastly, chemical annotations are supplied for the compound treatments applied.

Files:
------
The raw image data described in this article is also available at 'The Cell Image Library' repository as Plates 24277-26796. 
All data relating to a plate are within a folder named after the unique 5-digit identifier for each plate. This includes;
 illumination correction functions,
 metadata related to sample treatment
 image quality control,
 extracted morphological features,
 profiles,
With each data type existing in a separate sub-folder within the parent plate-ID folder. Each of the plate folders has been packed as tape archive (TAR, .tar), before being compressed using GNU Gzip (.gz) and can be downloaded individually.

download_cil_images.sh - A bash shell script to facilitate downloading the entire image set from  'The Cell Image Library' repository in batch.

chemical_annotations.csv - Table containing metadata for many of the compounds from Broad Institute’s Chemical Biology Informatics Platform (CBIP), including (where applicable) compound names, simplified molecular-input line-entry system annotations (SMILES), MLSMR sample identifiers, and PubChem compound identifiers (CID) and substance identifiers (SID).

pipelines.zip - The CellProfiler pipelines including illum.cp, analysis.cp and quaity_control.cppipe. All created using CellProfiler software. 

image_curation_statistics.csv - Table summarizing the curation statistics. The following items are listed for each plate; 
 - Plate ID: 5-digit identifier given by the ImageXpress microscope labeling the plate. 
 - Num_CIL_images: Total number of images for the plate hosted at The Cell Image Library (CIL).
 - Num_CIL_wells: Total number of wells represented in the plate hosted at CIL which have >1 site (i.e., field of view) included.
 - Num_CIL_complete wells: Total number of wells which have all sites included.
 - Num_CIL_sites: Total number of sites which have >1 channel included.
 - Num_CIL_complete_sites: Total number of sites which have all channels included.
 - Num_QC_stats: Total number of sites for which quality control data is included.
 - Num_blurry_sites: Total number of sites labelled as blurry/out-of-focus by the quality control workflow.
 - Num_saturated_sites: Total number of sites labelled as containing saturation artifacts by the quality control workflow.

COPYRIGHT
To the extent possible under law, Anne Carpenter has waived all copyright and related or neighboring rights to this dataset. This work is published from: United States.

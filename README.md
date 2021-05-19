# Scene-Segmentation
Scenes from various movie clips can be segmented by obtaining their intensity histograms and finding their similarity via a variety of distances. The exact steps performed are listed below:
  - Extract each individual frame from the movie clip
  - Pre-process each frame by downscaling, converting to grayscale, scaling image intensity values to range between 0 and 255 and reducing     noise by applying a Gaussian filter
  - Define the distance functions used: Correlation, Chi-squared, Intersection, Bhattacharyya
  - Calculate the histogram for each frame
  - Compare histograms by calculating the distance between them (with any of the above mentioned distance metrics) and a threshold obtained     via experimentation
  - Group frames into scenes accordingly
 
Results are in the form of a list of annotations containing the start and end frames of each segmented scene. A pre-defined list of annotations for each clip in the dataset provied below may be used as a reference for the results. A bried report is also included showcasing and discussing the results of a sample clip which was segmented.

**Dataset**

The Open Video Scene Detection Dataset (OVSD) was used as the source of the clips to be segmented. Also included are annotations of scenes for each clip.

https://www.research.ibm.com/haifa/projects/imt/video/Video_DataSetTable.shtml

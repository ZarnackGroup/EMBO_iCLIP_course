# iCLIP2 EMBO course 2024

Welcome to the bioinformatics part of the course! 

We have two practical sessions for you.

## Practical 1 - Exploring CLIP data with the UCSC genome browser

In this task, you will explore crosslink profiles and binding sites defined by different tools. We uploaded crosslink profiles of CSTF2 and SF3B1 to the UCSC genome browser for you. Have a look at https://genome.ucsc.edu/s/melinak/How_to_define_binding_iCLIP2_EMBO_course_bioinformatics_practial1. Go through the tasks below and make screenshots of the examples you find, so we can discuss your examples in the end.

- CSTF2 is a polyadenylation factor. Find some examples of crosslink peaks at polyadenylation sites and alternative polyadenylation sites. Are these sites also annotated in the genome annotation?

- For SF3B1 we uploaded the crosslinks from two different experiments: A very deep iCLIP2 experiment from Pacholewska *et al.* 2024 (https://doi.org/10.1101/2024.01.26.576051) and a less deep eCLIP experiment from the ENCODE database. Find some examples of overlaps and discrepancies in the crosslink profiles from both experiments.

- There are different methods to define binding sites CLIP data. We included in the session also crosslink peaks from PureCLIP, binding sites from BindingSiteFinder and enriched binding regions from DEW-seq. Compare the binding sites from the different methods.
  
- Another tool often used for binding site definition is clipper. Clipper binding sites are also provided in the ENCODE database for all ENCODE data sets. Add the clipper binding sites for CSTF2 to the UCSC genome browser session (see institutions below) and compare the binding sites to the other methods.

### How to load ENCODE data to the UCSC genome browser

- Go to https://www.encodeproject.org/ and click **Data > Experiment search**.
- Type your protein of interest in the **Search** field in the top right corner.
- On the left, you can choose **Data type > Dataset** to reduce the number of results. Then select the CSTF2 HepG2 eCLIP data set. You will now see a summary of this experiment.
- Scroll down to **Files** and click on **Output type > peaks** in the bar on the left to select the clipper peaks.
- Now you can click **Genome browser** to directly see the clipper peaks in a genome browser.
- To load the clipper peaks to the UCSC session with the other tracks, go to **File details** and click **Visualize**.



## Practical 2 - Finding binding motifs with XSTREME

In this task, you will predict binding motifs based on the sequences of binding sites. For this, we will use the XSTREME algorithm, which is part of the MEME suite. We provide you with fastq files from CSTF2, RBFOX2 and PUM2 binding sites.

- Go to the XSTREME web application at https://meme-suite.org/meme/meme_5.5.4/tools/xstreme.
- Upload the fastq file with **Browse** and choose the following settings:
  xx
  




# iCLIP2 EMBO course 2024

Welcome to the bioinformatics part of the course! 

We have two practical sessions for you.

## Practical 1 - Exploring CLIP data with the UCSC genome browser

In this task you will explore crosslink profiles and binding sites defined by different tools. We uploaded crosslink profiles of CSTF2 and SF3B1 to the UCSC genome browser for you. Have a look at https://genome.ucsc.edu/s/melinak/How_to_define_binding_iCLIP2_EMBO_course_bioinformatics_practial1. Go through the tasks below and make screen shots of the examples you find, so we can discuss your examples in the end.

- CSFT2 is a polyadenylation factor. Find some examples for crosslink peaks at polyadenylation sites and alternative polyadenylation sites. Are these sites also annotated in the genome annotation?

- For SF3B1 we uploaded the crosslinks from two different experiments: A very deep iCLIP2 experiment from Pacholewska *et al.* 2024 (https://doi.org/10.1101/2024.01.26.576051) and a less deep eCLIP experiment from the ENCODE data base. Find some examples for overlaps and discrepacies of the crosslink profiles from both experiments.

- There are different methods to define binding sites CLIP data. We included in the session also crosslink peaks from PureCLIP, binding sites form BindingSiteFinder and enriched binding regions from DEW-seq. Another othen used tool for binding site definition is clipper. Clipper binding sites are also provided at the ENCODE data base for all ENCODE data sets. Add the clipper binding sites for CSFT2 to the UCSC genome browser session (see instrcutions below) and compare the binding sites from the different methods.

### How to load ENCODE data to the UCSC genome browser

- Go to https://www.encodeproject.org/ and click **Data > Experiment search**.
- Type your protein of interest in the **Search** field on the top right corner.
- On the left you can choose **Data type > Dataset** to reduce the number of results. Then select the CSTF2 HepG2 eCLIP data set. You will now see a summary of this experiment.
- Scroll down to **Files** and click on **Output type > peaks** in the bar on the left to select the clipper peaks.
- Now you can click **Genome browser** to directly see the clipper peaks in a genome browser.
- To load the clipper peaks to the UCSC session with the other tracks, go on **File details**
- Find the bed file for the geome annotation GRCh38, that combines both replicates, download and unzip it.
- Open the bed file with a text editor. Then add the following first line to the file and save it:
  
  **track type=narrowPeak visibility=3 name="name_of_your_track"**

  (you can choose the name of the track with the "name = " setting)
- Now go back to the UCSC browser session and click **My Data** > **Custom Tracks**, select the bed file with **Browse** and **Submit**.
- Go back to the Genome Browser view by clicking **return to current position**, the newly uploaded track should be at the top.
- Right click the new track in the left bar and select **dense** for better visualisation.



## Practial 2 - Finding binding motifs with XSTREME

In this task, you will predict binding motifs based on the sequences of binding sites. For this we will use the XSTREME algorythm, which is part of the MEME suite. We provide you with fastq files from CSTF2, RBFOX2 and PUM2 binding sites.

- Go the the XSTREME web application at https://meme-suite.org/meme/meme_5.5.4/tools/xstreme.
- Upload the fastq file with **Browse** and choose the following settings:
  xx
  




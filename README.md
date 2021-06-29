# Protein-arginine-phosphorylation

These scripts where used in the data analysis of the described paper below. These scripts read in all necessary MQ output files which are deposited on Pride. The accession number will be published after the manuscript is accepted.

The scripts analyze the stability of synthetic pArg, fragmentation characteristics as well as retention time. 

**Extensive arginine phosphorylation in Staphylococcus aureus is influenced by Stp1**

Nadine Prust<sup>1,2</sup>,  Pieter C. van Breugel<sup>1,2</sup> and Simone Lemeer<sup>1,2,#</sup>

<sup>1</sup>**Biomolecular Mass Spectrometry and Proteomics**, Bijvoet Center for Biomolecular Research and Utrecht Institute for Pharmaceutical Sciences, Utrecht University, Padualaan 8, 3584 CH Utrecht, The Netherlands
<sup>2</sup>**Netherlands Proteomics Center**, Padualaan 8, 3584 CH Utrecht, The Netherlands

*<sup>#</sup>Correspondence to: Simone Lemeer, s.m.lemeer@uu.nl*

## Instructions for use

### Environment
The code is embedded in RMarkdown documents, one per analysis. RStudio (https://rstudio.com, no affiliation) is a convenient environment for "knitting" these documents, to create HTML or PDF output. The following packages need to be installed in R:

* tidyverse
* ggpubr
* reshape2
* stringr
* colorspace
* ggforce
* RColorbrewer
* VennDiagram
* psych

### Obtain the markdown documents
To obtain these documents, use git (available in RStudio as well) to download ('clone') the documents, or simply download the files as a zip file. The URL for cloning, or the link to download the zip, are availabe under the green "Code" button above the file listing.
We have added a project file for convenience, so you can double-click it to open the project in RStudio.

### Obtain the data
No data (MaxQuant output .txt files) is available in this repository, it needs to be downloaded from the Pride archive.
From there, obtain the MQ_output_txt.zip file and extract it in the same directory as the markdown documents. The scripts will locate the required .txt file in the subfolder and load all necessary libraries. 
Second, open the .Rmd file you are interested in and 'knit' the document. The scripts will generate the plots used in the above mentioned paper. 

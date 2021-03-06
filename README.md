# HyDML

A hybrid ensemble feature selection method for identifying differential methylation sites. HyDML uses R to implement the feature selection, 
and through the hybrid ensemble framework, it can achieve robust differential methylation sites selection.

# Installation

Download source code of HyDML by

https://github.com/TQBio/HyDML.git

1)Installation has been tested in Linux with R 3.4.4.

2)HyDMl uses the following dependencies: e1071; ecodist; glmnet; rmcfs; MDFS; sampling; pROC; 

You can install these packages first, by the following commands:

install.packages("e1071")

install.packages("ecodist")

install.packages("glmnet")

install.packages("rmcfs")

install.packages("MDFS")

install.packages("sampling")

install.packages("pROC")

Analysis function.r --- Some processing and functional functions for analyzing the obtained differential methylation sites.

HyDML_Main.r --- The set of main functions for HyDML, including sampling, feature selection, etc.

HyDML_preprocess.r --- The preprocessing function for methylation data from TCGA.

HyDML_preprocess_demo.r --- A example pipeline for the preprocessing of methylation data from TCGA.

# Data

We also uploaded differential methylation sites selected for each cancer data set and published the data for follow-up studies.

Additionally, we uploaded the "SNP" file to address the DML which were marked as a SNP in annotation file and it's accessible under 

"HyDML/Data/SNP/" file.


# Demo demonstration

You can download the "easy version" of HyDML from HyDML_demo.r and download the data from "Data" file;

then you can implement the analysis of robust DML selection with R/RStudio. 

You also could use HyDML for other feature selection domains with robustness problems, just make sure the input is a formal 'dataframe'
style.

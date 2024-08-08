

## DNA Methylation Signatures Underpinning Blood Neutrophil to Lymphocyte Ratio During First Week of Human Life

This repository contains the code and analysis scripts used in the study of epigenetic changes during human immune ontogney. 
The research investigates the dynamic epigenetic landscape across various postnatal time points (DAYS OF LIFE (DOL)0,1,3,7), providing insights into the regulatory mechanisms underlying developmental processes.

---

## Project Overview
This project aims to:

1. Characterize DNA methylation patterns in human whole blood samples over the first week of life.
2. Identify differentially methylated regions (DMRs) associated with days of life.
3. Explore the functional relevance of identified DMRs in relation to gene regulation.
4. Understand the dynamic landcape of immune cell populations and their associations with changing DNA methylation patters.
5. Explore potential genetic determinants.


## Data
The data used in this study were obtained from whole blood samples collected from human newborns at different postnatal time points. Detailed information about the samples, including demographics and collection procedures, can be found in the associated research article.

## Analaysis

The data analysis includes the following steps:

1. Quality Control: Extract control probe principal components from raw data: 00_Ctrl_Probe_Intensities.Rmd
2. Exploratory PCA analysis of EPIC-002 and EPIC-003 Gambian cohorts: 01_Data_prep_PCA.Rmd.
2. Cell-Type Deconvolution with EpiDISH: 02_cellcountanalysis.Rmd
4. Identify DMRs associated with DOL and using statistical models: 03_combined_ewas.Rmd
5. Annotating DMRs to genomic regions: 04_DMR_annot.Rmd
6. Differentially methylated cell type analysis: 05_DMCT.Rmd
7. Association of neutrophil to lymphocyte ratios with neonatal sepsis: 06_Sepsis.Rmd
8. Causal mediation analysis of transcription factors
9. Integrative anlaysis with RNA-seq: mCSEA.Rmd


---

## Packages

DNA methylation analysis was performed using the following Bioconductor packages:
Preprocessing of Illumina methylation array data was performed using Minfi (v1.40.0).
EpiDISH (v2.10.0) for cell-type deconvolution, 
Limma (v3.50.3) for differential methylation analysis, 
mixOmics (v6.18.1) for within subject variance estimation, 
DMRcate (v2.8.5) for identification of differentially methylated regions, 
MissMethyl (v1.28.0) for imputation of missing methylation values, mCSEA (v1.14) for methylation enrichment analysis, and 
methylclock (v1.0.1) for estimating epigenetic age acceleration. 
The tidyverse suite of packages (v2.0.0) was employed for data manipulation and visualization. 
Mediation analyses were performed using the mediation package (v4.5.0), and linear mixed effects models were fitted using lmerTest (v3.1-3).

## Associated Publication
The results of this analysis are described in detail in the following research article:


## Contact
For questions or feedback please contact the corresponding author:
david.martino@uwa.edu.au

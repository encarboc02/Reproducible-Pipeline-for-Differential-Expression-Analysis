# Reproducible-Pipeline-for-Differential-Expression-Analysis
This repository contains a reproducible RMarkdown pipeline for performing differential gene expression analysis using RNA-Seq data from the mouse hippocampus. The analysis is a practice exercise and is not intended to produce biologically significant results. It includes:

  -Data preprocessing and quality assessment (FastQC, Salmon)
  -Differential expression analysis using DESeq2
  -Exploratory data analysis (PCA, heatmaps)
  -Gene annotation using biomaRt and AnnotationHub
  -Functional enrichment analysis (GSEA, GO)

The workflow is designed to be fully reproducible and is suitable for training purposes.

## Pipeline Steps

  1. Set up the working directory and load libraries
  2. Import and quantify transcript-level counts using Salmon and tximport
  3. Create tx2gene mapping from Gencode annotation and add gene symbols using biomaRt
  4. Perform differential expression analysis with DESeq2
  5. Normalize counts and perform exploratory data analysis (PCA, heatmaps)
  6. Identify differentially expressed genes
  7. Visualize results using volcano plots and heatmaps
  8. Perform gene annotation and enrichment analysis (GSEA, GO: Biological Process, Molecular Function, Cellular Component)

Note: For this practice analysis, a permissive adjusted p-value cutoff of 0.5 is used. For biologically meaningful results, the adjusted p-value should be 0.05 or lower.

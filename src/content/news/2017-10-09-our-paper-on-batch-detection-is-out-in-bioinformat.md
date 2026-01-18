---
title: "Our paper on Batch Detection is out in Bioinformatics!"
date: 2017-10-09
summary: "DASC batch detection algorithm published in Bioinformatics, demonstrating superior performance in identifying hidden batch effects in RNA-seq data."
---
---

Ayush's paper on batch detection is out now! Congrats Ayush!

Detecting hidden batch factors through data adaptive adjustment for biological effects

DASC, the batch detection tool is available in Bioconductor: https://bioconductor.org/packages/devel/bioc/html/DASC.html

Abstract
Motivation: Batch effects are one of the major source of technical variations that affect the measurements in high throughput studies such as RNA sequencing. It has been well established that batch effects can be caused by different experimental platforms, laboratory conditions, different sources of samples and personnel differences. These differences can confound the outcomes of interest and lead to spurious results. A critical input for batch correction algorithms is the knowledge of batch factors, which in many cases are unknown or inaccurate. Hence, the primary motivation of our paper is to detect hidden batch factors that can be used in standard techniques to accurately capture the relationship between gene expression and other modeled variables of interest.
Results: We introduce a new algorithm based on data-adaptive shrinkage and semi-Nonnegative Matrix Factorization (NMF) for the detection of unknown batch effects. We test our algorithm on three different datasets – 1) Sequencing Quality Control (SEQC), 2) Topotecan RNA-Seq and 3) Single-cell RNA-Seq on Glioblastoma Multiforme (GBM). We have demonstrated a superior performance in identifying hidden batch effects as compared to existing algorithms for batch detection in all three datasets. In the Topotecan study, we were able to identify a new batch factor that has been missed by the original study, leading to under-representation of differentially expressed genes. For scRNA-Seq, we demonstrated the power of our method in detecting subtle batch effects.

&nbsp;

&nbsp;


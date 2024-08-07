# **Figure1Lab-InternshipEmulator_singlecellRNASeq**
## **Introduction**
This repository is meant to contain the work done in the process of attending the F1L Internship Emulator. Through this project, I will hopefully learn the basics of bioinformatics and computational biology and what it actually means to derive meaning from biological data using computational methods.

The repository will be split into weeks, corresponding to the ones described in the F1L newsletter.

## **WEEK 1**
The first week of the emulator has more of an introductory role, addressing the inception of formulating a scientific question. By breaking down the question that was provided into its constituent components, I will be able to understand the key concepts and work towards deepening my knowledge. The original question is as follows:

**Using available scRNA-seq data from cancer cell lines, how would you explore the use of the following FDA-approved antibody therapies in additional cancers?**

**Trastuzumab**: Targets HER2 and is used in the treatment of HER2-positive breast and gastric cancers.

**Bevacizumab**: Targets VEGF and is used for a variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer.

We need to identify and dissect the various elements involved to break down the key scientific question into its constituent components. Here's a detailed breakdown:

**What are we trying to explore?**
The potential use of trastuzumab and bevacizumab in cancers beyond their current FDA-approved indications.

**Why is this exploration important?**
To potentially expand the therapeutic use of existing antibody therapies, leading to improved treatment options for other cancer types.

**What is scRNA-seq?**
Single-cell RNA sequencing (scRNA-seq) is a technique that allows for the analysis of gene expression at the single-cell level.

**Why use scRNA-seq data from cancer cell lines?**
Identify gene expression patterns and molecular characteristics that may indicate responsiveness to antibody therapies.

**Trastuzumab:**
Target: HER2 (Human Epidermal Growth Factor Receptor 2)
Current Use: HER2-positive breast and gastric cancers.
Potential New Targets: Other cancers with overexpression or amplification of HER2.

**Bevacizumab:**
Target: VEGF (Vascular Endothelial Growth Factor)
Current Use: A variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer.
Potential New Targets: Other cancers with significant VEGF-driven angiogenesis.

## **WEEK 2**

I feel like the best way to answer these questions is with the exact sections in the article that reflect them.

**1. How did the authors handle the potential caveat of co-culturing cell lines before profiling by scRNA-seq? Why do you think that caveat was or was not adequately addressed?**

First, the patterns of heterogeneity were as similar between cell lines from the same pool as between cell lines of different pools (fig. S1B). Second, a control experiment was performed in which six cell lines were profiled with and without co-culturing for 3 days. Co-culturing had a modest effect on average gene expression in each cell line, while patterns of heterogeneity were highly consistent between the two conditions (fig. S1C–F).

**2. The authors identified discrete subpopulations of cells within a subset of individual cell lines (Fig. 2A-B). What might be the reason why some cell lines have these discrete subpopulations while others do not?**

Discrete clusters of cells within a cell line were found only for a minority (11%) of the cell lines: three cell lines had three or more clusters, three had two clusters of comparable sizes, and 16 had one major and one minor cluster (Fig. 2B and S2B). For each such cluster, we identified the top 50 upregulated genes compared to all other cells from the same cell line (Table S2). These expression programs showed limited similarities to one another, both within cell lines of the same cancer type and across different cancer types, **indicating that discrete subpopulations are typically unique and cell line-specific (Fig. 2C).**

**3. What are Recurrent Heterogeneous Programs (RHPs) and how were they defined?**

Recurrent Heterogeneous Programs (RHPs) are defined using robust expression programs, which are consistently observed as variable using different parameters. Robust expression programs are both continuous and discrete. By hierarchically clustering the NMF programs based on their shared genes, the RHPS can be identified, as being present in multiple cell lines.

**4. How do the identified RHPs relate to in vivo programs of heterogeneity in tumors, and what evidence supports this relationship?**

In vivo RHPs were defined previously in HNSCC5, melanoma6, glioblastoma24, and ovarian cancer25, and we defined additional RHPs by NMF analysis of scRNA-seq datasets in HNSCC5, melanoma6, breast cancer9 and lung cancer12 samples (fig. S3A and Table S7). Strikingly, 7 out of the 10 cell line RHPs are highly similar to the in vivo RHPs, as defined by highly significant overlap of signature genes (Fig. 4A, FDR-adjusted p<10−9 by hypergeometric test), as well as by high correlation of cell scores (Fig. 4B). The in vivo relevance of cell line RHPs was further demonstrated in melanoma and in HNSCC by a combined analysis of cells from cell lines and tumors, demonstrating their common patterns of variation as described below (Fig. 4C–F and S5).

**5. Where can you download the scRNA-seq data as shown in Figure 1B?**
https://singlecell.broadinstitute.org/single_cell/study/SCP542/pan-cancer-cell-line-heterogeneity#study-download

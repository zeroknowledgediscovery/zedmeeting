Sep 23, 2026 (Summaries from the week)

AJE paper is ready to submit.

Correlation matrix for a nonnumeric data?

Parsing the data 98% done in around 48 hours. 

<p align="center">
  <img src="IMG/gss_pert.png" width="600">
  <br>
  <em>Figure 1: Stability for the GSS 2018 dataset.</em>
</p>

Comments: 

1) AJE paper: add a newer synthetic data generator
2) Drift metric, maybe a meeting with Anna on Friday
3) Metabolomic next
4) Regenerate the dataset for PNAS paper, dataset and model compression: binary trees
5) Non-categorical data: quantization (preprocessing) ultimately for the use of LSM model. IXC is gonna give me the dataset. (Metabolomics workbench)
     metabolomics dataset:

Metabolomics Workbench study: ST000923
Project: PR000639
Title: “Longitudinal Metabolomics of the Human Microbiome in Inflammatory Bowel Disease”
Associated paper: Lloyd-Price et al., Nature 2019, “Multi-omics of the gut microbial ecosystem in inflammatory bowel diseases”
Data: 546 longitudinal fecal metabolomic samples spanning non-IBD/healthy, ulcerative colitis (UC), and Crohn’s disease (CD)
Untargeted LC–MS data with >80,000 de-isotoped features; about 597 annotated compounds plus many unannotated features.
This is the dataset where we subsequently discussed/tried the LSM analysis using the first sample from each longitudinal series, with a held-out set of 150, and saw roughly 0.96 AUC for healthy vs UC+CD and very strong UC-vs-CD separation.

6) Metabolomics AUC has an err: not a true out of sample error. Deadline: Dec or Jan 

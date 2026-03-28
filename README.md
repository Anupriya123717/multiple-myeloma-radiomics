# multiple-myeloma-radiomics
Automated MRI texture analysis pipeline for Multiple Myeloma bone marrow profiling.
Project Overview
OncoMap E3 is an automated bioinformatics pipeline designed to quantify bone marrow heterogeneity in Multiple Myeloma (MM) patients. Using T1-weighted MRI data from the Cancer Moonshot Biobank (CMB-MML), this project implements a "Virtual Biopsy" framework to detect high-risk medullary phenotypes through non-invasive texture analysis.

 Methodology & Tech Stack
The pipeline utilizes Gray-Level Co-occurrence Matrix (GLCM) algorithms to extract spatial relationship features from DICOM imaging data.

Data Acquisition: Automated retrieval via tcia_utils (NBIA API).

Image Processing: pydicom for metadata handling and scikit-image for feature extraction.

Feature Set:  Dissimilarity: Measures local intensity variation (Tumor Heterogeneity).

Homogeneity: Measures structural uniformity (Marrow Integrity).

Energy & Correlation: Signal intensity distribution and linear dependency.
Key Results (17-Patient Cohort)
Our analysis successfully mapped the radiomic "fingerprint" of 17 patients, identifying significant outliers with aggressive textural signatures.

The "Chaos Score" Discovery
We developed a composite Chaos Score to identify patients with extreme medullary disruption.

Top 3 Outliers: MSB-04950, MSB-01865, and MSB-04031.

Clinical Significance: These patients exhibited a >70% increase in textural dissimilarity compared to the cohort mean, indicating advanced tumor infiltration.

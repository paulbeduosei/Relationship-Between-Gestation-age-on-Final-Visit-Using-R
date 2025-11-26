# Relationship Between Gestation Age on Final Visit

Exploring latent profiles of toxicant exposure and biomarker levels among pregnant women and their relationship with gestational age at the final visit.

This repository contains data analysis scripts (R) to:
- Summarize participant characteristics (age, BMI, specific gravity, education, insurance, race, etc.)
- Perform unsupervised clustering on exposure/toxicant variables (Gaussian mixture models via mclust, k-means)
- Visualize cluster-specific distributions for toxicants and derived toxicant scores
- Reduce dimensionality of endogenous biomarkers (PCA)
- Explore factor structure (factor analysis) of biomarker data
- Fit regression models and a penalized (LASSO) model to assess associations between exposures / factors and gestational age (or another outcome of interest)

Requirements
- R >= 4.0
- R packages:
  - readxl, tidyverse (includes dplyr, tidyr, ggplot2), psych, mclust, factoextra, NbClust, ggfortify, nFactors, GPArotation, glmnet, cluster, proxy

Usage
1. Place your data Excel file (example.xlsx) in a known folder.
2. Update the `filepath` in the analysis script (analysis.R) to point to your Excel file.
3. Run the script: Use the code from description.
4. Inspect generated plots and model output in the console / plots pane.

Notes
- The provided analysis script includes careful handling of clustering assignments, plotting functions, and placeholders for the outcome variable used in regressions. Make sure to set the correct columns for exposures, biomarkers, toxicant scores, and the outcome variable before running models.
- Where variable names differ in your data, adapt the column index ranges or names used in the script.

Contact
- Repository owner: paulbeduosei

# Multistage Random-Effects Survival Modeling in AML

## Overview

This project implements a **multistage random-effects (RFX) machine learning framework** to quantify the prognostic contribution of **DNA methylation** relative to genetic, cytogenetic, clinical, and demographic factors in Acute Myeloid Leukemia (AML).
The framework is based on the multistage random-effects survival model developed by **Gerstung et al.**, adapted and extended to incorporate incorporate DNA methylation epitypes and epitype-mutation interaction terms.

---

## Data Integrated

The model integrates multiple modalities of AML patient data:

* Recurrent genetic alterations
* Cytogenetics
* Clinical variables
* Demographics
* Treatment protocol (nuisance variables)
* DNA methylation epitypes
* Epitype–mutation interaction terms

---

## Modeling Components

* Random-effects structure by feature class
* Time-dependent survival modeling
* Bootstrap-based variance estimation
* Wald testing with FDR correction
* Variance component decomposition
* Multistage state-transition modeling

---

# Main Results: 

## Key Results

Previously in our publication, we show how AML patients can be divided into 13 subtypes/epitypes according to their global DNA methylation patterns. In order to assess the impact of DNA methylation among other prognostic markers, we used multistage random effects (RFX)  model combining recurrent genetic alterations with clinical and demographic prognostic markers and outperforming ELN genetic-risk classification in the Alliance AML cohort. Adding Epitypes and Epitypes:Genetic terms explained a substantial fraction of inter-patient variability (aroune 30%), exceeding reliance on genetic predictors. Using Overall Survival model, the top significant predictors were mostly epitype-derived.  

<p align="center">
  <img src="figures/overall_variance_vp.png" width="900">
</p>



### Creating Multi-stage Model 
<p align="center">
  <img src="figures/Multistage_model.png" width="650">
</p>

Increasing oncogenic burden is associated with progressively worse overall survival, demonstrating robust clinical risk stratification captured by the model.

---

### Variance Contribution Across Feature Classes
<p align="center">
  <img src="results/variance_components.png" width="650">
</p>

DNA methylation features explain a substantial fraction of inter-patient variability in survival outcomes, comparable to or exceeding traditional genetic and clinical predictors.

---

### Feature-Level Associations with Outcome
<p align="center">
  <img src="results/volcano_os.png" width="650">
</p>

Epitypes, SHS, and epitype–mutation interactions emerge as among the most significant predictors of outcome, highlighting biologically interpretable drivers.

---

### Multistage Disease Trajectories
<p align="center">
  <img src="results/multistate_transitions.png" width="650">
</p>

Multistate modeling captures dynamic transitions between remission, relapse, and death over time following AML diagnosis.










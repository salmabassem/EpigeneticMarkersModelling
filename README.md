# Multistage Random-Effects Survival Modeling in AML

## Overview

This project implements a **multistage random-effects (RFX) machine learning framework** to quantify the prognostic contribution of **DNA methylation** relative to genetic, cytogenetic, clinical, and demographic factors in Acute Myeloid Leukemia (AML).
The framework is based on the multistage random-effects survival model developed by **Gerstung et al.**, adapted and extended to incorporate incorporate DNA methylation epitypes and epitype-mutation interaction terms.

---
## Methodological Framework

###  Model Type

**Multistage Random Effects Cox Model**

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

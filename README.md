# Interpretability under Perturbation

This repository contains the full analytical pipeline accompanying the manuscript:

**“Interpretability as stability under perturbation reveals systematic inconsistencies in feature attribution”**

---

## Overview

Feature attribution methods are widely used to interpret machine learning models. However, it remains unclear whether attribution magnitude reflects the true functional importance of features.

This repository implements a unified interpretability framework that integrates:

- permutation-based feature attribution  
- feature ablation (structural perturbation)  
- model-level permutation diagnostics  
- stability analysis across feature spaces  

The central finding of this work is that:

> **Interpretability does not arise from attribution magnitude alone, but from stability under perturbation.**

---

## Key Concepts

The framework introduces several core concepts:

- **Attribution magnitude** – sensitivity of model predictions to feature permutation  
- **Functional importance** – change in model performance after feature removal  
- **Stability** – consistency of feature behavior across perturbations  
- **Feature Reliability Score (FRS)** – composite metric integrating multiple dimensions  
- **Contradiction analysis** – quantification of disagreement between attribution and functional impact  

We define interpretable failure modes:

- **Attribution excess** – high attribution, low functional importance  
- **Latent dependence** – low attribution, high functional importance  
- **Convergent signal** – agreement across interpretability dimensions  

---

## Repository Structure

```text
.
├── S1_... S10_...          # model training and evaluation
├── S15_Interpretability_Unified_Framework.ipynb
├── S16_Interpretability_Contradictions_and_Typology.ipynb
├── data/                  # input data (not included if restricted)
├── outputs/               # generated tables and figures
└── README.md

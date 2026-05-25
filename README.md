# Heterogeneous Catalysis in the Low-Data Regime

## Overview

This project investigates machine learning approaches for heterogeneous catalysis in the low-data regime.  
The goal is to better understand model performance, encoder behavior, the role of different metrics, and optimization strategies across limited catalytic datasets.

---

## Repository Contents

The repository contains three Jupyter notebooks covering complementary tasks in catalysis modeling and optimization.

### 1. Model Evaluation

This notebook evaluates several machine learning models and metrics for:

- Reaction rate prediction
- Selectivity prediction
- Multi-target prediction using target-wise wrappers
- Native joint multi-output prediction

The notebook compares predictive performance across different modeling strategies.

---

### 2. Model and Encoder Comparison

This notebook compares different machine learning models, encoders, and metrics on two datasets:

- Formic Acid Decomposition
- Methanol Dehydrogenation

The datasets are also merged to create a combined catalysis dataset, which is used in the *Model Evaluation* notebook, and the models, encoders, and metrics are also compared on this merged dataset.

---

### 3. Bayesian Optimization

This notebook adapts the Bayesian Optimization code from class (see: https://colab.research.google.com/github/schwallergroup/ai4chem_course/blob/main/notebooks/10%20-%20Bayesian%20optimization/Buchwald-Hartwig-BO.ipynb#scrollTo=rcUMHxFXZ6Bz) by:

- Using an RBF kernel
- Constructing a design space around the ten experimental points with the highest reaction rates

The objective is to explore efficient optimization strategies in an experimental setting with little data.

---

## Objectives

- Study machine learning performance in catalysis problems with limited data
- Compare models, encoders, and metrics
- Explore multi-target learning strategies
- Apply Bayesian Optimization to maximize the rate of reaction

---

## Requirements

Two tabular models (TabPFN and TabICLv2) are used and may require the creation of a free account to be run.

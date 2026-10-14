# Inflammatory-Protein-Signatures-Distinguish-PANDAS-

## Overview
This repository contains R Markdown scripts supporting the machine-learning analyses described in the manuscript Inflammatory Protein Signatures Distinguish Pediatric Autoimmune Neuropsychiatric Disorders Associated With Streptococcal Infections From Other Psychiatric Conditions.

The analyses evaluate whether circulating inflammatory protein signatures distinguish individuals with PANDAS from healthy controls and individuals with other psychiatric conditions, including obsessive-compulsive disorder and restrictive eating disorders.

## Repository Contents
PrimaryModel1_PANDASvsHC.Rmd: Binary classification comparing PANDAS and healthy controls.

PrimaryModel2-PANDASvsOCDvsRED.Rmd: Multiclass classification comparing PANDAS, OCD, and restrictive eating disorders.

The scripts include comparisons of machine-learning algorithms, random forest feature selection, cross-validation procedures, and model performance evaluation.

## Data Availability and Confidentiality

Participant-level data are not publicly available because of privacy, confidentiality, and research participant protections.

The repository contains analysis code only. No individual-level protein measurements, clinical records, or participant identifiers are provided.

Access to appropriately de-identified data may be considered upon reasonable request to the corresponding author, subject to institutional approvals, applicable data-sharing agreements, and participant consent restrictions.

Please send requests to Dr. Breithaupt (lbreithauptlangston@mgh.harvard.edu).

## Requirements

R 4.5.1. Packages: tidyverse, conflicted, rpart, caret, pROC, randomForest, pheatmap, uwot, MASS, knitr, kableExtra, gridExtra, e1071, xgboost, inflection.

## Running the Analyses

The scripts require access to the corresponding participant-level analytic datasets, which are not included in this repository.

The binary classification script expects PrimaryModelOne.RData, and the multiclass classification script expects PrimaryModelTwo.RData. Additional data objects, including NPX_raw, are referenced within the scripts.

Users with authorized access to the analytic datasets should confirm that the required objects and variables are available before running the analyses.

The scripts use a random seed of 2025 for reproducibility.

## Statistical Methods

The repository includes random forest, classification tree, support vector machine, and gradient boosting analyses.

Analyses include protein preprocessing, age adjustment, feature selection, and cross-validation. The scripts contain both full-panel and reduced-panel analyses.

The distinction between fixed-signature evaluation and fully nested feature-selection evaluation should be maintained when interpreting model performance.

## Limitations

These analyses were developed for research purposes. The resulting models have not been established as clinically validated diagnostic tests and should not be used to make individual patient care decisions.

## Contact

Luke Dysart (ldysart@mgh.harvard.edu) & Lauren Breithaupt (lbreithauptlangston@mgh.harvard.edu).

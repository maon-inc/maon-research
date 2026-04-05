---
title: "Predicting cognitive scores from wearable-based digital physiological features using machine learning: data from a clinical trial in mild cognitive impairment"
authors: "Bosch de Basea M et al."
year: 2024
journal: "BMC Medicine"
doi: "10.1186/s12916-024-03252-y"
url: "https://bmcmedicine.biomedcentral.com/articles/10.1186/s12916-024-03252-y"
domains: [1, 7]
relevance: 8
tags: ["cognitive-score", "wearable", "HRV", "machine-learning", "prediction", "executive-function", "Empatica", "mild-cognitive-impairment", "digital-biomarker"]
---

## Summary

This study evaluated whether digital physiological features from a wrist-worn wearable (Empatica E4) could predict neuropsychological test scores in individuals with mild cognitive impairment (MCI). Data came from a 10-week single-arm clinical trial in older adults (ages 50-70, N=30). The machine learning model used HRV, electrodermal activity, and skin temperature features to predict composite cognitive scores across multiple domains.

## Key Findings

- Physiological features, especially heart rate variability measures, correlated most strongly with executive function compared to other cognitive composites
- The model predicted actual executive function scores with a correlation of r=0.69
- Intra-individual changes in executive function scores were predicted with r=0.61, showing the model can track cognitive changes over time
- HRV-derived features were the most informative predictors, followed by electrodermal activity
- Processing speed and memory composites were less accurately predicted than executive function
- The approach demonstrates feasibility of using wearable sensors for continuous, non-invasive cognitive assessment

## MAON Applicability

Highly relevant to MAON's cognitive scoring system, which computes a composite cognitive score from multiple wearable-derived inputs including HRV, sleep, steps, and resting heart rate. This paper validates the fundamental approach of deriving cognitive performance indicators from physiological signals measured by wrist-worn devices. The finding that HRV is the strongest predictor of cognitive function supports MAON's weighting of HRV data in its cognitive scoring algorithm. The longitudinal tracking capability (predicting changes over time) aligns with MAON's daily cognitive score snapshots and trend monitoring.

## Methodology Notes

Single-arm clinical trial with 30 participants diagnosed with amnestic MCI. Used Empatica E4 (medical-grade wrist wearable) collecting blood volume pulse, electrodermal activity, and skin temperature. Cognitive assessment via Neuropsychological Test Battery with composite scores for executive function, processing speed, immediate memory, delayed memory, and global cognition. Small sample size is a key limitation; the Empatica E4 is research-grade rather than consumer-grade, so findings may not directly transfer to Apple Watch or Garmin devices.

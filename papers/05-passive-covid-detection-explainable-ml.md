---
title: "Passive detection of COVID-19 with wearable sensors and explainable machine learning algorithms"
authors: "Gadaleta et al."
year: 2021
journal: "npj Digital Medicine"
doi: "10.1038/s41746-021-00533-1"
url: "https://www.nature.com/articles/s41746-021-00533-1"
domains: [5]
relevance: 9
tags: ["covid-19", "passive-detection", "explainable-ml", "gradient-boosting", "wearable", "large-scale"]
---

## Summary

Develops an explainable gradient-boosting model for COVID-19 detection using wearable sensor data from 38,911 individuals. The model adapts to available sensor data and explains feature importance for individual predictions.

## Key Findings

- AUC of 0.83 for symptomatic individuals using wearable data + symptoms
- AUC of 0.78 using only pre-test-date data (prospective detection capability)
- Gradient-boosted decision trees provide explainable predictions
- Model adapts to missing sensor data and absent self-reported symptoms
- Peripheral temperature and HRV changes are among the most important features
- Outperforms prior state-of-the-art algorithms

## MAON Applicability

The gradient-boosting approach and feature importance explanations are directly applicable to MAON's illness detection model. MAON uses LightGBM (a gradient-boosting framework), making this paper's methodology highly transferable. The explainability aspect helps MAON communicate why it suspects illness.

## Methodology Notes

Published in npj Digital Medicine (2021). 38,911 participants. Uses Fitbit/consumer wearable data. Explainable ML approach. Large-scale validation. Open access.

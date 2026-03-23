---
title: "A multi-modal deep learning approach for stress detection using physiological signals: integrating time and frequency domain features"
authors: "Various et al."
year: 2025
journal: "Scientific Reports"
doi: "10.1038/s41598-025-93521-4"
url: "https://pmc.ncbi.nlm.nih.gov/articles/PMC11997569/"
domains: [3, 1]
relevance: 8
tags: ["deep-learning", "stress-detection", "physiological-signals", "multimodal", "time-frequency", "ecg", "eda"]
---

## Summary

Develops a multi-modal deep learning approach combining time and frequency domain features from physiological signals for stress detection. Uses the WESAD dataset and achieves high classification accuracy.

## Key Findings

- Multi-modal deep learning integrating time and frequency domain features achieves high stress classification accuracy
- Binary stress vs. non-stress classification accuracy up to 93-99% depending on model architecture
- Three-class classification (baseline, stress, amusement) achieves up to 80% accuracy
- ECG, EDA, and respiration are the most reliable stress biomarkers
- Combining signals from both chest-worn and wrist-worn sensors improves performance

## MAON Applicability

Validates the multi-signal approach MAON uses for stress detection. While MAON uses LightGBM/ONNX rather than deep learning, the feature engineering insights (time and frequency domain HRV features) directly inform MAON's feature pipeline. The WESAD-trained benchmark is directly comparable to MAON's own training data.

## Methodology Notes

Published in Scientific Reports (2025). Uses WESAD dataset (15 subjects). Lab-based study with Trier Social Stress Test protocol. Compares multiple deep learning architectures. Open access.

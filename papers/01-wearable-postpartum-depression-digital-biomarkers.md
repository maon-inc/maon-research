---
title: "Harnessing Consumer Wearable Digital Biomarkers for Individualized Recognition of Postpartum Depression Using the All of Us Research Program Data Set"
authors: "McGinnis et al."
year: 2024
journal: "JMIR mHealth and uHealth"
doi: "10.2196/54622"
url: "https://mhealth.jmir.org/2024/1/e54622"
domains: [1, 5]
relevance: 8
tags: ["postpartum-depression", "wearable", "digital-biomarkers", "Fitbit", "machine-learning", "personalized", "heart-rate", "sleep", "activity"]
---

## Summary

A cross-sectional study using Fitbit data from the All of Us Research Program to develop intraindividual machine learning models that distinguish between postpartum depression (PPD) and non-depression periods. Random forest models achieved strong classification performance (mAUC = 0.85, kappa = 0.80) using digital biomarkers including heart rate, step count, sleep, and caloric expenditure to differentiate prepregnancy, pregnancy, postpartum without depression, and postpartum with depression periods.

## Key Findings

- Intraindividual random forest models achieved mAUC of 0.85 and kappa of 0.80 for distinguishing PPD from other periods
- The most predictive biomarker of PPD was calories burned during basal metabolic rate
- Heart rate patterns, sleep metrics, and daily step counts all contributed to PPD recognition
- Person-specific models outperformed population-level models, supporting the value of individual baselines
- Consumer wearable data (Fitbit) was sufficient for clinically meaningful classification accuracy
- The approach enables passive, continuous monitoring without active self-reporting

## MAON Applicability

This study validates the core approach MAON takes with its baseline engine: computing per-user, per-metric baselines and detecting deviations. The finding that intraindividual models substantially outperform population models supports MAON's use of personalized rolling baselines for heart rate, HRV, steps, and sleep. The study also demonstrates that consumer wearable data (similar to what MAON ingests from Apple Health and Garmin) can detect mood-related changes with high accuracy. MAON's proactive agent could apply similar pattern recognition to flag potential mood deterioration using the same data streams.

## Methodology Notes

Cross-sectional study using the All of Us Research Program dataset. Fitbit-derived digital biomarkers analyzed with multiple ML algorithms (random forest, SVM, logistic regression, gradient boosting). Intraindividual modeling approach using each participant as their own control across time periods. Limitation: cross-sectional design limits causal inference; PPD identified through EHR diagnosis codes rather than validated screening instruments.

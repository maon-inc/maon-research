---
title: "Digital phenotypes and digital biomarkers for health and diseases: a systematic review of machine learning approaches utilizing passive non-invasive signals collected via wearable devices and smartphones"
authors: "Menychtas et al."
year: 2024
journal: "Artificial Intelligence Review"
doi: "10.1007/s10462-024-11009-5"
url: "https://link.springer.com/article/10.1007/s10462-024-11009-5"
domains: [5, 4]
relevance: 8
tags: ["digital-phenotyping", "digital-biomarkers", "machine-learning", "passive-sensing", "wearable", "smartphone", "systematic-review"]
---

## Summary

A systematic review of 66 peer-reviewed studies examining machine learning approaches for digital phenotyping and digital biomarker discovery using passive, non-invasive signals from wearable devices and smartphones. The review covers applications across mental health, cardiovascular, neurological, and metabolic conditions, cataloging which signals and ML methods yield the best predictive performance.

## Key Findings

- Heart rate (67% of studies), movement/accelerometry (60%), and step count (40%) were the most commonly used passive biomarkers from wearables
- Depression and anxiety were the most studied conditions, representing 55% and 21% of studies respectively
- Wrist-worn devices were the dominant sensing platform (76% of studies)
- Traditional ML methods (random forests, SVMs) remain the most common, though deep learning is emerging for ECG and EEG signals
- Multimodal approaches combining wearable and smartphone data showed improved prediction accuracy over single-source models
- Median study sample size was 60.5 participants, with only 2% of studies performing external validation, highlighting significant methodological limitations

## MAON Applicability

Directly relevant to MAON's multimodal approach of combining Apple Health data (HR, HRV, steps, sleep), screen time, calendar, and location into a composite cognitive score. The paper validates the specific signals MAON collects (heart rate, step count, sleep, activity) as the most commonly used digital biomarkers in the literature. The finding that multimodal approaches outperform single-source models supports MAON's strategy of combining four domains into one composite score. The identified gap in external validation and small sample sizes suggests an opportunity for MAON to contribute real-world data at scale.

## Methodology Notes

Systematic review following PRISMA guidelines. Searched PubMed, Web of Science, Scopus, and IEEE Xplore for studies published up to June 2024. Included 66 papers meeting criteria for passive sensing with ML approaches. Published in Artificial Intelligence Review (Springer). Provides comprehensive taxonomy of signals, conditions, and ML methods used across the field.

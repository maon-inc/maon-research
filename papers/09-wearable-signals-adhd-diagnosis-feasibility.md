---
title: "Wearable Signals for Diagnosing Attention-Deficit/Hyperactivity Disorder in Adolescents: A Feasibility Study"
authors: "Jiang Z et al."
year: 2024
journal: "JAACAP Open"
doi: "10.1016/j.jaacop.2024.11.003"
url: "https://www.jaacapopen.org/article/S2949-7329(24)00091-7/fulltext"
domains: [9, 1]
relevance: 9
tags: ["adhd", "wearable", "actigraphy", "heart-rate", "sleep", "machine-learning", "diagnosis", "adolescents"]
---

## Summary

This feasibility study examined whether objective wearable signals (movement acceleration, heart rate, and sleep patterns from passive actigraphy) combined with machine learning could accurately classify ADHD in Chinese adolescents aged 16-17. Models using only objective measures achieved an AUC of 0.844, while combined subjective and objective models reached 0.933.

## Key Findings

- Machine learning models using solely objective wearable measures achieved AUC of 0.844 for ADHD classification
- Models combining subjective and objective measures reached AUC of 0.933
- ADHD medication status was classified with an AUC of 1.000 using objective measures alone
- Heart rate was the most important feature for classification, followed by sleep and activity metrics
- Movement acceleration, heart rate patterns, and sleep architecture provided complementary diagnostic signals
- Results support wearable-based screening as a viable supplement to traditional clinical assessment

## MAON Applicability

Highly relevant to MAON's Apple Health integration, which already captures heart rate, sleep, and activity data. The study validates that the exact biometric streams MAON collects (HR, HRV, sleep analysis, step count) carry meaningful signal for ADHD-related patterns. Could support development of ADHD awareness features or personalized insights for users who self-report ADHD.

## Methodology Notes

Cross-sectional feasibility study with Chinese adolescents ages 16-17. Collected objective measures via passive actigraphy (movement, heart rate, sleep) and subjective measures via parent and self-reported questionnaires. Multiple machine learning models tested including Random Forest. Small sample size typical of feasibility studies, but strong classification results warrant larger-scale validation.

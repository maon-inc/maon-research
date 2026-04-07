---
title: "Digital phenotyping in bipolar disorder: Using longitudinal Fitbit data and personalized machine learning to predict mood symptomatology"
authors: "Lipschitz et al."
year: 2025
journal: "Acta Psychiatrica Scandinavica"
doi: "10.1111/acps.13765"
url: "https://onlinelibrary.wiley.com/doi/10.1111/acps.13765"
domains: [2, 1]
relevance: 9
tags: ["bipolar-disorder", "fitbit", "digital-phenotyping", "personalized-ml", "mood-prediction", "consumer-wearable", "sleep", "longitudinal"]
---

## Summary

This study evaluated whether a novel personalized machine learning approach trained entirely on passive Fitbit data could accurately detect mood symptomatology in bipolar disorder patients. Analyzing data from 54 adults with BD who wore Fitbits and completed bi-weekly self-reports for 9 months, the Binary Mixed Model (BiMM) forest achieved ROC-AUC of 86.0% for depression and 85.2% for hypomania detection.

## Key Findings

- BiMM forest outperformed other ML algorithms for personalized mood prediction from consumer wearable data
- Depression detection achieved 80.1% accuracy using optimized thresholds, while hypomania detection reached 89.1% accuracy
- The approach used limited data filtering, making it more practical for real-world deployment compared to methods requiring extensive preprocessing
- Passive Fitbit data streams (sleep patterns, physical activity, heart rate) provided sufficient signal for clinically meaningful mood episode prediction
- The personalized modeling approach accounts for individual baselines, which is critical given the heterogeneity of bipolar disorder presentations
- 9-month longitudinal design captured multiple mood episodes per participant, strengthening the ecological validity

## MAON Applicability

Highly relevant to MAON's use of consumer wearable data (Apple Watch, Garmin) for tracking mental health patterns. The personalized ML approach aligns with MAON's goal of providing individualized insights rather than population-level averages. The finding that passive Fitbit data alone can predict mood episodes with high accuracy validates MAON's core premise that wearable biometrics can meaningfully inform mental wellness monitoring. The sleep and activity features used map directly to MAON's Clarity Score health domain.

## Methodology Notes

Longitudinal observational study with 54 adults diagnosed with bipolar disorder (BD-I or BD-II). Participants wore Fitbit devices continuously for 9 months and completed bi-weekly PHQ-8 (depression) and ASRM (mania) self-reports. Binary Mixed Model (BiMM) forest used for personalized prediction. Authors from Brigham and Women's Hospital, Harvard Medical School, and Harvard Kennedy School. Published in Acta Psychiatrica Scandinavica, 2025.

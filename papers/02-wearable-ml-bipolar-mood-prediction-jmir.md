---
title: "Using Wearable Device and Machine Learning to Predict Mood Symptoms in Bipolar Disorder: Development and Usability Study"
authors: "Various et al."
year: 2025
journal: "JMIR Medical Informatics"
doi: "10.2196/66277"
url: "https://medinform.jmir.org/2025/1/e66277"
domains: [2, 1]
relevance: 8
tags: ["bipolar-disorder", "mood-prediction", "wearable", "machine-learning", "digital-biomarker", "depression", "mania", "HRV", "sleep", "activity"]
---

## Summary

This development and usability study recruited 24 participants with bipolar disorder to build predictive models for depressive and manic symptoms using digital biomarkers collected from consumer wearable devices. Six machine learning algorithms were compared, with Extreme Gradient Boosting achieving the best performance for predicting mood symptom onset from passively collected wearable data.

## Key Findings

- The prediction model for depressive symptoms achieved 83% accuracy with an AUROC of 0.89 and F1 score of 0.65
- Digital biomarkers derived from wearable data (sleep, activity, heart rate) could predict both depressive and manic symptoms
- Extreme Gradient Boosting (XGBoost) outperformed other algorithms including Logistic Regression, Decision Tree, K-Nearest Neighbors, Random Forest, and AdaBoost
- The model demonstrates potential for early detection of mood episodes, enabling timely intervention
- Sleep-related features were among the most predictive biomarkers for both depressive and manic states
- Participants found the wearable monitoring acceptable and usable in daily life

## MAON Applicability

Relevant to MAON's use of wearable-derived data for mental health monitoring and its cognitive scoring system. The study validates the approach of using passively collected sleep, activity, and heart rate data to predict mood states -- the same types of data MAON collects through Apple Health and Garmin integrations. The high AUROC for depression prediction supports MAON's approach of combining multiple physiological streams into composite wellness indicators. The finding that consumer wearable data can predict mood symptoms with clinically useful accuracy strengthens the evidence base for MAON's daily health summaries and trend detection features.

## Methodology Notes

Prospective study with 24 bipolar disorder patients wearing consumer wearable devices over an extended monitoring period. Mood symptoms assessed via validated self-report instruments. Six ML algorithms compared with standard train-test splits. The sample size is modest but consistent with digital health pilot studies. Published in JMIR Medical Informatics (impact factor ~3.2), a respected journal for health informatics research. The usability component adds practical feasibility evidence beyond pure prediction accuracy.

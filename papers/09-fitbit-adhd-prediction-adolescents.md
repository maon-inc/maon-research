---
title: "Unlocking the Potential of Wearable Technology: Fitbit-Derived Measures for Predicting ADHD in Adolescents"
authors: "Cardenas-Iniguez C et al."
year: 2025
journal: "Frontiers in Child and Adolescent Psychiatry"
doi: "10.3389/frcha.2025.1504323"
url: "https://www.frontiersin.org/journals/child-and-adolescent-psychiatry/articles/10.3389/frcha.2025.1504323/full"
domains: [9, 7]
relevance: 9
tags: ["adhd", "fitbit", "wearable", "machine-learning", "adolescents", "resting-heart-rate", "actigraphy"]
---

## Summary

This study analyzed Fitbit data from 450 adolescents in the ABCD (Adolescent Brain Cognitive Development) study to test whether consumer-wearable physiological markers could predict ADHD diagnoses. Using machine learning, the researchers achieved high classification accuracy (AUC 0.95) based on three Fitbit-derived measures: resting heart rate, sedentary time, and energy expenditure.

## Key Findings

- A Random Forest classifier achieved cross-validation accuracy of 0.89, AUC of 0.95, precision of 0.88, recall of 0.90, and F1-score of 0.89
- Test set accuracy reached 0.88, demonstrating strong generalization
- Higher resting heart rate and greater energy expenditure were positively associated with ADHD diagnosis
- Increased sedentary time predicted lower odds of ADHD diagnosis
- Consumer-grade Fitbit wearables provided sufficient signal quality for clinically meaningful ADHD classification
- Results support the use of passively collected wearable data as an objective complement to subjective ADHD assessment

## MAON Applicability

Directly relevant to MAON's wearable integration (Apple Health, Garmin) and cognitive score feature. The finding that resting heart rate and activity levels are strong ADHD predictors maps onto data MAON already collects through Apple Health (resting HR, step count, active energy). Could inform future ADHD-related screening or risk-awareness features within the app.

## Methodology Notes

Observational study using data from 450 adolescents in the ABCD study, the largest long-term study of brain development in the US. Fitbit devices captured resting heart rate, sedentary time, and energy expenditure. Machine learning models (Random Forest, logistic regression) were trained with cross-validation. Large sample size from a well-established longitudinal cohort strengthens the findings.

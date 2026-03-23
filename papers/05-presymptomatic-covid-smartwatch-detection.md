---
title: "Pre-symptomatic detection of COVID-19 from smartwatch data"
authors: "Mishra et al."
year: 2020
journal: "Nature Biomedical Engineering"
doi: "10.1038/s41551-020-00640-6"
url: "https://www.nature.com/articles/s41551-020-00640-6"
domains: [5]
relevance: 10
tags: ["covid-19", "pre-symptomatic", "smartwatch", "illness-detection", "resting-heart-rate", "anomaly-detection"]
---

## Summary

A landmark study from Stanford demonstrating that consumer smartwatch data (resting heart rate, sleep, steps) can detect COVID-19 infection pre-symptomatically. Found that 63% of cases could be detected before symptom onset using resting heart rate elevations relative to individual baselines.

## Key Findings

- 81% (26/32) of COVID-19 cases showed detectable alterations in HR, steps, or sleep
- 63% of cases detected pre-symptomatically via RHR elevations relative to individual baseline
- Some cases detected up to 9 days before symptom onset
- Two-tiered warning system based on extreme RHR elevations proved effective
- Data sourced via Fitbit APIs and Apple HealthKit -- directly applicable to consumer devices

## MAON Applicability

Directly validates MAON's illness detection model architecture. MAON uses exactly the same signals (RHR, sleep, activity) and the same individualized baseline approach. The 63% pre-symptomatic detection rate provides a realistic performance benchmark for MAON's anomaly detection.

## Methodology Notes

Published in Nature Biomedical Engineering (2020). Retrospective analysis of 32 COVID-19 positive individuals from a larger cohort. Uses Fitbit and Apple HealthKit data. Highly cited (>700 citations). Open access.

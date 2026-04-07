---
title: "Mitigating data quality challenges in ambulatory wrist-worn wearable monitoring through analytical and practical approaches"
authors: "Van Der Donckt et al."
year: 2024
journal: "Scientific Reports"
doi: "10.1038/s41598-024-67767-3"
url: "https://www.nature.com/articles/s41598-024-67767-3"
domains: [5, 3]
relevance: 8
tags: ["data-quality", "wearable", "ambulatory", "non-wear", "compliance", "pipeline", "signal-processing"]
---

## Summary

This paper identifies and addresses key data quality challenges encountered when using wrist-worn wearable devices for ambulatory health monitoring in real-world settings. The authors present practical countermeasures including participant compliance visualizations, interaction-triggered questionnaires to assess personal bias, and an optimized pipeline for detecting non-wear periods.

## Key Findings

- Identified four primary data quality challenges in ambulatory wearable monitoring: data entry errors, non-wear periods, missing data, and wearable artifacts
- Developed a visualization-oriented approach to validate data processing pipelines using scalable tools (tsflex and Plotly-Resampler)
- Proposed participant compliance visualizations that allow real-time assessment of data collection quality
- Created interaction-triggered questionnaires to assess and correct for personal bias in self-reported annotations
- Built an optimized non-wear detection pipeline that outperforms standard approaches for wrist-worn accelerometer and physiological data
- Demonstrated that data quality issues can significantly impact downstream analysis if not properly addressed

## MAON Applicability

Highly relevant to MAON's Apple Health data pipeline, particularly the new two-phase onboarding sync with deferred backfill feature. The non-wear detection methods and data quality validation approaches can inform how MAON handles gaps in health data streams. The compliance visualization concepts align with MAON's cognitive score freshness tracking, which monitors data staleness and adjusts scores accordingly. The pipeline validation approach is also relevant to MAON's background sync and health data upload mechanisms.

## Methodology Notes

The study was conducted by researchers at IDLab (Ghent University-Imec) and the Department of Neurology at Ghent University Hospital. The approaches were validated using data from ambulatory monitoring studies involving wrist-worn Empatica E4 devices collecting accelerometer, electrodermal activity, blood volume pulse, and temperature data.

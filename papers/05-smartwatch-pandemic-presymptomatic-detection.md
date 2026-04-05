---
title: "Terminating pandemics with smartwatches"
authors: "Vesinurm et al."
year: 2025
journal: "PNAS Nexus"
doi: "10.1093/pnasnexus/pgaf044"
url: "https://academic.oup.com/pnasnexus/article/4/3/pgaf044/8046445"
domains: [5, 1]
relevance: 8
tags: ["smartwatch", "pandemic", "presymptomatic-detection", "infection", "heart-rate", "skin-temperature", "respiratory-rate", "COVID-19", "influenza"]
---

## Summary

This study develops a multiscale modeling framework integrating within-host viral dynamics and between-host transmission to evaluate whether consumer smartwatches can detect infections presymptomatically and reduce outbreak risk. Using physiological signals such as heart rate, respiratory rate, and skin temperature, the authors demonstrate that smartwatch-based detection achieves 88% accuracy for COVID-19 up to 4 days before symptom onset and 90% accuracy for influenza up to 24 hours before onset.

## Key Findings

- Consumer smartwatches detected COVID-19 with 88% accuracy at 4 days before symptom onset using resting heart rate, skin temperature, and respiratory rate changes
- Influenza detection reached 90% accuracy for both symptomatic and asymptomatic infections up to 24 hours before symptom onset
- The multiscale framework links individual physiological deviations to population-level transmission dynamics
- Presymptomatic alerting via wearables could substantially reduce effective reproduction numbers by enabling earlier isolation
- The approach works with existing commercial devices without requiring new hardware or FDA-cleared sensors
- Modeling suggests that even partial smartwatch adoption in a population can meaningfully curb outbreak trajectories

## MAON Applicability

Directly relevant to MAON's wearable anomaly detection pipeline, which monitors Apple Health and Garmin data for physiological deviations. The presymptomatic detection methods described here (resting heart rate anomalies, skin temperature shifts) align with the signals MAON already collects. Could inform threshold-based alerting for illness onset and support the proactive agent's health-check interventions.

## Methodology Notes

Computational modeling study combining within-host viral kinetics with agent-based transmission models. Validated against published wearable detection datasets from prior COVID-19 and influenza studies. Not a primary clinical trial but a synthesis and simulation framework grounded in empirical detection accuracy data from multiple consumer devices.

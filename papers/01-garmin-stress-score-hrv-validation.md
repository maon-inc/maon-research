---
title: "Assessing Stress Level Scores Against Wearables-Driven Physiological Measurements"
authors: "Rosenbach H et al."
year: 2025
journal: "Stress and Health"
doi: "10.1002/smi.70125"
url: "https://onlinelibrary.wiley.com/doi/full/10.1002/smi.70125"
domains: [1, 3]
relevance: 9
tags: ["Garmin", "stress-score", "HRV", "wearable-validation", "consumer-wearable", "autonomic", "stress-detection", "Vivosmart"]
---

## Summary

A two-phase validation study (pilot N=29, main N=60) assessed the Garmin Vivosmart 4 stress score against gold-standard ECG-derived HRV from the Polar H10 chest strap. The Garmin Stress Score (GSS) significantly differentiated stress from rest conditions and correlated meaningfully with HRV metrics, supporting its use as a proxy for physiological stress. However, tonic HRV, exercise habits, BMI, and sleep duration all moderated the score, indicating individual-level calibration matters.

## Key Findings

- Garmin Stress Score showed significant increases during experimentally induced stress vs. rest conditions
- GSS correlated significantly with mean HR, RMSSD (time-domain HRV), and SD2/SD1 (Poincare plot metrics) from gold-standard ECG
- High tonic HRV, regular exercise, and longer sleep duration were each associated with lower baseline stress scores
- BMI significantly influenced stress score values independent of acute stress state
- In real-life ambulatory settings (N=657 in a larger companion study), HRV-stress associations were weaker than in controlled lab settings
- Garmin's stress score is considered methodologically feasible as a proxy physiological stress marker when used with awareness of these moderating factors

## MAON Applicability

MAON integrates with Garmin devices via the Garmin Connect OAuth flow and reads HRV and stress data. This paper directly validates the Garmin Stress Score as a meaningful physiological signal, supporting MAON's use of Garmin data for proactive agent decisions and health summaries. The moderating factors (tonic HRV, sleep, exercise) also support MAON's multi-signal approach, where HRV is interpreted alongside sleep quality and activity data.

## Methodology Notes

Two-phase validation design. Pilot phase: N=29. Main study: N=60. Reference device: Polar H10 chest strap (ECG-based). Target device: Garmin Vivosmart 4. Both acute stress (Trier Social Stress Test or equivalent) and rest conditions measured. Authors: Hadar Rosenbach and Alon Itzkovitch (Tel Aviv University / University of Haifa, Israel). Published November 2025 in Stress and Health, volume 41(6):e70125.

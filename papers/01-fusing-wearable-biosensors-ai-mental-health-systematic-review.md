---
title: "Fusing Wearable Biosensors with Artificial Intelligence for Mental Health Monitoring: A Systematic Review"
authors: "Kargarandehkordi A et al."
year: 2025
journal: "Biosensors"
doi: "10.3390/bios15040202"
url: "https://www.mdpi.com/2079-6374/15/4/202"
domains: [1, 4]
relevance: 9
tags: ["wearable-biosensors", "AI", "mental-health", "multimodal", "HRV", "EDA", "accelerometry", "machine-learning", "systematic-review", "digital-phenotyping"]
---

## Summary

Systematic review of 48 studies examining how AI models use data from wearable biosensors (HR, HRV, EDA/GSR, accelerometry, GPS, audio, and usage metadata) to predict mental health conditions. Stress was the most studied condition (~60% of studies), followed by depression (~31%). Most studies used wrist-worn devices (76%) collecting heart rate (67%), movement index (60%), and step count (40%).

## Key Findings

- Multimodal sensor fusion combining physiological and behavioral signals consistently outperformed single-modality approaches for mental health prediction
- CNNs and LSTMs achieved up to 92% accuracy for anxiety detection, though these results came from small, controlled datasets
- Median sample size was only 60.5 participants (IQR 54-99), and 76% of studies used a single device, limiting ecological validity
- Only 1 of 42 studies (2%) performed external validation, raising concerns about generalizability
- Consumer wearables (Apple Watch, Fitbit, Garmin) were increasingly represented alongside research-grade sensors
- Battery drain, data heterogeneity across devices, and privacy concerns remain key deployment barriers

## MAON Applicability

Directly relevant to MAON's cognitive score feature, which fuses multiple data streams (HRV, steps, sleep, screen time, calendar, location) into a composite wellness signal. The review validates the multimodal approach MAON takes but also highlights the need for larger validation samples and external testing. The finding that consumer wearables perform comparably to research-grade devices supports MAON's reliance on Apple Watch and Garmin data.

## Methodology Notes

PRISMA-guided systematic review searching PubMed, IEEE Xplore, and Scopus. Included 48 studies with wearable biosensor data and AI/ML models targeting mental health outcomes. Quality assessment used the Joanna Briggs Institute critical appraisal tools. Publication bias was not formally tested due to heterogeneous outcome measures.

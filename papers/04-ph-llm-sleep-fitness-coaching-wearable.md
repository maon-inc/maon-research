---
title: "A Personal Health Large Language Model for Sleep and Fitness Coaching"
authors: "McDuff D et al."
year: 2025
journal: "Nature Medicine"
doi: "10.1038/s41591-025-03888-0"
url: "https://www.nature.com/articles/s41591-025-03888-0"
domains: [4, 2, 7]
relevance: 10
tags: ["LLM", "wearable", "sleep-coaching", "fitness-coaching", "personalized-health", "Gemini", "Google", "HRV", "behavior-change"]
---

## Summary

PH-LLM is a version of Gemini fine-tuned to generate personalized insights and recommendations from aggregated wearable sensor data, targeting sleep and fitness coaching. Evaluated across three benchmark datasets including 857 real-world case studies from consenting US users, PH-LLM outperformed human experts on domain knowledge exams and matched expert quality on personalized coaching responses.

## Key Findings

- PH-LLM exceeded a sample of human experts on sleep medicine multiple-choice exams (79% vs. 76%) and fitness exams (88% vs. 71%)
- Evaluated on 857 real-world case studies, PH-LLM performed comparably to human expert coaches for fitness-related tasks
- A multimodal encoder allowed PH-LLM to directly process raw wearable time-series data (HRV, respiratory rate, activity) alongside text
- PH-LLM accurately predicted self-reported sleep quality from longitudinal wearable data, surpassing the base Gemini model
- Fine-tuning on domain-specific behavioral health knowledge was essential for matching expert-level advice quality
- Three benchmark dimensions: expert domain knowledge, personalized insight generation, and longitudinal sleep quality prediction

## MAON Applicability

PH-LLM establishes that LLMs fine-tuned on wearable health data can deliver expert-level sleep and fitness coaching, directly validating MAON's approach of using an AI assistant with access to Apple Health and Garmin data. The model's use of HRV, sleep stages, and activity metrics mirrors MAON's `get_health_data` tool data. The finding that fine-tuning on domain knowledge outperforms general-purpose LLMs supports MAON's prompt engineering and system design decisions.

## Methodology Notes

Research by Google/Alphabet (all authors are Google employees). Published August 2025 in Nature Medicine, volume 31, issue 10, pages 3394-3403. Preprint: arXiv:2406.06474 ("Towards a Personal Health Large Language Model"). Data from consenting US-based users of consumer wearables. Three evaluation benchmark datasets created specifically for this study. Open-access publication.

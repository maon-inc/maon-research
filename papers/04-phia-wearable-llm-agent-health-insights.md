---
title: "Transforming Wearable Data into Personal Health Insights Using Large Language Model Agents"
authors: "Merrill MA et al."
year: 2025
journal: "Nature Communications"
doi: "10.1038/s41467-025-67922-y"
url: "https://www.nature.com/articles/s41467-025-67922-y"
domains: [4, 1]
relevance: 10
tags: ["LLM", "wearable", "health-insights", "agent", "personalized-coaching", "HRV", "sleep", "activity", "ReAct", "code-generation"]
---

## Summary

PHIA (Personal Health Insights Agent) is the first LLM-powered agent specifically designed to transform raw wearable sensor data into actionable personal health insights. Using iterative code generation, web search, and the ReAct framework, PHIA reasons over numerical time-series data from consumer wearables to answer health questions and generate personalized recommendations. It achieved 84% accuracy on objective numerical queries and 83% favorable ratings on open-ended questions in a large evaluation.

## Key Findings

- PHIA achieved 84% accuracy on objective, data-specific numerical health questions vs. wearable sensor data
- 83% of open-ended coaching responses received favorable ratings from independent evaluators
- PHIA was twice as likely as baseline LLMs to receive the highest quality rating on personalized health advice
- The ReAct framework (iterative reasoning + tool use) significantly outperformed single-pass LLM responses for numerical health data
- The system integrates HRV, sleep stages, activity, resting heart rate, and other consumer wearable metrics
- Code generation for data analysis was a key capability enabling accurate numerical reasoning over time-series data

## MAON Applicability

PHIA directly validates MAON's architecture: an LLM agent (Kimi K2.5) that calls tools to fetch Apple Health and Garmin data, then provides personalized insights via iMessage. The PHIA system's tool loop, personalized reasoning approach, and wearable data integration mirror MAON's own implementation. The 84% numerical accuracy benchmark sets a concrete performance target for MAON's `get_health_data` tool responses.

## Methodology Notes

Large-scale evaluation by Google Research, Seattle. Authors include Merrill, Paruchuri, Rezaei, Kovacs, Liu, McDuff, Althoff, Patel, and others from Google/Alphabet. Published September 2025 in Nature Communications, volume 17, article 1143. DOI: 10.1038/s41467-025-67922-y. Preprint available at arXiv:2406.06464.

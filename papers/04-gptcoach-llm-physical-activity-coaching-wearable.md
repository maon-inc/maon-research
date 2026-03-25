---
title: "GPTCoach: Towards LLM-Based Physical Activity Coaching"
authors: "Joerke M et al."
year: 2025
journal: "Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems"
doi: "10.1145/3706598.3713819"
url: "https://dl.acm.org/doi/10.1145/3706598.3713819"
domains: [4, 7]
relevance: 9
tags: ["LLM", "health-coaching", "physical-activity", "wearable", "motivational-interviewing", "behavior-change", "chatbot", "personalized-plan"]
---

## Summary

GPTCoach is an LLM-based health coaching chatbot that implements evidence-based onboarding conversations from the Active Choices program, uses motivational interviewing strategies, and integrates wearable device data to generate personalized physical activity plans. In a lab study with 16 participants using three months of their historical self-tracking data, GPTCoach used motivational interviewing-consistent or neutral behavior codes 93% of the time and outperformed vanilla GPT-4 in MI consistency.

## Key Findings

- GPTCoach can query and visualize a user's health data from wearable devices through tool use, enabling data-driven coaching conversations
- The system used motivational interviewing-consistent or neutral behavior codes 93% of the time, demonstrating reliable adherence to evidence-based coaching principles
- Formative interviews with 12 health professionals and 10 potential coaching recipients identified key design principles for LLM-based health coaches
- GPTCoach outperformed vanilla GPT-4 in motivational interviewing consistency, showing the value of structured prompt engineering for health applications
- Participants found the personalized physical activity plans generated at the end of coaching sessions to be relevant and actionable
- The research highlights how LLMs can structure conversations to center the client's agency and foster self-empowerment, which are critical aspects of successful health coaching

## MAON Applicability

Directly relevant to MAON's chat feature and proactive agent functionality. GPTCoach demonstrates how to combine wearable data (activity, sleep, heart rate) with LLM-based conversational agents to deliver personalized health coaching. The motivational interviewing approach and tool-use pattern for querying wearable data closely mirror MAON's architecture where the AI chat agent accesses Apple Health and Garmin data to provide contextual wellness guidance. The evidence-based coaching conversation structure could inform how MAON's proactive agent initiates and guides health conversations.

## Methodology Notes

Mixed-methods study combining formative interviews (12 health professionals, 10 potential recipients) with a single-session lab evaluation (16 participants). Participants used three months of their own historical wearable data. Evaluation assessed MI adherence using the Motivational Interviewing Treatment Integrity (MITI) coding system. Published at CHI 2025, a top-tier HCI venue with rigorous peer review.

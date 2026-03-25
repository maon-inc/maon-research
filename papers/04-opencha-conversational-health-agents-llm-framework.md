---
title: "Conversational Health Agents: A Personalized Large Language Model-Powered Agent Framework"
authors: "Abbasian M et al."
year: 2025
journal: "JAMIA Open"
doi: "10.1093/jamiaopen/ooaf067"
url: "https://academic.oup.com/jamiaopen/article/8/4/ooaf067/8186991"
domains: [4, 1]
relevance: 8
tags: ["LLM", "conversational-agent", "health-agent", "framework", "wearable-integration", "HRV", "PPG", "open-source", "personalized"]
---

## Summary

This paper introduces openCHA, an open-source LLM-powered framework for developing conversational health agents. The framework includes three core components (Interface, Orchestrator, and External Sources) and supports multimodal input including text, audio, and images. Its effectiveness is demonstrated through 2 main demonstrations and 5 use cases spanning diabetic patient management, food recommendation, mental health evaluation, empathetic conversation, and physiological data analysis including HRV from wearable PPG signals.

## Key Findings

- The framework's three-component architecture (Interface, Orchestrator, External Sources) provides a modular approach to building health-focused conversational agents
- Supports multimodal user input including text, audio, and images for comprehensive health interaction
- The Orchestrator processes queries using structured data transformation, interacting with healthcare data, knowledge bases, AI models, and translators
- Demonstrated wearable integration through processing PPG signals to estimate stress using HRV features and AI models
- Use cases span diverse health domains: diabetes management, nutrition, mental health evaluation, empathetic conversation, and physiological data analysis
- The open-source nature enables researchers and developers to build upon and customize the framework for specific health applications

## MAON Applicability

Directly relevant to MAON's architecture as a health-focused conversational AI system. The openCHA framework's approach to integrating wearable physiological data (HRV from PPG) with LLM-based conversation mirrors MAON's core design of combining Apple Health and Garmin data with AI chat. The mental health evaluation and empathetic conversation use cases align with MAON's wellness companion role. The modular architecture pattern (Interface, Orchestrator, External Sources) could inform MAON's own system design for its chat and proactive agent features.

## Methodology Notes

System design paper with 2 demonstrations and 5 use cases for evaluation. Published in JAMIA Open, a peer-reviewed journal from the American Medical Informatics Association. The framework is open-source and available for replication. Evaluation focused on system capability demonstrations rather than clinical outcomes.

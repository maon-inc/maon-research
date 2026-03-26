---
title: "Retrieval Augmented Generation for Large Language Models in Healthcare: A Systematic Review"
authors: "Amugongo LM et al."
year: 2025
journal: "PLOS Digital Health"
doi: "10.1371/journal.pdig.0000877"
url: "https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000877"
domains: [4]
relevance: 9
tags: ["RAG", "retrieval-augmented-generation", "LLM", "healthcare", "systematic-review", "knowledge-base", "clinical-decision-support", "hallucination-reduction"]
---

## Summary

A systematic review of 70 studies (2020-2025) examining how retrieval-augmented generation (RAG) enhances large language models in healthcare settings. The review categorizes RAG architectures into Naive, Advanced, and Modular approaches, finding that RAG significantly reduces hallucinations and improves factual accuracy for clinical tasks including diagnostic support, EHR summarization, and medical question answering.

## Key Findings

- 70 studies were included from an initial pool of 2,139 articles retrieved from Google Scholar and PubMed
- 78.9% of studies used English-language datasets; 21.1% used Chinese datasets
- Proprietary models such as GPT-3.5/4 were the most commonly used base models for RAG applications
- Three RAG architectures were identified: Naive RAG (basic retrieval + generation), Advanced RAG (with query rewriting, re-ranking), and Modular RAG (composable pipeline components)
- RAG-enhanced models substantially outperformed base LLMs on factual accuracy; one study showed RAG boosted differential diagnosis accuracy from 54% to 78%
- A significant gap exists in standardized evaluation frameworks for RAG-based healthcare applications

## MAON Applicability

Directly relevant to MAON's new crawler/AutoRAG pipeline, which crawls configured web sources, stores content in R2, and powers a web_search agent tool via AutoRAG. This review validates the approach of using RAG to ground AI health agents in curated knowledge bases, reducing hallucination risk when providing wellness guidance. The finding that domain-specific knowledge retrieval improves clinical accuracy supports MAON's strategy of building a curated research knowledge base for its proactive AI agent.

## Methodology Notes

Systematic review following PRISMA guidelines. Searched Google Scholar and PubMed with structured queries. Applied multiple exclusion steps to arrive at 70 included studies. Quality assessment addressed study design, evaluation metrics, and reproducibility. The review spans healthcare domains including radiology, pathology, general medicine, and patient-facing applications.

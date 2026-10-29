---
layout: research
title: "Norma - Modular Norm-Aware Deliberation for LLM-based Agents"
date: 2026-10-12
description: A dual-LLM architecture for norm-aware deliberation in the scientific collaboration domain
category: in-progress
authors: "Omkar J. Joshi, Fardin Saad, Munindar P. Singh"
venue: "under review at NAACL 2027"
year: 2026
location: TBD
link: TBD
---

## Research Problem

Norma is a modular LLM-agent architecture that enables agents to account for normative consequences while pursuing their goals in scientific collaboration. 
It addresses the challenge of reducing norm violations without sacrificing goal achievement.

## Research Contribution

- Separates goal-directed reasoning from normative evaluation using ReasonerLLM and ArbiterLLM.
- Integrates agent memory and a deterministic Norm Engine for norm-aware deliberation.
- Evaluates norm-aware deliberation across scientific collaboration scenarios involving resource allocation, research governance, and ethical obligations.
- Compares modular deliberation against norm-unaware and single-reasoner baselines.

## Methodology and Evaluation

Norma proposes candidate actions through ReasonerLLM and independently evaluates them through ArbiterLLM, which approves actions or requests revisions based on applicable norms. 
The architecture was evaluated on 50 curated scientific collaboration scenarios, comparing three agent configurations and two underlying LLMs.
Norma achieved:
- Reduced the norm violation rate from 23% to 4% compared with the norm-unaware baseline.
- Improved goal success from 78.4% to 97.3% when goal achievement was compatible with norm compliance.
- Maintained 84.6% goal success in goal–norm tension scenarios while substantially reducing norm violations.
- Recorded zero incorrect rejections across 112 ArbiterLLM proposals.

## Technologies

Large language models, multiagent systems, normative reasoning, Model Context Protocol (MCP), agent memory, tool-augmented LLMs, Python.
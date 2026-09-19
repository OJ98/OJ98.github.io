---
layout: research
title: "ReFeedGraph: Graph-grounded Reusable Feedback for Debate Improvement"
date: 2026-08-02
description: An LLM-based architecture for programming-free enactment of multiagent interaction protocols
category: publication
authors: "Omkar J. Joshi*, Priya Pitre*, Timon Ziegenbein, Henning Wachsmuth"
venue: "EMNLP Main Conference"
year: 2026
location: Budapest, Hungary
link: https://openreview.net/pdf?id=CDuZqKVuUO
---

## Research Problem

ReFeedGraph is a graph-grounded LLM feedback system that converts debate critiques into reusable revision principles for improving weaker debate arguments.

## Research Contribution

- Integrates feedback from multiple debate-judging frameworks.
- Stores failure–repair patterns in a reusable graph.
- Retrieves and adapts relevant revision principles.
- Generates targeted feedback for debate participants.
- Evaluated on DebateArt, IQ2, and British Parliamentary datasets.

## Methodology and Evaluation

The system extracts generalizable principles from judge feedback, organizes them in a graph, and retrieves relevant principles to generate targeted revisions for future debates.
ReFeedGraph was evaluated on the DebateArt, IQ2, and British Parliamentary datasets. It achieved:
- Up to 0.491 average score improvement over the original weaker-side arguments.
- Up to 85.1% improved cases across the evaluated datasets.
- Up to 89.7% winner-flip rate, indicating that the revised argument was judged stronger than the original winning side in a substantial portion of cases.

## Technologies

Large language models, knowledge graphs, retrieval-augmented generation, debate analysis, natural language processing, Python.
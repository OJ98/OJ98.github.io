---
layout: research
title: "ArgAnalysis35K"
date: 2023-07-01
description: A large-scale dataset for argument mining and analysis with 35K annotated examples
category: publication
authors: "Omkar J. Joshi*, Priya Pitre*, Yashodhara Haribhakta"
venue: "ACL Main Conference"
year: 2023
location: "Toronto, Canada"
link: https://aclanthology.org/2023.acl-long.778.pdf
---

## Research Problem

Existing argument-quality datasets often evaluate arguments without explicitly modeling the reasoning that supports them. ArgAnalysis35K investigates how argument quality can be studied jointly with the quality and relevance of supporting analysis.

## Research Contribution

ArgAnalysis35K introduces a dataset of 34,890 argument–analysis pairs from parliamentary debate. It provides separate quality scores for arguments and their supporting analysis, incorporates topic relevance modeling, and estimates annotator reliability at the individual-instance level.

## Methodology and Evaluation

The dataset combines contributions from debaters with arguments extracted from tournament speeches. Each example was evaluated by multiple annotators using several aggregation methods, including an instance-based reliability model. The dataset achieved an average Cohen’s kappa of 0.89, while BERT-based models reached Pearson and Spearman correlations of up to 0.54 and 0.55, respectively.

## Technical Details

BERT, Bi-LSTM, GloVe, argument mining, natural language processing, machine learning, annotator agreement analysis, Python.
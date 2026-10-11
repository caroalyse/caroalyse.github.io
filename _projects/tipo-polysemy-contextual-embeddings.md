---
layout: page
title: Contextual Embeddings for the Polysemy of tipo
description: A reproducible Python pipeline for studying lexical polysemy in Spanish and Portuguese.
img: assets/img/publication_preview/kmeans_12-clusters-label.png
importance: 2
category: research
related_publications: true
---

This project is a reusable computational pipeline for studying the meanings of the taxonomic noun _tipo_ (“type”) in context. It grew out of collaborative research with Patrícia Amaral on Spanish _tipo_ {% cite AmodeoWilliams2026WhatTI %} and was later expanded to support Portuguese and multilingual comparisons.

The pipeline uses contextualized transformer embeddings to represent each occurrence of a target word or phrase individually. It then clusters those representations and compares the resulting structure with meaning categories proposed in linguistic research. This makes it possible to investigate fuzzy boundaries between taxonomic, ad hoc categorization, and discourse-pragmatic uses without assuming that every occurrence belongs to a sharply defined sense from the outset.

## What the pipeline does

- Finds single- and multiword targets using longest-first matching
- Extracts and mean-pools contextual embeddings for each target span
- Records part-of-speech and morphological context for interpretation
- Evaluates candidate KMeans clustering solutions
- Builds centroid-similarity networks among clusters
- Produces occurrence-level and cluster-level qualitative summaries
- Supports external evaluation with human-reviewed sense annotations

The current release provides tested configurations for Spanish with BETO or multilingual BERT and Portuguese with Albertina or multilingual BERT. It also includes a guided notebook, reproducible configuration files, run manifests, and tests for target matching and token alignment.

## Research development

The code brings together three stages of the research: the original Spanish study using Europarl and TEDx data, a Portuguese study that introduced semantic-network analysis and improved occurrence tracking, and a current bilingual study comparing two encoders per language across three corpora.

The public repository does not redistribute the research corpora, model weights, or human-reviewed annotations. A synthetic sample is included for testing and learning the workflow.

## Technology

- Python 3.10+
- PyTorch and Hugging Face Transformers
- BETO, multilingual BERT, and Albertina
- spaCy
- scikit-learn
- KMeans clustering and cosine-similarity networks
- Jupyter

## Links

- [View the code and guided notebook on GitHub](https://github.com/caroalyse/tipo-polysemy-contextual-embeddings)
- [Read the associated article](https://doi.org/10.3765/plsa.v11i1.6145)

## Citation

When using or adapting the software, please cite:

Amodeo Williams, Caroline. (2026). _tipo-polysemy-contextual-embeddings: Reproducible contextual-embedding pipeline for lexical polysemy and taxonomic nouns_ (Version 0.1.0) [Computer software]. [GitHub repository](https://github.com/caroalyse/tipo-polysemy-contextual-embeddings).

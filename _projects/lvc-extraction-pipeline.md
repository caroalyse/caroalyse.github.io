---
layout: page
title: LVC Extraction Pipeline
description: A computational pipeline for extracting light verb constructions from text.
#redirect: https://github.com/caroalyse/LVC_Extraction_Pipeline
#github: https://github.com/caroalyse/LVC_Extraction_Pipeline
importance: 1
category: research
---

This project, developed in the class LING-L605 SP26 with Dr. Luke Gessler, builds a small **LLM-assisted pipeline for identifying and analyzing light verb constructions (LVCs) in Spanish** using a combination of rule-based filtering and LLM-based annotation from corpus data.

Light verb constructions, or LVCs (e.g., dar un paseo, hacer una pregunta), are challenging to detect because meaning is not categorical and is shared between the verb and its complement. This project uses a hybrid approach to classify LVCs:

- Rule-based candidate extraction
- Structured data transformation
- LLM-assisted semantic annotation

The output is a structured dataset annotated with linguistic features such as predicate type, lexical aspect (_Aktionsart_), and animacy.

---

## Motivation

This project addresses a key challenge in descriptive and computational linguistics:

> LVCs are difficult to identify due to semantic ambiguity and gradient classification.
> LVCs raise interesting questions about language change, such as verb auxiliarization and grammaticalization.

By combining rule-based filtering with LLM-based annotation, this pipeline explores a scalable approach to semantic classification in corpus data.

---

## Future Work

- Improve LLM classification accuracy
- Model predicate relationships
- Scale to larger, messier corpora (e.g., Reddit comments)
- Evaluate against annotated linguistic datasets

---

## Technology

- Python
- JSON structuring
- LLM API (e.g., Gemma / LLaMA)
- Regex-based text processing

---

## How to Cite

If you use this project, please cite it as follows:

### General:

Amodeo Williams, Caroline. (2026). _LVC Detection Pipeline for Spanish Verbs_. [GitHub repository](https://github.com/caroalyse/LVC_Extraction_Pipeline).

---

For full details, see the [LVC Extraction Pipeline GitHub repository](https://github.com/caroalyse/LVC_Extraction_Pipeline).

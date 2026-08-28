# Awesome Multilingual LLM Reliability

A curated collection of research papers, datasets, tools, implementations, and learning resources on the reliability of large language models (LLMs) when used across languages for scientific literature analysis — including translation, summarization, question answering, and fact verification.

This repository organizes and extends an earlier AI-assisted research paper on the same topic, together with a citation-integrity audit of that paper's references.

## Contents

- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Citation Integrity Audit](#citation-integrity-audit)
- [Curated Research Papers](#curated-research-papers)
- [Datasets](#datasets)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Tutorials and Learning Resources](#tutorials-and-learning-resources)
- [License](#license)

## Overview

Large language models are increasingly used to screen, summarize, translate, and answer questions about scientific literature. Because roughly 98% of indexed scientific output is published in English while most researchers are not native English speakers, multilingual LLMs are often promoted as a route to more equitable access to science. However, reliability is not uniform across languages: benchmarks consistently show that accuracy, factual grounding, and confidence calibration degrade as a model moves from high-resource languages like English or Chinese toward typologically distant or lower-resource languages.

This repository collects the empirical and methodological literature behind that finding. It covers the mechanisms that drive cross-lingual unreliability — translation-induced information loss, uneven pretraining data, and language-specific hallucination patterns — as well as current mitigation strategies such as retrieval-augmented generation, cross-lingual chain-of-thought prompting, and multilingual factuality metrics. It also includes domain-specific evidence from biomedical and general-purpose multilingual benchmarks. The overall conclusion of the underlying research is that targeted interventions narrow the cross-lingual reliability gap for individual tasks, but no current approach eliminates it — which is why every resource collected here was independently verified rather than accepted on the strength of an AI-generated citation.

## AI-Assisted Research Paper

**Evaluating Multilingual Reliability of Large Language Models in Scientific Literature Analysis** — a review of methods, evidence, and open problems in cross-lingual LLM reliability for scientific-literature-facing tasks (translation, summarization, QA, and fact verification).

[View Paper](paper/Evaluating_Multilingual_Reliability_of_LLMs_in_Scientific_Literature_Analysis.docx)

## Citation Integrity Audit

Every one of the 24 formal references was individually verified for correct title, authors, year, venue, and DOI/arXiv ID against publisher pages, DOI resolution, PubMed, ACL Anthology, arXiv, and dblp. Two entries had real attribution errors (both now corrected in `references/references.md`), and four in-text claims in the source paper cite nothing that exists in its reference list.

[View Audit — Citation_Integrity_Audit.pdf](citation-audit/Citation_Integrity_Audit.pdf) (also available as [Markdown](citation-audit/CITATION_INTEGRITY_AUDIT.md))

## Curated Research Papers

24 verified papers, organized by category:

- [Survey and Review Papers](references/references.md#survey-and-review-papers)
- [Foundational Papers](references/references.md#foundational-papers)
- [Evaluation Benchmarks](references/references.md#evaluation-benchmarks)
- [Applications and Domain Studies](references/references.md#applications-and-domain-studies)

Full list with authors, venues, DOIs, and one-line relevance notes: [`references/references.md`](references/references.md)

## Datasets

Four multilingual/cross-lingual evaluation benchmarks (XTREME, MMLU-ProX, MedExpQA, PubMedQA) with source, description, application, and links: [`datasets/datasets.md`](datasets/datasets.md)

## Tools and Libraries

Five actively maintained tools for multilingual evaluation and retrieval-augmented generation (Transformers, lm-evaluation-harness, LangChain, Haystack, SacreBLEU): [`tools/tools.md`](tools/tools.md)

## GitHub Implementations

Five implementations tied directly to papers or models discussed in the review (MMLU-ProX, XTREME, LLaMA, mT5, BLOOM training code): [`implementations/github-repositories.md`](implementations/github-repositories.md)

## Tutorials and Learning Resources

Five authoritative resources for learning multilingual NLP, transformer fine-tuning, and benchmark evaluation: [`tutorials/tutorials.md`](tutorials/tutorials.md)

## License

Repository content (this README, the audit, and the curated resource lists) is released under the [MIT License](LICENSE). Individual linked papers, datasets, and tools retain their own original licenses — see each linked source for details. No copyrighted paper PDFs are redistributed in this repository; only the author's own paper and citation audit are included as files.

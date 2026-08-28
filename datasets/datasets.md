# Datasets and Benchmarks

Four multilingual/cross-lingual benchmark datasets referenced in the paper, each verified against its original publication and official hosting page.

- **XTREME**
  Source: Google Research / [github.com/google-research/xtreme](https://github.com/google-research/xtreme)
  Description: A cross-lingual benchmark aggregating classification, structured-prediction, question-answering, and retrieval tasks across 40 typologically diverse languages.
  Application: Used in this paper as the early standard against which later benchmarks (e.g., MMLU-ProX) are compared.
  Paper: Hu et al., 2020 (ICML) — see [`../references/references.md`](../references/references.md).

- **MMLU-ProX**
  Source: [huggingface.co/collections](https://huggingface.co/li-lab) (dataset) / [github.com/weihao1115/MMLU-ProX](https://github.com/weihao1115/MMLU-ProX) (official evaluation code)
  Description: Extends the reasoning-focused MMLU-Pro benchmark to 29 typologically diverse languages, with ~11,829 parallel multiple-choice questions per language.
  Application: Central evidence in Section 3.1 for the ~30-point accuracy gap between best- and worst-performing languages.
  Paper: Xuan et al., 2025 — see [`../references/references.md`](../references/references.md).

- **MedExpQA**
  Source: HiTZ Center / see the [Artificial Intelligence in Medicine article](https://doi.org/10.1016/j.artmed.2024.102938) for the official data-access statement.
  Description: The first multilingual medical question-answering benchmark to include gold-standard explanations alongside answers.
  Application: Used in Section 3.1 to show a ~10-point English-to-other-language accuracy drop in a domain-specific (medical) setting.
  Paper: García-Ferrero et al., 2024 — see [`../references/references.md`](../references/references.md).

- **PubMedQA**
  Source: [github.com/pubmedqa/pubmedqa](https://github.com/pubmedqa/pubmedqa)
  Description: A biomedical research question-answering dataset built from PubMed abstracts, with yes/no/maybe labels grounded in the abstract text.
  Application: Referenced as a monolingual (English) biomedical QA baseline against which multilingual degradation can be measured.
  Paper: Jin et al., 2019 (EMNLP-IJCNLP) — see [`../references/references.md`](../references/references.md).

> Note: this topic is benchmark-centric rather than raw-corpus-centric — the "datasets" most relevant to multilingual LLM reliability are these evaluation benchmarks, not general-purpose training corpora. This is noted here per the assignment's instruction to explain when a resource category needs adaptation to the topic.

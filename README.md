# awesome-Multilingual-Reliability-of-LLMs-in-Scientific-Literature-Analysis
Curated, verified resources on multilingual LLM reliability in scientific literature analysis

# Verified Research Papers

All entries below were checked for correct title, authors, year, venue, and a working DOI/arXiv/publisher link before inclusion. See [`../citation-audit/CITATION_INTEGRITY_AUDIT.md`](../citation-audit/CITATION_INTEGRITY_AUDIT.md) for the verification method and the issues found in the source paper's *in-text* (as opposed to formal-list) citations.

## Contents
- [Survey and Review Papers](#survey-and-review-papers)
- [Foundational Papers](#foundational-papers)
- [Evaluation Benchmarks](#evaluation-benchmarks)
- [Applications and Domain Studies](#applications-and-domain-studies)

---

## Survey and Review Papers

- **Survey of Hallucination in Natural Language Generation**
  Ji, Z., Lee, N., Frieske, R., Yu, T., Su, D., Xu, Y., Ishii, E., Bang, Y. J., Madotto, A., & Fung, P., 2023, ACM Computing Surveys, 55(12), Article 248.
  [DOI](https://doi.org/10.1145/3571730)
  Establishes the factuality-vs-faithfulness hallucination taxonomy the paper builds on in Section 2.3.

- **A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions**
  Huang, L., Yu, W., Ma, W., Zhong, W., Feng, Z., Wang, H., Chen, Q., Peng, W., Feng, X., Qin, B., & Liu, T., 2025, ACM Transactions on Information Systems, 43(2), Article 42.
  [Publisher page](https://dl.acm.org/journal/tois)
  Extends the hallucination taxonomy and reviews mitigation strategies across training-time, retrieval-based, and post-hoc correction methods.

- **A Survey of Multilingual Large Language Models**
  Qin, L., Chen, Q., Zhou, Y., Chen, Z., Li, Y., Liao, L., Li, M., Che, W., & Yu, P. S., 2025, Patterns, 6(1), 101118.
  [DOI](https://doi.org/10.1016/j.patter.2024.101118)
  Provides the alignment-strategy taxonomy (parameter-, representation-, and prompting-level) used to frame cross-lingual transfer.

- **A Systematic Survey of Text Summarization: From Statistical Methods to Large Language Models**
  Zhang, H., Yu, P. S., & Zhang, J., 2024, arXiv:2406.11289.
  [arXiv](https://arxiv.org/abs/2406.11289)
  Background on summarization methods relevant to cross-lingual scientific summarization pipelines.

- **Generative Large Language Models in Automated Fact-Checking: A Survey**
  Vykopal, I., Pikuliak, M., Ostermann, S., & Šimko, M., 2024, arXiv:2407.02351.
  [arXiv](https://arxiv.org/abs/2407.02351)
  Source for the finding that LLM-based fact-verification systems remain biased toward high-resource languages.

## Foundational Papers

- **mT5: A Massively Multilingual Pre-trained Text-to-Text Transformer**
  Xue, L., Constant, N., Roberts, A., Kale, M., Al-Rfou, R., Siddhant, A., Barua, A., & Raffel, C., 2021, NAACL-HLT 2021, 483–498.
  [ACL Anthology](https://aclanthology.org/2021.naacl-main.41/)
  Early text-to-text multilingual transformer spanning 101 languages; foundational architecture referenced in Section 2.1.

- **BLOOM: A 176B-Parameter Open-Access Multilingual Language Model**
  BigScience Workshop, Le Scao, T., Fan, A., Akiki, C., et al., 2022, arXiv:2211.05100.
  [DOI](https://doi.org/10.48550/arXiv.2211.05100)
  Openly released 176B multilingual model covering 46 natural + 13 programming languages, trained via international collaboration.

- **LLaMA: Open and Efficient Foundation Language Models**
  Touvron, H., Lavril, T., Izacard, G., Martinet, X., et al., 2023, arXiv:2302.13971.
  [arXiv](https://arxiv.org/abs/2302.13971)
  General-purpose model with emergent (not explicitly trained) multilingual competence.

- **GPT-4 Technical Report**
  OpenAI, 2023, arXiv:2303.08774.
  [DOI](https://doi.org/10.48550/arXiv.2303.08774)
  Reference model for general-purpose LLM capability discussed throughout the paper.

- **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks**
  Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., Küttler, H., Lewis, M., Yih, W., Rocktäschel, T., Riedel, S., & Kiela, D., 2020, NeurIPS 33, 9459–9474.
  [NeurIPS proceedings](https://proceedings.neurips.cc/paper/2020/hash/6b493230205f780e1bc26945df7481e5-Abstract.html)
  Originates the RAG architecture proposed in Section 4 as a mitigation for cross-lingual factuality gaps.

## Evaluation Benchmarks

- **XTREME: A Massively Multilingual Multi-Task Benchmark for Evaluating Cross-Lingual Generalization**
  Hu, J., Ruder, S., Siddhant, A., Neubig, G., Firat, O., & Johnson, M., 2020, ICML 2020, PMLR 119, 4411–4421.
  [PMLR](https://proceedings.mlr.press/v119/hu20b.html)
  Early standardized cross-lingual benchmark aggregating QA and structured-prediction tasks.

- **MMLU-ProX: A Multilingual Benchmark for Advanced Large Language Model Evaluation**
  Xuan, W., Yang, R., Qi, H., Zeng, Q., Xiao, Y., et al., 2025, arXiv:2503.10497 (accepted EMNLP 2025).
  [arXiv](https://arxiv.org/abs/2503.10497) · [Official code](https://github.com/weihao1115/MMLU-ProX)
  Documents a ~30-point accuracy gap between best- and worst-performing languages on reasoning-focused questions.

- **MedExpQA: Multilingual Benchmarking of Large Language Models for Medical Question Answering**
  Alonso, I., Oronoz, M., & Agerri, R., 2024, Artificial Intelligence in Medicine, 155, 102938. *(Corrected author list — see citation audit: the source paper misattributed this to García-Ferrero et al., the authors of a different paper, "Medical mT5.")*
  [DOI](https://doi.org/10.1016/j.artmed.2024.102938)
  First multilingual medical QA benchmark with gold-standard explanations; reports a ~10-point English-to-other-language accuracy drop.

- **MlingConf: A Comprehensive Study of Multilingual Confidence Estimation on Large Language Models**
  Xue, B., Wang, H., Wang, R., Wang, S., Wang, Z., Du, Y., Liang, B., & Wong, K.-F., 2024, arXiv:2402.13606.
  [arXiv](https://arxiv.org/abs/2402.13606)
  Documents the "linguistic dominance effect" and the "native-tone prompting effect" in model confidence calibration.

- **PubMedQA: A Dataset for Biomedical Research Question Answering**
  Jin, Q., Dhingra, B., Liu, Z., Cohen, W. W., & Lu, X., 2019, EMNLP-IJCNLP 2019, 2567–2577.
  [ACL Anthology](https://aclanthology.org/D19-1259/)
  Widely used biomedical QA dataset; relevant baseline for domain-specific factuality evaluation.

- **EcomEval: Towards Reliable Evaluation of Large Language Models for Multilingual and Multimodal E-Commerce Applications**
  Xie, S., Liew, Z., Zhang, H., Zhang, H., Hu, L., Zhou, Z., Liu, S., & Zeng, A., 2025, arXiv:2510.20632.
  [arXiv](https://arxiv.org/abs/2510.20632)
  Included as a comparison point for how multilingual reliability evaluation generalizes outside the scientific domain.

## Applications and Domain Studies

- **The Emergence of Large Language Models as Tools in Literature Reviews: A Large Language Model-Assisted Systematic Review**
  Scherbakov, D., Hubig, N., Jansari, V., Bakumenko, A., & Lenert, L. A., 2025, JAMIA, 32(6), 1071–1086.
  [DOI](https://doi.org/10.1093/jamia/ocaf063) · [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12089777/)
  Large-scale review of 172 studies on LLM-assisted evidence synthesis; motivates the paper's human-in-the-loop recommendation.

- **Transforming Literature Screening: The Emerging Role of Large Language Models in Systematic Reviews**
  Delgado-Chaves, F. M., Jennings, M. J., Atalaia, A., Wolff, J., Horvath, R., Mamdouh, Z. M., Baumbach, J., & Baumbach, L., 2025, Proceedings of the National Academy of Sciences, 122(2), e2411962122. *(Authors added — the source paper's reference list omitted all 8 authors; see citation audit.)*
  [DOI](https://doi.org/10.1073/pnas.2411962122)
  Evaluates 18 LLMs on title/abstract screening replication across three systematic reviews.

- **Capabilities of GPT-4 on Medical Challenge Problems**
  Nori, H., King, N., McKinney, S. M., Carignan, D., & Horvitz, E., 2023, arXiv:2303.13375.
  [arXiv](https://arxiv.org/abs/2303.13375)
  English-language medical benchmark performance used as a comparison point for multilingual medical QA gaps.

- **Towards Building Multilingual Language Model for Medicine**
  Qiu, P., Wu, C., Zhang, X., Lin, W., Wang, H., Zhang, Y., Wang, Y., & Xie, W., 2024, Nature Communications, 15, 8384.
  [DOI](https://doi.org/10.1038/s41467-024-52417-z)
  Introduces MMed-Llama 3; shows targeted multilingual instruction tuning narrows but does not close the reliability gap.

- **Science Across Languages: Assessing LLM Multilingual Translation of Scientific Papers**
  Kleidermacher, H. C., & Zou, J., 2025, arXiv:2502.17882.
  [DOI](https://doi.org/10.48550/arXiv.2502.17882)
  Evaluates full-article translation across 28 languages with JATS XML structure preservation; documents overtranslation and terminology-consistency failures.

- **Low-Resource Cross-Lingual Summarization through Few-Shot Learning with Large Language Models**
  Park, G., Hwang, S., & Lee, H., 2024, arXiv:2406.04630.
  [arXiv](https://arxiv.org/abs/2406.04630)
  Shows few-shot prompting narrows but does not close the summarization quality gap for low-resource target languages.

- **Massively Multilingual Language Models for Cross-Lingual Fact Extraction from Low-Resource Indian Languages**
  Singh, B., Kandru, P., Sharma, A., & Varma, V., 2023, arXiv:2302.04790.
  [arXiv](https://arxiv.org/abs/2302.04790)
  Shows structured fact-extraction lags well behind monolingual English extraction for low-resource Indian languages.

- **The Manifold Costs of Being a Non-Native English Speaker in Science**
  Amano, T., Ramírez-Castañeda, V., Berdejo-Espinola, V., Borokini, I., Chowdhury, S., et al., 2023, PLOS Biology, 21(7), e3002184.
  [DOI](https://doi.org/10.1371/journal.pbio.3002184) · [PMID: 37463136](https://pubmed.ncbi.nlm.nih.gov/37463136/)
  Survey of 908 environmental scientists quantifying the structural costs of non-native English-speaker status in science, motivating the paper's equity framing.

# Tools and Libraries

Five actively maintained tools relevant to multilingual LLM evaluation, retrieval-augmented generation, and translation-quality assessment.

- **Hugging Face Transformers** — [github.com/huggingface/transformers](https://github.com/huggingface/transformers)
  Model library providing access to mT5, BLOOM, LLaMA-family, and most multilingual LLMs discussed in the paper, plus a reference RAG (`RagSequenceForGeneration`) implementation.

- **EleutherAI lm-evaluation-harness** — [github.com/EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)
  Few-shot evaluation framework used to run standardized benchmarks (including MMLU-ProX) across languages and models; backend for Hugging Face's Open LLM Leaderboard.

- **LangChain** — [github.com/langchain-ai/langchain](https://github.com/langchain-ai/langchain)
  Orchestration framework for building retrieval-augmented generation pipelines, useful for implementing the RAG mitigation strategy discussed in Section 4.1.

- **Haystack** — [github.com/deepset-ai/haystack](https://github.com/deepset-ai/haystack)
  Open-source framework for building retrieval-augmented QA and search pipelines with multilingual document stores and retrievers.

- **SacreBLEU** — [github.com/mjpost/sacrebleu](https://github.com/mjpost/sacrebleu)
  Standardized, reproducible BLEU/ChrF scoring tool for machine-translation quality, relevant to evaluating the translation-mediated information loss discussed in Section 3.4.

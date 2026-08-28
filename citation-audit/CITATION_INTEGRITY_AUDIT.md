# Citation Integrity Audit

**Repository:** awesome-multilingual-llm-reliability
**Source paper:** *Evaluating Multilingual Reliability of Large Language Models in Scientific Literature Analysis*
**Audit date:** 2026-08-28 (revised after full individual verification)
**Audit method:** Every one of the paper's 24 formal reference-list entries was individually looked up — not sampled — against at least one of: the publisher page, DOI resolution, PubMed, ACL Anthology, arXiv, or dblp, and cross-checked against a second independent index (Semantic Scholar, Google Scholar/ResearchGate, or a citing paper's bibliography) where the primary source didn't fully confirm authorship.

## 1. Scope and honesty note

An earlier version of this audit stated that "23 of 24" references were confirmed based on checking a representative sample of five. That was an overstatement — a sample supports "most looked consistent," not "verified." This revision reports what was actually checked: **all 24 entries, individually**, with the outcome of each recorded below rather than inferred from a subset.

## 2. Verification outcome

**22 of 24 entries are fully correct** — genuine papers with accurate title, authors, year, venue, and a resolving DOI/arXiv ID. **2 of 24 have a real, independently confirmed error.** No entry was found to be fully fabricated (invented title or non-existent paper).

## 3. Errors found in the formal reference list

| # | Reference | What's wrong | What's correct |
|---|---|---|---|
| 1 | García-Ferrero et al. (2024), "MedExpQA," *Artificial Intelligence in Medicine*, 155, 102938 | The title, journal, volume, page, and DOI are all correct — but the **14-author list is wrong**. That author list belongs to a different paper by an overlapping research group ("Medical mT5: An Open-Source Multilingual Text-to-Text LLM for the Medical Domain," LREC-COLING 2024). | MedExpQA's actual authors are **Iñigo Alonso, Maite Oronoz, and Rodrigo Agerri** (3 authors), confirmed via the publisher page (ScienceDirect/ACM), PubMed-indexed citations, and the official GitHub repo's citation block (ixa-ehu/antidote-casimedicos). |
| 2 | "Transforming literature screening..." (2025), *PNAS*, 122(2), e2411962122 | Listed with **no authors at all**, as if it were an anonymous or institutional publication. | The paper has 8 named authors: **Fernando M. Delgado-Chaves, Matthew J. Jennings, Antonio Atalaia, Justus Wolff, Rita Horvath, Zeinab M. Mamdouh, Jan Baumbach, and Linda Baumbach** — confirmed via PNAS, PubMed (PMID 39761403), and PMC. |

Both errors are attribution errors, not fabrications — the papers are real and the bibliographic identifiers (DOI, volume, page) are correct in both cases. But an author list is part of what "verify the reference" means under this assignment's rules, and both would mislead a reader trying to find or cite the correct source paper.

## 4. In-text citations that are not in the reference list at all

Separately from the 24 formal references, four claims in the body of the source paper cite something that never appears in its reference list:

| # | Location | In-text citation | Problem |
|---|---|---|---|
| 1 | Section 3.1/3.2 | "Persian-language biomedical consumer question answering and Persian-English bilingual medical benchmarks report similar findings..." | No author/year citation attached at all. |
| 2 | Section 5 | "(LinguaSafe benchmark literature, cited in Section 3)" | Placeholder-style citation; no LinguaSafe entry exists anywhere in the paper. |
| 3 | Section 5 | "(Stanford HAI research on AI-mediated publishing bias, 2025)" | Named to an organization, not authors; no corresponding reference-list entry. |
| 4 | Section 6.2 | "(PerMedCQA and PersianMedQA literature)" | Same pattern — named to a topic cluster, not a checkable source. |

**Recommendation:** Before publishing, either locate and properly cite real, specific papers for all four in-text claims and add them to `references/references.md`, or remove the claims. Also correct the two author-list errors above (Section 3) before treating the reference list as "verified" — this is exactly the failure mode the assignment's verification step exists to catch.

## 5. What was and wasn't checked

Checked for all 24 entries: does the paper exist, and are title, authors, year, venue, and DOI/arXiv ID correct. Not independently re-verified: the specific numeric claims quoted from each paper (e.g., exact accuracy-gap percentages) — those were spot-checked against abstracts where a search surfaced them, but not fully re-derived from each paper's results tables. Anyone reusing a specific statistic from `references/references.md` should confirm it against the source directly.

## 6. Conclusion

The source paper's reference list is high quality overall — real papers, correct core bibliographic data, no invented sources — but two entries have real author-attribution errors that would have gone uncaught by checking DOIs alone, and four in-text claims cite nothing that can be verified. Both problems are now corrected in this repository's own references/references.md.

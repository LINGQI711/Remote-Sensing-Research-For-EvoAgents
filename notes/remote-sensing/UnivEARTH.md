# Towards LLM Agents for Earth Observation

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ACL-Findings/Towards%20LLM%20Agents%20for%20Earth%20Observation.pdf) · [Source version](https://arxiv.org/abs/2504.12110v2) · [Publication](https://aclanthology.org/2026.findings-acl.124/)

**Venue:** Findings of ACL 2026

**Version read:** v2

**Topic:** Evidence-grounded Earth observation coding benchmark

## 1. What problem does it address?

Answering an Earth science question from model memory is not equivalent to deriving an answer from satellite evidence. The benchmark asks whether agents can choose appropriate data and produce executable analyses.

## 2. How does it solve the problem?

Questions originate from NASA Earth Observatory articles and are checked for answerability with Google Earth Engine. Models generate analysis code, execute it, and derive answers from the results. The archived v2 compares tool-grounded answers with internal-knowledge and web-search settings.

## 3. What experiments were conducted?

- The archived arXiv v2 contains 140 yes/no questions across 13 topics and 17 satellite sensors.
- Evaluates zero-shot, three-shot, and reflexion prompting with GEE, and an open-model fine-tuning study.
- Table 1 and Section 3.1 report roughly 33% best overall accuracy, with code execution or unavailable-data failures exceeding 58%; Appendix C examines improvements from synthetic-data fine-tuning.

## 4. What are the conclusions?

Reliable code execution and correct data-source selection are central bottlenecks. A correct-looking answer alone is insufficient evidence of scientific validity. The small v2 benchmark has no questions whose ground-truth answer is inconclusive.

**Reading pointers:** Sections 2-3 and Table 1 for the archived v2 benchmark and evaluation; Section 4 for limitations; Appendix C for fine-tuning. The linked Findings of ACL 2026 publication has 408 questions and updated results; those should not be compared directly with the v2 figures above.

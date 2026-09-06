# Trace2Skill: Distill Trajectory-Local Lessons into Transferable Agent Skills

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf) · [Source version](https://arxiv.org/abs/2603.25158v5)

**Venue:** arXiv preprint

**Version read:** v5

**Topic:** Distilling portable skills from execution traces

## 1. What problem does it address?

Execution traces contain useful local lessons, but directly accumulating them produces redundant, conflicting guidance that transfers poorly.

## 2. How does it solve the problem?

Parallel analysts inspect trajectories and propose evidence-grounded skill patches. Hierarchical consolidation resolves overlaps and conflicts into a portable skill directory. The framework can deepen an existing skill or build a new one from experience.

## 3. What experiments were conducted?

- Evaluates SpreadsheetBench with a 200/200 evolution-test split, broader spreadsheet subsets, and WikiTableQuestions and HiTab transfer.
- Extends evaluation to mathematical reasoning, DocVQA, and PDF, DOCX, and PPTX tasks, with multiple author and user models.
- Compares success, error, and combined traces; parallel versus sequential analysis; and consolidated skills versus retrieval-style memory.

## 4. What are the conclusions?

Trajectory analysis can produce reusable guidance that transfers across tasks and models, and parallel consolidation can reduce evolution time. Improvements are not uniform: some task/model combinations regress. This entry concerns the Qwen-Applications agent-skill method, rather than a separate EDA paper with the same short name.

**Reading pointers:** Method, main experiments, and extensions; Tables 1–4; PDF pages 3–10.

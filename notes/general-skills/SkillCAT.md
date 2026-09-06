# SkillCAT: Contrastive, Assessment-Augmented and Topology-Aware Skill Self-Evolution for LLM Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf) · [Source version](https://arxiv.org/abs/2606.13317v2)

**Venue:** arXiv preprint

**Version read:** v2

**Topic:** Contrastive extraction, patch assessment, and skill routing

## 1. What problem does it address?

Skill evolution can extract unreliable lessons from isolated trajectories, merge harmful patches, and overload inference with irrelevant skill text.

## 2. How does it solve the problem?

Contrastive Causal Extraction compares same-task successes and failures. Assessment-Augmented Evolution replays candidate patches on source-task clones and filters harmful changes before hierarchical merging. Topology-Aware Task Execution loads relevant sub-skill nodes instead of the entire collection.

## 3. What experiments were conducted?

- Uses SpreadsheetBench Verified with 200 evolution and 200 held-out tasks, WikiTableQuestions for distribution shift, and DocVQA with 2,700 evolution and 2,649 test examples.
- Compares human and generated initial skills, competing evolution methods, cross-model transfer, and three-seed averages.
- Ablates extraction, assessment, and routing; Table 2 reports 55.00 for the full configuration versus 26.00 without assessment.

## 4. What are the conclusions?

Explicit patch validation and selective routing make evolved skills more useful in the reported settings. Gains vary across tasks and models; the method is not the best in every table cell. Source-task replay filters local regressions but does not guarantee that a patch improves every future task.

**Reading pointers:** Sections on CCE, AAE, TTE, and experiments; Tables 1–2; PDF pages 3–8.

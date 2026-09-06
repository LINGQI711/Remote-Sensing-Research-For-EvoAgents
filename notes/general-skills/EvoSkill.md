# EvoSkill: Automated Skill Discovery for Multi-Agent Systems

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [Source version](https://arxiv.org/abs/2603.02766v1)

**Venue:** arXiv preprint

**Version read:** v1

**Topic:** Validated iterative skill discovery

## 1. What problem does it address?

Handwritten agent skills are expensive to maintain and do not automatically adapt to recurring task failures.

## 2. How does it solve the problem?

An executor produces task evidence, a proposer identifies promising improvements, and a skill builder implements candidate skills. Validation selects useful candidates and maintains an improvement frontier for subsequent evolution.

## 3. What experiments were conducted?

- Uses a Claude Code/Opus 4.5 setup on OfficeQA, with small evolution subsets and a separate 17-question validation set.
- Tests SealQA and zero-shot transfer to BrowseComp, and studies differing amounts of evolution data.
- OfficeQA includes 246 questions over a large Treasury document collection, with exact and tolerance-based answer scoring.

## 4. What are the conclusions?

The reported OfficeQA exact score increases from 60.6 to 67.9 and SealQA from 26.6 to 38.7; BrowseComp transfer improves by 5.3 percentage points. These results support iterative, validated skill discovery in the evaluated harness, rather than proving equal gains across arbitrary models or environments.

**Reading pointers:** Method and evaluation sections; PDF pages 2–8.

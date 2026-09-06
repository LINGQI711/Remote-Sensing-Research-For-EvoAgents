# SkillOpt: Executive Strategy for Self-Evolving Agent Skills

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf) · [Source version](https://arxiv.org/abs/2605.23904v2)

**Venue:** arXiv preprint

**Version read:** v2

**Topic:** Controlled optimization of textual agent skills

## 1. What problem does it address?

Unconstrained skill editing can overreact to individual failures, forget useful strategies, and accept changes that do not generalize.

## 2. How does it solve the problem?

SkillOpt treats a compact textual skill as the optimization state while keeping the model frozen. Bounded rollout-and-reflection edits, a textual learning rate, slower meta-updates, a held-out acceptance gate, and rejected-edit memory control the optimization process.

## 3. What experiments were conducted?

- Evaluates SearchQA, SpreadsheetBench, OfficeQA, DocVQA, LiveMath, and ALFWorld across seven target models and three execution harnesses.
- Compares alternative optimizers and ablates the mechanisms that bound or validate edits. Harness-based studies omit ALFWorld where its stateful setup does not match.

## 4. What are the conclusions?

Controlled editing improves average performance in the reported comparisons. For GPT-5.5 in direct chat, the six-task average rises from 58.8 to 82.3, versus 76.9 for the strongest listed baseline. This supports disciplined skill optimization, while results remain tied to the evaluated models, data, and execution budgets.

**Reading pointers:** Optimizer design and experimental sections; main comparison and ablation tables.

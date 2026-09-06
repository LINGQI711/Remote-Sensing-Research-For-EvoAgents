# ExpeL: LLM Agents Are Experiential Learners

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [Source version](https://arxiv.org/abs/2308.10144v3)

**Venue:** AAAI 2024

**Version read:** v3

**Topic:** Natural-language lessons and experience retrieval

## 1. What problem does it address?

LLM agents often treat tasks independently and fail to turn prior successes and failures into better future decisions.

## 2. How does it solve the problem?

ExpeL gathers trajectories, extracts natural-language insights from successful and failed experiences, and retrieves relevant successful demonstrations at inference time. Learning occurs in external experience and insight memory rather than through model-weight updates.

## 3. What experiments were conducted?

- Evaluates HotpotQA, ALFWorld, and WebShop with question-answer accuracy, task success, and environment rewards.
- Studies transfer to FEVER and compares against acting and reasoning-agent baselines using repeated evaluation folds.

## 4. What are the conclusions?

Combining abstract lessons with retrieved demonstrations improves experiential reuse across the studied tasks. Its skills are primarily verbal guidance and examples rather than a library of executable APIs. This makes it a useful conceptual baseline for later trajectory-to-skill methods, but not an identical implementation of skill files.

**Reading pointers:** Experience collection, insight extraction, and experimental sections.
